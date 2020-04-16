---
title: Procédure d'exportation des déclarations tierces intracommunautaires
description: En Belgique, un déclarant tiers doit renseigner la déclaration D.E.B (Intrastat). Le déclarant tiers doit être une personne ou une société externe.
services: project-madeira
documentationcenter: ''
author: sorenfriisalexandersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: soalex
ms.openlocfilehash: 921e60496ad85c62f92677187f633d3c69ad260e
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/01/2020
ms.locfileid: "3180896"
---
# <a name="export-intrastat-third-party-declarations"></a><span data-ttu-id="4e50e-104">Exporter les déclarations tierces intracommunautaires</span><span class="sxs-lookup"><span data-stu-id="4e50e-104">Export Intrastat Third-Party Declarations</span></span>
<span data-ttu-id="4e50e-105">En Belgique, un déclarant tiers doit renseigner la déclaration D.E.B (Intrastat).</span><span class="sxs-lookup"><span data-stu-id="4e50e-105">In Belgium, you must have a third-party declarant fill out the Intrastat declaration.</span></span> <span data-ttu-id="4e50e-106">Le déclarant tiers doit être une personne ou une société externe.</span><span class="sxs-lookup"><span data-stu-id="4e50e-106">The third-party declarant must be an external person or company.</span></span> 

## <a name="to-export-the-third-party-declaration"></a><span data-ttu-id="4e50e-107">Pour exporter la déclaration tierce</span><span class="sxs-lookup"><span data-stu-id="4e50e-107">To export the third-party declaration</span></span>  
<span data-ttu-id="4e50e-108">Avant d'exporter le fichier, il est conseillé d'afficher un aperçu de l'état.</span><span class="sxs-lookup"><span data-stu-id="4e50e-108">Before you export the file, it's a good idea to preview the report.</span></span> <span data-ttu-id="4e50e-109">Pour plus d'informations, voir [Imprimer l'état du formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md).</span><span class="sxs-lookup"><span data-stu-id="4e50e-109">For more information, see [Print the Intrastat Form Report](how-to-print-the-intrastat-form-report.md).</span></span>  

1.  <span data-ttu-id="4e50e-110">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Feuilles intracomm.**, puis choisissez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="4e50e-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Intrastat Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4e50e-111">Choisissez l'action **Créer fichier**.</span><span class="sxs-lookup"><span data-stu-id="4e50e-111">Choose the **Create File** action.</span></span>  
3.  <span data-ttu-id="4e50e-112">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="4e50e-112">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="4e50e-113">Champ</span><span class="sxs-lookup"><span data-stu-id="4e50e-113">Field</span></span>|<span data-ttu-id="4e50e-114">Désignation</span><span class="sxs-lookup"><span data-stu-id="4e50e-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="4e50e-115">**Déclaration Nihil**</span><span class="sxs-lookup"><span data-stu-id="4e50e-115">**Nihil declaration**</span></span>|<span data-ttu-id="4e50e-116">Sélectionnez ce champ si vous n'avez aucune transaction commerciale avec des pays/régions de l'Union européenne (UE) et que vous souhaitez envoyer une déclaration vide.</span><span class="sxs-lookup"><span data-stu-id="4e50e-116">Select if you do not have any trade transactions with European Union (EU) countries/regions and want to send an empty declaration.</span></span>|  
    |<span data-ttu-id="4e50e-117">**Informations de contrepartie**</span><span class="sxs-lookup"><span data-stu-id="4e50e-117">**Counter party info**</span></span>|<span data-ttu-id="4e50e-118">Activez ce champ pour inclure des informations de contrepartie dans le fichier de déclaration d'échanges de biens intracommunautaires (nouvelle exigence à partir de 2019).</span><span class="sxs-lookup"><span data-stu-id="4e50e-118">Check this field to include counter party information in the Intrastat file (new requirement from 2019).</span></span> <span data-ttu-id="4e50e-119">La déclaration de contrepartie ajoutée au fichier est issue des champs **Code pays/région origine** et **ID partenaire** de la Feuille intracomm.</span><span class="sxs-lookup"><span data-stu-id="4e50e-119">The counter party information added to the file is taken from the **Country/Region of Origin Code** and **Partner ID** fields from the Intrastat Journal.</span></span>|  
    |<span data-ttu-id="4e50e-120">**N° entreprise/N° id. intracomm.**</span><span class="sxs-lookup"><span data-stu-id="4e50e-120">**Enterprise No./VAT Reg. No.**</span></span>|<span data-ttu-id="4e50e-121">Entrez le numéro d'entreprise ou d'enregistrement de TVA.</span><span class="sxs-lookup"><span data-stu-id="4e50e-121">Enter the enterprise or VAT registration number.</span></span>|  
    
4.  <span data-ttu-id="4e50e-122">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="4e50e-122">Choose the **OK** button.</span></span>  

<span data-ttu-id="4e50e-123">Ensuite, envoyez la déclaration au portail OneGate.</span><span class="sxs-lookup"><span data-stu-id="4e50e-123">Next, submit the declaration to the OneGate portal.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4e50e-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4e50e-124">See Also</span></span>  
 <span data-ttu-id="4e50e-125">[États intracommunautaires belges](belgian-intrastat-reporting.md) </span><span class="sxs-lookup"><span data-stu-id="4e50e-125">[Belgian Intrastat Reporting](belgian-intrastat-reporting.md) </span></span>  
 <span data-ttu-id="4e50e-126">[Paramétrer des types de déclarations](how-to-set-up-declaration-types.md) </span><span class="sxs-lookup"><span data-stu-id="4e50e-126">[Set Up Declaration Types](how-to-set-up-declaration-types.md) </span></span>  
 <span data-ttu-id="4e50e-127">[Paramétrer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="4e50e-127">[Set Up Belgian Tariff Numbers](how-to-set-up-belgian-tariff-numbers.md) </span></span>  
 <span data-ttu-id="4e50e-128">[Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="4e50e-128">[Set Up Intrastat Establishment Numbers](how-to-set-up-intrastat-establishment-numbers.md) </span></span>  
 [<span data-ttu-id="4e50e-129">Imprimer l'état Formulaire de D.E.B.</span><span class="sxs-lookup"><span data-stu-id="4e50e-129">Print the Intrastat Form Report</span></span>](how-to-print-the-intrastat-form-report.md)
