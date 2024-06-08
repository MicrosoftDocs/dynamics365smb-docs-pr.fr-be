---
title: Analyse ad hoc des données de ventes
description: Découvrez comment utiliser le mode d’analyse des données pour analyser les données ventes.
author: brentholtorf
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 04/28/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="ad-hoc-analysis-of-sales-data"></a>Analyse ad hoc des données de ventes

Cet article vous apprenez à utiliser fonction **analyse les données** pour analyser des pages de vente directement de liste de pages et requêtes. Vous n’avez pas besoin d’exécuter un rapport ou de passer à une autre application, telle qu’Excel. La fonction fournit un moyen interactif et polyvalent de calculer, résumer et examiner les données. Plutôt que d’exécuter des rapports à l’aide d’options et de filtres, vous pouvez ajouter plusieurs onglets qui représentent différentes tâches ou vues sur les données. Quelques exemples sont "Mes clients" ou "Statistiques vente", ou toute autre vue que vous pouvez imaginer. Pour en savoir plus sur l’utilisation de la fonctionnalité **Analyse des données** , accédez à [Analyser la liste et interroger les données avec le mode d’analyse](analysis-mode.md).

Utilisez les pages de liste suivantes pour une analyse ad hoc des processus de vente :

- [Commandes vente](https://businesscentral.dynamics.com/?page=9305)
- Écritures comptables
- [Écritures comptables client](https://businesscentral.dynamics.com/?page=25)
- Écritures comptables article
- Factures vente validées
- Retours vente

## <a name="sales-ad-hoc-analysis-scenarios"></a>Scénarios d’analyse ad hoc des ventes

Utilisez la fonctionnalité **Analyse des données** pour une vérification rapide des faits et une analyse ad hoc :

- Si vous ne souhaitez pas générer de rapport.
- S’il n’existe pas de rapport correspondant à votre besoin spécifique.
- Si vous souhaitez effectuer une itération rapide pour avoir une bonne vue d’ensemble sur une partie de votre entreprise.

Les sections suivantes fournissent des exemples de scénarios de vente dans [!INCLUDE [prod_short](includes/prod_short.md)].

| Zone | Pour... | Ouvrir cette page en mode analyse | Utiliser ces champs |
| ---- | ----- | ------------------------------- |------------------- |
| [Ventes (volume de ventes prévu)](#example-sales-expected-sales-volume) | Analysez votre volume de ventes attendu. | [Commandes vente](https://businesscentral.dynamics.com/?page=9305) | **Nom du client vendeur**, **Numéro de client vendeur**, **N°** , **Montant**, **Année du document**, et **Document Date Mois**. |
| [Ventes (ventes clients en volume)](#example-sales-customer-sales-by-volume) | Bref aperçu des clients qui achètent le plus et de ceux qui doivent le plus d'argent | [Écritures comptables client](https://businesscentral.dynamics.com/?page=25) | **Nom du client**, **N° de document**, **Montant**, et **Montant restant**. |
| [Finance (Comptabilités client)](#example-finance-accounts-receivables) | Voyez par exemple ce que vos clients vous doivent, décomposé en intervalles de temps pendant lesquels les montants sont dus. | [Écritures comptables client](https://businesscentral.dynamics.com/?page=25) | **Nom du client**, **Date d’échéance**, et **Montant restant**. |

## <a name="example-sales-expected-sales-volume"></a>Exemples : Ventes (volume de ventes prévu)

Pour analyser votre volume de ventes prévu et les montants des ventes pour les commandes non expédiées pour chaque client par année ou par mois, procédez comme suit :

1. Ouvrez le [Commandes vente](https://businesscentral.dynamics.com/?page=9305) liste et activez le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Allumer **Pivot** mode (situé directement au-dessus du **Recherche** champ).
1. Glisser **Nom du client vendeur**, **Numéro de client vendeur**, et **N°** Champs vers le **Groupes de lignes** zone. Faites glisser les champs dans cet ordre.
1. Faites glisser le champ **Montant** champ vers le **Valeurs** zone.
1. Faites glisser le **Année du document** et **Document Date Mois** champs vers le **Étiquettes de colonnes** zone. Faites glisser les champs dans cet ordre.
1. Pour effectuer l’analyse pour une année ou un trimestre donné, appliquez un filtre dans le **Filtres supplémentaires** menu. Le menu se trouve à droite de la page, juste en dessous du **Colonnes** menu.
1. Renommez votre onglet d’analyse en **Volume vente prévu** ou quelque chose qui décrit cette analyse pour vous.

## <a name="example-sales-customer-sales-by-volume"></a>Exemple : Ventes (ventes clients en volume)

Bref aperçu des clients qui achètent le plus et de ceux qui doivent le plus d'argent, comme suit :

1. Ouvrez le [Écritures comptables client](https://businesscentral.dynamics.com/?page=25) liste et activez le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Faites glisser le **Nom du client** champ vers le **Groupes de lignes** zone, et le **Numéro de document** champ en dessous.
1. Choisir la **Montant** et **Montant restant** des champs.
1. Pour effectuer l’analyse pour une année ou un trimestre donné, appliquez un filtre dans le **Filtres supplémentaires** menu. Le menu se trouve à droite de la page, juste en dessous du **Colonnes** menu.
1. Renommez votre onglet d’analyse en **Clients par Volume vente** ou quelque chose qui décrit cette analyse pour vous.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-customer-ledger-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures comptables" lightbox="media/data-analysis-customer-ledger-entries.png":::

## <a name="example-finance-accounts-receivables"></a>Exemple : Finance (Comptabilités client)

Pour voir ce que vos clients vous doivent, décomposé en intervalles de temps pendant lesquels les montants sont dus, comme suit :

1. Ouvrez le [Écritures comptables client](https://businesscentral.dynamics.com/?page=25) liste et activez le mode d’analyse.
1. À la **Colonnes** menu, supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Allumer **Pivot** mode (situé directement au-dessus du **Recherche** champ).
1. Faites glisser le **Nom du client** champ vers le **Groupes de lignes** zone et faites glisser le champ **Montant restant** au **Valeurs** zone.
1. Glisser le **Mois de la date d’échéance** champ vers le **Étiquettes de colonnes** zone.
1. Pour effectuer l’analyse pour une année ou un trimestre donné, appliquez un filtre dans le **Filtres supplémentaires** menu. Le menu se trouve à droite de la page, juste en dessous du **Colonnes** menu.
1. Renommez votre onglet d’analyse en **Comptes âgés par mois** ou quelque chose qui décrit cette analyse pour vous.

## <a name="data-foundation-for-ad-hoc-analysis-on-sales"></a>Base de données pour une analyse ad hoc des ventes

Après entré les informations de la commande de vente et ajouter toutes lignes commande vente vous pouvez la valider commande. Validation crée une expédition et une facture. [!INCLUDE [prod_short](includes/prod_short.md)] mettre à jour le compte, les écritures de paiement, comptabilité :

- Pour chaque commande vente, une écriture vente est créée sur la table **Écriture comptable**. Une écriture est également créée dans le compte client de la table **Écriture comptable client** et une écriture comptable est créée dans le compte client approprié. De plus, la validation de la commande peut avoir pour résultat la création d’une écriture TVA et d’une écriture comptable pour le montant de la remise.
- Pour chaque ligne commande vente, une écriture comptable article est créée dans la table **Écriture comptable article** (si les lignes vente contiennent des numéros des articles) ou une écriture comptable est créée dans la table **Écriture comptable** (si les lignes vente contiennent un compte général). En outre, les commandes vente sont toujours enregistrées dans les tables **En-tête expédition vente** et **En-tête facture vente**.

Pour en savoir plus sur la validation des ventes, consultez [Validation ventes](ui-post-sales.md).

## <a name="see-also"></a>Voir aussi

[Validation des ventes](ui-post-sales.md)  
[Analyse des données de liste et de requête avec le mode d’analyse](analysis-mode.md)  
[Vue d’ensemble de l’analyse vente](sales-analytics-overview.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)  
[Vue d’ensemble des ventes](sales-manage-sales.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
