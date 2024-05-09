---
title: Comprendre la comptabilité et le plan comptable
description: 'Décrit la comptabilité, le plan comptable, et les catégories de compte. Utilisez la page Paramètres comptabilité pour préciser la gestion des problèmes comptables dans votre société.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'analysis, history, track'
ms.search.form: '18, 20, 37, 65, 99, 312, 314, 313, 395, 552, 569, 570, 634, 790, 791, 1158'
ms.date: 04/19/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Comprendre la comptabilité et le plan comptable

La comptabilité (comptes généraux) stocke vos données financières, et le plan comptable (COA) affiche les comptes sur lesquels valider toutes les écritures comptables. [!INCLUDE[prod_short](includes/prod_short.md)] inclut un plan comptable standard prêt à prendre en charge votre société.

## Paramètres comptabilité et paramètres comptabilisation

La configuration des écritures comptables est le composant principal des processus financiers car elle définit comment vous validez les données. Deux pages jouent un rôle particulièrement important dans la configuration de vos processus financiers :  

* **Paramètres comptabilité**
* **Paramètres comptabilisation**

### La page **Paramètres comptabilité**

Utiliser la page **Paramètres comptabilité**, vous spécifiez comment gérer certains problèmes comptables dans votre société, par exemple :  

* Les détails arrondi facture  
* Les formats d’adresse  
* Les états financiers

> [!TIP]
> La page **Paramètres comptabilité** comprend des champs génériques et des champs spécifiques à votre pays ou région. Si vous n’êtes pas sûr de la signification d’un champ, nous vous suggérons de travailler avec votre comptable pour déterminer s’il est pertinent pour votre organisation. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

