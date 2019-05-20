---
title: TVA belge
description: Les améliorations belges de la fonction de déclaration de TVA vous permettent d'imprimer des détails sur les transactions TVA.
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
ms.openlocfilehash: 260365ce5f1e88bb1cc243a1af16b184ba95a9a4
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237669"
---
# <a name="belgian-vat"></a><span data-ttu-id="25e84-103">TVA belge</span><span class="sxs-lookup"><span data-stu-id="25e84-103">Belgian VAT</span></span>
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="25e84-104">comprend des améliorations de la Belgique à la fonction de report de TVA qui vous permet d'imprimer les détails de transaction TVA.</span><span class="sxs-lookup"><span data-stu-id="25e84-104">includes Belgium enhancements to VAT reporting feature that enables you to print VAT transaction details.</span></span> <span data-ttu-id="25e84-105">Vous devez envoyer les états suivants aux autorités fiscales belges :</span><span class="sxs-lookup"><span data-stu-id="25e84-105">You must send the following reports to the Belgian tax authorities:</span></span>  

-   <span data-ttu-id="25e84-106">Déclaration mensuelle/trimestrielle - Cet état permet de créer des déclarations de TVA mensuelles ou trimestrielles, en fonction des revenus de votre société.</span><span class="sxs-lookup"><span data-stu-id="25e84-106">Monthly/Quarterly declaration - This report is used to create monthly or quarterly VAT declarations, depending on your company revenue.</span></span>  

-   <span data-ttu-id="25e84-107">Listing TVA annuel (sur papier/disquette) - Cet état permet de déclarer annuellement tous les montants facturés pour les biens et les services à toutes les sociétés belges avec un numéro de TVA enregistré.</span><span class="sxs-lookup"><span data-stu-id="25e84-107">VAT annual listing (on paper/disk) - This report is used to annually report all amounts invoiced for both goods and services to all Belgian companies with a registered VAT number.</span></span>  

-   <span data-ttu-id="25e84-108">Listing TVA-VIES (sur papier/disquette) - Cet état permet de déclarer les ventes de marchandises à d'autres pays.</span><span class="sxs-lookup"><span data-stu-id="25e84-108">VAT-VIES listing (on paper/disk) - This report is used to report the sales of goods to other countries.</span></span>  

<span data-ttu-id="25e84-109">Vous êtes également tenu de fournir un relevé imprimé détaillant les transactions TVA aux autorités fiscales belges.</span><span class="sxs-lookup"><span data-stu-id="25e84-109">You are also required to provide a printed statement detailing the VAT transactions to the Belgian tax authorities.</span></span> <span data-ttu-id="25e84-110">Pour plus d'informations, voir Déclaration TVA.</span><span class="sxs-lookup"><span data-stu-id="25e84-110">For more information, see VAT Statement.</span></span>  

## <a name="non-deductible-vat"></a><span data-ttu-id="25e84-111">TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="25e84-111">Non-Deductible VAT</span></span>  
 <span data-ttu-id="25e84-112">En Belgique, la TVA peut être entièrement ou partiellement déductible.</span><span class="sxs-lookup"><span data-stu-id="25e84-112">In Belgium, VAT can be fully or partially deductible.</span></span> <span data-ttu-id="25e84-113">Des dépenses comme les frais de représentation ou les achats de voitures ne sont que partiellement déductibles et la transaction doit spécifier quel pourcentage de la TVA est non déductible.</span><span class="sxs-lookup"><span data-stu-id="25e84-113">Expenses such as representation cost or purchases of cars are only partially deductible, and the transaction must specify how much of the VAT is non-deductible.</span></span> <span data-ttu-id="25e84-114">Par exemple, vous créez un compte général pour les immobilisations comme les voitures, et un autre compte pour les frais de représentation.</span><span class="sxs-lookup"><span data-stu-id="25e84-114">For example, you create a general ledger account for fixed assets such as cars, and another account for representation cost.</span></span> <span data-ttu-id="25e84-115">Pour chaque compte, vous spécifiez quel pourcentage de la TVA déclarée est non déductible en définissant le champ Pourcentage TVA non déductible.</span><span class="sxs-lookup"><span data-stu-id="25e84-115">For each account, you specify how much of the reported VAT is non-deductible by setting the Percentage Non deductible VAT field.</span></span> <span data-ttu-id="25e84-116">Ensuite, lorsque vous validez une transaction, la TVA déductible sera validée sur le compte TVA correspondant, et la TVA non déductible sera ajoutée au montant de base et validée sur le même compte que les immobilisations corporelles et incorporelles.</span><span class="sxs-lookup"><span data-stu-id="25e84-116">Then, when you post a transaction, the deductible VAT will post to the corresponding VAT account, and the non-deductible VAT will be added to the base amount and posted to the same account as the tangible or intangible asset.</span></span>  

 <span data-ttu-id="25e84-117">Pour les immobilisations, la TVA non déductible est amortie simplement comme le coût d'acquisition de base de l'immobilisation.</span><span class="sxs-lookup"><span data-stu-id="25e84-117">For fixed assets, the non-deductible VAT depreciates just like the base acquisition cost of the fixed asset.</span></span> <span data-ttu-id="25e84-118">Vous devez paramétrer des groupes comptabilisation immobilisation distincts pour chaque pourcentage de TVA non déductible, étant donné que chaque groupe comptabilisation immobilisation est validé sur un compte général où le champ Pourcentage TVA non déductible spécifie quel pourcentage de TVA doit être validé sur le même compte que l'immobilisation.</span><span class="sxs-lookup"><span data-stu-id="25e84-118">You must set up separate fixed asset posting groups for each percentage of non-deductible VAT since each fixed asset posting group posts to a general ledger account where the Percentage Non deductible VAT field specifies how much VAT must post to the same account as the fixed asset.</span></span>  

 <span data-ttu-id="25e84-119">Si vous sélectionnez le champ TVA non déductible comprise dans une ligne déclaration TVA, la TVA non déductible est incluse dans le montant TVA.</span><span class="sxs-lookup"><span data-stu-id="25e84-119">If you select the Incl. Non Deductible VAT field in a VAT statement line, non-deductible VAT is included in the VAT amount.</span></span> <span data-ttu-id="25e84-120">L'état **Calculer et valider décl. TVA** ajoute la partie non déductible de ce montant aux champs **Montant TVA non déductible** et **Montant TVA devise origine non déductible** dans les écritures TVA résultantes.</span><span class="sxs-lookup"><span data-stu-id="25e84-120">The **Calc. and Post VAT Settlement** report adds the non-deductible part of that amount to the **Non Ded. VAT Amount** and **Non Ded. Source Curr. VAT Amt.** fields in the resulting VAT entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="25e84-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="25e84-121">See Also</span></span>  
 <span data-ttu-id="25e84-122">[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="25e84-122">[Belgium Local Functionality](belgium-local-functionality.md) </span></span>  
 <span data-ttu-id="25e84-123">[Imprimer des états TVA périodiques](how-to-print-periodic-vat-reports.md) </span><span class="sxs-lookup"><span data-stu-id="25e84-123">[Print Periodic VAT Reports](how-to-print-periodic-vat-reports.md) </span></span>  
 [<span data-ttu-id="25e84-124">Configurer la TVA non déductible</span><span class="sxs-lookup"><span data-stu-id="25e84-124">Set Up Non-Deductible VAT</span></span>](how-to-set-up-non-deductible-vat.md)
