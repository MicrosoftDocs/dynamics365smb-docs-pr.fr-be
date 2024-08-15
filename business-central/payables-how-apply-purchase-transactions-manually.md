---
title: Rapprocher les reçus de paiement fournisseur ou les remboursements dans la feuille paiement
description: 'Pour traiter, mettre en correspondance, ou rapprocher des paiements ou des remboursements fournisseur manuellement, vous lettrez le montant dans une ou plusieurs écritures comptables fournisseur ouvertes.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'payment application, payment processing, match payments'
ms.search.form: '62, 233, 522, 623'
ms.date: 07/19/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# Rapprocher les paiements des fournisseurs avec le journal des paiements ou à partir des écritures du grand livre des fournisseurs
Lorsque vous envoyez un règlement à un fournisseur ou recevez un remboursement de sa part, vous devez décider si vous souhaitez lettrer le paiement ou le remboursement avec une ou plusieurs écritures ouvertes. Vous pouvez indiquer le montant exact que vous souhaitez lettrer avec la réception paiement ou le remboursement, puis ne lettrer que partiellement les écritures comptables fournisseur. Vous devez lettrer toutes les écritures comptables fournisseur pour obtenir des statistiques fournisseur et des rapports corrects des états financiers et des intérêts de retard.

> [!NOTE]  
>   Les fournisseurs préfèrent parfois procéder à un remboursement plutôt que de créer un avoir déductible des prochaines factures, notamment si vous renvoyez des articles que vous avez déjà payés ou si vous avez versé un montant trop élevé pour une facture.

Vous pouvez lettrer les écritures comptables fournisseur de trois manières différentes :

* En saisissant des informations dans des pages dédiées, telles que la page **Journaux de paiement** et la page **Journaux de rapprochement des paiements** .
* À partir des documents avoir achat.
* À partir des écritures comptables fournisseur une fois que les documents achat sont validés mais non lettrés.

> [!NOTE]  
>   Si le champ **Mode de lettrage** de la fiche fournisseur contient **Au plus ancien**, les paiements sont automatiquement lettrés avec l'écriture de crédit ouverte la plus ancienne si vous ne spécifiez pas avec quelle écriture lettrer. Si le mode de lettrage pour un client est **Manuel**, vous devez lettrer les écritures manuellement.

Vous pouvez appliquer manuellement les paiements des fournisseurs à leurs documents d’achat associés lorsque vous enregistrez les paiements sur la page **Journaux des paiements** . Pour plus d'informations sur comment renseigner la feuille paiement, reportez-vous à [Effectuer des paiements](payables-make-payments.md).

Vous pouvez également lettrer des paiements fournisseur et des paiements client après que les paiements apparaissent en tant que des transactions bancaires négatives au niveau de votre banque. Sur la page **Journaux de rapprochement des paiements**, vous pouvez utiliser les fonctions d’importation de relevés bancaires, d’application automatique et de rapprochement de comptes bancaires. Pour plus d'informations, voir [Rapprocher les paiements à l'aide du lettrage automatique](receivables-how-reconcile-payments-auto-application.md).

