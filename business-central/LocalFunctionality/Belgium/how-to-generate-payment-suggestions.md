---
title: Génération des suggestions de règlement
description: Après avoir configuré les opérations bancaires électroniques, vous pouvez commencer à générer des suggestions de règlement. Pour cela, utilisez la feuille paiement.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: d656ea8d17ce8ad42351d4072075e8348e2ad1b8
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/08/2019
ms.locfileid: "826486"
---
# <a name="generate-payment-suggestions"></a><span data-ttu-id="5268d-104">Générer des suggestions de règlement</span><span class="sxs-lookup"><span data-stu-id="5268d-104">Generate Payment Suggestions</span></span>
<span data-ttu-id="5268d-105">Après avoir configuré les opérations bancaires électroniques, vous pouvez commencer à générer des suggestions de règlement.</span><span class="sxs-lookup"><span data-stu-id="5268d-105">After you have set up electronic banking, you can start generating payment suggestions.</span></span> <span data-ttu-id="5268d-106">Pour cela, utilisez la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="5268d-106">You can do this in the payment journal.</span></span>  

## <a name="to-generate-payment-suggestions"></a><span data-ttu-id="5268d-107">Pour générer des suggestions de règlement</span><span class="sxs-lookup"><span data-stu-id="5268d-107">To generate payment suggestions</span></span>  

1.  <span data-ttu-id="5268d-108">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles paiement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="5268d-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5268d-109">Sélectionnez la feuille appropriée, puis choisissez l'action **Proposer paiements fournisseur**.</span><span class="sxs-lookup"><span data-stu-id="5268d-109">Select the appropriate journal batch, and then choose the **Suggest Vendor Payments** action.</span></span>  
3.  <span data-ttu-id="5268d-110">Dans la page **Proposer paiements fournisseur**, dans le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5268d-110">In the **Suggest Vendor Payments EB**  page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5268d-111">Champ</span><span class="sxs-lookup"><span data-stu-id="5268d-111">Field</span></span>|<span data-ttu-id="5268d-112">Désignation</span><span class="sxs-lookup"><span data-stu-id="5268d-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5268d-113">**Dernière date d'échéance**</span><span class="sxs-lookup"><span data-stu-id="5268d-113">**Last Due Date**</span></span>|<span data-ttu-id="5268d-114">Entrez la dernière date d'échéance qui peut s'afficher sur les écritures comptables fournisseur à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="5268d-114">Enter the last due date that can appear on the vendor ledger entries to be included in the batch job.</span></span>|  
    |<span data-ttu-id="5268d-115">**Accepter les avoirs**</span><span class="sxs-lookup"><span data-stu-id="5268d-115">**Take Credit Memos**</span></span>|<span data-ttu-id="5268d-116">Sélectionnez ce champ pour inclure les avoirs en attente pour les fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="5268d-116">Select to include outstanding credit memos for vendors.</span></span> <span data-ttu-id="5268d-117">Les avoirs sont soustraits du montant dû.</span><span class="sxs-lookup"><span data-stu-id="5268d-117">The credit memos will be subtracted from the amount due.</span></span> <span data-ttu-id="5268d-118">Lorsque vous sélectionnez des avoirs, la date d'échéance n'est pas utilisée.</span><span class="sxs-lookup"><span data-stu-id="5268d-118">When selecting credit memos, the due date is not used.</span></span>|  
    |<span data-ttu-id="5268d-119">**Accepter les escomptes**</span><span class="sxs-lookup"><span data-stu-id="5268d-119">**Take Payment Discounts**</span></span>|<span data-ttu-id="5268d-120">Sélectionnez ce champ pour inclure les écritures comptables fournisseur pour lesquelles vous pouvez obtenir un escompte.</span><span class="sxs-lookup"><span data-stu-id="5268d-120">Select to include vendor ledger entries for which you can receive a payment discount.</span></span>|  
    |<span data-ttu-id="5268d-121">**Date d'escompte**</span><span class="sxs-lookup"><span data-stu-id="5268d-121">**Payment Discount Date**</span></span>|<span data-ttu-id="5268d-122">Entrez la date qui est utilisée pour calculer un escompte.</span><span class="sxs-lookup"><span data-stu-id="5268d-122">Enter the date that will be used to calculate a payment discount.</span></span>|  
    |<span data-ttu-id="5268d-123">**Montant disponible**</span><span class="sxs-lookup"><span data-stu-id="5268d-123">**Available Amount**</span></span>|<span data-ttu-id="5268d-124">S'il y a un montant maximal disponible pour les paiements, vous pouvez le saisir ici.</span><span class="sxs-lookup"><span data-stu-id="5268d-124">If there is a maximum amount available for payments, you can enter it here.</span></span> <span data-ttu-id="5268d-125">Le traitement par lots crée ensuite une suggestion de paiement sur la base de ce montant et de la priorité des fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="5268d-125">The batch job will then create a payment suggestion based on this amount and the priority of vendors.</span></span>|  
    |<span data-ttu-id="5268d-126">**Date de validation**</span><span class="sxs-lookup"><span data-stu-id="5268d-126">**Posting Date**</span></span>|<span data-ttu-id="5268d-127">Saisissez la date qui s'affiche comme date comptabilisation sur les lignes que le traitement par lots insère dans la feuille paiements.</span><span class="sxs-lookup"><span data-stu-id="5268d-127">Enter the date that will appear as the posting date on the lines that the batch job inserts in the payment journal.</span></span>|  

4.  <span data-ttu-id="5268d-128">Dans le raccourci **Fournisseur**, entrez les critères du filtre.</span><span class="sxs-lookup"><span data-stu-id="5268d-128">On the **Vendor** FastTab, enter the filter criteria.</span></span>  
5.  <span data-ttu-id="5268d-129">Pour démarrer le traitement par lots, cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="5268d-129">Choose the **OK** button to start the batch job.</span></span>  

<span data-ttu-id="5268d-130">Lorsque le traitement par lots est terminé, la feuille paiement contient toutes les écritures comptables fournisseur correspondant aux filtres.</span><span class="sxs-lookup"><span data-stu-id="5268d-130">When the batch job is finished, the payment journal contains all vendor ledger entries that match the filters.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5268d-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5268d-131">See Also</span></span>  
 <span data-ttu-id="5268d-132">[Paiements électroniques, Belgique](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="5268d-132">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="5268d-133">[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="5268d-133">[Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="5268d-134">[Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="5268d-134">[Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="5268d-135">[Tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="5268d-135">[Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 <span data-ttu-id="5268d-136">[Gérer les lignes de paiement électronique](how-to-manage-electronic-payment-lines.md) </span><span class="sxs-lookup"><span data-stu-id="5268d-136">[Manage Electronic Payment Lines](how-to-manage-electronic-payment-lines.md) </span></span>  
 [<span data-ttu-id="5268d-137">Imprimer les fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="5268d-137">Print Payment Files</span></span>](how-to-print-payment-files.md)
