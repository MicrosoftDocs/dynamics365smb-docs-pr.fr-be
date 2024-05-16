---
title: Analyse ad hoc des données financières
description: Découvrez comment utiliser le mode d’analyse des données pour analyser les données finance.
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 05/02/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="ad-hoc-analysis-of-finance-data"></a>Analyse ad hoc des données financières

Cet article vous apprenez à utiliser fonction **analyse les données** pour analyser des pages de finance directement de liste de pages et requêtes. Vous n’avez pas besoin d’exécuter un rapport ou de passer à une autre application, telle qu’Excel. La fonction fournit un moyen interactif et polyvalent de calculer, résumer et examiner les données. Plutôt que d’exécuter des rapports à l’aide d’options et de filtres, vous pouvez ajouter plusieurs onglets qui représentent différentes tâches ou vues sur les données. Quelques exemples sont "Actifs totaux au fil du temps", "Comptes clients", "Comptes fournisseurs" ou toute autre vue que vous pouvez imaginer. Pour en savoir plus sur l’utilisation de la fonctionnalité **Analyse des données** , accédez à [Analyser la liste et interroger les données avec le mode d’analyse](analysis-mode.md).

Utilisez les pages de liste suivantes pour commencer une analyse ad hoc des processus finance :

- [Écritures comptables](https://businesscentral.dynamics.com/?page=20)
- [Écritures comptables client](https://businesscentral.dynamics.com/?page=25)
- [Écritures fournisseur](https://businesscentral.dynamics.com/?page=29)

## <a name="finance-ad-hoc-analysis-scenarios"></a>Scénarios d’analyse ad hoc finance

Utilisez la fonctionnalité **Analyse des données** pour une vérification rapide des faits et une analyse ad hoc :

- Si vous ne souhaitez pas générer de rapport.
- S’il n’existe pas de rapport correspondant à votre besoin spécifique.
- Si vous souhaitez effectuer une itération rapide pour avoir une bonne vue d’ensemble sur une partie de votre entreprise.

Les sections suivantes fournissent des exemples de scénarios de finance dans [!INCLUDE [prod_short](includes/prod_short.md)].

| Zone | Pour... | Ouvrir cette page en mode analyse | Utiliser ces champs |
| ---- | ----- | ------------------------------- |------------------- |
| [Finance (Comptabilité client)](#example-finance-accounts-receivables) | Voyez par exemple ce que vos clients vous doivent, décomposé en intervalles de temps pendant lesquels les montants sont dus. | [Écritures comptables client](https://businesscentral.dynamics.com/?page=25) | **Nom du client**, **Date d’échéance**, et **Montant restant** |
| [Finances (comptabilité fournisseur)](#example-finance-accounts-payable) | Voyez ce que vous devez à vos fournisseurs décomposé en intervalles de temps pendant lesquels les montants sont dus. | [Écritures fournisseur](https://businesscentral.dynamics.com/?page=29) | **Nom du fournisseur**, **Type de document**, **N° du document**, **Année de la date d’échéance**, **Mois de la date d’échéance** et **Montant restant**. |
| [Finance (comptes de gestion)](#example-finance-income-statement) | Consultez vos revenus sur les comptes de revenus à partir des plan comptable, par exemple, décomposés en intervalles de temps pour la comptabilisation des montants. | [Écritures comptables](https://businesscentral.dynamics.com/?page=20) | **N° compte général**, **Date comptabilisation** et **Montant**. |
| [Finance (Actifs total)](#example-finance-total-assets) | Consultez vos actifs sur les comptes de actifs à partir du plan comptable, par exemple, décomposés en intervalles de temps pour la comptabilisation des montants. | [Écritures comptables](https://businesscentral.dynamics.com/?page=20) | **N° compte général**, **Date comptabilisation** et **Montant**. |

### <a name="example-finance-accounts-receivables"></a>Exemple : Finance (Comptabilités client)

Pour voir ce que vos clients vous doivent, décomposé en intervalles de temps pendant lesquels les montants sont dus, comme suit :

1. Ouvrez le [Écritures comptables client](https://businesscentral.dynamics.com/?page=25) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du *Recherche* champ à droite).
1. Allumer **Pivot* mode** (situé directement au-dessus du **Recherche** champ droite).
1. Faites glisser le **Nom du client** champ vers le **Groupes de lignes** zone et faites glisser **Montant restant** au **Valeurs** zone.
1. Glisser le **Mois de la date d’échéance** champ vers le **Étiquettes de colonnes** zone.
1. Pour l’analyse à une année/un trimestre donné, appliquez un filtre dans le **Filtres analyse** menu (à droite page, juste en dessous du **Colonnes** menu).
1. Renommez votre onglet d’analyse en **Comptes âgés par mois** ou quelque chose qui décrit cette analyse.

### <a name="example-finance-accounts-payable"></a>Exemple : Finance (Comptabilités fournisseur)

Pour voir ce que vous devez fournisseur, décomposé en intervalles de temps pendant lesquels les montants sont dus, comme suit :

1. Ouvrez le [Écritures comptables fournisseur](https://businesscentral.dynamics.com/?page=29) liste page et choisir :::image type="content" source="media/analysis-mode-icon.png" alt-text="Entrer le mode d’analyse":::. pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Allumer **Pivot mode** (situé directement au-dessus du **Recherche** champ droite).
1. Faites glisser le **Nom du fournisseur**, **Type de document**, et **Numéro de document** champs vers le **Groupes de lignes** zone, puis faites glisser le **Montant restant** champ vers le **Valeurs** zone.
1. Faites glisser le **Année date dû** et **Mois Date dû** champs vers le **Étiquettes de colonnes** zone. Faites glisser les champs dans cet ordre.
1. Pour l’analyse à une année/un trimestre donné, appliquez un filtre dans le **Filtres analyse** menu (à droite page, juste en dessous du **Colonnes** menu).
1. Renommez votre onglet d’analyse en **Comptes fournisseur âgés par mois** ou quelque chose qui décrit cette analyse.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-vendor-ledger-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures comptables" lightbox="media/data-analysis-vendor-ledger-entries.png":::

### <a name="example-finance-income-statement"></a>Exemple : Finance (comptes de gestion)

Pour consultez vos revenus sur les comptes de revenus à partir du plan comptable décomposés en intervalles de temps pour la comptabilisation des montants comme suit :

1. Ouvrez le [Écritures comptabilité](https://businesscentral.dynamics.com/?page=20) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Allumer **Pivot mode** (situé directement au-dessus du **Recherche** champ droite).
1. Faites glisser le **N° compte général** champ vers le **Groupes de lignes** zone et faites glisser **Montant** au **Valeurs** zone.
1. Glisser le **Mois de la date validation** champ vers le **Étiquettes de colonnes** zone.
1. Pour le compte de résultat, filtrez sur les comptes que vous utilisez. Dans les [!INCLUDE [prod_short](includes/prod_short.md)] données de démonstration, ces comptes commencent par "4", mais votre plan comptable peut être différent. Définissez un filtre sur le comptes appropriés dans le menu **Filtres analyse** (à droite, juste en dessous du menu **Colonnes**).

   > [!TIP]
   > voir quels comptes sont utilisés dans votre configuration, vous exécutez le rapport [Balance générale par période](https://businesscentral.dynamics.com/?report=38).

1. Renommez votre onglet d’analyse en **Revenus par mois** ou quelque chose qui décrit cette analyse.

### <a name="example-finance-total-assets"></a>Exemple : Finance (Actifs total)

Pour consultez vos actifs sur les comptes de actifs à partir du plan comptable décomposés en intervalles de temps pour la comptabilisation des montants comme suit :

1. Ouvrez le [Écritures comptabilité](https://businesscentral.dynamics.com/?page=20) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Allumer **Pivot mode** (situé directement au-dessus du **Recherche** champ droite).
1. Faites glisser le **N° compte général** champ vers le **Groupes de lignes** zone et faites glisser **Montant** au **Valeurs** zone.
1. Glisser le **Mois de la date validation** champ vers le **Étiquettes de colonnes** zone.
1. Pour le relevé du total des actifs, filtrez sur les comptes que vous utilisez. Dans les [!INCLUDE [prod_short](includes/prod_short.md)] données de démonstration, ces comptes commencent par "10", mais votre plan comptable peut être différent. Définissez un filtre sur les comptes appropriés dans le menu **Filtres supplémentaires** (à droite, juste en dessous du menu **Colonnes**).

   > [!TIP]
   > voir quels comptes sont utilisés dans votre configuration, vous exécutez le rapport [Balance générale par période](https://businesscentral.dynamics.com/?report=38).

1. Renommez votre onglet d’analyse en **Revenus par mois** ou quelque chose qui décrit cette analyse.

## <a name="data-foundation-for-ad-hoc-analysis-on-finance"></a>Base de données pour une analyse ad hoc finance

Lorsque vous validez des journaux, [!INCLUDE [prod_short](includes/prod_short.md)] crée des entrées dans le **Écriture comptable** table. Par conséquent, une analyse ad hoc des finances générales est généralement effectuée sur la page [Écriture comptable](https://businesscentral.dynamics.com/?page=20) . Pour les comptes clients et fournisseurs, vous pouvez analyser les [écritures comptables client](https://businesscentral.dynamics.com/?page=25) et [écritures comptables fournisseur](https://businesscentral.dynamics.com/?page=29), respectivement.

Pour en savoir plus, consultez les articles suivants :

- [Base de données pour une analyse ad hoc des ventes](ad-hoc-analysis-sales.md#data-foundation-for-ad-hoc-analysis-on-sales)
- [Base de données pour une analyse ad hoc des achats](ad-hoc-analysis-purchasing.md#data-foundation-for-ad-hoc-analysis-on-purchasing)

## <a name="see-also"></a>Voir aussi

[Analyse des données de liste et de requête avec le mode d’analyse](analysis-mode.md)  
[Présentation des analyses financières](bi.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)  
[Vue d’ensemble de Finance](finance.md)   
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
