---
title: Définitions de ligne dans Financial Reporting
description: Décrit les définitions de ligne dans les états financiers.
author: kennieNP
ms.author: kepontop
ms.reviewer: bnielse
ms.topic: how-to
ms.date: 03/27/2024
ms.custom: bap-template
ms.search.keywords: 'bi, power BI, analysis, KPI, account schedule, financial report'
ms.search.form: '103, 104, 108, 195, 196, 197, 198, 489, 490, 764, 765, 766'
ms.service: dynamics-365-business-central
---

# <a name="row-definitions-in-financial-reporting"></a>Définitions de ligne dans Financial Reporting

Les définitions de lignes dans les états financiers fournissent un emplacement pour les calculs qui ne peuvent pas être effectués directement dans le plan comptable. Par exemple, vous pouvez créer des sous-totaux pour des groupes de comptes, puis inclure ce total dans d’autres totaux. Vous pouvez également calculer des étapes intermédiaires qui ne sont pas affichées dans le rapport final.

## <a name="create-or-edit-a-row-definition"></a>Créer ou modifier une définition de ligne

Pour créer ou modifier une définition de ligne, procédez comme suit :

1. Sur la page **États financiers**, sélectionnez l’état financier voulu, puis sélectionnez l’action **Modifier la définition de ligne**.
1. Choisissez les action **Insérer des comptes généraux**, **Insérer des comptes CF**, et **Insérer des types de coût** pour créer une ligne pour chaque élément financier que vous souhaitez analyser. Par exemple, vous pouvez avoir une ligne pour les actifs à court terme et une autre ligne pour les immobilisations. Pour avoir de l’inspiration, explorez les états financiers de la société de démonstration CRONUS.

    > [!NOTE]
    > Le champ **N° ligne** affiche les 10 premiers caractères d’un identifiant, par exemple, un numéro de compte. Si vous ajoutez des éléments avec des identifiants qui commencent par les mêmes 10 caractères, vous aurez des doublons dans le champ **N° ligne** . Si nécessaire, vous pouvez modifier manuellement les identifiants après avoir inséré les éléments. Les identifiants complets sont affichés dans le champ **Totalisation**.

> [!NOTE]
> Les colonnes que vous définissez sur chaque ligne de la définition de ligne représentent les colonnes 3 et supérieures de la page **État financier**. Les deux premières colonnes, **N° ligne** et **Description**, sont fixes.  

## <a name="built-in-row-definitions"></a>Définitions de ligne intégrées

[!INCLUDE[prod_short](includes/prod_short.md)] fournit des exemples de définitions de lignes qui peuvent vous aider à démarrer rapidement la configuration de rapports financiers adaptés à vos besoins.

<!-- update this when we release the new templates in 24.1
| Row definition code | Description | How to use this row definition | 
| ------------------- | ----------- | ------------------------------ | 
| TBA 1 | TBA 1 | TBA 1 |
| TBA 2 | TBA 2 | TBA 2 |
| TBA 3 | TBA 3 | TBA 3 |
| TBA 4 | TBA 4 | TBA 4 | 
-->

> [!NOTE]
> Les exemples de rapports financiers présentés dans [!INCLUDE[prod_short](includes/prod_short.md)] ne sont pas prêt à être utilisés directement. En fonction de la façon dont vous configurez vos comptes généraux, vos dimensions, vos catégories de comptes généraux et vos budgets, ajuster les exemples de définitions de lignes et de colonnes ainsi que les rapports financiers qui les utilisent pour correspondre à votre configuration.

## <a name="use-gl-account-categories-to-change-the-layout-of-your-financial-statements"></a>Utiliser les catégories de compte général pour modifier la présentation de vos états financiers

Vous pouvez utiliser les catégories de compte général pour modifier la présentation de vos états financiers. Par exemple, après configuré vos catégories de compte sur la page **Catégories de compte général**, vous pouvez choisir l’action **Générer les états financiers**, et mettre à jour les états financiers sous-jacents pour les états financiers de base. La prochaine fois que vous exécuterez l’un de ces états, par exemple l’état **Relevé de solde**, de nouveaux totaux et des sous-entrées seront ajoutés.

