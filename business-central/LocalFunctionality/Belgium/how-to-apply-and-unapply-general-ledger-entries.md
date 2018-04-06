---
title: "Comment lettrer et délettrer des écritures comptables"
description: "Le lettrage d'écritures comptables permet aux sociétés de travailler avec des comptes temporaires et de transfert dans la comptabilité. Les comptes temporaires et les comptes de transfert sont utilisés pour stocker les écritures comptables temporaires en attente d'un traitement ultérieur dans le grand livre."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 220bc78e7dda958a931bb8c8c4ef904a687d905e
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="apply-and-unapply-general-ledger-entries"></a><span data-ttu-id="b10f1-104">Lettrer et délettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="b10f1-104">Apply and Unapply General Ledger Entries</span></span>
<span data-ttu-id="b10f1-105">Le lettrage d'écritures comptables temporaires permet aux entreprises de travailler avec des comptes temporaires et des comptes de transfert dans le grand livre.</span><span class="sxs-lookup"><span data-stu-id="b10f1-105">Applying temporary general ledger entries allows companies to work with temporary and transfer accounts in the general ledger.</span></span> <span data-ttu-id="b10f1-106">Les comptes temporaires et de transfert sont utilisés pour répertorier les écritures comptables en attente de traitement dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="b10f1-106">Temporary and transfer accounts are used to store temporary ledger entries that are waiting for further processing into the general ledger.</span></span>  

 <span data-ttu-id="b10f1-107">Vous pouvez utiliser les comptes temporaires pour :</span><span class="sxs-lookup"><span data-stu-id="b10f1-107">You can use temporary accounts for:</span></span>  

- <span data-ttu-id="b10f1-108">Les transferts d'argent d'un compte bancaire à l'autre.</span><span class="sxs-lookup"><span data-stu-id="b10f1-108">Money transfers from one bank account to another.</span></span>  
- <span data-ttu-id="b10f1-109">Les transferts de transactions financières d'un système à l'autre, dans lesquels une partie des informations est temporairement hébergée dans le système d'origine.</span><span class="sxs-lookup"><span data-stu-id="b10f1-109">Financial transaction transfers from one system to another in which part of the information temporarily resides on the original system.</span></span>  
- <span data-ttu-id="b10f1-110">Les transactions pour lesquelles vous avez émis une facture vente à un client, mais n'avez pas encore reçu la facture achat correspondante du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="b10f1-110">Transactions for which you have issued a sales invoice to a customer but have not yet received the corresponding purchase invoice from the vendor.</span></span>  

 <span data-ttu-id="b10f1-111">Lorsque les écritures comptables ont été traitées, vous pouvez utiliser la fonction de lettrage des écritures pour mettre à jour les écritures comptables validées et le type de compte de validation.</span><span class="sxs-lookup"><span data-stu-id="b10f1-111">When the ledger entries have been processed, you can use the apply entries function to update the posted ledger entries and the posting account type.</span></span>  

 <span data-ttu-id="b10f1-112">Vous pouvez délettrer les écritures comptables lettrées, puis ouvrir les écritures clôturées pour effectuer les modifications.</span><span class="sxs-lookup"><span data-stu-id="b10f1-112">You can unapply the applied general ledger entries and then open the closed entries to make changes.</span></span>  

## <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="b10f1-113">Pour lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="b10f1-113">To apply general ledger entries</span></span>  

1.  <span data-ttu-id="b10f1-114">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Historiques des transactions comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="b10f1-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b10f1-115">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-115">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="b10f1-116">Dans la fenêtre **Écritures comptables**, choisissez l'action **Lettrer écritures**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-116">In the **General Ledger Entries** window, choose the **Apply Entries** action.</span></span>  

    <span data-ttu-id="b10f1-117">Toutes les écritures comptables ouvertes pour le compte général s'affichent dans la fenêtre **Lettrer écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-117">All open ledger entries for the general ledger account are displayed in the **Apply General Ledger Entries** window.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="b10f1-118">Par défaut, le champ **Inclure écritures** est défini sur **Ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-118">By default, the **Include Entries** field is set to **Open**.</span></span> <span data-ttu-id="b10f1-119">Vous pouvez modifier la valeur du champ **Inclure écritures** et la définir sur **Toutes** ou **Clôturées**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-119">You can change the value of the **Include Entries** field to **All** or **Closed**.</span></span> <span data-ttu-id="b10f1-120">Vous pouvez uniquement lettrer les écritures comptables qui sont **Ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-120">You can only apply general ledger entries that are **Open**.</span></span>  

4.  <span data-ttu-id="b10f1-121">Sélectionnez l'écriture comptable concernée, puis, dans l'onglet **Naviguer**, dans le groupe **Lettrage**, sélectionnez **Définir ID lettrage**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-121">Select the relevant general ledger entry, and then, on the **Navigate** tab, in the **Application** group, choose **Set Applies-to ID**.</span></span>  

    <span data-ttu-id="b10f1-122">Le champ **Définir ID lettrage** est mis à jour avec le code utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b10f1-122">The **Applies-to ID** field is updated with the user ID.</span></span> <span data-ttu-id="b10f1-123">Le montant restant s'affiche dans le champ **Solde** dans la fenêtre **Lettrer écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-123">The remaining amount is displayed in the **Balance** field in the **Apply General Ledger Entries** window.</span></span>  

