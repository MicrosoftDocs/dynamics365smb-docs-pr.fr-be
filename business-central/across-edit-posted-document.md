---
title: Modifier les documents vente et achat validés
description: Cette rubrique explique comment mettre à jour les informations sur un document publié comme une expédition de vente ou une facture d’achat lorsque des informations pertinentes ont changé.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.reviewer: bholtorf
ms.search.keywords: 'Posted document, editable, posted sales shipment, posted purchase invoice, posted return shipment, posted return receipt, Business Central, business document'
ms.search.form: '130, 138, 142, 146, 6660, 6662, 6650, 6652'
ms.date: 06/10/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="edit-posted-documents"></a>Valider les documents validés

Parfois, vous devez mettre à jour un document validé, car les informations pertinentes pour le document ont été modifiées. Sur un document de vente validé, il peut s'agir du numéro de suivi du colis du transporteur, par exemple. Sur un document d'achat validé, il peut s'agir d'un texte de référence de paiement.

Vous effectuez la modification sur une version modifiable du document d'origine, indiquée par «  **- Mettre à jour** » dans le titre de la page. La page contient un sous-ensemble des champs sur le document d'origine, dont certains sont des champs non modifiables affichés uniquement à titre d'information.

La fonctionnalité est disponible pour les documents suivants dans tous les marchés pris en charge :

- Expédition vente validée
- Facture achat enregistrée
- Expédition retour validée
- Réceptions retour enregistrées

Les documents supplémentaires suivants peuvent être modifiés dans les pays ou régions spécifiés :

- ES : facture vente enregistrée, avoir vente enregistré, avoir achat validé
- APAC : avoir vente enregistré, avoir achat validé
- RU : avoir vente enregistré
- IT : expédition de transfert validée, expédition de service validée

## <a name="to-edit-a-posted-sales-shipment"></a>Pour modifier une expédition vente enregistrée

Ce qui suit explique comment modifier une expédition vente enregistrée Les étapes sont similaires pour les autres documents pris en charge.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Expéditions vente enreg.**, puis sélectionnez le lien associé.
2. Sélectionnez le document que vous souhaitez modifier, puis sélectionnez l'action **Mettre à jour le document**. Sinon, ouvrez le document, puis choisissez l'action.
3. Sur la page **Expédition vente enregistrée - Mettre à jour**, modifiez le champ **N° de suivi du colis** par exemple.
4. Cliquez sur le bouton **OK**.

L'expédition vente enregistrée est mise à jour.

## <a name="see-also"></a>Voir aussi

[Validation des documents et des feuilles](ui-post-documents-journals.md)  
[Recherche des écritures associées aux documents](ui-find-entries.md)  
[Achats](purchasing-manage-purchasing.md)  
[Fonctionnalités marché](ui-across-business-areas.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
