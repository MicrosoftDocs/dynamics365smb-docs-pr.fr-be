---
title: Comment configurer des nomenclatures produits belges
description: "Les administrations douanières et fiscales belges ont établi un code article à 8 chiffres pour certains articles de la nomenclature."
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
ms.openlocfilehash: 6c549b770c94c186f14e0591c3164f1417c592b9
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-belgian-tariff-numbers"></a><span data-ttu-id="ec5d3-103">Configurer les nomenclatures produits belges</span><span class="sxs-lookup"><span data-stu-id="ec5d3-103">Set Up Belgian Tariff Numbers</span></span>
<span data-ttu-id="ec5d3-104">Les autorités douanières et fiscales belges ont établi un code article à huit unités pour divers articles tarifaires.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-104">The Belgian customs and tax authorities have established an 8-digit item code for various tariff items.</span></span>  

### <a name="to-set-up-tariff-numbers"></a><span data-ttu-id="ec5d3-105">Pour configurer des nomenclatures produits</span><span class="sxs-lookup"><span data-stu-id="ec5d3-105">To set up tariff numbers</span></span>  

1.  <span data-ttu-id="ec5d3-106">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Nomenclatures produits**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tariff Numbers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ec5d3-107">Choisissez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-107">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="ec5d3-108">Dans la fenêtre **Nomenclatures produits**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-108">In the **Tariff Numbers** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="ec5d3-109">Champ</span><span class="sxs-lookup"><span data-stu-id="ec5d3-109">Field</span></span>|<span data-ttu-id="ec5d3-110">Description</span><span class="sxs-lookup"><span data-stu-id="ec5d3-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="ec5d3-111">**Facteur de conversion**</span><span class="sxs-lookup"><span data-stu-id="ec5d3-111">**Conversion Factor**</span></span>|<span data-ttu-id="ec5d3-112">Entrez le facteur de conversion pour la nomenclature produits.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-112">Enter the conversion factor for the tariff number.</span></span> <span data-ttu-id="ec5d3-113">Le facteur de conversion est le facteur par lequel vous devez multiplier l'unité d'article pour obtenir l'unité imposée par les échanges intracommunautaires.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-113">The conversion factor is the factor by which you have to multiply the item unit to obtain the unit imposed by Intrastat.</span></span> <span data-ttu-id="ec5d3-114">Le facteur de conversion peut être utilisé lorsque l'unité d'article diffère de l'unité imposée par les échanges intracommunautaires.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-114">The conversion factor can be used when the item unit differs from the imposed Intrastat unit.</span></span> <span data-ttu-id="ec5d3-115">Le champ est disponible lorsque l'option **Unités supplémentaires** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-115">The field is available when **Supplementary Units** is selected.</span></span>|  
    |<span data-ttu-id="ec5d3-116">**Unité**</span><span class="sxs-lookup"><span data-stu-id="ec5d3-116">**Unit of Measure**</span></span>|<span data-ttu-id="ec5d3-117">Entrez l'unité de mesure de la nomenclature produits.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-117">Enter the unit of measure for the tariff number.</span></span> <span data-ttu-id="ec5d3-118">Le champ est disponible lorsque l'option **Unités supplémentaires** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-118">The field is available when **Supplementary Units** is selected.</span></span>|  
    |<span data-ttu-id="ec5d3-119">**Masse obligatoire**</span><span class="sxs-lookup"><span data-stu-id="ec5d3-119">**Weight Mandatory**</span></span>|<span data-ttu-id="ec5d3-120">Sélectionnez ce champ pour afficher le poids des articles.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-120">Select this field to show the weight of the items.</span></span>|  

4.  <span data-ttu-id="ec5d3-121">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-121">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="ec5d3-122">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec5d3-122">See Also</span></span>  
 <span data-ttu-id="ec5d3-123">[État intracommunautaire belge](belgian-intrastat-reporting.md) </span><span class="sxs-lookup"><span data-stu-id="ec5d3-123">[Belgian Intrastat Reporting](belgian-intrastat-reporting.md) </span></span>  
 <span data-ttu-id="ec5d3-124">[Configurer des types de déclaration](how-to-set-up-declaration-types.md) </span><span class="sxs-lookup"><span data-stu-id="ec5d3-124">[Set Up Declaration Types](how-to-set-up-declaration-types.md) </span></span>  
 <span data-ttu-id="ec5d3-125">[Configurer les numéros d'établissement intracomm.](how-to-set-up-intrastat-establishment-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="ec5d3-125">[Set Up Intrastat Establishment Numbers](how-to-set-up-intrastat-establishment-numbers.md) </span></span>  
 <span data-ttu-id="ec5d3-126">[Exporter les déclarations de tiers intracomm.](how-to-export-intrastat-third-party-declararations.md) </span><span class="sxs-lookup"><span data-stu-id="ec5d3-126">[Export Intrastat Third-Party Declararations](how-to-export-intrastat-third-party-declararations.md) </span></span>  
 [<span data-ttu-id="ec5d3-127">Imprimer le rapport de formulaire intracomm.</span><span class="sxs-lookup"><span data-stu-id="ec5d3-127">Print the Intrastat Form Report</span></span>](how-to-print-the-intrastat-form-report.md)

