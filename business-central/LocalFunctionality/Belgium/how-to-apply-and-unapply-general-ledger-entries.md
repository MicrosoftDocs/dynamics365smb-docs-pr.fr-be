---
title: Lettrage et délettrage des écritures comptables
description: Le lettrage des écritures comptables temporaires permet aux sociétés d'utiliser des comptes temporaires et de transfert dans la comptabilité. Les comptes temporaires et de transfert sont utilisés pour stocker les écritures comptables temporaires qui sont en attente d'un traitement ultérieur dans la comptabilité.
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
ms.openlocfilehash: f21b23039c57a29d06a260b0abe74d8b57d00f71
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2019
ms.locfileid: "911689"
---
# <a name="apply-and-unapply-general-ledger-entries"></a><span data-ttu-id="9b97e-104">Lettrer et délettrer les écritures comptables</span><span class="sxs-lookup"><span data-stu-id="9b97e-104">Apply and Unapply General Ledger Entries</span></span>
<span data-ttu-id="9b97e-105">Le lettrage des écritures comptables temporaires permet aux sociétés d'utiliser des comptes temporaires et de transfert dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="9b97e-105">Applying temporary general ledger entries allows companies to work with temporary and transfer accounts in the general ledger.</span></span> <span data-ttu-id="9b97e-106">Les comptes temporaires et de transfert sont utilisés pour stocker les écritures comptables temporaires qui sont en attente d'un traitement ultérieur dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="9b97e-106">Temporary and transfer accounts are used to store temporary ledger entries that are waiting for further processing into the general ledger.</span></span>  

 <span data-ttu-id="9b97e-107">Vous pouvez utiliser les comptes temporaires pour :</span><span class="sxs-lookup"><span data-stu-id="9b97e-107">You can use temporary accounts for:</span></span>  

- <span data-ttu-id="9b97e-108">Les transferts d'argent d'un compte bancaire à un autre.</span><span class="sxs-lookup"><span data-stu-id="9b97e-108">Money transfers from one bank account to another.</span></span>  
- <span data-ttu-id="9b97e-109">Les transferts de transaction financière d'un système à un autre où une partie des informations réside temporairement dans le système d'origine.</span><span class="sxs-lookup"><span data-stu-id="9b97e-109">Financial transaction transfers from one system to another in which part of the information temporarily resides on the original system.</span></span>  
- <span data-ttu-id="9b97e-110">Les transactions pour lesquelles vous avez émis une facture vente à un client mais vous n'avez pas encore reçu la facture achat correspondante du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="9b97e-110">Transactions for which you have issued a sales invoice to a customer but have not yet received the corresponding purchase invoice from the vendor.</span></span>  

 <span data-ttu-id="9b97e-111">Lorsque les écritures comptables ont été traitées, vous pouvez utiliser la fonction Lettrer écritures pour mettre à jour les écritures comptables validées et le type de compte de validation.</span><span class="sxs-lookup"><span data-stu-id="9b97e-111">When the ledger entries have been processed, you can use the apply entries function to update the posted ledger entries and the posting account type.</span></span>  

 <span data-ttu-id="9b97e-112">Vous pouvez délettrer les écritures comptables lettrées puis ouvrir les écritures clôturées pour apporter des modifications.</span><span class="sxs-lookup"><span data-stu-id="9b97e-112">You can unapply the applied general ledger entries and then open the closed entries to make changes.</span></span>  

## <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="9b97e-113">Pour lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="9b97e-113">To apply general ledger entries</span></span>  

1.  <span data-ttu-id="9b97e-114">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Hist. trans. comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="9b97e-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9b97e-115">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-115">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="9b97e-116">Dans la page **Écritures comptables**, choisissez l'action **Lettrer écritures**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-116">On the **General Ledger Entries** page, choose the **Apply Entries** action.</span></span>  

    <span data-ttu-id="9b97e-117">Toutes les écritures comptables ouvertes pour le compte général sont affichées sur la page **Lettrer écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-117">All open ledger entries for the general ledger account are displayed on the **Apply General Ledger Entries** page.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9b97e-118">Par défaut, le champ **Inclure écritures** est défini sur **Ouvert**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-118">By default, the **Include Entries** field is set to **Open**.</span></span> <span data-ttu-id="9b97e-119">Vous pouvez modifier la valeur du champ **Inclure écritures** sur **Tous** ou **Clôturé**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-119">You can change the value of the **Include Entries** field to **All** or **Closed**.</span></span> <span data-ttu-id="9b97e-120">Vous pouvez lettrer uniquement les écritures comptables qui ont le statut **Ouvert**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-120">You can only apply general ledger entries that are **Open**.</span></span>  

4.  <span data-ttu-id="9b97e-121">Sélectionnez l'écriture comptable appropriée, puis, sous l'onglet **Naviguer**, dans le groupe **Lettrage**, choisissez **Lettrer**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-121">Select the relevant general ledger entry, and then, on the **Navigate** tab, in the **Application** group, choose **Set Applies-to ID**.</span></span>  

    <span data-ttu-id="9b97e-122">Le champ **ID lettrage** est mis à jour avec l'ID utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9b97e-122">The **Applies-to ID** field is updated with the user ID.</span></span> <span data-ttu-id="9b97e-123">Le montant restant est affiché dans le champ **Solde** de la page **Lettrer écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-123">The remaining amount is displayed in the **Balance** field on the **Apply General Ledger Entries** page.</span></span>  

