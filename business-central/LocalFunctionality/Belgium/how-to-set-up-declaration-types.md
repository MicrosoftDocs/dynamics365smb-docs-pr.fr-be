---
title: Procédure pour définir des types de déclarations
description: Dans Business Central, il existe deux types de déclarations.
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
ms.openlocfilehash: 7df3a8d81b2c8ffbe3e884c705aeb947e3cccc18
ms.sourcegitcommit: 5b6dd8d881c0eb65ece6936a94dfda3185574335
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/28/2019
ms.locfileid: "1711010"
---
# <a name="set-up-declaration-types"></a><span data-ttu-id="48888-103">Paramétrer des types de déclarations</span><span class="sxs-lookup"><span data-stu-id="48888-103">Set Up Declaration Types</span></span>
<span data-ttu-id="48888-104">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], il existe deux types de déclarations :</span><span class="sxs-lookup"><span data-stu-id="48888-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], there are two types of declaration:</span></span>  

- <span data-ttu-id="48888-105">Déclaration simplifiée</span><span class="sxs-lookup"><span data-stu-id="48888-105">Simplified declaration</span></span>  
- <span data-ttu-id="48888-106">Déclaration étendue</span><span class="sxs-lookup"><span data-stu-id="48888-106">Extended declaration</span></span>  

<span data-ttu-id="48888-107">Le type de déclaration dépend de la quantité de biens expédiés ou reçus.</span><span class="sxs-lookup"><span data-stu-id="48888-107">The type of declaration depends on the amount of shipped or received goods.</span></span> <span data-ttu-id="48888-108">Pour déterminer le type de déclaration à utiliser, visitez le site Web de la [Banque Nationale de Belgique](https://aka.ms/BelgianNationalBank).</span><span class="sxs-lookup"><span data-stu-id="48888-108">To determine the type of declaration that you should use, visit the [National Bank of Belgium](https://aka.ms/BelgianNationalBank) website.</span></span>  

<span data-ttu-id="48888-109">Lorsque vous utilisez la déclaration étendue, vous devez également configurer un Incoterm dans la déclaration intracommunautaire pour chaque méthode de livraison.</span><span class="sxs-lookup"><span data-stu-id="48888-109">When using the extended declaration, you will also need to set up an Incoterm in Intrastat Declaration for each shipping method.</span></span> <span data-ttu-id="48888-110">Si vous ne voyez pas le champ **Incoterm dans la déclaration D.E.B.** de la page **Conditions de livraison**, vous devrez peut-être personnaliser la page et ajouter le champ.</span><span class="sxs-lookup"><span data-stu-id="48888-110">If you do not see the **Incoterm in Intrastat Decl.** field on the **Shipment Method** page, you might need to customize the page and add the field.</span></span>

## <a name="to-set-up-declaration-types"></a><span data-ttu-id="48888-111">Pour paramétrer des types de déclarations</span><span class="sxs-lookup"><span data-stu-id="48888-111">To set up declaration types</span></span>  

1.  <span data-ttu-id="48888-112">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="48888-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="48888-113">Activez la case à cocher **Déclaration D.E.B. simplifiée** pour configurer un type de déclaration simplifiée.</span><span class="sxs-lookup"><span data-stu-id="48888-113">Select the **Simplified Intrastat Decl.** check box to set up a simplified declaration type.</span></span> <span data-ttu-id="48888-114">Effacez ce champ pour utiliser la déclaration étendue.</span><span class="sxs-lookup"><span data-stu-id="48888-114">Clear this field to use extended declaration.</span></span>  
3.  <span data-ttu-id="48888-115">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="48888-115">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="48888-116">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="48888-116">See Also</span></span>  
 <span data-ttu-id="48888-117">[États intracommunautaires belges](belgian-intrastat-reporting.md) </span><span class="sxs-lookup"><span data-stu-id="48888-117">[Belgian Intrastat Reporting](belgian-intrastat-reporting.md) </span></span>  
 <span data-ttu-id="48888-118">[Paramétrer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="48888-118">[Set Up Belgian Tariff Numbers](how-to-set-up-belgian-tariff-numbers.md) </span></span>  
 <span data-ttu-id="48888-119">[Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="48888-119">[Set Up Intrastat Establishment Numbers](how-to-set-up-intrastat-establishment-numbers.md) </span></span>  
 <span data-ttu-id="48888-120">[Exporter les déclarations tierces intracommunautaires](how-to-export-intrastat-third-party-declararations.md) </span><span class="sxs-lookup"><span data-stu-id="48888-120">[Export Intrastat Third-Party Declararations](how-to-export-intrastat-third-party-declararations.md) </span></span>  
 [<span data-ttu-id="48888-121">Imprimer l'état du formulaire de D.E.B.</span><span class="sxs-lookup"><span data-stu-id="48888-121">Print the Intrastat Form Report</span></span>](how-to-print-the-intrastat-form-report.md)
