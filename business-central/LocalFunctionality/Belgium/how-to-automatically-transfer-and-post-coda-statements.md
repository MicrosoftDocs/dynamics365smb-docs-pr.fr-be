---
title: Comment transférer et valider automatiquement les relevés CODA
description: Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: d249493a9278d462741015cf66c1f3536aa566ba
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237682"
---
# <a name="automatically-transfer-and-post-coda-statements"></a><span data-ttu-id="61dd9-103">Transférer et publier automatiquement des relevés CODA</span><span class="sxs-lookup"><span data-stu-id="61dd9-103">Automatically Transfer and Post CODA Statements</span></span>
<span data-ttu-id="61dd9-104">Après avoir appliqué et traité toutes les lignes de relevés CODA, vous pouvez transférer les lignes de relevés CODA vers une feuille financière.</span><span class="sxs-lookup"><span data-stu-id="61dd9-104">After you have applied and processed all CODA statement lines, you can transfer the CODA statement lines to a financial journal.</span></span>  

<span data-ttu-id="61dd9-105">Après avoir transféré les lignes relevé, vous pouvez valider les lignes vers une feuille comptabilité correspondante.</span><span class="sxs-lookup"><span data-stu-id="61dd9-105">After transferring the statement lines, you can post the lines in a corresponding general journal.</span></span> <span data-ttu-id="61dd9-106">S'il n'existe aucune feuille comptabilité, vous ne pouvez pas transférer les lignes.</span><span class="sxs-lookup"><span data-stu-id="61dd9-106">If no such general journal exists, you cannot transfer the lines.</span></span> <span data-ttu-id="61dd9-107">Vous pouvez créer une feuille pour traiter les relevés CODA.</span><span class="sxs-lookup"><span data-stu-id="61dd9-107">You can create a journal to handle CODA statements.</span></span> <span data-ttu-id="61dd9-108">Pour plus d'informations, voir [Créer des feuilles financières](how-to-create-financial-journals.md).</span><span class="sxs-lookup"><span data-stu-id="61dd9-108">For more information, see [Create Financial Journals](how-to-create-financial-journals.md).</span></span>  

<span data-ttu-id="61dd9-109">Vous pouvez aussi transférer et valider manuellement les relevés CODA.</span><span class="sxs-lookup"><span data-stu-id="61dd9-109">Alternatively, you can manually transfer and post CODA statements.</span></span> <span data-ttu-id="61dd9-110">Pour plus d'informations, voir [Transférer et publier manuellement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="61dd9-110">For information, see [Manually Transfer and Post CODA Statements](how-to-manually-transfer-and-post-coda-statements.md).</span></span>  

## <a name="to-automatically-transfer-statement-lines"></a><span data-ttu-id="61dd9-111">Pour transférer automatiquement les lignes relevé</span><span class="sxs-lookup"><span data-stu-id="61dd9-111">To automatically transfer statement lines</span></span>  

1.  <span data-ttu-id="61dd9-112">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="61dd9-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="61dd9-113">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="61dd9-113">Select the bank account, and then choose **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="61dd9-114">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="61dd9-114">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="61dd9-115">Choisissez l'action **Transférer à FS**.</span><span class="sxs-lookup"><span data-stu-id="61dd9-115">Choose the **Transfer to General Ledger** action.</span></span>  
5.  <span data-ttu-id="61dd9-116">Cliquez sur le bouton **Oui**.</span><span class="sxs-lookup"><span data-stu-id="61dd9-116">Choose the **Yes** button.</span></span>  

<span data-ttu-id="61dd9-117">Le traitement par lots transfèrera à présent les lignes relevé CODA à la feuille financière.</span><span class="sxs-lookup"><span data-stu-id="61dd9-117">The batch job will now transfer the CODA statement lines to the financial journal.</span></span>  

<span data-ttu-id="61dd9-118">Après avoir transféré les lignes relevé vers la feuille, vous pouvez valider les lignes relevé vers la feuille financière correspondante.</span><span class="sxs-lookup"><span data-stu-id="61dd9-118">After transferring the statement lines to the journal, you can post the statement lines in the corresponding financial journal.</span></span>  

## <a name="see-also"></a><span data-ttu-id="61dd9-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="61dd9-119">See Also</span></span>  
 <span data-ttu-id="61dd9-120">[Relevés bancaires CODA](coda-bank-statements.md) </span><span class="sxs-lookup"><span data-stu-id="61dd9-120">[CODA Bank Statements](coda-bank-statements.md) </span></span>  
 <span data-ttu-id="61dd9-121">[Importer des relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="61dd9-121">[Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="61dd9-122">[Lettrer des relevés CODA](how-to-apply-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="61dd9-122">[Apply CODA Statements](how-to-apply-coda-statements.md) </span></span>  
 <span data-ttu-id="61dd9-123">[Créer des feuilles financières](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="61dd9-123">[Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 [<span data-ttu-id="61dd9-124">Transférer et publier manuellement des relevés CODA</span><span class="sxs-lookup"><span data-stu-id="61dd9-124">Manually Transfer and Post CODA Statements</span></span>](how-to-manually-transfer-and-post-coda-statements.md)
