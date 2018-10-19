---
title: "Annuler une validation en validant une écriture opposée| Microsoft Docs"
description: "Si vous avez effectué une validation erronée dans la feuille comptabilité, vous pouvez utiliser la fonction de contrepassation de transaction pour annuler la validation avec une piste d'audit correcte."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: beed335b93ef9211e4fc53c25f97b3fed6137348
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="reverse-postings"></a><span data-ttu-id="a9741-103">Inversion d'une validation</span><span class="sxs-lookup"><span data-stu-id="a9741-103">Reverse Postings</span></span>
<span data-ttu-id="a9741-104">Pour annuler une validation feuille erronée, sélectionnez l'écriture et créez une écriture inverse (écritures identiques aux écritures originales mais avec le signe opposé) portant les mêmes numéro de document et date comptabilisation que l'écriture d'origine.</span><span class="sxs-lookup"><span data-stu-id="a9741-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="a9741-105">Une fois l'écriture contrepassée, créez l'écriture correcte.</span><span class="sxs-lookup"><span data-stu-id="a9741-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="a9741-106">Vous pouvez uniquement inverser les écritures validées à partir d'une ligne feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="a9741-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="a9741-107">Une écriture ne peut être contrepassée qu'une fois.</span><span class="sxs-lookup"><span data-stu-id="a9741-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="a9741-108">Pour plus d'informations sur la validation d'une feuille comptabilité, voir [Valider les transactions directement vers la comptabilité](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="a9741-108">For more information about posting from a general journal, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="a9741-109">Si vous avez effectué une validation de quantité négative incorrecte, comme une commande achat avec, par exemple, un nombre d'articles incorrect et que vous l'avez validée comme étant reçue (mais non facturée), vous pouvez annuler cette validation.</span><span class="sxs-lookup"><span data-stu-id="a9741-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span></span>

<span data-ttu-id="a9741-110">Si vous avez effectué une validation de quantité positive incorrecte, comme une commande retour achat avec, par exemple, un nombre d'articles incorrect et que vous l'avez validée comme étant livrée (mais non facturée), vous pouvez annuler cette validation.</span><span class="sxs-lookup"><span data-stu-id="a9741-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span></span>   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="a9741-111">Pour contrepasser la validation feuille d'une écriture comptable</span><span class="sxs-lookup"><span data-stu-id="a9741-111">To reverse the journal posting of a general ledger entry</span></span>
<span data-ttu-id="a9741-112">Vous pouvez inverser des écritures dans toutes les fenêtres **Écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="a9741-112">You can reverse entries from all **Ledger Entries** windows.</span></span> <span data-ttu-id="a9741-113">La procédure suivante se base dans la fenêtre **Écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="a9741-113">The following procedure is based in the **General Ledger Entries** window.</span></span>
1. <span data-ttu-id="a9741-114">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Écritures comptables**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="a9741-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="a9741-115">Sélectionnez l'écriture à contrepasser, puis cliquez sur l'action **Contrepasser la transaction**.</span><span class="sxs-lookup"><span data-stu-id="a9741-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="a9741-116">Notez que cela doit être émis depuis une validation feuille.</span><span class="sxs-lookup"><span data-stu-id="a9741-116">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="a9741-117">Dans la fenêtre **Contrepasser les écritures de transaction**, sélectionnez l'écriture voulue, puis sélectionnez l'action **Contrepasser**.</span><span class="sxs-lookup"><span data-stu-id="a9741-117">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="a9741-118">Cliquez sur le bouton **Oui** dans le message de confirmation.</span><span class="sxs-lookup"><span data-stu-id="a9741-118">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a><span data-ttu-id="a9741-119">Pour annuler une validation de quantité sur une réception d'achat enregistrée</span><span class="sxs-lookup"><span data-stu-id="a9741-119">To undo a quantity posting on a posted purchase receipt</span></span>  

1.  <span data-ttu-id="a9741-120">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Réceptions achat enregistrées**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="a9741-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a9741-121">Ouvrez la réception enregistrée à annuler.</span><span class="sxs-lookup"><span data-stu-id="a9741-121">Open the posted receipt that you want to undo.</span></span>  
3.  <span data-ttu-id="a9741-122">Sélectionnez la ligne ou les lignes à annuler.</span><span class="sxs-lookup"><span data-stu-id="a9741-122">Select the line or lines that you want to undo.</span></span>  
4.  <span data-ttu-id="a9741-123">Choisissez l'action **Annuler réception**.</span><span class="sxs-lookup"><span data-stu-id="a9741-123">Choose **Undo Receipt** action.</span></span>

    <span data-ttu-id="a9741-124">Une ligne de correction est insérée sous la ligne de la réception sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="a9741-124">A corrective line is inserted under the selected receipt line.</span></span>  

    <span data-ttu-id="a9741-125">Si la quantité a été reçue dans une réception entrepôt, une ligne de correction est insérée dans la réception entrepôt enregistrée.</span><span class="sxs-lookup"><span data-stu-id="a9741-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span></span>  

    <span data-ttu-id="a9741-126">Les champs **Quantité reçue** et **Qté reçue non facturée** de la commande achat associée sont remis à zéro.</span><span class="sxs-lookup"><span data-stu-id="a9741-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span></span>

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a><span data-ttu-id="a9741-127">Pour annuler, puis effectuer à nouveau la validation de quantité sur les expéditions retour enregistrées</span><span class="sxs-lookup"><span data-stu-id="a9741-127">To undo and then redo a quantity posting on a posted return shipment</span></span>

1.  <span data-ttu-id="a9741-128">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Expéditions retour enreg.**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="a9741-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Return Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a9741-129">Ouvrez l'expédition retour validée à annuler.</span><span class="sxs-lookup"><span data-stu-id="a9741-129">Open the posted return shipment that you want to undo.</span></span>
3. <span data-ttu-id="a9741-130">Sélectionnez la ligne ou les lignes à annuler.</span><span class="sxs-lookup"><span data-stu-id="a9741-130">Select the line or lines you want to undo.</span></span>  

4.  <span data-ttu-id="a9741-131">Choisissez l'action **Annuler expédition retour**.</span><span class="sxs-lookup"><span data-stu-id="a9741-131">Choose the **Undo Return Shipment** action.</span></span>  

    <span data-ttu-id="a9741-132">Une ligne de correction est insérée dans le document validé et les champs **Qté retour expédiée** et **Expédition retour non facturée** du retour sont remis à zéro.</span><span class="sxs-lookup"><span data-stu-id="a9741-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span></span>  

    <span data-ttu-id="a9741-133">Retournez à présent au retour achat pour une nouvelle validation.</span><span class="sxs-lookup"><span data-stu-id="a9741-133">Now go back to the purchase return order to redo the posting.</span></span>  

5.  <span data-ttu-id="a9741-134">Dans la fenêtre **Expédition retour enregistrée**, notez le numéro situé dans le champ **N° retour**</span><span class="sxs-lookup"><span data-stu-id="a9741-134">In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.**</span></span> <span data-ttu-id="a9741-135">.</span><span class="sxs-lookup"><span data-stu-id="a9741-135">field.</span></span>  
6.  <span data-ttu-id="a9741-136">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Retours achat**, et sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="a9741-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Return Orders**, and then select the related link.</span></span>  
7.  <span data-ttu-id="a9741-137">Ouvrez la commande retour concernée, puis sélectionnez l'action **Rouvrir**.</span><span class="sxs-lookup"><span data-stu-id="a9741-137">Open the return order in question, and then choose the **Reopen** action.</span></span>  
8.  <span data-ttu-id="a9741-138">Corrigez l'écriture dans le champ **Quantité** et publiez à nouveau le retour achat.</span><span class="sxs-lookup"><span data-stu-id="a9741-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span></span>  

## <a name="to-post-a-negative-entry"></a><span data-ttu-id="a9741-139">Pour valider une écriture négative</span><span class="sxs-lookup"><span data-stu-id="a9741-139">To post a negative entry</span></span>  
<span data-ttu-id="a9741-140">Vous pouvez utiliser le champ **Correction** pour valider un débit négatif au lieu d'un crédit, ou pour valider un crédit négatif au lieu d'un débit sur un compte.</span><span class="sxs-lookup"><span data-stu-id="a9741-140">You can use the **Correction** field to post a negative debit instead of a credit, or to post a negative credit instead of a debit on an account.</span></span> <span data-ttu-id="a9741-141">Pour répondre aux exigences légales, ce champ est visible par défaut sur toutes les feuilles.</span><span class="sxs-lookup"><span data-stu-id="a9741-141">To meet legal requirements, this field is visible by default in all journals.</span></span> <span data-ttu-id="a9741-142">Les champs **Montant débit** et **Montant crédit** comprennent l'écriture initiale et l'écriture corrigée.</span><span class="sxs-lookup"><span data-stu-id="a9741-142">The **Debit Amount** and **Credit Amount** fields include both the original entry, and the corrected entry.</span></span> <span data-ttu-id="a9741-143">Ces champs n'ont aucune incidence sur le solde du compte.</span><span class="sxs-lookup"><span data-stu-id="a9741-143">These fields have no effect on the account balance.</span></span>  

1.  <span data-ttu-id="a9741-144">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles comptabilité**, puis sélectionnez le lien associé</span><span class="sxs-lookup"><span data-stu-id="a9741-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link</span></span>  
2.  <span data-ttu-id="a9741-145">Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille requis.</span><span class="sxs-lookup"><span data-stu-id="a9741-145">In the **Batch Name** field, select the required batch name.</span></span>  
3.  <span data-ttu-id="a9741-146">Entrez les informations dans les champs pertinents.</span><span class="sxs-lookup"><span data-stu-id="a9741-146">Enter information into the relevant fields.</span></span>  
4.  <span data-ttu-id="a9741-147">Dans la ligne feuille que vous souhaitez activer pour les écritures négatives, sélectionnez la case à cocher **Correction**.</span><span class="sxs-lookup"><span data-stu-id="a9741-147">In the journal line that you want to activate for negative entries, select the **Correction** check box.</span></span>  
5.  <span data-ttu-id="a9741-148">Pour valider la feuille, sélectionnez l'action **Valider**, puis le bouton **Oui**.</span><span class="sxs-lookup"><span data-stu-id="a9741-148">To post the journal, choose the **Post** action, and then choose the **Yes** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="a9741-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a9741-149">See Also</span></span>
[<span data-ttu-id="a9741-150">Valider les transactions directement vers la comptabilité</span><span class="sxs-lookup"><span data-stu-id="a9741-150">Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="a9741-151">Utilisation de feuilles comptabilité</span><span class="sxs-lookup"><span data-stu-id="a9741-151">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="a9741-152">Finances</span><span class="sxs-lookup"><span data-stu-id="a9741-152">Finance</span></span>](finance.md)  
<span data-ttu-id="a9741-153">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a9741-153">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

