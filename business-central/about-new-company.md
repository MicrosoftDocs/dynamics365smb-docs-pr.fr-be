---
title: Créer des sociétés en utilisant le guide de configuration assistée
description: 'Il est facile de créer une nouvelle société vide dans Business Central. Un guide de configuration assistée vous aide à l’aide de procédures, et vous pouvez importer vos données métier.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 03/08/2024
ms.custom: bap-template
ms.search.keywords: 'company, setup wizard'
ms.search.form: '1803, 9020, 9022, 9026, 9027, 9030, 9000, 9009, 9004, 9005, 9024, 9006, 9007, 9010, 9016, 9017'
ms.service: dynamics-365-business-central
---
# <a name="create-new-companies-in-"></a>Créer des sociétés dans [!INCLUDE[prod_short](includes/prod_short.md)]

Dans [!INCLUDE[prod_short](includes/prod_short.md)], le conteneur pour les données métier appartenant à une unité commerciale ou une entité juridique sont désignés en tant que *société*. Lorsque vous vous connectez à [!INCLUDE[prod_short](includes/prod_short.md)], une société de démonstration et une société vide vous sont attribuées, *Ma société*. Le basculement entre sociétés est facile : accédez simplement à **Mes paramètres** et passez à l’autre société. Vous pouvez également créer de nouvelles sociétés dans [!INCLUDE[prod_short](includes/prod_short.md)], selon les besoins de votre activité.  

> [!NOTE]
> Pour créer une entreprise, vous devez être affecté à l’ensemble d’autorisations **Super**.

Lorsque vous créez une société, un guide de configuration assistée vous permet d’obtenir les fondements de base. Ensuite, vous pouvez importer des données à partir de votre système hérité ou d’une autre société dans [!INCLUDE[prod_short](includes/prod_short.md)].  

[!INCLUDE [about-ui-learn](includes/about-ui-learn.md)]

## <a name="choose-the-right-template"></a>Choisir le bon modèle

Si vous décidez d’ajouter une société à votre [!INCLUDE[prod_short](includes/prod_short.md)], vous pouvez utiliser le guide de configuration assistée **Créer une nouvelle société** pour démarrer. Le guide de configuration est disponible à partir de la page **Sociétés** et depuis la zone de recherche dans le champ **Société** de la page **Mes paramètres**.  

Le guide de configuration propose trois modèles et une option vierge :

- **Évaluation — Exemples de données**  
    Crée une société qui est similaire à la société de démonstration avec des exemples de données et des données de configuration. Ce type de société est à votre disposition sans passer à une période d’essai de 30 jours, ce qui est le cas des autres types.  
- **Évaluation avancée – Exemples de données complets** Créez une entreprise avec la portée des fonctionnalités avancées, qui dispose de tout ce dont vous avez besoin pour évaluer le produit pour les entreprises dotées de processus avancés. Ce type de société est à votre disposition sans passer à une période d’essai de 30 jours, ce qui est le cas des autres types.
- **Production — Données de configuration uniquement**  
    Créez une société similaire à **Mon entreprise**, avec des données de configuration telles qu’un plan comptable, des modes de paiement et des définitions de rapports financiers, mais sans exemples de données. Vous pouvez utiliser cette société pour une version d’évaluation pendant 30 jours.
- **Créer — Pas de données**  
    Crée une société vide sans données de configuration. Vous pouvez utiliser cette société pour une version d’évaluation pendant 30 jours.  

Si vous souhaitez démarrer facilement avec une nouvelle société, sélectionnez **Production - Données de configuration uniquement**, puis importez vos propres données métier, telles que les clients, les articles et les fournisseurs. Sélectionnez le modèle **Nouveau** si vous souhaitez tout redéfinir à zéro. Dans ce cas, vous pouvez utiliser le guide de configuration assistée **Configuration de la société** pour vous aider à commencer par des données de configuration essentielles.  

> [!NOTE]  
> Lorsque vous créez une société, cela prend quelques minutes avant de pouvoir y accéder dans [!INCLUDE[prod_short](includes/prod_short.md)]. L’état de configuration sur la page **Sociétés** s’affiche lorsque la nouvelle société est prête pour vous. Ensuite, vous pouvez basculer vers la nouvelle société en utilisant **Mes paramètres**.  

