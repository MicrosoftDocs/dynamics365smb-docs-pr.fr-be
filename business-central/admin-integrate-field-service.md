---
title: Intégration à Microsoft Dynamics 365 Field Service
description: Intégrer Business Central dans Field Service.
ms.date: 02/21/2024
ms.topic: article
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.custom: bap-template
---

# <a name="integrate-with-microsoft-dynamics-365-field-service"></a>Intégration à Microsoft Dynamics 365 Field Service

Les organisations de services ont besoin d’une application front-to-back dans laquelle les finances, les stocks et les achats sont étroitement liés à la prestation de services. Ils génèrent des données financières à chaque transaction. Chaque ordre de travail représente des coûts et des revenus, et chaque ressource génère des profits et des pertes. Les interactions avec les clients ajoutent des écritures comptabilité. L’intégration entre [!INCLUDE [prod_short](includes/prod_short.md)] et [!INCLUDE [field-service-short](includes/field-service-short.md)] rationalise le processus de bout en bout de gestion des opérations de service et garantit un flux fluide d’informations entre les deux systèmes.  

Vous pouvez facilement créer et gérer des ordres de travail dans [!INCLUDE [field-service-short](includes/field-service-short.md)], suivre la progression des tâches de service, attribuer des ressources et capturer les détails de la consommation. Lorsque vous complétez un bon de travail dans [!INCLUDE [field-service-short](includes/field-service-short.md)], l’intégration permet le transfert fluide des données vers [!INCLUDE [prod_short](includes/prod_short.md)] pour un traitement ultérieur.  

L’intégration facilite également la facturation et l’exécution des bons de travail dans [!INCLUDE [prod_short](includes/prod_short.md)]. Vous pouvez générer des factures précises basées sur les activités de service et la consommation enregistrées dans [!INCLUDE [field-service-short](includes/field-service-short.md)].  

Grâce à l’intégration [!INCLUDE [prod_short](includes/prod_short.md)] avec [!INCLUDE [field-service-short](includes/field-service-short.md)], vous n’avez pas besoin de saisir les données manuellement ni de dupliquer les efforts. L’intégration fournit également une vue complète des opérations et des finances des services, permettant une meilleure prise de décision et une meilleure efficacité opérationnelle.

## <a name="prerequisites"></a>Conditions préalables

