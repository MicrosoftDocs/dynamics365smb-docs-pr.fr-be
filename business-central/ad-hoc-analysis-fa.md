---
title: Analyse ad hoc des données Immobilisations
description: Découvrez comment utiliser le mode d’analyse des données dans les données immobilisation.
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '5604, 20'
ms.date: 05/02/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="ad-hoc-analysis-of-fixed-assets-data"></a>Analyse ad hoc des données Immobilisations

Cet article vous apprenez à utiliser fonction **analyse les données** pour analyser des pages de Immobilisations directement de liste de pages et requêtes. Vous n’avez pas besoin d’exécuter un rapport ou de passer à une autre application, telle qu’Excel. La fonction fournit un moyen interactif et polyvalent de calculer, résumer et examiner les données. Plutôt que d’exécuter des rapports à l’aide d’options et de filtres, vous pouvez ajouter plusieurs onglets qui représentent différentes tâches ou vues sur les données. Quelques exemples sont « Actifs totaux », « Amortissement » ou toute autre vue que vous pouvez imaginer. Pour en savoir plus sur l’utilisation de la fonctionnalité **Analyse des données** , accédez à [Analyser la liste et interroger les données avec le mode d’analyse](analysis-mode.md).

Utilisez les pages de liste suivantes pour commencer une analyse ad hoc des processus Immobilisations :

