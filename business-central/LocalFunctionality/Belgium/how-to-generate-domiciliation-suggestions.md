---
title: "Comment générer des propositions de domiciliation"
description: "Après avoir créé des domiciliations, vous pouvez commencer à générer des propositions de domiciliation. Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous ne pouvez créer que des suggestions de domiciliation pour les clients nationaux."
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
ms.openlocfilehash: 192696338f47d400ea54b95dbae0c2efe70a2ef6
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="generate-domiciliation-suggestions"></a><span data-ttu-id="2513a-104">Générer les propositions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="2513a-104">Generate Domiciliation Suggestions</span></span>
<span data-ttu-id="2513a-105">Après avoir créé des domiciliations, vous pouvez commencer à générer des propositions de domiciliation.</span><span class="sxs-lookup"><span data-stu-id="2513a-105">After you have set up domiciliations, you can start generating domiciliation suggestions.</span></span> <span data-ttu-id="2513a-106">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux.</span><span class="sxs-lookup"><span data-stu-id="2513a-106">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can only create domiciliation suggestions for domestic customers.</span></span>  

## <a name="to-generate-domiciliation-suggestions"></a><span data-ttu-id="2513a-107">Pour générer des propositions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="2513a-107">To generate domiciliation suggestions</span></span>  

1.  <span data-ttu-id="2513a-108">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille saisie domiciliation**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="2513a-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Domiciliation Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2513a-109">Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Proposer domiciliations**.</span><span class="sxs-lookup"><span data-stu-id="2513a-109">In the **Batch Name** field, select the required journal batch, and then choose the **Suggest Domiciliations** action.</span></span>  
3.  <span data-ttu-id="2513a-110">Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="2513a-110">On the **Options** FastTab, fill in the fields as displayed in the following table.</span></span>  

    |<span data-ttu-id="2513a-111">Champ</span><span class="sxs-lookup"><span data-stu-id="2513a-111">Field</span></span>|<span data-ttu-id="2513a-112">Description</span><span class="sxs-lookup"><span data-stu-id="2513a-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="2513a-113">**Date besoin**</span><span class="sxs-lookup"><span data-stu-id="2513a-113">**Due Date**</span></span>|<span data-ttu-id="2513a-114">Entrez la date d'échéance à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="2513a-114">Enter the due date to be included in the batch job.</span></span> <span data-ttu-id="2513a-115">Seules les écritures ayant une date d'échéance antérieure ou identique à cette date seront incluses.</span><span class="sxs-lookup"><span data-stu-id="2513a-115">Only entries that have a due date before or on this date will be included.</span></span>|  
    |<span data-ttu-id="2513a-116">**Obtenir escomptes**</span><span class="sxs-lookup"><span data-stu-id="2513a-116">**Take Payment Discounts**</span></span>|<span data-ttu-id="2513a-117">Sélectionnez si vous souhaitez que le traitement par lots comprenne les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.</span><span class="sxs-lookup"><span data-stu-id="2513a-117">Select if you want the batch job to include customer ledger entries for which you can receive a payment discount.</span></span>|  
    |<span data-ttu-id="2513a-118">**Date d'escompte**</span><span class="sxs-lookup"><span data-stu-id="2513a-118">**Payment Discount Date**</span></span>|<span data-ttu-id="2513a-119">Entrez la date qui sera utilisée pour calculer l'escompte.</span><span class="sxs-lookup"><span data-stu-id="2513a-119">Enter the date that will be used to calculate the payment discount.</span></span>|  
    |<span data-ttu-id="2513a-120">**Inclure remboursements poss.**</span><span class="sxs-lookup"><span data-stu-id="2513a-120">**Select Possible Refunds**</span></span>|<span data-ttu-id="2513a-121">Sélectionnez si vous souhaitez que le traitement par lots inclue les remboursements.</span><span class="sxs-lookup"><span data-stu-id="2513a-121">Select if you want the batch job to include refunds.</span></span>|  
    |<span data-ttu-id="2513a-122">**Date comptabilisation**</span><span class="sxs-lookup"><span data-stu-id="2513a-122">**Posting Date**</span></span>|<span data-ttu-id="2513a-123">Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="2513a-123">Enter the date that will appear as the posting date on the lines that the batch job inserts in the domiciliation journal.</span></span>|  

4.  <span data-ttu-id="2513a-124">Dans le raccourci **Client**, entrez les éventuels critères de filtre supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="2513a-124">On the **Customer** FastTab, enter any additional filter criteria.</span></span>  
5.  <span data-ttu-id="2513a-125">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="2513a-125">Choose the **OK** button.</span></span>  

<span data-ttu-id="2513a-126">Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes qui correspondent aux filtres.</span><span class="sxs-lookup"><span data-stu-id="2513a-126">When the batch job is finished, the domiciliation journal contains all open customer ledger entries that match the filters.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2513a-127">Les suggestions de domiciliation ne concernent que les clients disposant d'un numéro de domiciliation.</span><span class="sxs-lookup"><span data-stu-id="2513a-127">The domiciliation suggestions will only include customers who have a Domiciliation number set up.</span></span> <span data-ttu-id="2513a-128">Pour plus d'informations, reportez-vous à [Paramétrer les domiciliations](how-to-set-up-domiciliations.md).</span><span class="sxs-lookup"><span data-stu-id="2513a-128">For more information, see [Set Up Domiciliations](how-to-set-up-domiciliations.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="2513a-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2513a-129">See Also</span></span>  
 <span data-ttu-id="2513a-130">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="2513a-130">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="2513a-131">[Prélèvements bancaires avec domiciliation](direct-debit-using-domiciliation.md) </span><span class="sxs-lookup"><span data-stu-id="2513a-131">[Direct Debit Using Domiciliation](direct-debit-using-domiciliation.md) </span></span>  
 <span data-ttu-id="2513a-132">[Paramétrer les domiciliations](how-to-set-up-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="2513a-132">[Set Up Domiciliations](how-to-set-up-domiciliations.md) </span></span>  
 <span data-ttu-id="2513a-133">[Tester les domiciliations](how-to-test-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="2513a-133">[Test Domiciliations](how-to-test-domiciliations.md) </span></span>  
 <span data-ttu-id="2513a-134">[Modifier et supprimer des lignes de domiciliation](how-to-edit-and-delete-domiciliation-lines.md) </span><span class="sxs-lookup"><span data-stu-id="2513a-134">[Edit and Delete Domiciliation Lines](how-to-edit-and-delete-domiciliation-lines.md) </span></span>  
 [<span data-ttu-id="2513a-135">Exporter et valider les domiciliations</span><span class="sxs-lookup"><span data-stu-id="2513a-135">Export and Post Domiciliations</span></span>](how-to-export-and-post-domiciliations.md)

