---
title: "Comment générer des propositions de paiement"
description: "Après avoir créé des transactions bancaires électroniques, vous pouvez commencer à générer des propositions de paiement. Pour cela, utilisez une feuille paiement."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 1c7a748f48cb36b30851795119a072ab6d77c961
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="generate-payment-suggestions"></a><span data-ttu-id="f964d-104">Générer des propositions de paiement</span><span class="sxs-lookup"><span data-stu-id="f964d-104">Generate Payment Suggestions</span></span>
<span data-ttu-id="f964d-105">Après avoir créé des transactions bancaires électroniques, vous pouvez commencer à générer des propositions de paiement.</span><span class="sxs-lookup"><span data-stu-id="f964d-105">After you have set up electronic banking, you can start generating payment suggestions.</span></span> <span data-ttu-id="f964d-106">Vous pouvez le faire dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="f964d-106">You can do this in the payment journal.</span></span>  

## <a name="to-generate-payment-suggestions"></a><span data-ttu-id="f964d-107">Pour générer des propositions de paiement</span><span class="sxs-lookup"><span data-stu-id="f964d-107">To generate payment suggestions</span></span>  

1.  <span data-ttu-id="f964d-108">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles paiement**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="f964d-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f964d-109">Sélectionnez la feuille adéquate, puis choisissez l'action **Proposer paiements fournisseur**.</span><span class="sxs-lookup"><span data-stu-id="f964d-109">Select the appropriate journal batch, and then choose the **Suggest Vendor Payments** action.</span></span>  
3.  <span data-ttu-id="f964d-110">Dans la fenêtre **Proposer paiements fournisseur**, dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="f964d-110">In the **Suggest Vendor Payments EB**  window, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="f964d-111">Champ</span><span class="sxs-lookup"><span data-stu-id="f964d-111">Field</span></span>|<span data-ttu-id="f964d-112">Description</span><span class="sxs-lookup"><span data-stu-id="f964d-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="f964d-113">**Dern. date d'échéance**</span><span class="sxs-lookup"><span data-stu-id="f964d-113">**Last Due Date**</span></span>|<span data-ttu-id="f964d-114">Entrez la dernière date d'échéance qui peut apparaître sur les écritures comptables fournisseur à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f964d-114">Enter the last due date that can appear on the vendor ledger entries to be included in the batch job.</span></span>|  
    |<span data-ttu-id="f964d-115">**Tenir compte des avoirs**</span><span class="sxs-lookup"><span data-stu-id="f964d-115">**Take Credit Memos**</span></span>|<span data-ttu-id="f964d-116">Sélectionnez pour inclure les avoirs restants pour les fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="f964d-116">Select to include outstanding credit memos for vendors.</span></span> <span data-ttu-id="f964d-117">Les avoirs seront soustraits du montant dû.</span><span class="sxs-lookup"><span data-stu-id="f964d-117">The credit memos will be subtracted from the amount due.</span></span> <span data-ttu-id="f964d-118">Lorsque vous sélectionnez des avoirs, la date d'échéance n'est pas utilisée.</span><span class="sxs-lookup"><span data-stu-id="f964d-118">When selecting credit memos, the due date is not used.</span></span>|  
    |<span data-ttu-id="f964d-119">**Obtenir escomptes**</span><span class="sxs-lookup"><span data-stu-id="f964d-119">**Take Payment Discounts**</span></span>|<span data-ttu-id="f964d-120">Sélectionnez pour inclure les écritures comptables fournisseur pour lesquelles vous pouvez obtenir un escompte.</span><span class="sxs-lookup"><span data-stu-id="f964d-120">Select to include vendor ledger entries for which you can receive a payment discount.</span></span>|  
    |<span data-ttu-id="f964d-121">**Date d'escompte**</span><span class="sxs-lookup"><span data-stu-id="f964d-121">**Payment Discount Date**</span></span>|<span data-ttu-id="f964d-122">Entrez la date qui sera utilisée pour calculer un escompte.</span><span class="sxs-lookup"><span data-stu-id="f964d-122">Enter the date that will be used to calculate a payment discount.</span></span>|  
    |<span data-ttu-id="f964d-123">**Montant disponible**</span><span class="sxs-lookup"><span data-stu-id="f964d-123">**Available Amount**</span></span>|<span data-ttu-id="f964d-124">S'il y a un montant maximal disponible pour les paiements, vous pouvez l'entrer ici.</span><span class="sxs-lookup"><span data-stu-id="f964d-124">If there is a maximum amount available for payments, you can enter it here.</span></span> <span data-ttu-id="f964d-125">Le traitement par lots créera alors une proposition de paiement basée sur ce montant et la priorité des fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="f964d-125">The batch job will then create a payment suggestion based on this amount and the priority of vendors.</span></span>|  
    |<span data-ttu-id="f964d-126">**Date comptabilisation**</span><span class="sxs-lookup"><span data-stu-id="f964d-126">**Posting Date**</span></span>|<span data-ttu-id="f964d-127">Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="f964d-127">Enter the date that will appear as the posting date on the lines that the batch job inserts in the payment journal.</span></span>|  

4.  <span data-ttu-id="f964d-128">Dans le raccourci **Fournisseur**, entrez les critères de filtre.</span><span class="sxs-lookup"><span data-stu-id="f964d-128">On the **Vendor** FastTab, enter the filter criteria.</span></span>  
5.  <span data-ttu-id="f964d-129">Cliquez sur le bouton **OK** pour démarrer le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f964d-129">Choose the **OK** button to start the batch job.</span></span>  

<span data-ttu-id="f964d-130">Une fois le traitement par lots terminé, la feuille paiement contient toutes les écritures comptables fournisseur qui correspondent aux filtres.</span><span class="sxs-lookup"><span data-stu-id="f964d-130">When the batch job is finished, the payment journal contains all vendor ledger entries that match the filters.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f964d-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f964d-131">See Also</span></span>  
 <span data-ttu-id="f964d-132">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="f964d-132">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="f964d-133">[Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="f964d-133">[Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="f964d-134">[Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="f964d-134">[Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="f964d-135">[Tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="f964d-135">[Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 <span data-ttu-id="f964d-136">[Gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md) </span><span class="sxs-lookup"><span data-stu-id="f964d-136">[Manage Electronic Payment Lines](how-to-manage-electronic-payment-lines.md) </span></span>  
 [<span data-ttu-id="f964d-137">Imprimer des fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="f964d-137">Print Payment Files</span></span>](how-to-print-payment-files.md)

