---
title: Paramétrage de la TVA non déductible
description: Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3798454967217fb3b10d22e2c168ed8c2185722f
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779201"
---
# <a name="set-up-non-deductible-vat"></a><span data-ttu-id="fada7-103">Paramétrer la TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="fada7-103">Set Up Non-Deductible VAT</span></span>
<span data-ttu-id="fada7-104">Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA.</span><span class="sxs-lookup"><span data-stu-id="fada7-104">You can calculate VAT amounts for specific types of expenses that can be partially declared as VAT.</span></span> <span data-ttu-id="fada7-105">Par exemple, dans la page **Fiche compte général**, si vous entrez 75 dans le champ **% de TVA non déductible**, 75 % du montant de TVA normal sont considérés comme des frais supplémentaires et sont ajoutés au montant net lors de la validation.</span><span class="sxs-lookup"><span data-stu-id="fada7-105">For example, on the **G/L Account Card** page, if you enter 75 in the **% Non-Deductible VAT** field, then 75 percent of the regular VAT amount is considered an additional cost and will be added to the net amount during posting.</span></span> <span data-ttu-id="fada7-106">Les 25 % restants sont validés en tant que TVA normale.</span><span class="sxs-lookup"><span data-stu-id="fada7-106">The remaining 25 percent will be posted as regular VAT.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fada7-107">Si aucune valeur n'est entrée dans le champ **% de TVA non déductible**, le montant de TVA est déductible à 100 %.</span><span class="sxs-lookup"><span data-stu-id="fada7-107">If no value is entered in the **% Non-Deductible VAT** field, the VAT amount is 100 percent deductible.</span></span>  

## <a name="to-set-up-the-non-deductible-vat-percentage"></a><span data-ttu-id="fada7-108">Pour définir le pourcentage de TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="fada7-108">To set up the non-deductible VAT percentage</span></span>  

1.  <span data-ttu-id="fada7-109">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Plan comptable**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="fada7-109">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fada7-110">Sélectionnez un compte frais général qui requiert la déduction partielle, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="fada7-110">Select a general ledger expense account that requires the partial deduction, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="fada7-111">Saisissez le montant dans le champ **% de TVA non déductible**.</span><span class="sxs-lookup"><span data-stu-id="fada7-111">Enter the amount in **% Non deductible VAT** field.</span></span>  
4.  <span data-ttu-id="fada7-112">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="fada7-112">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fada7-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fada7-113">See Also</span></span>  
 <span data-ttu-id="fada7-114">[TVA belge](belgian-vat.md) </span><span class="sxs-lookup"><span data-stu-id="fada7-114">[Belgian VAT](belgian-vat.md) </span></span>  
 [<span data-ttu-id="fada7-115">Imprimer les déclarations de TVA périodiques</span><span class="sxs-lookup"><span data-stu-id="fada7-115">Print Periodic VAT Reports</span></span>](how-to-print-periodic-vat-reports.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]