Étant donné que [!INCLUDE [field-service-short](includes/field-service-short.md)] est construit sur Dynamics 365 Sales, vous devez [configurer une connexion pour Dataverse](/dynamics365/business-central/admin-how-to-set-up-a-dynamics-crm-connection#to-use-the-dataverse-connection-setup-assisted-setup-guide) et [activer l’intégration à Dynamics 365 Sales](/dynamics365/business-central/admin-prepare-dynamics-365-for-sales-for-integration#connection-settings-in-the-setup-guide).

Vous devez télécharger l’application Field Service Integration depuis [AppSource](https://go.microsoft.com/fwlink/?linkid=2277917) et l’installer [!INCLUDE [prod_short](includes/prod_short.md)].

### <a name="permissions-and-security-roles-for-user-accounts"></a>Autorisations et rôles de sécurité pour les comptes d’utilisateur

Lorsque vous installez la solution d’intégration, les autorisations pour le compte d’utilisateur d’intégration sont configurées. Si ces autorisations changent, vous devrez peut-être les réinitialiser. Pour le faire en réinstallant la solution d’intégration dans **Paramètres de la connexion Dynamics 365** sur la page **Redéployer la solution d’intégration**. Les sections suivantes répertorient les autorisations et les rôles de sécurité que la solution déploie pour chaque application.

#### <a name="sales"></a>Vente

* Administrateur d’intégration [!INCLUDE [prod_short](includes/prod_short.md)] Dynamics 365
* Utilisateur d’intégration [!INCLUDE [prod_short](includes/prod_short.md)] Dynamics 365
* Utilisateur de disponibilité produit [!INCLUDE [prod_short](includes/prod_short.md)] Dynamics 365

#### <a name="business-central"></a>Business Central

Les utilisateurs qui publient des journaux de projet doivent disposer de l’ensemble d’autorisations suivant :

* Intégration Dynamics 365 Sales

#### <a name="field-service"></a>Field Service

Pour utiliser les données intégrées, les utilisateurs doivent disposer du rôle de sécurité suivant :

* Intégration Business Central dans Field Service

Par exemple, les utilisateurs doivent disposer de ce rôle pour connecter les ordres de travail à [!INCLUDE [prod_short](includes/prod_short.md)] en vue de leur traitement.

> [!NOTE]
> Assurez-vous que les utilisateurs sont affectés aux rôles et profils de sécurité standard dans [!INCLUDE [field-service-short](includes/field-service-short.md)].  
>
> Pour en savoir plus sur les profils de sécurité des colonnes dans [!INCLUDE [field-service-short](includes/field-service-short.md)], accédez à [Rôles de sécurité Field Service](/dynamics365/field-service/users-licenses-permissions#field-service-security-roles).
>
> Les administrateurs doivent ajouter l’un des profils de sécurité de colonne appropriés aux utilisateurs dans Power Platform. Pour en savoir plus, accédez à [Ajouter des équipes ou des utilisateurs à un profil de sécurité de colonne pour contrôler l’accès](/power-platform/admin/add-teams-users-field-security-profile).

> [!NOTE]
> Pour utiliser l’action **Ouvrir dans Business Central** dans Sales, vous devez disposer des privilèges suivants pour les tables suivantes :
>
> * Vous devez disposer des autorisations de **lecture** pour la table **Dynamics 365 Business Central Connexion** (nav_connection).
> * Vous devez disposer des autorisations de **lecture**, **d’écriture** et de **suppression** pour la table **Connexion par défaut Dynamics 365 Business Central (nav_defaultconnection)**.

### <a name="other-settings-in-field-service"></a>Autres paramètres dans Field Service

Sur la page **Paramètres Field Service** , définissez les modifications suivants :

* Dans l’onglet **Achat** , décochez le champ **Utilisation des produits en rupture de stock** . Sinon, vous pourriez recevoir un avertissement "en rupture de stock" lorsque vous choisissez un produit qui est en rupture de stock à [!INCLUDE [field-service-short](includes/field-service-short.md)], mais qui est en stock à [!INCLUDE [prod_short](includes/prod_short.md)].
* Dans l’onglet **Bon de travail/Réservation** , désactivez les options **Calculer le prix** et **Calculer Coût** bascule. Dans le champ **Création facture ordre de travail**, sélectionnez **Jamais**.

> [!NOTE]
> La configuration d’une connexion à [!INCLUDE [field-service-short](includes/field-service-short.md)] supprime le couplage entre les ressources et les produits. Pour rendre [!INCLUDE [prod_short](includes/prod_short.md)] les éléments disponibles dans [!INCLUDE [field-service-short](includes/field-service-short.md)], mettez à jour le **Type de produit de service sur site** pour qu’il corresponde au **Tapez** champ sur les éléments dans [!INCLUDE [prod_short](includes/prod_short.md)]. Pour en savoir plus, accédez à [Créer un produit ou un service](/dynamics365/field-service/create-product-or-service#create-a-product-or-service).

## <a name="set-up-the-integration-in-business-central"></a>Configurer de l'intégration dans Business Central

Une fois que vous êtes connecté à Dataverse et à Sales, vous pouvez configurer votre intégration à [!INCLUDE [field-service-short](includes/field-service-short.md)].

* Téléchargez et installez l’application Field Service Integration depuis [AppSource](https://go.microsoft.com/fwlink/?linkid=2277917). Ensuite, sur la page **Gestion des extensions**, recherchez l’application Field Service Integration et choisissez l’action **Configurer** pour exécuter la configuration assistée guide.
* Sur la page **Configuration assistée** de [!INCLUDE [prod_short](includes/prod_short.md)], choisissez **Configurer l’intégration pour Dynamics 365 Field Service** pour exécuter le guide de configuration assistée.

Cette section décrit les paramètres clés du guide.

Pour permettre aux utilisateurs de publier la consommation d’articles et de services dans [!INCLUDE [field-service-short](includes/field-service-short.md)] bons de travail, spécifiez le **modèle de journal de projet** et **le lot de journal de projet** à utiliser pour publier la consommation de produits et de services.

Étant donné que les services sont exprimés en durée en [!INCLUDE [field-service-short](includes/field-service-short.md)], spécifiez l’ **Unité de mesure des heures** à utiliser pour convertir les durées en quantités en [!INCLUDE [prod_short](includes/prod_short.md)].

Vous pouvez aussi spécifier quand synchroniser les produits d’ordre de travail et les lignes de services d’ordres de travail [!INCLUDE [prod_short](includes/prod_short.md)]. Par exemple, ils peuvent se synchroniser lorsque les lignes d’ordre de travail sont utilisées ou lorsque quelqu’un termine un bon de travail. Choisissez l’option appropriée dans le **Synchroniser les produits/services des bons de travail** champ.

Après la synchronisation des produits et services du bon de travail avec les journaux de projet dans [!INCLUDE [prod_short](includes/prod_short.md)], vous pouvez choisir de valider manuellement les journaux de projet. Choisissez l’option appropriée dans le **Publier automatiquement les lignes des journaux de projet** champ :

* Quand l’ordre de travail est terminé.
* Lorsque des produits ou services d’ordre de travail sont utilisés.

Une fois la configuration terminée, exécutez une synchronisation complète à partir du **Dynamics 365 Field Service Configuration de l’intégration** page. Cette action synchronise les mappages de tables pour des éléments tels que :

* Tâches de projet pour les projets avec le **Appliquer le lien d’utilisation** ensemble. Cette synchronisation fait [!INCLUDE [prod_short](includes/prod_short.md)] projets disponibles à la sélection dans [!INCLUDE [field-service-short](includes/field-service-short.md)].
* Les ressources qui ne sont pas bloquées n’ont pas **Utiliser la feuille de temps** sélectionné, et j’ai **Heures** spécifiée comme unité de mesure sur le **Dynamics 365 Field Service Configuration de l’intégration** page.
* Articles de service (nécessite que vous utilisiez l’expérience Premium dans [!INCLUDE [prod_short](includes/prod_short.md)]).

## <a name="standard-field-service-entity-mapping-for-synchronization"></a>Mappage d’entité Field Service standard pour la synchronisation

La base de la synchronisation des données consiste à mapper les tables et les champs dans [!INCLUDE [prod_short](includes/prod_short.md)] avec des tables et des colonnes dans Dataverse afin qu’ils échangent les données. Le mappage s’effectue via des tables d’intégration. Pour en savoir plus sur les mappages de tables, accédez à [Mappage des tables et des champs à synchroniser](/dynamics365/business-central/admin-how-to-modify-table-mappings-for-synchronization).

Intégration avec [!INCLUDE [field-service-short](includes/field-service-short.md)] présente les mappages de tables d’intégration standard suivants :

* **PJLINE-WORDERPRODUCT** – Mappe les produits d’ordre de travail dans [!INCLUDE [field-service-short](includes/field-service-short.md)] aux lignes de journal du projet [!INCLUDE [prod_short](includes/prod_short.md)].
* **PJLINE-WORDERSERVICE** – Mappe les services d’ordre de travail dans [!INCLUDE [field-service-short](includes/field-service-short.md)] aux lignes de journal du projet [!INCLUDE [prod_short](includes/prod_short.md)].
* **PROJECTTASK** – Mappe les projets et les tâches de projet dans [!INCLUDE [prod_short](includes/prod_short.md)] aux produits de projets externes dans [!INCLUDE [field-service-short](includes/field-service-short.md)].
* **RESOURCE-BOOKABLERSC** – Mappe les ressources dans [!INCLUDE [prod_short](includes/prod_short.md)] aux ressources réservables dans [!INCLUDE [field-service-short](includes/field-service-short.md)].
* **SVCITEM-CUSTASSET** – (Expérience Premium uniquement) Mappe les éléments de service dans [!INCLUDE [prod_short](includes/prod_short.md)] aux actifs du client dans [!INCLUDE [field-service-short](includes/field-service-short.md)].

## <a name="use-data-in-both-applications"></a>Utiliser les données dans les deux applications

Les sections suivantes décrivent les fonctionnalités permettant d’utiliser les données provenant de [!INCLUDE [prod_short](includes/prod_short.md)] et [!INCLUDE [field-service-short](includes/field-service-short.md)].

### <a name="field-service-1"></a>Field Service

Vous pouvez [créer des bons de travail](/dynamics365/field-service/create-work-order) à l’aide du **compte de service** et **Compte de facturation** de [!INCLUDE [prod_short](includes/prod_short.md)]. Sur les bons de travail, vous devez sélectionner la **Tâche de projet Business Central** dans le champ **Projet externe** . La sélection d’un projet vous permet de synchroniser les produits et services de l’ordre de travail avec la tâche de projet appropriée dans [!INCLUDE [prod_short](includes/prod_short.md)].

Vous pouvez ajouter des articles en stock et hors stock en tant que **Produits d’ordre de travail** sur les bons de travail et obtenir la quantité disponible ainsi que les coûts et les prix [!INCLUDE [prod_short](includes/prod_short.md)]. Pour en savoir plus, accédez à [Créer un bon de travail à partir du formulaire de bon de travail et de la liste d’enregistrement](/dynamics365/field-service/create-work-order#create-a-work-order-from-the-work-order-form-and-record-list).

Vous pouvez ajouter des articles du type service en tant que **Services d’ordre de travail** et obtenir les coûts et les prix à partir de [!INCLUDE [prod_short](includes/prod_short.md)]. Pour en savoir plus, accédez à l’ [onglet Produits et services](/dynamics365/field-service/work-order-experience#products-and-services-tab).

> [!NOTE]
> Lorsque un statut d’un produit ou d’un service sur un bon de travail passe de **Estimé** à **Utilisé** dans [!INCLUDE [field-service-short](includes/field-service-short.md)], ils seront synchronisés avec les lignes du journal du projet dans [!INCLUDE [prod_short](includes/prod_short.md)].

Vous pouvez réserver une ressource et associer les **réservations** aux services d’ordre de travail à l’aide d’une **ressource réservable** de [!INCLUDE [prod_short](includes/prod_short.md)].

### <a name="business-central-1"></a>Business Central

En fonction de vos paramètres sur la page **Configuration de l’intégration de Field Service** , lorsque les ordres de travail incluent des produits et des services, les informations de consommation sont transférées et publiées à l’aide d’un **Projet. Journal** dans [!INCLUDE [prod_short](includes/prod_short.md)].

Les valeurs **Quantité à facturer** et **Durée à facturer** sont copiées dans la **Quantité. pour transférer vers le champ Facture** . Sur la base de ces valeurs, vous pouvez créer et valider des factures de vente dans [!INCLUDE [prod_short](includes/prod_short.md)] pour facturer le client. Une fois la facture validée ou la consommation traitée dans [!INCLUDE [prod_short](includes/prod_short.md)], la quantité facturée et la quantité consommée s’affichent dans l’ [!INCLUDE [prod_short](includes/prod_short.md)] onglet du **Produit de l’ordre de travail** et **Service de bon de travail** pages.  

Utilisez la page **Lignes de planification de projet** pour suivre la validation et la facturation de la consommation sur les ordres de travail. À partir de la page **Lignes de planification de projet** , vous pouvez créer et valider des factures de vente dans [!INCLUDE [prod_short](includes/prod_short.md)]. Ensuite, vous pouvez les synchroniser avec [!INCLUDE [field-service-short](includes/field-service-short.md)] et suivre l’état des factures.

> [!NOTE]
> Les services d’ordre de travail avec une réservation qui utilise une ressource réservable couplée à une [!INCLUDE [prod_short](includes/prod_short.md)] ressource synchronisée avec deux lignes de journal de projet : une ligne de type **Budget** pour la ressource couplée, et une autre ligne de type **Facturable** pour l’article en cours de service.
>
> Le produit choisi sur le service de bon de travail doit être couplé à un article de type **Service** dans [!INCLUDE [prod_short](includes/prod_short.md)]. De plus, l’unité de mesure de base de l’article doit être définie sur **unité de mesure des heures** choisie dans la **Dynamics 365 Field Service configuration de l’intégration** page.
>
> Vous pouvez créer une facture pour un article du type **Service** à partir de la ligne de planification du projet facturable et utiliser la ligne de planification du projet budgétaire pour enregistrer le coût auprès de la ressource.

## <a name="see-also"></a>Voir aussi

[Intégration à Microsoft Dataverse via la synchronisation des données](admin-common-data-service.md)  
[Mappage des tables et des champs à synchroniser](admin-how-to-modify-table-mappings-for-synchronization.md)
