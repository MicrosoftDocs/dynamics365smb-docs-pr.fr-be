---
title: "Comment configurer la TVA non déductible"
description: "Vous pouvez calculer les montants TVA pour les types spécifiques de frais pouvant être partiellement déclarés comme TVA."
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
ms.openlocfilehash: 00fe4c0fc0450585cd3e7a6cbb14b9b4b6d57f54
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-non-deductible-vat"></a><span data-ttu-id="77304-103">Configurer la TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="77304-103">Set Up Non-Deductible VAT</span></span>
<span data-ttu-id="77304-104">Vous pouvez calculer les montants TVA pour les types spécifiques de frais pouvant être partiellement déclarés comme TVA.</span><span class="sxs-lookup"><span data-stu-id="77304-104">You can calculate VAT amounts for specific types of expenses which can be partially declared as VAT.</span></span> <span data-ttu-id="77304-105">Par exemple, dans la fenêtre **Fiche compte général**, si vous entrez 75 % dans le champ **% TVA non déductible**, 75 % du montant de TVA habituel seront considérés comme un coût supplémentaire et seront ajoutés au montant net lors de la validation.</span><span class="sxs-lookup"><span data-stu-id="77304-105">For example, in the **G/L Account Card** window, if you enter 75 percent in the **% Non-Deductible VAT** field, then 75 percent of the regular VAT amount is considered an additional cost and will be added to the net amount during posting.</span></span> <span data-ttu-id="77304-106">Les 25 % restants seront validés comme montant de TVA habituel.</span><span class="sxs-lookup"><span data-stu-id="77304-106">The remaining 25 percent will be posted as regular VAT.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="77304-107">Si aucune valeur n'est entrée dans le champ **% TVA non déductible**, le montant de TVA est 100 % déductible.</span><span class="sxs-lookup"><span data-stu-id="77304-107">If no value is entered in the **% Non-Deductible VAT** field, the VAT amount is 100 percent deductible.</span></span>  

## <a name="to-set-up-the-non-deductible-vat-percentage"></a><span data-ttu-id="77304-108">Pour configurer le pourcentage de TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="77304-108">To set up the non-deductible VAT percentage</span></span>  

1.  <span data-ttu-id="77304-109">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Plan comptable**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="77304-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="77304-110">Sélectionnez un compte dépenses général qui nécessite la déduction partielle, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="77304-110">Select a general ledger expense account that requires the partial deduction, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="77304-111">Dans le raccourci **Validation**, saisissez le montant dans le champ **% TVA non déductible**.</span><span class="sxs-lookup"><span data-stu-id="77304-111">On the **Posting** FastTab, enter the amount in **% Non deductible VAT** field.</span></span>  
4.  <span data-ttu-id="77304-112">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="77304-112">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="77304-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="77304-113">See Also</span></span>  
 <span data-ttu-id="77304-114">[TVA belge](belgian-vat.md) </span><span class="sxs-lookup"><span data-stu-id="77304-114">[Belgian VAT](belgian-vat.md) </span></span>  
 [<span data-ttu-id="77304-115">Imprimer des états TVA périodiques</span><span class="sxs-lookup"><span data-stu-id="77304-115">Print Periodic VAT Reports</span></span>](how-to-print-periodic-vat-reports.md)

