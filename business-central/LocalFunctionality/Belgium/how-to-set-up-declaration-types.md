---
title: Procédure pour définir des types de déclarations
description: Dans Business Central, il existe deux types de déclarations.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: f4a1cc1950fbaee6743fe8ae41c903cfdf667243
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749719"
---
# <a name="set-up-declaration-types"></a><span data-ttu-id="79c85-103">Paramétrer des types de déclarations</span><span class="sxs-lookup"><span data-stu-id="79c85-103">Set Up Declaration Types</span></span>
<span data-ttu-id="79c85-104">Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], il existe deux types de déclarations :</span><span class="sxs-lookup"><span data-stu-id="79c85-104">In [!INCLUDE[prod_short](../../includes/prod_short.md)], there are two types of declaration:</span></span>  

- <span data-ttu-id="79c85-105">Déclaration simplifiée</span><span class="sxs-lookup"><span data-stu-id="79c85-105">Simplified declaration</span></span>  
- <span data-ttu-id="79c85-106">Déclaration étendue</span><span class="sxs-lookup"><span data-stu-id="79c85-106">Extended declaration</span></span>  

<span data-ttu-id="79c85-107">Le type de déclaration dépend de la quantité de biens expédiés ou reçus.</span><span class="sxs-lookup"><span data-stu-id="79c85-107">The type of declaration depends on the amount of shipped or received goods.</span></span> <span data-ttu-id="79c85-108">Pour déterminer le type de déclaration à utiliser, visitez le site Web de la [Banque Nationale de Belgique](https://aka.ms/BelgianNationalBank).</span><span class="sxs-lookup"><span data-stu-id="79c85-108">To determine the type of declaration that you should use, visit the [National Bank of Belgium](https://aka.ms/BelgianNationalBank) website.</span></span>  

<span data-ttu-id="79c85-109">Lorsque vous utilisez la déclaration étendue, vous devez également configurer un Incoterm dans la déclaration intracommunautaire pour chaque méthode de livraison.</span><span class="sxs-lookup"><span data-stu-id="79c85-109">When using the extended declaration, you will also need to set up an Incoterm in Intrastat Declaration for each shipping method.</span></span> <span data-ttu-id="79c85-110">Si vous ne voyez pas le champ **Incoterm dans la déclaration D.E.B.** de la page **Conditions de livraison**, vous devrez peut-être personnaliser la page et ajouter le champ.</span><span class="sxs-lookup"><span data-stu-id="79c85-110">If you do not see the **Incoterm in Intrastat Decl.** field on the **Shipment Method** page, you might need to customize the page and add the field.</span></span>

## <a name="to-set-up-declaration-types"></a><span data-ttu-id="79c85-111">Pour paramétrer des types de déclarations</span><span class="sxs-lookup"><span data-stu-id="79c85-111">To set up declaration types</span></span>  

1.  <span data-ttu-id="79c85-112">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Paramètres comptabilité**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="79c85-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="79c85-113">Activez la case à cocher **Déclaration D.E.B. simplifiée** pour configurer un type de déclaration simplifiée.</span><span class="sxs-lookup"><span data-stu-id="79c85-113">Select the **Simplified Intrastat Decl.** check box to set up a simplified declaration type.</span></span> <span data-ttu-id="79c85-114">Effacez ce champ pour utiliser la déclaration étendue.</span><span class="sxs-lookup"><span data-stu-id="79c85-114">Clear this field to use extended declaration.</span></span>  
3.  <span data-ttu-id="79c85-115">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="79c85-115">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="79c85-116">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79c85-116">See Also</span></span>  
 <span data-ttu-id="79c85-117">[États intracommunautaires belges](belgian-intrastat-reporting.md) </span><span class="sxs-lookup"><span data-stu-id="79c85-117">[Belgian Intrastat Reporting](belgian-intrastat-reporting.md) </span></span>  
 <span data-ttu-id="79c85-118">[Paramétrer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="79c85-118">[Set Up Belgian Tariff Numbers](how-to-set-up-belgian-tariff-numbers.md) </span></span>  
 <span data-ttu-id="79c85-119">[Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="79c85-119">[Set Up Intrastat Establishment Numbers](how-to-set-up-intrastat-establishment-numbers.md) </span></span>  
 <span data-ttu-id="79c85-120">[Exporter les déclarations de tiers intracomm.](how-to-export-intrastat-third-party-declararations.md) </span><span class="sxs-lookup"><span data-stu-id="79c85-120">[Export Intrastat Third-Party Declararations](how-to-export-intrastat-third-party-declararations.md) </span></span>  
 [<span data-ttu-id="79c85-121">Imprimer l'état Formulaire de D.E.B.</span><span class="sxs-lookup"><span data-stu-id="79c85-121">Print the Intrastat Form Report</span></span>](how-to-print-the-intrastat-form-report.md)
