---
title: Définition d’une stratégie de validation des factures pour les utilisateurs
description: Utilisez les stratégies de validation des factures pour contrôler si un utilisateur peut valider des factures de vente et d’achat.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 06/12/2024
ms.custom: bap-template
ms.search.forms: '119, 9807,'
ms.service: dynamics-365-business-central
---

# <a name="define-an-invoice-posting-policy-for-users"></a>Définir une stratégie de validation des factures pour les utilisateurs

Les entreprises ont souvent des processus uniques pour valider les factures de vente et d’achat et les expéditions. Par exemple, les processus peuvent varier d’une personne validant tout sur un bon de commande à plusieurs employés. Vous pouvez empêcher les utilisateurs de valider des factures ou exiger que les factures soient validées avec les expéditions ou les réceptions.

## <a name="to-specify-a-posting-policy"></a>Pour préciser une stratégie de validation

Sur la page **Configuration de l’utilisateur**, dans les champs **Stratégie validation facture vente** et **Stratégie validation facture achat**, choisissez l’une des options suivantes :

* **Autorisé** (Par défaut) : conservez le comportement actuel, où un utilisateur peut choisir l’option de validation à utiliser, comme **Expédier**, **Facturer**, et **Expédier et facturer**. 
* **Interdit** : empêchez l’utilisateur de valider des factures. [!INCLUDE [prod_short](includes/prod_short.md)] affiche une boîte de dialogue de confirmation qui fournit uniquement le **Bateau** et **facture** option.
* **Obligatoire** : autorisez l’utilisateur à valider des factures avec les reçus ou les expéditions. [!INCLUDE [prod_short](includes/prod_short.md)] affiche une boîte de dialogue de confirmation qui propose uniquement les options **Expédier et facturer** ou **Recevoir et facturer**.

## <a name="effect-on-documents"></a>Effet sur les documents

La table suivante décrit comment les stratégies de validation des factures affectent les documents.

> [!NOTE]
> Lorsque vous validez des factures de vente et d’achat et des notes de crédit, vous ne disposez d’aucune option de validation. Les documents présentent toujours les transactions physiques et financières ensemble. Vous ne pouvez pas valider partiellement les factures et les avoirs.

|Document | Option 1 : Autoriser <br>Affiche une série d’options| Option 2 : Interdit <br>Boîte de dialogue de confirmation | Option 3 : obligatoire <br>Boîte de dialogue de confirmation|
|--|--|--|--|
|Commande vente |- Expédier <br>- Facturer <br>- Expédier et facturer |Souhaitez-vous valider l’expédition ? |Souhaitez-vous valider l’expédition et la facture ?|
|Facturation des ventes|Aucune option| La publication est interdite selon la Paramètres utilisateur|Souhaitez-vous valider la facture ?|
|Avoir vente|Aucune option|La publication est interdite selon la Paramètres utilisateur|Souhaitez-vous valider l’avoir ?|
|Retour vente |- Recevoir <br>- Facturer <br>- Réceptionner et facturer |Souhaitez-vous valider cette réception ? |Souhaitez-vous valider la réception et la facture ?|
|Prélèvement de stock |- Expédier <br>- Expédier et facturer |Souhaitez-vous valider l’expédition ? |Souhaitez-vous valider l’expédition et la facture ?|
|Commande achat |- Recevoir <br>- Facturer <br>- Réceptionner et facturer |Souhaitez-vous valider cette réception ? |Souhaitez-vous valider la réception et la facture ?|
|Facture achat|Aucune option|La publication est interdite selon la Paramètres utilisateur|Souhaitez-vous valider la facture ?|
|Avoir achat|Aucune option|La publication est interdite selon la Paramètres utilisateur|Souhaitez-vous valider l’avoir ?|
|Ordre de retour achat |- Expédier <br>- Facturer <br>- Expédier et facturer |Souhaitez-vous valider l’expédition ? |Souhaitez-vous valider l’expédition et la facture ?|
|Rangmt stk invent |- Recevoir <br>- Réceptionner et facturer |Souhaitez-vous valider cette réception ? |Souhaitez-vous valider la réception et la facture ?|
|Expédition entrepôt |- Expédier <br>- Expédier et facturer | Souhaitez-vous valider l’expédition ? |Souhaitez-vous valider l’expédition et la facture ?|

   > [!Note]
   > Le paramètre n’affecte pas la validation des lignes du journal général où vous pouvez sélectionner **Facture** dans le champ **Type de document**.

## <a name="see-also"></a>Voir aussi

[Facturer des ventes](sales-how-invoice-sales.md)  
[Enregistrer les achats avec les factures achat et les commandes](purchasing-how-record-purchases.md)  
[Acheter des articles pour une vente en créant des factures achat](purchasing-how-purchase-products-sale.md)
[Préparation aux activités commerciales](ui-get-ready-business.md)  