- [Écritures comptables immoblisation](https://businesscentral.dynamics.com/?page=5604)
- [Écritures comptables](https://businesscentral.dynamics.com/?page=20)

## <a name="fixed-assets-ad-hoc-analysis-scenarios"></a>Scénarios analyse ad hoc des Immobilisations

Utilisez la fonctionnalité **Analyse des données** pour une vérification rapide des faits et une analyse ad hoc :

- Si vous ne souhaitez pas générer de rapport.
- S’il n’existe pas de rapport correspondant à votre besoin spécifique.
- Si vous souhaitez effectuer une itération rapide pour avoir une bonne vue d’ensemble sur une partie de votre entreprise.

Les sections suivantes fournissent des exemples de scénarios de Immobilisations dans [!INCLUDE [prod_short](includes/prod_short.md)].

| Zone | Pour... | Ouvrir cette page en mode analyse | Utiliser ces champs |
| ---- | ----- | ------------------------------- |------------------- |
| [Immobilisations (valeur actuelle)](#example-fixed-assets-current-value) | Suivez la valeur des actifs, à la fois sur tous les actifs et sur un seul actif. | [Écritures comptables immoblisation](https://businesscentral.dynamics.com/?page=5604) | **Livre d’amortissement**, **N° immo.**, **Date de comptabilisation FA**, **Type compta. immo.** et **Montant** |
| [La valeur des actifs change au fil du temps](#example-asset-value-changes-over-time) | Suivez les modifications de valeur des actifs au fil du temps. | [Écritures comptables immoblisation](https://businesscentral.dynamics.com/?page=5604) | **Type compta. immo.**, **Date de publication immo.** et **Montant** |
|[Amortissements des immobilisations au fil du temps](#example-fixed-asset-depreciations-over-time) | Suivez les Amortissement au fil du temps, à la fois sur tous les actifs et sur un seul actif. | [Écritures comptables immoblisation](https://businesscentral.dynamics.com/?page=5604) | **Livre d’amortissement**, **N° immo.**, **exercice de comptabilisation FA**, **Mois de comptabilisation FA**, **Montant** et **Type compta. immo.** |

### <a name="example-fixed-assets-current-value"></a>Exemple: valeur actuelle Immobilisations

Pour suivre la valeur d’une ou plusieurs immobilisations, procédez comme suit :

1. Ouvrez le [Écritures comptables immobilisation](https://businesscentral.dynamics.com/?page=5604) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Faites glisser les champs **Loi d’amortissement** et **N° immo.** vers les **Groupes de lignes** zone.
1. Choisissez les champs **Date de publication immo.** et **Type compta. immo.** .
1. Faites glisser **Montant** champ vers le **Valeurs** zone.
1. Renommez votre onglet d’analyse en **Vue d’ensemble des immobilisations – valeur** ou quelque chose qui décrit cette analyse.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png" alt-text="Exemple de comment effectuer une analyse de données sur la page Écritures comptables immobilisation pour voir la valeur d’un actif." lightbox="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png":::

### <a name="example-asset-value-changes-over-time"></a>Exemple : la valeur des actifs change au fil du temps

Pour suivre les changements de valeur des actifs au fil du temps, procédez comme suit :

1. Ouvrez le [Écritures comptables immobilisation](https://businesscentral.dynamics.com/?page=5604) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Allumer **Pivot mode** (situé directement au-dessus du **Recherche** champ droite).
1. Faites glisser le champ **Type compta. immo.** vers la zone **Groupes de lignes**.
1. Faites glisser le **exercice compta. immo.** et **Mois compta. immo.** champs vers le **Étiquettes de colonnes** zone.
1. Faites glisser **Montant** champ vers le **Valeurs** zone.
1. Renommez votre onglet d’analyse en **Changements de la valeur d’actifs au fil du temps** ou quelque chose qui décrit cette analyse.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-fa-ledger-entries-asset-changes-over-time.png" alt-text="Exemple de comment effectuer une analyse de données sur la page Écritures comptables immobilisation pour voir les changements de la valeur des actifs au fil du temps." lightbox="media/data-analysis-fa-ledger-entries-asset-changes-over-time.png":::

### <a name="example-fixed-asset-depreciations-over-time"></a>Exemple : amortissements des immobilisations au fil du temps

Pour suivre l’Amortissement d’une ou plusieurs immobilisations, procédez comme suit :

1. Ouvrez le [Écritures comptables immobilisation](https://businesscentral.dynamics.com/?page=5604) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Allumer **Pivot mode** (situé directement au-dessus du **Recherche** champ droite).
1. Faites glisser les champs **Loi d’amortissement** et **N° immo.** vers les **Groupes de lignes** zone.
1. Faites glisser le **exercice compta. immo.** et **Mois compta. immo.** champs vers le **Étiquettes de colonnes** zone.
1. Faites glisser **Montant** champ vers le **Valeurs** zone.
1. Dans le champ filtre **Type compta. immo**, sélectionnez **Amortissement**.
1. Renommez votre onglet d’analyse en **Amortissements fil du temps** ou quelque chose qui décrit cette analyse.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-fa-ledger-entries-depreciation-by-asset.png" alt-text="Exemple de comment effectuer une analyse de données sur la page Écritures comptables immobilisation pour voir l’Amortissement fil du temps." lightbox="media/data-analysis-fa-ledger-entries-depreciation-by-asset.png":::

## <a name="data-foundation-for-ad-hoc-analysis-on-fixed-assets"></a>Base de données pour une analyse ad hoc des immobilisations

Lorsque vous validez des journaux immobilisations, [!INCLUDE [prod_short](includes/prod_short.md)] crée des entrées dans le **Écriture immobilisation** table. Par conséquent, une analyse ad hoc des Immobilisations est généralement effectuée sur la page [Écritures comptables immobilisation](https://businesscentral.dynamics.com/?page=5604) .

## <a name="contributors"></a>Contributeurs

*Microsoft maintient cet article. Certaines parties des exemples ont été initialement écrites par le contributeur suivant.*

* [Aldona Stec](https://www.linkedin.com/in/aldona-stec-25283bb1) | [!INCLUDE[prod_short](includes/prod_short.md)] Consultante

## <a name="see-also"></a>Voir aussi

[Analyse des données de liste et de requête avec le mode d’analyse](analysis-mode.md)  
[Vue d’ensemble de l’analyse des immobilisations](fa-analytics-overview.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)  
[Vue d’ensemble des immobilisations](fa-manage.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
