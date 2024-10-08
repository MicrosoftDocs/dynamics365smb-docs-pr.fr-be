---
title: Explorer et parcourir les pages et les rapports par rôle
description: Vous pouvez obtenir une vue d’ensemble de toutes les fonctionnalités métier disponibles pour votre rôle et pour d’autres rôles.
author: jswymer
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'role explorer, find features, navigate'
ms.search.form: 'RoleExplorer, 9020, 9022, 9027, 9024'
ms.date: 07/15/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---

# <a name="finding-pages-and-reports-with-the-role-explorer"></a>Recherche de pages et états avec l’explorateur de rôles

Vous pouvez obtenir une vue d’ensemble de toutes les fonctionnalités métier disponibles pour votre rôle et pour d’autres rôles si vous allez encore plus loin. Cet article réfère à la fonctionnalité est appelée *explorateur de rôles*.

Chaque élément de l’explorateur de rôles est une action qui ouvre une page ou état. Par conséquent, vous pouvez également utiliser l’explorateur de rôles pour naviguer dans [!INCLUDE[prod_short](includes/prod_short.md)].

[!INCLUDE [about-ui-learn](includes/about-ui-learn.md)]

## <a name="open-the-role-explorer"></a>Ouvrir l’explorateur de rôles

Vous pouvez ouvrir l’explorateur de rôles à partir du Tableau de bord, de toutes les pages de liste et de la fenêtre **La fenêtre de recherche**.

- Sur votre tableau de bord ou sur n’importe quelle page de liste, choisissez le ![bouton Menu.](media/ui_menu_button.png "Bouton Menu") à droite de la barre de navigation ou appuyez sur <kbd>Maj</kbd>+<kbd>F12</kbd>.
- Dans la fenêtre **Tell Me**, choisissez l’action **exploration** en bas.

Lorsque vous ouvrez le tableau de bord des rôles pour la première fois, il affiche des liens vers la plupart des fonctionnalités disponibles pour votre rôle.

## <a name="open-the-role-explorer-filtered-to-show-reports"></a>Ouvrez l’explorateur de rôles filtré pour afficher les rapports

Vous pouvez ouvrir l’explorateur de rôles dans une vue filtrée pour afficher états dans le centre de rôles, de toutes les pages de liste et de la fenêtre **de recherche** :

- Sur votre Tableau de bord ou une page de liste, choisissez le lien **Tous rapports** à droite de la barre de navigation.
- Dans **La fenêtre de recherche**, choisissez l’action **exploration des rapports** en bas.

## <a name="navigate-features"></a>Naviguer dans les fonctionnalités

Les actions qui ouvrent des pages ou états sont organisées sous des nœuds nommés d’après les fonctions ou les domaines d’application. Réduisez ou développé chaque nœud individuellement ou tous les nœuds ensemble.

- Pour développer/réduire un nœud distinct, choisissez-le. Ceci s’applique aux nœuds de niveau supérieur et aux sous-nœuds.
- Pour développer/réduire tous les nœuds de niveau supérieur sur la page, mais laisser les sous-nœuds tels qu’ils sont, choisissez **...** en haut, puis choisissez **Développer** ou **Réduire**.
- Pour développer/réduire tous les nœuds de niveau supérieur et tous les sous-nœuds en-dessous, choisissez **...** en haut, puis choisissez l’action **Développer tout** ou **Réduire tout**.

## <a name="search-for-features"></a>Rechercher des fonctionnalités

Pour localiser rapidement des fonctionnalités, Sélectionner **Rechercher**, puis saisissez un mot ou une expression pour la fonctionnalité que vous essayez de trouver. Le tableau de bord des rôles met en surbrillance tout texte correspondant. Si une fonctionnalité est masquée dans le nœud réduit, le nœud réduit est marqué d’un point. 

## <a name="explore-other-roles"></a>Découvrir d’autres rôles

Pour explorer des rôles autres que le vôtre, sélectionnez **Explorer plus de rôles**. Le tableau de bord des rôles affiche chaque rôle sous son propre titre, avec des liens vers ses fonctionnalités. Vous pouvez ensuite rechercher et naviguer et trouver des fonctionnalités comme vous le faites lorsque vous explorez votre rôle.

> [!NOTE]
> Vous ne verrez que les rôles d'accès configurés pour s’afficher dans l’explorateur de rôles. Si un rôle n’est pas disponible, il n’est probablement pas configuré pour lui. Pour plus d’informations, voir [Gérer les profils](admin-users-profiles-roles.md). 

Lorsque vous explorez d’autres rôles, vous pouvez également affiner l’exploration en utilisant les actions **Rapport et analyse** et **Administration** en haut du tableau de bord des rôles.

- **Rapport et analyse** affiche uniquement les fonctionnalités classées en tant que fonctionnalités d’état et d’analyse.
- **Administration** affiche uniquement les fonctionnalités classées comme fonctionnalités d’administration.

> [!TIP]
> Pour les développeurs, vous catégorisez les pages et les états en définissant la [Propriété UsageCategory](/dynamics365/business-central/dev-itpro/developer/properties/devenv-usagecategory-property) dans le code AL de l’objet.
<!--
 
## <a name="role-explorer-actions"></a>Role explorer actions

There a several actions along the top of the role explorer to help you locate features of your role and other roles.

|Action|Description|
|------|------|
|**All**|Shows all features that are related to the role.|
|**Find**|Lets you enter a word or phrase to quickly locate feature names that match.|
|**Explore more roles**|All business features that are available for all roles including your own. When exploring all roles, the other actions work the same way, except for all roles shown. **NOTE:** You can only access roles that are set up to show in role explorer. For more information, see [Manage Profiles](admin-users-profiles-roles.md).  |
|**Report & Analysis**|This action Shows only those features that are categorized as reports and analysis features.|
|**Administration**|Shows only those features that are categorized as administration features.|



<!--
Choose the **Find** action at the top of the role explorer to quickly locate feature names that contain a certain term.

Choose the **Explore more roles** action at the top of the role explorer to get an overview of all business features that are available for all roles including your own.

> [!NOTE]
> Only Role Center actions for profiles where the **Show in Role Explorer** check box is selected will appear on the extended version of the role explorer (shown with the **Explore more roles** action). For more information, see [Manage Profiles](admin-users-profiles-roles.md).
-->

## <a name="expand-and-collapse-nodes-on-the-role-explorer"></a>Développer et réduire des nœuds dans l’explorateur de rôles

Les actions qui ouvrent des pages sont organisées sous des nœuds nommés d’après les fonctions ou les domaines d’application. Chaque nœud peut être réduit ou développé individuellement et vous pouvez réduire/développer tous les nœuds ensemble.

- Pour développer/réduire un nœud, choisissez-le. Ceci s’applique aux nœuds de niveau supérieur et aux sous-nœuds.
- Pour développer/réduire tous les nœuds de niveau supérieur de la page, choisissez l’action **Développer** ou **Réduire** dans le coin supérieur droit.
- Pour développer/réduire tous les nœuds de niveau supérieur et tous les sous-nœuds en dessous, effectuez l’une des étapes suivantes :
  - Appuyez sur les touches <kbd>Ctrl</kbd>+<kbd>Maj</kbd> pendant que vous choisissez l’action **Développer** ou **Réduire** dans le coin supérieur droit.
  - Choisissez **...** dans le coin supérieur droit, puis choisissez l’action **Développer tout** ou **Réduire tout**.

## <a name="see-also"></a>Voir aussi

[Recherche de pages et d’informations avec la fenêtre de recherche](ui-search.md)  
[Gestion des profils](admin-users-profiles-roles.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
