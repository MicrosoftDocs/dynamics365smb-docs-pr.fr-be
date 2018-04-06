---
title: "Comment configurer des types de déclaration"
description: "Dans Business Central, il existe deux types de déclarations."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/07/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 12e62f47ee6ac0db6d2dab4daea271456804609b
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-declaration-types"></a><span data-ttu-id="4a44b-103">Configurer des types de déclaration</span><span class="sxs-lookup"><span data-stu-id="4a44b-103">Set Up Declaration Types</span></span>
<span data-ttu-id="4a44b-104">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], il existe deux types de déclaration :</span><span class="sxs-lookup"><span data-stu-id="4a44b-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], there are two types of declaration:</span></span>  

- <span data-ttu-id="4a44b-105">Déclaration simplifiée</span><span class="sxs-lookup"><span data-stu-id="4a44b-105">Simplified declaration</span></span>  
- <span data-ttu-id="4a44b-106">Déclaration étendue</span><span class="sxs-lookup"><span data-stu-id="4a44b-106">Extended declaration</span></span>  

<span data-ttu-id="4a44b-107">Le type de déclaration dépend du montant des marchandises expédiées ou reçues.</span><span class="sxs-lookup"><span data-stu-id="4a44b-107">The type of declaration depends on the amount of shipped or received goods.</span></span> <span data-ttu-id="4a44b-108">Pour déterminer le type de déclaration à utiliser, visitez le site web [Banque nationale de Belgique](http://go.microsoft.com/fwlink/?LinkId=163064).</span><span class="sxs-lookup"><span data-stu-id="4a44b-108">To determine the type of declaration that you should use, see the [National Bank of Belgium](http://go.microsoft.com/fwlink/?LinkId=163064) web site.</span></span>  

<span data-ttu-id="4a44b-109">Si vous utilisez la déclaration étendue, vous devez également paramétrer un Incoterm dans la déclaration intracommunautaire pour chaque méthode de livraison.</span><span class="sxs-lookup"><span data-stu-id="4a44b-109">When using the extended declaration, you will also need to set up an Incoterm in Intrastat Declaration for each shipping method.</span></span> <span data-ttu-id="4a44b-110">Si vous ne voyez pas **Incoterme dans la déclaration intracommunautaire** dans la page **Conditions de livraison**, vous devrez peut-être personnaliser la page et ajouter le champ.</span><span class="sxs-lookup"><span data-stu-id="4a44b-110">If you do not see the **Incoterm in Intrastat Decl.** on the **Shipment Method** page, you may need to customize the page and add the field.</span></span> 

## <a name="to-set-up-declaration-types"></a><span data-ttu-id="4a44b-111">Pour configurer des types de déclaration</span><span class="sxs-lookup"><span data-stu-id="4a44b-111">To set up declaration types</span></span>  

1.  <span data-ttu-id="4a44b-112">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="4a44b-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4a44b-113">Sur le raccourci **Général**, sélectionnez la case à cocher **D.E.B. simplifiée** pour configurer un type de déclaration simplifiée.</span><span class="sxs-lookup"><span data-stu-id="4a44b-113">On the **General** FastTab, select the **Simplified Intrastat Decl.** check box to set up a simplified declaration type.</span></span> <span data-ttu-id="4a44b-114">Effacez ce champ pour utiliser la déclaration étendue.</span><span class="sxs-lookup"><span data-stu-id="4a44b-114">Clear this field to use extended declaration.</span></span>  
3.  <span data-ttu-id="4a44b-115">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="4a44b-115">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4a44b-116">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a44b-116">See Also</span></span>  
 <span data-ttu-id="4a44b-117">[État intracommunautaire belge](belgian-intrastat-reporting.md) </span><span class="sxs-lookup"><span data-stu-id="4a44b-117">[Belgian Intrastat Reporting](belgian-intrastat-reporting.md) </span></span>  
 <span data-ttu-id="4a44b-118">[Configurer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="4a44b-118">[Set Up Belgian Tariff Numbers](how-to-set-up-belgian-tariff-numbers.md) </span></span>  
 <span data-ttu-id="4a44b-119">[Configurer les numéros d'établissement intracomm.](how-to-set-up-intrastat-establishment-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="4a44b-119">[Set Up Intrastat Establishment Numbers](how-to-set-up-intrastat-establishment-numbers.md) </span></span>  
 <span data-ttu-id="4a44b-120">[Exporter les déclarations de tiers intracomm.](how-to-export-intrastat-third-party-declararations.md) </span><span class="sxs-lookup"><span data-stu-id="4a44b-120">[Export Intrastat Third-Party Declararations](how-to-export-intrastat-third-party-declararations.md) </span></span>  
 [<span data-ttu-id="4a44b-121">Imprimer le rapport de formulaire intracomm.</span><span class="sxs-lookup"><span data-stu-id="4a44b-121">Print the Intrastat Form Report</span></span>](how-to-print-the-intrastat-form-report.md)

