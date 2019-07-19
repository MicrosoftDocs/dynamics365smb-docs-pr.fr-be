---
title: Paramétrage de la TVA non déductible
description: Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA.
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
ms.openlocfilehash: bb3889e6cb7c53888755e3e3f0d6166eff9bb7bb
ms.sourcegitcommit: 5b6dd8d881c0eb65ece6936a94dfda3185574335
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/28/2019
ms.locfileid: "1711000"
---
# <a name="set-up-non-deductible-vat"></a><span data-ttu-id="fffe5-103">Paramétrer la TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="fffe5-103">Set Up Non-Deductible VAT</span></span>
<span data-ttu-id="fffe5-104">Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA.</span><span class="sxs-lookup"><span data-stu-id="fffe5-104">You can calculate VAT amounts for specific types of expenses that can be partially declared as VAT.</span></span> <span data-ttu-id="fffe5-105">Par exemple, dans la page **Fiche compte général**, si vous entrez 75 dans le champ **% de TVA non déductible**, 75 % du montant de TVA normal sont considérés comme des frais supplémentaires et sont ajoutés au montant net lors de la validation.</span><span class="sxs-lookup"><span data-stu-id="fffe5-105">For example, on the **G/L Account Card** page, if you enter 75 in the **% Non-Deductible VAT** field, then 75 percent of the regular VAT amount is considered an additional cost and will be added to the net amount during posting.</span></span> <span data-ttu-id="fffe5-106">Les 25 % restants sont validés en tant que TVA normale.</span><span class="sxs-lookup"><span data-stu-id="fffe5-106">The remaining 25 percent will be posted as regular VAT.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fffe5-107">Si aucune valeur n'est entrée dans le champ **% de TVA non déductible**, le montant de TVA est déductible à 100 %.</span><span class="sxs-lookup"><span data-stu-id="fffe5-107">If no value is entered in the **% Non-Deductible VAT** field, the VAT amount is 100 percent deductible.</span></span>  

## <a name="to-set-up-the-non-deductible-vat-percentage"></a><span data-ttu-id="fffe5-108">Pour définir le pourcentage de TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="fffe5-108">To set up the non-deductible VAT percentage</span></span>  

1.  <span data-ttu-id="fffe5-109">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="fffe5-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fffe5-110">Sélectionnez un compte frais général qui requiert la déduction partielle, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="fffe5-110">Select a general ledger expense account that requires the partial deduction, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="fffe5-111">Saisissez le montant dans le champ **% de TVA non déductible**.</span><span class="sxs-lookup"><span data-stu-id="fffe5-111">Enter the amount in **% Non deductible VAT** field.</span></span>  
4.  <span data-ttu-id="fffe5-112">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="fffe5-112">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fffe5-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fffe5-113">See Also</span></span>  
 <span data-ttu-id="fffe5-114">[TVA belge](belgian-vat.md) </span><span class="sxs-lookup"><span data-stu-id="fffe5-114">[Belgian VAT](belgian-vat.md) </span></span>  
 [<span data-ttu-id="fffe5-115">Imprimer les déclarations de TVA périodiques</span><span class="sxs-lookup"><span data-stu-id="fffe5-115">Print Periodic VAT Reports</span></span>](how-to-print-periodic-vat-reports.md)
