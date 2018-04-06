---
title: "Comment générer des propositions de domiciliation"
description: "Après avoir configuré des domiciliations, vous pouvez commencer à générer des propositions de domiciliation. Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux."
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
ms.openlocfilehash: 7010dc672eb56992fdefe41a95852ff3dcf9d8e1
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="generate-domiciliation-suggestions"></a><span data-ttu-id="78eca-104">Générer les propositions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="78eca-104">Generate Domiciliation Suggestions</span></span>
<span data-ttu-id="78eca-105">Après avoir créé des domiciliations, vous pouvez commencer à générer des propositions de domiciliation.</span><span class="sxs-lookup"><span data-stu-id="78eca-105">After you have set up domiciliations, you can start generating domiciliation suggestions.</span></span> <span data-ttu-id="78eca-106">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux.</span><span class="sxs-lookup"><span data-stu-id="78eca-106">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can only create domiciliation suggestions for domestic customers.</span></span>  

## <a name="to-generate-domiciliation-suggestions"></a><span data-ttu-id="78eca-107">Pour générer des propositions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="78eca-107">To generate domiciliation suggestions</span></span>  

1.  <span data-ttu-id="78eca-108">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille saisie domiciliation**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="78eca-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Domiciliation Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="78eca-109">Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Proposer domiciliations**.</span><span class="sxs-lookup"><span data-stu-id="78eca-109">In the **Batch Name** field, select the required journal batch, and then choose the **Suggest Domiciliations** action.</span></span>  
3.  <span data-ttu-id="78eca-110">Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="78eca-110">On the **Options** FastTab, fill in the fields as displayed in the following table.</span></span>  

    |<span data-ttu-id="78eca-111">Champ</span><span class="sxs-lookup"><span data-stu-id="78eca-111">Field</span></span>|<span data-ttu-id="78eca-112">Description</span><span class="sxs-lookup"><span data-stu-id="78eca-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="78eca-113">**Date besoin**</span><span class="sxs-lookup"><span data-stu-id="78eca-113">**Due Date**</span></span>|<span data-ttu-id="78eca-114">Entrez la date d'échéance à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="78eca-114">Enter the due date to be included in the batch job.</span></span> <span data-ttu-id="78eca-115">Seules les écritures ayant une date d'échéance antérieure ou identique à cette date seront incluses.</span><span class="sxs-lookup"><span data-stu-id="78eca-115">Only entries that have a due date before or on this date will be included.</span></span>|  
    |<span data-ttu-id="78eca-116">**Obtenir escomptes**</span><span class="sxs-lookup"><span data-stu-id="78eca-116">**Take Payment Discounts**</span></span>|<span data-ttu-id="78eca-117">Sélectionnez si vous souhaitez que le traitement par lots comprenne les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.</span><span class="sxs-lookup"><span data-stu-id="78eca-117">Select if you want the batch job to include customer ledger entries for which you can receive a payment discount.</span></span>|  
    |<span data-ttu-id="78eca-118">**Date d'escompte**</span><span class="sxs-lookup"><span data-stu-id="78eca-118">**Payment Discount Date**</span></span>|<span data-ttu-id="78eca-119">Entrez la date qui sera utilisée pour calculer l'escompte.</span><span class="sxs-lookup"><span data-stu-id="78eca-119">Enter the date that will be used to calculate the payment discount.</span></span>|  
    |<span data-ttu-id="78eca-120">**Inclure remboursements poss.**</span><span class="sxs-lookup"><span data-stu-id="78eca-120">**Select Possible Refunds**</span></span>|<span data-ttu-id="78eca-121">Sélectionnez si vous souhaitez que le traitement par lots inclue les remboursements.</span><span class="sxs-lookup"><span data-stu-id="78eca-121">Select if you want the batch job to include refunds.</span></span>|  
    |<span data-ttu-id="78eca-122">**Date comptabilisation**</span><span class="sxs-lookup"><span data-stu-id="78eca-122">**Posting Date**</span></span>|<span data-ttu-id="78eca-123">Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="78eca-123">Enter the date that will appear as the posting date on the lines that the batch job inserts in the domiciliation journal.</span></span>|  

4.  <span data-ttu-id="78eca-124">Dans le raccourci **Client**, entrez les éventuels critères de filtre supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="78eca-124">On the **Customer** FastTab, enter any additional filter criteria.</span></span>  
5.  <span data-ttu-id="78eca-125">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="78eca-125">Choose the **OK** button.</span></span>  

<span data-ttu-id="78eca-126">Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes qui correspondent aux filtres.</span><span class="sxs-lookup"><span data-stu-id="78eca-126">When the batch job is finished, the domiciliation journal contains all open customer ledger entries that match the filters.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="78eca-127">Les propositions de domiciliation incluront uniquement les clients qui ont un numéro de domiciliation configuré.</span><span class="sxs-lookup"><span data-stu-id="78eca-127">The domiciliation suggestions will only include customers who have a Domiciliation number set up.</span></span> <span data-ttu-id="78eca-128">Pour plus d'informations, reportez-vous à [Paramétrer les domiciliations](how-to-set-up-domiciliations.md).</span><span class="sxs-lookup"><span data-stu-id="78eca-128">For more information, see [Set Up Domiciliations](how-to-set-up-domiciliations.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="78eca-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="78eca-129">See Also</span></span>  
 <span data-ttu-id="78eca-130">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="78eca-130">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="78eca-131">[Prélèvements bancaires avec domiciliation](direct-debit-using-domiciliation.md) </span><span class="sxs-lookup"><span data-stu-id="78eca-131">[Direct Debit Using Domiciliation](direct-debit-using-domiciliation.md) </span></span>  
 <span data-ttu-id="78eca-132">[Paramétrer les domiciliations](how-to-set-up-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="78eca-132">[Set Up Domiciliations](how-to-set-up-domiciliations.md) </span></span>  
 <span data-ttu-id="78eca-133">[Tester les domiciliations](how-to-test-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="78eca-133">[Test Domiciliations](how-to-test-domiciliations.md) </span></span>  
 <span data-ttu-id="78eca-134">[Modifier et supprimer des lignes de domiciliation](how-to-edit-and-delete-domiciliation-lines.md) </span><span class="sxs-lookup"><span data-stu-id="78eca-134">[Edit and Delete Domiciliation Lines](how-to-edit-and-delete-domiciliation-lines.md) </span></span>  
 [<span data-ttu-id="78eca-135">Exporter et valider les domiciliations</span><span class="sxs-lookup"><span data-stu-id="78eca-135">Export and Post Domiciliations</span></span>](how-to-export-and-post-domiciliations.md)