## Pour lettrer un paiement à une seule ou à plusieurs écritures comptable fournisseur
1. Choisissez l’![icône en forme d’ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles paiement**, puis choisissez le lien associé.
2. Sur la page **Journaux de paiement**, sur la première ligne de journal, saisissez les informations pertinentes sur l’écriture de paiement.
3. Pour lettrer une seule écriture comptable fournisseur :
   1. Dans le champ **N° doc. lettrage**, sélectionnez le champ permettant d'ouvrir la page **Lettrer écritures fournisseur**.
   2. Sur la page **Lettrer écritures fournisseur**, sélectionnez l'écriture à laquelle lettrer le paiement.
   3. Sur la ligne du champ **Montant à lettrer**, entrez le montant à lettrer à l'écriture.
4. Ou, pour lettrer plusieurs écritures comptables fournisseur :

   1. Sélectionnez l'action **Lettrer écritures**.
   2. Sur la page **Lettrer écritures fournisseur**, sélectionnez les lignes contenant les écritures auxquelles lettrer le paiement.
   3. Sélectionnez l'action **Définir ID lettrage**.  
   4. Sur chaque ligne du champ **Montant à lettrer**, entrez le montant à lettrer à l'écriture.

      Si vous ne saisissez pas de montant, le montant maximum est automatiquement appliqué. Au bas de la page **Lettrer écritures fournisseur**, vous voyez le montant dans le champ Montant lettré et vous constatez si le lettrage est équilibré.
5. Cliquez sur le bouton **OK**.
6. Sélectionnez l'action **Valider** pour valider la feuille paiement.

## Pour lettrer un avoir à une seule ou à plusieurs écritures comptables fournisseur
1. Sélectionnez l’![icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Avoirs achat**, puis sélectionnez le lien associé.
2. Ouvrez l'avoir à lettrer.
3. Entrez les informations nécessaires dans l'en-tête.
4. Pour lettrer une seule écriture comptable fournisseur, dans le raccourci **Lettrage**, dans le champ **N° doc. lettrage**, sélectionnez l'écriture sur laquelle lettrer le crédit puis, dans le champ **Montant à lettrer**, entrez le montant à lettrer sur l'écriture.
5. Ou, pour lettrer plusieurs écritures comptables fournisseur :

   1. Sélectionnez l'action **Lettrer écritures**.
   2. Sélectionnez les lignes contenant les écritures auxquelles lettrer l'avoir.
   3. Sélectionnez l'action **Définir ID lettrage**.  
   4. Sur chaque ligne du champ **Montant à lettrer**, entrez le montant à lettrer à l'écriture.

       Si vous ne saisissez pas de montant, le montant maximum est automatiquement appliqué. Au bas de la page **Lettrer écritures fournisseur**, vous voyez le montant dans le champ **Montant lettré** et vous constatez si le lettrage est équilibré.
6. Cliquez sur le bouton **OK**.  
   La page  **Avoirs d’achat** affiche l’entrée que vous avez sélectionnée dans le champ  **Type de document applicable** et le champ  **N° de document applicable** . La page affiche également le montant de l'avoir à valider, escomptes éventuels déduits.
7. Cliquez sur le bouton **Valider** pour valider l'avoir achat.

## Pour lettrer des écritures comptables fournisseur validées
1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Fournisseurs**, puis choisissez le lien associé.
2. Ouvrez le fournisseur approprié possédant des écritures déjà validées.
3. Sélectionnez l'action **Écritures comptables**, puis sélectionnez l'action **Lettrer écritures**.
4. Sur la page **Lettrer écritures fournisseur**, les écritures ouvertes de ce fournisseur s'affichent.
5. Sélectionnez la ligne où figure l'écriture qui sera lettrée.
6. Sélectionnez l'action **Définir ID lettrage**.

    Le champ **ID lettrage** affiche trois astérisques si vous travaillez dans un système mono-utilisateur ou votre code utilisateur si vous travaillez dans un système multi-utilisateur.  
7. Pour chaque ligne du champ **Montant à lettrer**, entrez le montant à lettrer à l'écriture.

    Si vous ne saisissez pas de montant, le montant maximum est automatiquement appliqué. Vous pouvez voir le montant dans le champ **Montant lettré** au bas de la page **Lettrer écritures fournisseur**.
8. Sélectionnez l'action **Valider le lettrage**.  

    La page **Valider le lettrage** s'ouvre avec le numéro de document de l'écriture lettrage et la date comptabilisation de l'écriture ayant la date comptabilisation la plus récente.
9. Cliquez sur **OK** pour valider le lettrage.

## Pour lettrer des écritures comptables fournisseur en devises différentes les unes avec les autres
Si vous achetez des produits auprès d'un fournisseur dans une devise et que vous effectuez le paiement dans une autre devise, vous pouvez tout de même lettrer la facture avec le paiement.

Si vous lettrez une écriture (Écriture 1) dans une devise avec une autre écriture (Écriture 2) dont la devise est différente, la date de comptabilisation de l'Écriture 1 est utilisée pour trouver le taux de change adéquat et convertir les montants de l'Écriture 2. Le taux de change approprié se trouve sur la page **Taux de change devise**. Dans ce cas, vous devez activer le lettrage d'écritures comptables fournisseur en devises différentes. Pour plus d'informations, voir [Activer le lettrage d'écritures comptables client en devises différentes](finance-how-enable-application-ledger-entries-different-currencies.md)

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles paiement**, puis choisissez le lien associé.
2. Ouvrez la feuille que vous souhaitez, puis renseignez la première ligne vide de la feuille à l'aide d'un code devise.
3. Sélectionnez l'action **Lettrer écritures**.
4. Sélectionnez la ligne comportant l'écriture à lettrer avec l'écriture de la feuille paiement. Sélectionnez ensuite l'action **Définir ID lettrage**, puis sélectionnez l'écriture sur laquelle le lettrage doit être effectué.
5. Cliquez sur le bouton **OK** pour revenir à la feuille de paiement.
6. Validez la feuille paiement.

> [!IMPORTANT]  
>   Lorsque vous lettrez des écritures les unes aux autres en devises différentes, les écritures sont converties en USD. Bien que le taux de change des deux devises concernées soit fixe, comme entre le USD et l'EUR, la conversion de ces montants en devise en une somme en USD peut donner un petit montant résiduel. Le programme valide ces petits montants résiduels en tant que gains et pertes dans le compte défini dans les champs **Cpte gains constatés report** ou **Cpte pertes constatées report** de la page **Devises**. La valeur du champ **Montant (USD)** est également ajustée sur les écritures comptables fournisseur concernées.

## Pour délettrer un lettrage des écritures fournisseur
Lorsque vous annulez une application erronée, des entrées de correction identiques à l’entrée d’origine mais avec un logarithme opposé dans le champ du montant sont créées et comptabilisées pour toutes les entrées, y compris toutes les écritures comptabilité dérivées de l’application, telles que les escomptes de paiement et les gains/pertes de change. Les écritures qui sont fermées par l'application sont rouvertes.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Fournisseurs**, puis choisissez le lien associé.
2. Ouvrez la fiche fournisseur appropriée.
3. Sélectionnez l'action **Écritures comptables**.
4. Sélectionnez l'écriture comptable appropriée, puis sélectionnez l'action **Délettrer les écritures**.
5. Sinon, sélectionnez l'action **Écritures comptables détaillées**.
6. Sélectionnez l'écriture de lettrage appropriée, puis sélectionnez l'action **Délettrer les écritures**.
7. Renseignez les champs de l'en-tête, puis sélectionnez l'action **Délettrer**.

> [!IMPORTANT]  
>   Si une écriture a été lettrée par plusieurs écritures lettrage, vous devez commencer par délettrer la dernière écriture lettrage.

## Voir aussi
[Fournisseurs](payables-manage-payables.md)  
[Achats](purchasing-manage-purchasing.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]