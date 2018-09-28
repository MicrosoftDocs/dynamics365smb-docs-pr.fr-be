---
title: "Procédure : Configurer les fournisseurs pour les propositions de paiement automatique"
description: "Vous pouvez configurer chaque fournisseur afin que les factures impayées de ce fournisseur soient automatiquement incluses dans les propositions de paiement."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 35406d6af618e4a04aec0ecff23d3a71570e6413
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-vendors-for-automatic-payment-suggestions"></a><span data-ttu-id="5d70c-103">Configurer des fournisseurs pour les propositions de paiement automatique</span><span class="sxs-lookup"><span data-stu-id="5d70c-103">Set Up Vendors for Automatic Payment Suggestions</span></span>
<span data-ttu-id="5d70c-104">Vous pouvez configurer chaque fournisseur afin que les factures impayées de ce fournisseur soient automatiquement incluses dans les propositions de paiement.</span><span class="sxs-lookup"><span data-stu-id="5d70c-104">You can set up each vendor so that unpaid invoices from that vendor are automatically included in payment suggestions.</span></span> <span data-ttu-id="5d70c-105">Pour chaque vendeur, vous devez déterminer si vous souhaitez générer automatiquement des propositions de paiement.</span><span class="sxs-lookup"><span data-stu-id="5d70c-105">For each vendor, you must decide whether you want to automatically generate payment suggestions.</span></span> <span data-ttu-id="5d70c-106">Si vous ne souhaitez pas générer des propositions de paiement pour un fournisseur, ne cochez pas la case **Proposer paiements**.</span><span class="sxs-lookup"><span data-stu-id="5d70c-106">If you do not want to generate payment suggestions for a vendor, you should not select the **Suggest Payments** check box.</span></span> <span data-ttu-id="5d70c-107">Les écritures comptables ouvertes pour ce fournisseur ne seront alors pas incluses dans les propositions de paiement.</span><span class="sxs-lookup"><span data-stu-id="5d70c-107">This way the outstanding ledger entries for the vendor will not be included in payment suggestions.</span></span>  

## <a name="to-set-up-a-vendor-to-be-included-in-the-payment-suggestion-batch"></a><span data-ttu-id="5d70c-108">Pour configurer un fournisseur pour qu'il soit inclus dans le lot de propositions de paiement</span><span class="sxs-lookup"><span data-stu-id="5d70c-108">To set up a vendor to be included in the payment suggestion batch</span></span>  

1.  <span data-ttu-id="5d70c-109">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Fournisseurs**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="5d70c-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5d70c-110">Dans la fenêtre **Fournisseurs**, sélectionnez un fournisseur pertinent, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="5d70c-110">In the **Vendors** window, select a relevant vendor, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="5d70c-111">Dans le raccourci **Paiements**, cochez la case **Proposer paiements**.</span><span class="sxs-lookup"><span data-stu-id="5d70c-111">On the **Payments** FastTab, select the **Suggest Payments** check box.</span></span>  

    <span data-ttu-id="5d70c-112">Si ce champ n'est pas sélectionné, aucune proposition de paiement ne sera générée pour ce fournisseur.</span><span class="sxs-lookup"><span data-stu-id="5d70c-112">If this field is not selected, no payment suggestions will be generated for the vendor.</span></span>  

4.  <span data-ttu-id="5d70c-113">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="5d70c-113">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="5d70c-114">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5d70c-114">See Also</span></span>  
 <span data-ttu-id="5d70c-115">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-115">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="5d70c-116">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-116">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="5d70c-117">[Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-117">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 <span data-ttu-id="5d70c-118">[Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-118">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="5d70c-119">[Générer des propositions de paiement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-119">[Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 <span data-ttu-id="5d70c-120">[Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-120">[Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="5d70c-121">[Tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-121">[Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 <span data-ttu-id="5d70c-122">[Gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md) </span><span class="sxs-lookup"><span data-stu-id="5d70c-122">[Manage Electronic Payment Lines](how-to-manage-electronic-payment-lines.md) </span></span>  
 [<span data-ttu-id="5d70c-123">Imprimer des fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="5d70c-123">Print Payment Files</span></span>](how-to-print-payment-files.md)

