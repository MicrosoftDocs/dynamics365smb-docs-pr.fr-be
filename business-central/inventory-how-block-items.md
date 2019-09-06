---
title: Comment bloquer des articles pour la vente ou pour l'achat
description: Dans Business Central, un article peut être signalé comme bloqué pour la vente, bloqué pour l'achat ou bloqué dans tous les cas.
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
ms.openlocfilehash: 8c98e4b893783c795a49e05ab04dc70b03161c6a
ms.sourcegitcommit: bf5f89dfaf5ad9f8f9902941cf3dac3e9f3553e5
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 05/22/2019
ms.locfileid: "1594276"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="71dd4-103">Bloquer des articles pour la vente ou pour l'achat</span><span class="sxs-lookup"><span data-stu-id="71dd4-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="71dd4-104">Vous pouvez bloquer un article pour la saisie dans des lignes de vente ou d'achat, et vous pouvez le bloquer pour la validation dans n'importe quelle transaction.</span><span class="sxs-lookup"><span data-stu-id="71dd4-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="71dd4-105">Le tableau suivant illustre ce qui se produit lorsque les articles sont bloqués.</span><span class="sxs-lookup"><span data-stu-id="71dd4-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="71dd4-106">Option</span><span class="sxs-lookup"><span data-stu-id="71dd4-106">Option</span></span>|<span data-ttu-id="71dd4-107">Désignation</span><span class="sxs-lookup"><span data-stu-id="71dd4-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="71dd4-108">**Bloqué à la vente**</span><span class="sxs-lookup"><span data-stu-id="71dd4-108">**Sales Blocked**</span></span>|<span data-ttu-id="71dd4-109">Vous ne pouvez pas saisir l'article dans un document vente ou dans une feuille article vente.</span><span class="sxs-lookup"><span data-stu-id="71dd4-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="71dd4-110">**Bloqué à l'achat**</span><span class="sxs-lookup"><span data-stu-id="71dd4-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="71dd4-111">Vous ne pouvez pas saisir l'article dans un document achat, dans une feuille article d'achat, ou dans les processus de planification achat.</span><span class="sxs-lookup"><span data-stu-id="71dd4-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="71dd4-112">**Bloqué**</span><span class="sxs-lookup"><span data-stu-id="71dd4-112">**Blocked**</span></span>|<span data-ttu-id="71dd4-113">Vous ne pouvez pas utiliser l'article pour une transaction d'article.</span><span class="sxs-lookup"><span data-stu-id="71dd4-113">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="71dd4-114">Les articles bloqués peuvent être retournés.</span><span class="sxs-lookup"><span data-stu-id="71dd4-114">Blocked items can be returned.</span></span> <span data-ttu-id="71dd4-115">Cela signifie qu'aucun des paramètres ci-dessus ne s'applique lorsque l'article est utilisé sur des commandes retour et des avoirs.</span><span class="sxs-lookup"><span data-stu-id="71dd4-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="71dd4-116">Pour bloquer un article pour la saisie sur des lignes vente</span><span class="sxs-lookup"><span data-stu-id="71dd4-116">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="71dd4-117">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Articles**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="71dd4-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="71dd4-118">Sélectionnez l'article que vous souhaitez bloquer, puis sélectionnez la case à cocher **Bloqué à la vente**.</span><span class="sxs-lookup"><span data-stu-id="71dd4-118">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="71dd4-119">Si vous essayez de saisir l'article sur un document vente ou une ligne feuille, vous recevez désormais un message d'erreur indiquant que l'article est bloqué.</span><span class="sxs-lookup"><span data-stu-id="71dd4-119">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="71dd4-120">Pour bloquer un article pour la saisie sur des lignes achat</span><span class="sxs-lookup"><span data-stu-id="71dd4-120">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="71dd4-121">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Articles**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="71dd4-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="71dd4-122">Sélectionnez l'article que vous souhaitez bloquer, puis sélectionnez la case à cocher **Bloqué à l'achat**.</span><span class="sxs-lookup"><span data-stu-id="71dd4-122">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="71dd4-123">Si vous essayez de saisir l'article sur un document achat ou une ligne feuille, vous recevez désormais un message d'erreur indiquant que l'article est bloqué.</span><span class="sxs-lookup"><span data-stu-id="71dd4-123">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="71dd4-124">Pour bloquer un article à valider</span><span class="sxs-lookup"><span data-stu-id="71dd4-124">To block an item from being posted</span></span>
1. <span data-ttu-id="71dd4-125">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Articles**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="71dd4-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="71dd4-126">Sélectionnez l'article que vous souhaitez bloquer, puis sélectionnez la case à cocher **Bloqué**.</span><span class="sxs-lookup"><span data-stu-id="71dd4-126">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="71dd4-127">Si vous essayez de valider tout type de transaction pour l'article, un message d'erreur indiquant que l'article est bloqué s'affiche désormais.</span><span class="sxs-lookup"><span data-stu-id="71dd4-127">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="71dd4-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71dd4-128">See Also</span></span>  
[<span data-ttu-id="71dd4-129">Enregistrer de nouveaux articles</span><span class="sxs-lookup"><span data-stu-id="71dd4-129">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="71dd4-130">STOCKS ET EN-COURS</span><span class="sxs-lookup"><span data-stu-id="71dd4-130">Inventory</span></span>](inventory-manage-inventory.md)  