5.  <span data-ttu-id="9b97e-124">Sélectionnez **Valider le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-124">Choose the **Post Application**.</span></span>  

    <span data-ttu-id="9b97e-125">Vous pouvez valider le lettrage même si le solde est égal à 0.</span><span class="sxs-lookup"><span data-stu-id="9b97e-125">You can post the application even if the balance amount is equal to 0.</span></span> <span data-ttu-id="9b97e-126">Une fois validé, le champ **Montant restant** est affecté comme suit :</span><span class="sxs-lookup"><span data-stu-id="9b97e-126">When posted, the **Remaining Amount** field is affected as follows:</span></span>  

    - <span data-ttu-id="9b97e-127">Si le **Solde** est égal à 0, le champ **Montant restant** de toutes les écritures comptables est défini sur 0.</span><span class="sxs-lookup"><span data-stu-id="9b97e-127">If the **Balance** is equal to 0, then the **Remaining Amount** field on all ledger entries is set to 0.</span></span>  

    - <span data-ttu-id="9b97e-128">Si le **Solde** n'est pas égal à 0, le montant du champ **Solde** est transféré vers le champ **Montant restant** pour l'écriture comptable qui a été sélectionnée lors de la validation du lettrage.</span><span class="sxs-lookup"><span data-stu-id="9b97e-128">If the **Balance** is not equal to 0, then the amount in the **Balance** field is transferred to the **Remaining Amount** field for the general ledger entry that was selected when you posted the application.</span></span>  

    - <span data-ttu-id="9b97e-129">Pour toutes les autres écritures comptables, le champ **Montant restant** est défini sur 0 et les champs **Ouvert**, **N° séquence lettrage final**, **Montant lettrage final** et **Date de clôture** sont mis à jour.</span><span class="sxs-lookup"><span data-stu-id="9b97e-129">For all other general ledger entries, the **Remaining Amount** field is set to 0 and the **Open**, **Closed by Entry No.**, **Closed by Amount**, and **Closed at Date** fields are updated.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9b97e-130">Une fois validées, les écritures comptables qui mettent à jour le champ **ID lettrage** sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="9b97e-130">When posted, the general ledger entries which update the **Applies-to ID** field are deleted.</span></span>  

6.  <span data-ttu-id="9b97e-131">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-131">Choose the **OK** button.</span></span>  

## <a name="to-view-the-applied-general-ledger-entries"></a><span data-ttu-id="9b97e-132">Pour afficher les écritures comptables lettrées</span><span class="sxs-lookup"><span data-stu-id="9b97e-132">To view the applied general ledger entries</span></span>  

1.  <span data-ttu-id="9b97e-133">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Hist. trans. comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="9b97e-133">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9b97e-134">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-134">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="9b97e-135">Sélectionnez l'écriture comptable appropriée, puis choisissez l'action **Écritures lettrées**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-135">Select the relevant general ledger entry, and then choose the **Applied Entries** action.</span></span>  

    <span data-ttu-id="9b97e-136">Vous pouvez afficher toutes les écritures comptables lettrées.</span><span class="sxs-lookup"><span data-stu-id="9b97e-136">You can view all the applied general ledger entries.</span></span>  

4.  <span data-ttu-id="9b97e-137">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-137">Choose the **OK** button.</span></span>  

## <a name="to-unapply-general-ledger-entries"></a><span data-ttu-id="9b97e-138">Pour délettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="9b97e-138">To unapply general ledger entries</span></span>  

1.  <span data-ttu-id="9b97e-139">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Hist. trans. comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="9b97e-139">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9b97e-140">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-140">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="9b97e-141">Sélectionnez l'écriture comptable que vous souhaitez délettrer, puis choisissez l'action **Annuler le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-141">Select the general ledger entry that you want to unapply, and then choose the **Undo Application** action.</span></span>  

    <span data-ttu-id="9b97e-142">Les écritures comptables lettrées sont delettrées.</span><span class="sxs-lookup"><span data-stu-id="9b97e-142">The applied general ledger entries are unapplied.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9b97e-143">Si une écriture est lettrée par plusieurs écritures lettrage, vous devez commencer par délettrer la dernière écriture lettrage.</span><span class="sxs-lookup"><span data-stu-id="9b97e-143">If an entry is applied to more than one application entry, you must unapply the latest application entry first.</span></span> <span data-ttu-id="9b97e-144">Par défaut, la dernière écriture s'affiche.</span><span class="sxs-lookup"><span data-stu-id="9b97e-144">By default, the latest entry is displayed.</span></span>  

4.  <span data-ttu-id="9b97e-145">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="9b97e-145">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9b97e-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9b97e-146">See Also</span></span>  
[<span data-ttu-id="9b97e-147">Fonctionnalité locale, Belgique</span><span class="sxs-lookup"><span data-stu-id="9b97e-147">Belgium Local Functionality</span></span>](belgium-local-functionality.md)
