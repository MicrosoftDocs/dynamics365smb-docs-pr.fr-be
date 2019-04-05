---
title: Paramétrage des nomenclatures produits belges
description: Les autorités douanières et fiscales belges ont établi un code article à 8 unités pour diverses nomenclatures produits.
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
ms.openlocfilehash: 89de76c494be0b37cc2d5f649c71bb66d0758efb
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/08/2019
ms.locfileid: "826493"
---
# <a name="set-up-belgian-tariff-numbers"></a><span data-ttu-id="a6e4b-103">Paramétrer les nomenclatures produits belges</span><span class="sxs-lookup"><span data-stu-id="a6e4b-103">Set Up Belgian Tariff Numbers</span></span>
<span data-ttu-id="a6e4b-104">Les autorités douanières et fiscales belges ont établi un code article à 8 unités pour diverses nomenclatures produits.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-104">The Belgian customs and tax authorities have established an 8-digit item code for various tariff items.</span></span>  

### <a name="to-set-up-tariff-numbers"></a><span data-ttu-id="a6e4b-105">Pour paramétrer les nomenclatures produits</span><span class="sxs-lookup"><span data-stu-id="a6e4b-105">To set up tariff numbers</span></span>  

1.  <span data-ttu-id="a6e4b-106">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Nomenclatures produits**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tariff Numbers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a6e4b-107">Sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-107">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="a6e4b-108">Dans la page **Nomenclatures produits**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-108">On the **Tariff Numbers** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="a6e4b-109">Champ</span><span class="sxs-lookup"><span data-stu-id="a6e4b-109">Field</span></span>|<span data-ttu-id="a6e4b-110">Désignation</span><span class="sxs-lookup"><span data-stu-id="a6e4b-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="a6e4b-111">**Facteur de conversion**</span><span class="sxs-lookup"><span data-stu-id="a6e4b-111">**Conversion Factor**</span></span>|<span data-ttu-id="a6e4b-112">Entrez le facteur de conversion pour la nomenclature produit.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-112">Enter the conversion factor for the tariff number.</span></span> <span data-ttu-id="a6e4b-113">Le facteur de conversion est le facteur par lequel vous devez multiplier l'unité article pour obtenir l'unité imposée par la D.E.B.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-113">The conversion factor is the factor by which you have to multiply the item unit to obtain the unit imposed by Intrastat.</span></span> <span data-ttu-id="a6e4b-114">Le facteur de conversion peut être utilisé lorsque l'unité article diffère de l'unité imposée par la D.E.B.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-114">The conversion factor can be used when the item unit differs from the imposed Intrastat unit.</span></span> <span data-ttu-id="a6e4b-115">Le champ est disponible lorsque le champ **Unités supplémentaires** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-115">The field is available when **Supplementary Units** is selected.</span></span>|  
    |<span data-ttu-id="a6e4b-116">**Unité**</span><span class="sxs-lookup"><span data-stu-id="a6e4b-116">**Unit of Measure**</span></span>|<span data-ttu-id="a6e4b-117">Entrez l'unité de mesure pour la nomenclature produit.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-117">Enter the unit of measure for the tariff number.</span></span> <span data-ttu-id="a6e4b-118">Le champ est disponible lorsque le champ **Unités supplémentaires** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-118">The field is available when **Supplementary Units** is selected.</span></span>|  
    |<span data-ttu-id="a6e4b-119">**Poids obligatoire**</span><span class="sxs-lookup"><span data-stu-id="a6e4b-119">**Weight Mandatory**</span></span>|<span data-ttu-id="a6e4b-120">Sélectionnez ce champ pour afficher le poids des articles.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-120">Select this field to show the weight of the items.</span></span>|  

4.  <span data-ttu-id="a6e4b-121">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-121">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a6e4b-122">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a6e4b-122">See Also</span></span>  
 <span data-ttu-id="a6e4b-123">[États intracommunautaires belges](belgian-intrastat-reporting.md) </span><span class="sxs-lookup"><span data-stu-id="a6e4b-123">[Belgian Intrastat Reporting](belgian-intrastat-reporting.md) </span></span>  
 <span data-ttu-id="a6e4b-124">[Paramétrer des types de déclarations](how-to-set-up-declaration-types.md) </span><span class="sxs-lookup"><span data-stu-id="a6e4b-124">[Set Up Declaration Types](how-to-set-up-declaration-types.md) </span></span>  
 <span data-ttu-id="a6e4b-125">[Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="a6e4b-125">[Set Up Intrastat Establishment Numbers](how-to-set-up-intrastat-establishment-numbers.md) </span></span>  
 <span data-ttu-id="a6e4b-126">[Exporter les déclarations tierces intracommunautaires](how-to-export-intrastat-third-party-declararations.md) </span><span class="sxs-lookup"><span data-stu-id="a6e4b-126">[Export Intrastat Third-Party Declararations](how-to-export-intrastat-third-party-declararations.md) </span></span>  
 [<span data-ttu-id="a6e4b-127">Imprimer l'état du formulaire de D.E.B.</span><span class="sxs-lookup"><span data-stu-id="a6e4b-127">Print the Intrastat Form Report</span></span>](how-to-print-the-intrastat-form-report.md)
