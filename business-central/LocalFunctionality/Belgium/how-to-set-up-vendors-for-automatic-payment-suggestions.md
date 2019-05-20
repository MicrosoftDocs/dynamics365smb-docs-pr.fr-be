---
title: Paramétrage des fournisseurs pour des suggestions de règlement automatique
description: Vous pouvez paramétrer chaque fournisseur afin que les factures impayées de ce fournisseur soient automatiquement incluses dans les suggestions de paiement.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 4baec5644de8d60f4c6943bb1529d133f63cd104
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237721"
---
# <a name="set-up-vendors-for-automatic-payment-suggestions"></a><span data-ttu-id="f93f5-103">Paramétrer les fournisseurs pour des suggestions de règlement automatique</span><span class="sxs-lookup"><span data-stu-id="f93f5-103">Set Up Vendors for Automatic Payment Suggestions</span></span>
<span data-ttu-id="f93f5-104">Vous pouvez paramétrer chaque fournisseur afin que les factures impayées de ce fournisseur soient automatiquement incluses dans les suggestions de paiement.</span><span class="sxs-lookup"><span data-stu-id="f93f5-104">You can set up each vendor so that unpaid invoices from that vendor are automatically included in payment suggestions.</span></span> <span data-ttu-id="f93f5-105">Pour chaque fournisseur, vous devez décider si vous souhaitez générer automatiquement des suggestions de paiement.</span><span class="sxs-lookup"><span data-stu-id="f93f5-105">For each vendor, you must decide whether you want to automatically generate payment suggestions.</span></span> <span data-ttu-id="f93f5-106">Si vous ne souhaitez pas générer des suggestions de paiement pour un fournisseur, vous ne devez pas activer la case à cocher **Proposer paiements**.</span><span class="sxs-lookup"><span data-stu-id="f93f5-106">If you do not want to generate payment suggestions for a vendor, you should not select the **Suggest Payments** check box.</span></span> <span data-ttu-id="f93f5-107">Ainsi, les écritures comptables en attente pour le fournisseur ne seront pas incluses dans les suggestions de paiement.</span><span class="sxs-lookup"><span data-stu-id="f93f5-107">This way the outstanding ledger entries for the vendor will not be included in payment suggestions.</span></span>  

## <a name="to-set-up-a-vendor-to-be-included-in-the-payment-suggestion-batch"></a><span data-ttu-id="f93f5-108">Pour paramétrer un fournisseur pour l'inclure dans le traitement par lots de suggestion de paiement</span><span class="sxs-lookup"><span data-stu-id="f93f5-108">To set up a vendor to be included in the payment suggestion batch</span></span>  

1.  <span data-ttu-id="f93f5-109">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="f93f5-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f93f5-110">Dans la page **Fournisseurs**, sélectionnez un fournisseur approprié, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="f93f5-110">On the **Vendors** page, select a relevant vendor, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="f93f5-111">Dans le raccourci **Paiements**, activez la case à cocher **Proposer paiements**.</span><span class="sxs-lookup"><span data-stu-id="f93f5-111">On the **Payments** FastTab, select the **Suggest Payments** check box.</span></span>  

    <span data-ttu-id="f93f5-112">Si ce champ n'est pas sélectionné, aucune suggestion de paiement n'est générée pour le fournisseur.</span><span class="sxs-lookup"><span data-stu-id="f93f5-112">If this field is not selected, no payment suggestions will be generated for the vendor.</span></span>  

4.  <span data-ttu-id="f93f5-113">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="f93f5-113">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f93f5-114">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f93f5-114">See Also</span></span>  
 <span data-ttu-id="f93f5-115">[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-115">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="f93f5-116">[Paiements électroniques, Belgique](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-116">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="f93f5-117">[Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-117">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 <span data-ttu-id="f93f5-118">[Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-118">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="f93f5-119">[Générer des suggestions de règlement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-119">[Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 <span data-ttu-id="f93f5-120">[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-120">[Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="f93f5-121">[Tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-121">[Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 <span data-ttu-id="f93f5-122">[Gérer les lignes de paiement électronique](how-to-manage-electronic-payment-lines.md) </span><span class="sxs-lookup"><span data-stu-id="f93f5-122">[Manage Electronic Payment Lines](how-to-manage-electronic-payment-lines.md) </span></span>  
 [<span data-ttu-id="f93f5-123">Imprimer les fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="f93f5-123">Print Payment Files</span></span>](how-to-print-payment-files.md)