Pour ouvrir la page maintenant, utilisez le lien suivant [Paramètres comptabilité](https://businesscentral.dynamics.com/?page=118).

### La page **Paramètres comptabilisation**

Utilisez la page **Paramètres comptabilisation** pour configurer des combinaisons de groupes comptabilisation marché et de groupes comptabilisation produits. Les groupes comptabilisation mappent des entités telles que les clients, les fournisseurs, les éléments, les ressources et les documents vente et achat dans des comptes généraux. Saisissez une ligne pour chaque combinaison de groupes comptabilisation marché et de groupes comptabilisation produit. Mais vous pouvez également ouvrir chaque ligne dans sa propre fiche paramètres comptabilisation. Pour plus d’informations, consultez [Configurer les groupes comptabilisation](finance-posting-groups.md).  

> [!TIP]
> Si vous ne pouvez pas voir les champs que vous recherchez sur la page **Paramètres comptabilisation**, utilisez la barre de défilement horizontale au bas de la page pour faire défiler l’affichage vers la droite.  

Pour ouvrir la page maintenant, utilisez le lien suivant [Paramètres comptabilisation](https://businesscentral.dynamics.com/?page=314).

## Le plan comptable

Le **plan comptable** affiche tous les comptes généraux. Vous pouvez effectuer les opérations suivantes à partir du plan comptable :  

* Afficher les états qui affichent les écritures comptables et les soldes.  
* Clôturer votre exercice comptable.  
* Ouvrir la fiche compte général pour ajouter ou modifier des paramètres.  
* Consulter la liste des groupes comptabilisation pour ce compte.
* Afficher les soldes débit et crédit d’un seul compte.

Pour en savoir plus, allez à [Familiarisation avec le plan comptable](finance-chart-of-accounts.md).

## Catégories de compte

Vous pouvez personnaliser la structure de vos états financiers en mappant les comptes généraux aux catégories de comptes.  

La page **Catégories de compte général** affiche vos catégories et sous-catégories et les comptes généraux qui leurs sont affectés. Vous pouvez créer des sous-catégories et affecter ces catégories à des comptes existants.  

Vous pouvez créer un groupe des catégories en effectuant une indentation d’autres sous-catégories sous une ligne de la page **Catégories de compte général**. Les groupes de catégorie facilitent l’obtention d’une vue d’ensemble, car chaque groupement affiche un solde final. Par exemple, vous pouvez créer des sous-catégories pour différents types d’actifs, puis créer des groupes des catégories pour différencier les immobilisations des actifs à court terme, par exemple.  

Vous pouvez définir si des types d’états spécifiques doivent inclure les comptes de chaque sous-catégorie. Les catégories de compte vous aident à définir la présentation de vos états financiers.  

### Exemple :

Par exemple, le solde relevé par défaut solde est doté d’une sous-catégorie pour la *trésorerie* dans *Actifs à court terme*. Si vous souhaitez que le solde relevé tienne compte du fonds de caisse et du compte chèque, vous pouvez donc procéder comme suit :

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Catégories de compte général**, puis choisissez le lien associé.
   1. Sinon, ouvrez la page [ici](https://businesscentral.dynamics.com/?page=790).
2. Choisissez l’action **Modifier la liste**.
3. Ajoutez deux nouvelles sous-catégories : une pour le fonds de caisse, et l’autre pour le compte chèque.
   1. Sélectionnez la catégorie **Actifs à court terme**.
   2. Sélectionnez l’action **Nouveau**.
   3. Entrez le nom de la sous-catégorie dans le champ **Description**.
   4. Dans le champ **Comptes généraux dans une catégorie**, sélectionnez le compte général approprié.
   5. Dans le champ **Définition d’état supplémentaire**, sélectionnez l’option **Comptes de trésorerie**.
4. Effectuer une indentation sous la sous-catégorie **Trésorerie**.
   1. Sélectionnez la sous-catégorie créée à l’étape 3.
   2. Sélectionnez l’action **Indenter**.
   3. Choisissez l’action **Déplacer vers le bas**.
   4. Sélectionnez l’action **Indenter** pour définir une indentation sous la sous-catégorie **Trésorerie**.

Lorsque vous sélectionnez l’action **Générer des états financiers**, ou la prochaine fois que le rapport sera généré, votre relevé de solde affichera les lignes suivantes :

* Solde total en espèces.
* Lignes avec soldes pour le fonds de caisse et le compte courant.  

> [!NOTE]
> Si vous créez un compte général sans affecter de catégorie de compte, lorsque vous affectez le compte à un groupe comptabilisation [!INCLUDE[prod_short](includes/prod_short.md)] attribue automatiquement la catégorie de compte du compte général immédiatement au-dessus du compte dans votre plan comptable. Cependant, pour inclure le nouveau compte dans vos états financiers, vous devez choisir l’action **Générer des états financiers** sur la page **Catégories de compte général**. Vous pouvez également ouvrir la page Fiche Compte général, spécifier la catégorie de compte, puis régénérer votre état financier.

## Accès pour créer et modifier des comptes général et des catégories de comptes

Dans une petite organisation, comme la société de démonstration CRONUS, la plupart des utilisateurs peuvent modifier les entités finance comme Compte général, catégories compte et le plan comptable, à l’exception des utilisateurs disposant d’une licence MEMBRE D’ÉQUIPE. Cependant, les grandes organisations utilisent généralement des rôles et des autorisations d’utilisation pour limiter l’accès pour modifier les entités. Si vous êtes administrateur ou si vous avez le rôle de *Gestionnaire d’activité* ou de *Comptable*, vous pouvez contrôler les autorisations utilisateur pour vous assurer que les bonnes personnes ont accès aux tables pertinentes. Pour plus d’informations, consultez [Pour afficher ou modifier les autorisations d’un utilisateur](ui-define-granular-permissions.md#get-an-overview-of-a-users-permissions).  

## Utilisez des dimensions pour simplifier votre plan comptable

Les axes analytiques sont des valeurs qui permettent de catégoriser les écritures afin de pouvoir les suivre et les analyser sur les documents, tels que les commandes vente. Ils peuvent par exemple indiquer de quel projet ou département provient une écriture. Ainsi, au lieu de configurer des comptes généraux distincts pour chaque service et projet, vous pouvez utiliser les axes analytiques comme base d’analyse et éviter d’avoir à créer un plan comptable compliqué.

Pour en savoir plus sur les axes analytiques, aller [configurer des axes analytiques par défaut pour les clients, les fournisseurs et d’autres comptes](finance-dimensions.md#to-set-up-default-dimensions-for-customers-vendors-and-other-accounts).

## Voir aussi

[Comprendre du plan comptable](finance-chart-of-accounts.md)  
[Utilisation des axes analytiques](finance-dimensions.md)  
[Affectation des autorisations aux utilisateurs et aux groupes](ui-define-granular-permissions.md)  
[Veille économique](bi.md)  
[Finances](finance.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