Au cours de votre période d’évaluation de 30 jours, vous pouvez créer autant de sociétés que vous voulez, mais elles ne sont disponibles que durant cette période d’évaluation. Pour plus d’informations, contactez votre partenaire [!INCLUDE[prod_short](includes/prod_short.md)]. Voir aussi l’article [FAQ sur la version d’essai Dynamics 365 Business Central](trial-faq.md).  

Votre administrateur peut en savoir plus sur les essais et les abonnements [ici](/dynamics365/business-central/dev-itpro/administration/trials-subscriptions).  

## <a name="copy-a-company"></a>Copier une société

Sur la page **Sociétés**, vous pouvez utiliser l’action **Copier** pour créer une deuxième société sur la base du contenu d’une société existante. La copie de Société est utile, par exemple, lorsque vous souhaitez tester une société sans perturber les données de production.

> [!Important]
> N’utilisez pas l’action Copier pour effectuer une sauvegarde d’une société. Pour effectuer une sauvegarde, commencez par exporter la base de données sous forme de fichier .bacpac. Pour plus d’informations, voir [Exportation de bases de données](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-database-export) dans Aide dédiée au développement et à l’administration.

[!INCLUDE [email-copy-company](includes/email-copy-company.md)]

[!INCLUDE [dataverse-copy-company](includes/dataverse-copy-company.md)]

## <a name="set-up-the-company"></a>Configurer la société

Lorsque vous vous connectez à une nouvelle société, le guide de configuration assistée **Configuration de la société** vous permet de démarrer. Le guide demande vous sera demandé des informations sur votre activité, telles que l’adresse, les coordonnées bancaires et le mode d’évaluation du stock. Ces informations constituent la base de nombreuses zones de [!INCLUDE[prod_short](includes/prod_short.md)] vous n’aurez donc pas à les configurer manuellement.  

Par exemple, [!INCLUDE [prod_short](includes/prod_short.md)] inclut l’adresse de votre entreprise dans les factures et autres documents et vos coordonnées bancaires dans les paiements. Le mode d’évaluation du stock est utilisé pour calculer les prix, ainsi que pour l’évaluation du stock.  

Une fois les bases en place, vous pouvez configurer les zones de base restantes. Maintenant, vous êtes prêt à ajouter des données métier, telles que les clients et les fournisseurs. Pour plus d’informations, consultez [Configurer [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md).  

## <a name="companies-and-environments"></a>Sociétés et environnements

[!INCLUDE [company_environment](includes/company_environment.md)]

Pour plus d’informations, voir [Passer à une autre entreprise ou un autre environnement](ui-organization-switch.md). Pour plus d’informations sur les environnements, voir [Comprendre l’infrastructure de Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-environment-topology) (en anglais uniquement).  

## <a name="changing-a-companys-name"></a>Changer le nom d’une société

Une fois une entreprise créée, vous ne pouvez pas changer son nom. Mais vous pouvez changer son **Nom d'affichage**, qui est le texte qui affiche pour l’entreprise tout au long de l’application.  

> [!TIP]
> Vous pouvez renommer une entreprise si vous utilisez [!INCLUDE[prod_short](includes/prod_short.md)] sur site.

## <a name="add-contoso-coffee"></a>Ajouter Contoso Coffee

L’application Contoso Coffee fournit des données de démonstration pour vous aider à explorer les fonctionnalités avancées de [!INCLUDE [prod_short](includes/prod_short.md)]. Trouvez l’application dans AppSource et installez-la dans une société vide, par exemple une société dans un environnement sandbox. Pour plus d’informations, voir [Présentation des données de démonstration Contoso Coffee](contoso-coffee/contoso-coffee-intro.md).  

## <a name="see-also"></a>Voir aussi

[Personnalisation de Business Central](ui-customizing-overview.md)  
[Configuration de [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Importation des données métier à partir d’autres systèmes financiers](across-import-data-configuration-packages.md)  
[Modifier les paramètres de base](ui-change-basic-settings.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Comprendre l’infrastructure de Business Central Online (en anglais uniquement)](/dynamics365/business-central/dev-itpro/administration/tenant-environment-topology)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
