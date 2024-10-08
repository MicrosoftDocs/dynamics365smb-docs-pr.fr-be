---
title: Aperçu des tâches permettant de gérer les paiements aux fournisseurs
description: 'Décrit les tâches permettant de gérer les paiements aux fournisseurs ou aux créditeurs, y compris la validation de lignes paiement et d''obtenir un aperçu du solde échu.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: overview
ms.search.keywords: 'print check, vendor payment, creditor, debt, balance due, AP'
ms.search.form: '254, 256, 1190, 1191, 1227, 1228, 1229'
ms.date: 07/15/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="make-payments"></a>Exécution des paiements

Vous effectuez des paiements aux fournisseurs ou aux clients, ou des remboursements aux salariés, en validez les lignes paiement sur la page **Feuille paiement**. La feuille paiement est une feuille comptabilité qui est optimisée pour effectuer les paiements et offre beaucoup d'actions puissantes. Par exemple, le **Suggérer des paiements au fournisseur** action qui recherche les paiements des fournisseurs qui sont dus, et le **Fournisseur – Récapitulatif de l’ancienneté** rapport qui montre un aperçu des paiements fournisseurs dus.  

Vous pouvez lancer le processus de paiement depuis des listes, des fiches, et des écritures comptables pour les fournisseurs, les clients, ainsi que les salariés. Chacune de ces pages a un bouton démarrant le flux de paiement et vous permettant de renseigner la feuille paiement.  

À partir de la feuille de paiements, vous pouvez imprimer des chèques informatiques ou effectuer un enregistrement lorsque les chèques sont rédigés. Si vous sélectionnez **Informatique** dans le champ **Mode émission paiement**, imprimez les lignes représentant des chèques avant de valider les lignes feuille.

Une fois les paiements sont validés, vous pouvez les exporter-vers un fichier bancaire à télécharger vers votre banque pour traitement.

Une fois les paiements effectués au niveau de votre banque, vous devez les lettrer avec les écritures comptables fournisseur ou salarié ouvertes correspondantes. Vous pouvez les lettrer manuellement ou en important un fichier de relevé bancaire et en lettrant les paiements automatiquement. Pour plus d'informations, reportez-vous à [Lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md).

Le tableau suivant décrit une série de tâches et inclut des liens vers les articles qui les décrivent.

| À | Voir |
| --- | --- |
|Comprendre les fonctions de base de la page **Feuille paiement**, qui est basée sur la feuille comptabilité, pour préparer la validation des paiements aux fournisseurs ou employés.|[Utilisation des feuilles comptabilité](ui-work-general-journals.md)|
|Valider les paiements aux fournisseurs ou aux salariés, et les remboursements aux clients et lettrer éventuellement les paiements aux factures/avoirs impayés pour les clôturer comme payés.|[Enregistrer des paiements et des remboursements](payables-how-post-payments-refunds.md)|
| Utiliser une fonction sur la page **Feuille paiement** pour proposer des paiements fournisseur en fonction de critères sélectionnés, tels que la date d'échéance, la possibilité d'escompte et vos liquidités. |[Proposer paiements fournisseur](payables-how-suggest-vendor-payments.md) |
| Émettre des chèques pour les paiements fournisseur ou les remboursements client, sous forme de documents imprimés ou de chèques informatiques. Annuler des chèques avant ou après la validation. |[Effectuer des paiements par chèque](payables-how-work-checks.md) |
|Effectuer des paiements électroniques conformément à la norme de virement SEPA de l'UE.|[Réalisation de paiements avec l’extension AMC Banking 365 Fundamentals ou le virement SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)|
| Payez un fournisseur en liquide ou par chèque et validez le paiement lorsque vous validez la facture. |[Établir rapidement des factures achat](finance-how-to-settle-purchase-invoices-promptly.md) |
| Assurez-vous que la banque efface uniquement les chèques et les montants validés en envoyant un fichier contenant des informations de paiement, du chèque et du fournisseur. |[Exportation du fichier Positive Pay](finance-how-positive-pay.md) |

## <a name="see-also"></a>Voir aussi

[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Achats](purchasing-manage-purchasing.md)  
[Gestion des comptes client](receivables-manage-receivables.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
