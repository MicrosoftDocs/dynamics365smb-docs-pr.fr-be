---
title: Analyse ad hoc des données stock
description: Découvrez comment utiliser le mode d’analyse des données pour analyser les données stock.
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 05/03/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Analyse ad hoc des données stock

Cet article vous apprenez à utiliser fonction **analyse les données** pour analyser des pages stock directement de liste de pages et requêtes. Vous n’avez pas besoin d’exécuter un rapport ou de passer à une autre application, telle qu’Excel. La fonction fournit un moyen interactif et polyvalent de calculer, résumer et examiner les données. Plutôt que d’exécuter des rapports à l’aide d’options et de filtres, vous pouvez ajouter plusieurs onglets qui représentent différentes tâches ou vues sur les données. Quelques exemples sont "stock expiration" ou "meilleures vente", ou toute autre vue que vous pouvez imaginer. Pour en savoir plus sur l’utilisation de la fonctionnalité **Analyse des données** , accédez à [Analyser la liste et interroger les données avec le mode d’analyse](analysis-mode.md).

Utilisez les pages de liste suivantes pour une analyse ad hoc des processus de stock :

- [Écritures comptables article](https://businesscentral.dynamics.com/?page=38)

## Scénarios d’analyse ad hoc des stock

Utilisez la fonctionnalité **Analyse des données** pour une vérification rapide des faits et une analyse ad hoc :

- Si vous ne souhaitez pas générer de rapport.
- S’il n’existe pas de rapport correspondant à votre besoin spécifique.
- Si vous souhaitez effectuer une itération rapide pour avoir une bonne vue d’ensemble sur une partie de votre entreprise.

Les sections suivantes fournissent des exemples de scénarios de stock dans [!INCLUDE [prod_short](includes/prod_short.md)].

| Zone | Pour... | Ouvrir cette page en mode analyse | Utiliser ces champs |
| ---- | ----- | ------------------------------- |------------------- |
| [Stock disponible](#example-inventory-on-hand) | Obtenez un aperçu des articles disponibles dans votre inventaire. | [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) | **N° article**, **Quantité restante** |
|[Exemple : suivre les stocks expirés ou anciens](#example-track-expiring-or-old-stock) | Obtenez un aperçu des articles de votre inventaire qui sont en stock depuis longtemps et qui ne se vendent pas bien. | [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) | **Date de publication Année**, **Date de publication Mois**, **N° d’article**, **Date de comptabilisation**, **Type d’entrée**, **Quantité** et **Quantité restante**. |
| [Articles retournés par motif de retour](#example-returned-items-by-return-reason) | Obtenez un aperçu des marchandises que les clients retournent, classées par motif de retour. Utilisez-le pour l’analyse pour le contrôle qualité. | [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) | **Code de motif de retour**, **Date de comptabilisation Mois**, **Quantité** , **Montant du coût**, **Date de comptabilisation**, **Type de document**, **Article n°** et  **Document n°** . |
| Débit d’inventaire | Obtenez un aperçu des achats et des ventes dans votre inventaire par mois ou trimestre. | [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) | **Date de publication Année**, **Date de publication Mois**, **N° d’article**, **Quantité**, **Montant des ventes**, **Montant du coût (réel)**, et **Date de publication Mois** |
| [Mouvements de stock] | Obtenez un aperçu de la façon dont les marchandises de votre inventaire se déplacent entre les emplacements. | [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) | **Code d’emplacement**, **Quantité**, **Date de publication**, **Numéro d’article.** |

## Exemple : Stock disponible

Pour analyser les articles de votre inventaire qui sont en stock, procédez comme suit :

1. Ouvrez le [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Faites glisser le champ **N° article** champ vers le **Groupes lignes** zone. Faites glisser les champs dans cet ordre.
1. Faites glisser le champ **Quantité restante** champ vers le **Valeurs** zone.
1. Définir un **Inégal** filtrer pour **0** sur **Quantité restante**. Si vous n’autorisez pas les niveaux de stock négatifs, définissez un **Plus grand que** filtrer pour **0**.
1. Vous pouvez éventuellement ajouter d’autres champs à l’analyse et peut-être pivoter sur l’emplacement ou sur d’autres champs.
1. Renommez votre onglet d’analyse en **Stock disponible** ou quelque chose qui décrit cette analyse.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-inventory-on-hand.png" alt-text="Exemple de comment effectuer une analyse des données disponibles d’inventaire." lightbox="media/data-analysis-inventory-on-hand.png":::

## Exemple : suivre les stocks expirés ou anciens

Pour analyse des articles de votre inventaire qui sont en stock depuis longtemps et qui ne se vendent pas bien ces étapes :

1. Ouvrez le [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Faites glisser le **Date de publication Année**, **Date de publication Mois** et **Numéro d’article** champs vers le **Groupes de lignes** zone. Faites glisser les champs dans cet ordre.
1. Dans le **Colonnes** zone, choisissez la **Date d’affichage**, **Type d’entrée**, **Quantité**, et **Quantité restante** des champs.
1. Définir un **Moins que** filtrer pour **Date d’affichage** pour définir ce que vous entendez par "ancien".
1. Renommez votre onglet d’analyse en **Stock ancien** ou quelque chose qui décrit cette analyse.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-inventory-dead-stock.png" alt-text="Exemple de comment effectuer une analyse des données de stock vide sur la page des écritures comptables articles" lightbox="media/data-analysis-inventory-dead-stock.png":::

## Exemple : articles retournés par motif de retour

Pour analyser les articles retournés triés par motif de retour, procédez comme suit :

1. Ouvrir [écritures comptables article](https://businesscentral.dynamics.com/?page=38) liste.
1. Pour personnalisant la page, ajouter champ **code motif retour**. Dans le menu **Paramètres** , choisissez **Personnaliser**.
1. Quittez le mode personnalisation.
1. Choisir :::image type="content" source="media/analysis-mode-icon.png" alt-text="Entrer en mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Faites glisser les champs **Code de motif de retour** et **Date de publication Mois** vers les **Groupes de lignes** zone. Faites glisser les champs dans cet ordre.
1. Faites glisser les champs **Quantité** et **Montant du coût** vers les **Valeurs** zone.
1. Ajoutez tous les autres champs de votre choix dans l’analyse et activez-les dans la zone **Colonnes**. Par exemple, vous pouvez ajouter la **Date de publication**, **Type de document**, **N° d’article** et **N° du document** champs.
1. Renommez votre onglet d’analyse en **Articles retournés par motif de retour** ou quelque chose qui décrit cette analyse.  

## Exemple : Débit d’inventaire

1. Ouvrez le [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Allumer **Pivot mode** (situé directement au-dessus du **Recherche** champ droite).
1. Faites glisser le **Date de publication Année**, **Date de publication Mois** et **Numéro d’article** champs vers le **Groupes de lignes** zone.
1. Faites glisser les champs **Quantité**, **Montant vente** et **Montant du coût (réel)** vers les **Valeurs** zone.
1. Glisser le **Mois de la date validation** champ vers le **groupes de colonnes** zone.
1. Renommez votre onglet d’analyse en **Débit stock par mois** ou quelque chose qui décrit cette analyse.  

## Mouvements de stock

Pour suivre les mouvements de stock entre les emplacements, procédez comme suit :

1. Ouvrez le [Écritures comptables article](https://businesscentral.dynamics.com/?page=38) liste et activez :::image type="content" source="media/analysis-mode-icon.png" alt-text="Saisissez le mode d’analyse."::: pour activer le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ à droite).
1. Faites glisser le champ **Code magasin** champ vers le **Groupes lignes** zone.
1. Faites glisser le champ **Quantité** vers le **Valeurs** zone.
1. Ajoutez tous les autres champs de votre choix dans l’analyse et activez-les dans la zone **Colonnes**. Par exemple, vous pouvez ajouter le champ **Numéro d’article** .
1. Renommez votre onglet d’analyse en **Mouvements Stock** ou quelque chose qui décrit cette analyse.  

   > [!TIP]
   > Si vous ajoutez le champ Date comptable, vous pouvez également suivre les mouvements au fil du temps.

## Base de données pour une analyse ad hoc du stock

Lorsqu’une commande vente est validée, [!INCLUDE [prod_short](includes/prod_short.md)] met à jour le compte du client, les écritures comptables et les écritures comptables article.

- Pour chaque ligne de commande client, une écriture comptable d’articles est créée dans la table **Écriture comptable d’articles** (si les lignes de vente contiennent des numéros d’articles). En outre, les commandes vente sont toujours enregistrées dans les tables **En-tête expédition vente** et **En-tête facture vente**. Pour en savoir plus sur la validation des ventes, consultez [Validation ventes](ui-post-sales.md).

Lorsqu’un document achat est validé, [!INCLUDE [prod_short](includes/prod_short.md)] le compte du fournisseur, les écritures comptables, les écritures comptables article et les écritures comptables ressource sont mis à jour.

- Pour chaque ligne d’achat, le cas échéant, des écritures sont créées dans le tableau **Écriture comptable des articles** (si la ligne d’achat est de type Article). En outre, les documents achat sont toujours enregistrés dans les tables **En-tête réception achat** et **En-tête facture achat**. Pour en savoir plus, accédez à [Valider des achats](purchasing-how-record-purchases.md#posting-purchases).

## Voir aussi

[Analyse des données de liste et de requête avec le mode d’analyse](analysis-mode.md)  
[Vue d’ensemble de l’analyse stock](inventory-analytics-overview.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)  
[Vue d’ensemble du stock](inventory-manage-inventory.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]