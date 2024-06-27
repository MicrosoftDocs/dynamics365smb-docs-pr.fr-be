---
title: Enregistrer les paiements et remboursements dans la feuille paiement
description: Découvrez comment enregistrer les paiements effectués aux fournisseurs et les remboursements effectués aux clients sur la page Feuille paiement.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'payment journal, print check, vendor payment, customer refund, refund check, creditor, debt, balance due, AP'
ms.search.form: '256, 233, 624, 1228'
ms.date: 06/06/2024
ms.service: dynamics-365-business-central
---
# Enregistrer les paiements et remboursements dans la feuille paiement

Sur la page **Feuille paiement**, vous enregistrez les paiements effectués aux fournisseurs et les remboursements effectués aux clients. Lorsque vous validez une ligne feuille paiement, le montant payé est enregistré sur le compte bancaire spécifié. Vous devez ensuite effectuer des actions pour procéder au transfert d’argent réel à partir du compte bancaire associé.  

Les feuilles paiement sont une feuille comptabilité optimisée pour effectuer les paiements. Vous pouvez rapidement ajouter des lignes manuellement, vous pouvez laisser [!INCLUDE[prod_short](includes/prod_short.md)] proposer des paiements fournisseur, et vous pouvez lettrer le paiement dans les documents validés. Bien que vous effectuez des paiements, vous entrez un montant positif dans le champ **Montant du document**. Selon le type de document de la ligne feuille, ce montant est ensuite converti en montant négatif dans les transactions sous-jacentes. Ainsi, il est plus rapide pour vous avez d’ajouter des lignes feuille manuellement. Si vous préférez saisir des montants négatifs, vous pouvez personnaliser la feuille paiement pour afficher le champ **Montant** à la place. Pour en savoir plus sur les pages de personnalisation, accédez à [Commencer à personnaliser en utilisant le mode de personnalisation](ui-personalization-user.md#start-personalizing-by-using-the-personalization-mode).  

- Lettrer des paiements dans des factures ou des avoirs

    Si vous renseignez le champ **N° doc. lettrage** avec la facture ou l’avoir qui doit être payé ou remboursé, le document en question est défini sur **Payé** lorsque vous validez la feuille. Ce paramètre s'appelle « lettré. » Outre le lettrage lors de la validation du paiement, vous pouvez utiliser les pages **Lettrer écritures fournisseur** et **Lettrer écritures client** après avoir validé le paiement. Pou plus d’informations, allez par exemple [Rapprocher des paiements fournisseur avec la feuille paiement ou à partir des écritures comptables fournisseur](payables-how-apply-purchase-transactions-manually.md).  

- Obtenir des suggestions de paiements aux fournisseurs ou aux salariés

    Les actions **Proposer paiements fournisseur** et **Proposer paiements aux salariés** peuvent vous aider à renseigner automatiquement les lignes feuille paiement en fonction de la priorité des fournisseurs et des dates d’échéance. Pour en savoir plus, rendez-vous sur [Suggérer des paiements au fournisseur](payables-how-suggest-vendor-payments.md). Avec cette fonction, le champ **N° doc. lettrage** est toujours renseigné.  

- Imprimer des chèques et envoyer des paiements électroniques à votre banque

    Outre l’enregistrement du paiement, vous pouvez également utiliser la page **Feuille paiement** pour générer le paiement à des fins de traitement par votre banque. Pour plus d’informations, allez [Effectuer des paiements par chèque](payables-how-work-checks.md) et [Effectuer des paiements électroniques](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file).  

## Pour effectuer des paiements dans la feuille paiement

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Feuilles paiement**, puis choisissez le lien associé.
2. Ouvrez la feuille utilisée aux paiements.
3. Si vous savez qui payer, renseignez les champs manuellement. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Pour lettrer également le paiement à la facture ou l’avoir associé, sélectionnez le champ **N° doc. lettrage**, sur la page **Lettrer écritures fournisseur**, sélectionnez la facture ou l’avoir approprié, puis cliquez sur le bouton **OK**.

    De nombreux champs, tels que **Montant du document** et **Date d’échéance**, maintenant contiennent les informations du document sélectionné.
5. Sinon, utilisez la action **Proposer paiements fournisseur**. Tous les montants et informations de lettrage sont également saisis sur les lignes feuille. Pour en savoir plus, rendez-vous sur [Suggérer des paiements au fournisseur](payables-how-suggest-vendor-payments.md).
6. Lorsque toutes les lignes feuille paiement sont renseignées, cliquez sur **Valider**.

## Pour émettre un chèque de remboursement

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Feuilles paiement**, puis sélectionnez le lien associé.
2. Dans le champ **Type document**, sélectionnez **Remboursement**.  
3. Dans le champ **N° de document externe**, entrez référence pour le chèque de remboursement (par exemple, numéro de commande de retour).  
4. Dans le champ **Type compte**, sélectionnez **Client**.  
5. Dans le champ **N° de compte**, sélectionnez le numéro de compte du client auquel le chèque de remboursement est émis.  
6. Dans le champ **Montant**, entrez le total à rembourser.  
7. Dans le champ **Type compte contrepartie**, sélectionnez **Compte bancaire**.  
8. Dans le champ **N° compte contrepartie**, sélectionnez le compte bancaire duquel le chèque est prélevé.  
9. Dans le champ **N° doc. lettrage**, sélectionnez les documents nécessitant un remboursement.  
10. Lorsque toutes les lignes du journal des paiements sont remplies, choisissez l’action **Valider/Imprimer**, puis choisissez l’action **Valider et imprimer** puis **Oui**.  
  
## Voir aussi

[Exécution des paiements par chèque](payables-how-work-checks.md)  
[Désignation des paiements électroniques](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file)  
[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Paramétrage des opérations bancaires](bank-setup-banking.md)  
[Exporter un fichier Positive Pay](finance-how-positive-pay.md)  
[Utiliser des feuilles comptabilité](ui-work-general-journals.md)  
[Personnaliser votre espace de travail](ui-personalization-user.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