5.  <span data-ttu-id="b10f1-124">Choisissez **Valider le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-124">Choose the **Post Application**.</span></span>  

    <span data-ttu-id="b10f1-125">Vous pouvez valider le lettrage même si le solde est nul.</span><span class="sxs-lookup"><span data-stu-id="b10f1-125">You can post the application even if the balance amount is equal to 0.</span></span> <span data-ttu-id="b10f1-126">Après la validation, le champ **Montant restant** est affecté comme suit :</span><span class="sxs-lookup"><span data-stu-id="b10f1-126">When posted, the **Remaining Amount** field is affected as follows:</span></span>  

    - <span data-ttu-id="b10f1-127">Si le **Solde** est nul, le champ **Montant restant** de toutes les écritures comptables est défini sur 0.</span><span class="sxs-lookup"><span data-stu-id="b10f1-127">If the **Balance** is equal to 0, then the **Remaining Amount** field on all ledger entries is set to 0.</span></span>  

    - <span data-ttu-id="b10f1-128">Si le **Solde** n'est pas nul, le montant figurant dans le champ **Solde** est transféré au champ **Montant restant** pour l'écriture comptable qui était sélectionnée lorsque vous avez validé le lettrage.</span><span class="sxs-lookup"><span data-stu-id="b10f1-128">If the **Balance** is not equal to 0, then the amount in the **Balance** field is transferred to the **Remaining Amount** field for the general ledger entry that was selected when you posted the application.</span></span>  

    - <span data-ttu-id="b10f1-129">Pour toutes les autres écritures comptables, le champ **Montant restant** est nul, et les champs **Ouvertes**, **N° séquence lettrage final**, **Montant lettrage final** et **Date de clôture** sont mis à jour.</span><span class="sxs-lookup"><span data-stu-id="b10f1-129">For all other general ledger entries, the **Remaining Amount** field is set to 0 and the **Open**, **Closed by Entry No.**, **Closed by Amount**, and **Closed at Date** fields are updated.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="b10f1-130">Lors de la validation, les écritures comptables qui mettent à jour le champ **ID lettrage** sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="b10f1-130">When posted, the general ledger entries which update the **Applies-to ID** field are deleted.</span></span>  

6.  <span data-ttu-id="b10f1-131">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-131">Choose the **OK** button.</span></span>  

## <a name="to-view-the-applied-general-ledger-entries"></a><span data-ttu-id="b10f1-132">Pour afficher les écritures comptables lettrées</span><span class="sxs-lookup"><span data-stu-id="b10f1-132">To view the applied general ledger entries</span></span>  

1.  <span data-ttu-id="b10f1-133">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Historiques des transactions comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="b10f1-133">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b10f1-134">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-134">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="b10f1-135">Sélectionnez l'écriture comptabilité pertinente, puis choisissez l'action **Écritures lettrées**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-135">Select the relevant general ledger entry, and then choose the **Applied Entries** action.</span></span>  

    <span data-ttu-id="b10f1-136">Vous pouvez afficher toutes les écritures comptables lettrées.</span><span class="sxs-lookup"><span data-stu-id="b10f1-136">You can view all the applied general ledger entries.</span></span>  

4.  <span data-ttu-id="b10f1-137">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-137">Choose the **OK** button.</span></span>  

## <a name="to-unapply-general-ledger-entries"></a><span data-ttu-id="b10f1-138">Pour délettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="b10f1-138">To unapply general ledger entries</span></span>  

1.  <span data-ttu-id="b10f1-139">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Historiques des transactions comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="b10f1-139">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b10f1-140">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-140">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="b10f1-141">Sélectionnez l'écriture comptable que vous souhaitez délettrer, puis choisissez l'action **Annuler le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-141">Select the general ledger entry that you want to unapply, and then choose the **Undo Application** action.</span></span>  

    <span data-ttu-id="b10f1-142">Les écritures comptables lettrées sont délettrées.</span><span class="sxs-lookup"><span data-stu-id="b10f1-142">The applied general ledger entries are unapplied.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="b10f1-143">Si une écriture est lettrée à une ou plusieurs écritures de lettrage, vous devez délettrer la dernière écriture de lettrage en premier.</span><span class="sxs-lookup"><span data-stu-id="b10f1-143">If an entry is applied to more than one application entry, you must unapply the latest application entry first.</span></span> <span data-ttu-id="b10f1-144">Par défaut, la dernière écriture s'affiche.</span><span class="sxs-lookup"><span data-stu-id="b10f1-144">By default, the latest entry is displayed.</span></span>  

4.  <span data-ttu-id="b10f1-145">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="b10f1-145">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b10f1-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b10f1-146">See Also</span></span>  
[<span data-ttu-id="b10f1-147">Fonctionnalité locale pour la Belgique</span><span class="sxs-lookup"><span data-stu-id="b10f1-147">Belgium Local Functionality</span></span>](belgium-local-functionality.md)