Un autre avantage de l’utilisation des catégories de comptes généraux par rapport aux comptes généraux bruts dans vos définitions de lignes est qu’une modification dans la structure de votre plan comptable n’affecte pas vos rapports financiers.

> [!NOTE]
> Les catégories de compte de niveau supérieur, telles que le nœud **Passif**, sont fixes et vous ne pouvez pas ajouter les vôtres. Cependant, vous pouvez supprimer et ajouter des catégories de compte à des niveaux inférieurs et définir la façon dont l’état financier associé apparaît dans les états.
>
> Il est recommandé de créer et de structurer vos propres catégories de compte général de niveau inférieur à partir de zéro, dans une hiérarchie si nécessaire, plutôt que d’essayer de réorganiser les catégories existantes. Par exemple, vous pouvez restructurer le nœud **Passif** pour contenir un nouveau nœud **Équité** suivi des nœuds **Passif à court terme** et **Passif à long terme**. Pour en savoir plus, consultez [Mappage des comptes du grand livre aux catégories de comptes](finance-general-ledger.md#account-categories).

## <a name="best-practices-for-working-with-row-definitions"></a>Meilleures pratiques pour utiliser les définitions de lignes

Les définitions de lignes ne sont pas versionnées. Lorsque vous modifiez une définition de ligne, l’ancienne version est remplacée lorsque votre modification est enregistrée dans la base de données. La liste suivante contient quelques bonnes pratiques pour utiliser les définitions de lignes :

- Si vous ajoutez des définitions de ligne, choisissez un bon code et remplissez le champ de description avec un texte significatif tout en sachant à quoi vous utilisez la définition de ligne. Ces informations aident vos collègues (et votre futur moi) à travailler avec le Financial Reporting et peut-être à modifier la définition de ligne.
- Avant de modifier une définition de ligne, envisagez d’en faire une copie comme sauvegarde, au cas où votre modification ne fonctionnerait pas comme prévu. Vous pouvez soit simplement copier la définition (lui donner un bon nom), soit l’exporter. Pour en savoir plus, voir [importer ou exporter des définitions de lignes](#import-or-export-financial-reporting-row-definitions).
- Si vous avez besoin d’une nouvelle copie d’une définition [!INCLUDE[prod_short](includes/prod_short.md)] fournie, un moyen simple d’en obtenir une consiste à créer une nouvelle société contenant uniquement des données de configuration. Ensuite, exportez la définition et importez-la dans l’entreprise où la définition doit être actualisée.

## <a name="import-or-export-financial-reporting-row-definitions"></a>Importer ou exporter des définitions de lignes de Financial Reporting

Vous pouvez importer et exporter des définition de lignes comme des packages de configuration RapidStart. Par exemple, les packages de configuration s’avèrent utiles pour le partage d’informations avec d’autres sociétés. Le package est créé dans un fichier .rapidstart, qui compresse le contenu.

> [!NOTE]
> Lorsque vous importez définition de ligne des états financiers, les enregistrements existants portant les mêmes noms que ceux que vous importez sont remplacés par les nouvelles définitions. Le package de configuration d’une définition de rapport n’écrasera aucune définition de ligne ou de colonne existante utilisée dans la définition de rapport.

Pour importer ou exporter des définitions de lignes de rapports financiers, procédez comme suit :

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 4.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Définitions de ligne**, puis sélectionnez le lien associé.
1. Choisissez la définition de ligne, puis choisissez l’action **Importer définition de ligne** ou **Exporter définition de ligne**, selon ce que vous voulez faire.

## <a name="see-also"></a>Voir aussi

[Définitions de colonne dans les états financiers](bi-column-definitions.md)  
[Préparation de l’état financier](bi-how-work-account-schedule.md)  
[Business Intelligence financière](bi.md)  
[Finances](finance.md)  
[Configuration de Finance](finance-setup-finance.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
