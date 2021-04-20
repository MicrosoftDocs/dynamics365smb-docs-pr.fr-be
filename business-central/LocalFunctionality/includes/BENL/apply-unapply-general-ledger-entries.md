---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 26683f68ae60db3651d7caf3e1487a35ca867851
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779350"
---
<span data-ttu-id="60dff-101">En lettrant des écritures comptables temporaires, les sociétés peuvent utiliser des comptes temporaires et de transfert dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="60dff-101">By applying temporary general ledger entries, companies can work with temporary and transfer accounts in the general ledger.</span></span> <span data-ttu-id="60dff-102">Les comptes temporaires et de transfert sont utilisés pour stocker les écritures comptables temporaires qui sont en attente d'un traitement ultérieur dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="60dff-102">Temporary and transfer accounts are used to store temporary ledger entries that are waiting for further processing into the general ledger.</span></span>  

<span data-ttu-id="60dff-103">Vous pouvez utiliser les comptes temporaires pour :</span><span class="sxs-lookup"><span data-stu-id="60dff-103">You can use temporary accounts for:</span></span>  

- <span data-ttu-id="60dff-104">Les transferts d'argent d'un compte bancaire à un autre.</span><span class="sxs-lookup"><span data-stu-id="60dff-104">Money transfers from one bank account to another.</span></span>  
- <span data-ttu-id="60dff-105">Les transferts de transaction financière d'un système à un autre où une partie des informations réside temporairement dans le système d'origine.</span><span class="sxs-lookup"><span data-stu-id="60dff-105">Financial transaction transfers from one system to another in which part of the information temporarily resides on the original system.</span></span>  
- <span data-ttu-id="60dff-106">Les transactions pour lesquelles vous avez émis une facture vente à un client mais vous n'avez pas encore reçu la facture achat correspondante du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="60dff-106">Transactions for which you have issued a sales invoice to a customer but have not yet received the corresponding purchase invoice from the vendor.</span></span>  

<span data-ttu-id="60dff-107">Lorsque les écritures comptables ont été traitées, vous pouvez utiliser la fonction **Lettrer écritures** pour mettre à jour les écritures comptables validées et le type de compte de validation.</span><span class="sxs-lookup"><span data-stu-id="60dff-107">When the ledger entries have been processed, you can use the **Apply Entries** function to update the posted ledger entries and the posting account type.</span></span>  

<span data-ttu-id="60dff-108">Vous pouvez délettrer les écritures comptables lettrées puis ouvrir les écritures clôturées pour apporter des modifications.</span><span class="sxs-lookup"><span data-stu-id="60dff-108">You can unapply the applied general ledger entries and then open the closed entries to make changes.</span></span>  

## <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="60dff-109">Pour lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="60dff-109">To apply general ledger entries</span></span>  

1. <span data-ttu-id="60dff-110">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Historiques des transactions comptabilité**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="60dff-110">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2. <span data-ttu-id="60dff-111">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="60dff-111">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3. <span data-ttu-id="60dff-112">Dans la page **Écritures comptables**, choisissez l'action **Lettrer écritures**.</span><span class="sxs-lookup"><span data-stu-id="60dff-112">On the **General Ledger Entries** page, choose the **Apply Entries** action.</span></span>  

    <span data-ttu-id="60dff-113">Toutes les écritures comptables ouvertes pour le compte général sont affichées sur la page **Lettrer écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="60dff-113">All open ledger entries for the general ledger account are displayed on the **Apply General Ledger Entries** page.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="60dff-114">Par défaut, le champ **Inclure écritures** est défini sur **Ouvert**.</span><span class="sxs-lookup"><span data-stu-id="60dff-114">By default, the **Include Entries** field is set to **Open**.</span></span> <span data-ttu-id="60dff-115">Vous pouvez modifier la valeur du champ **Inclure écritures** sur **Tous** ou **Clôturé**.</span><span class="sxs-lookup"><span data-stu-id="60dff-115">You can change the value of the **Include Entries** field to **All** or **Closed**.</span></span> <span data-ttu-id="60dff-116">Vous pouvez lettrer uniquement les écritures comptables qui ont le statut **Ouvert**.</span><span class="sxs-lookup"><span data-stu-id="60dff-116">You can only apply general ledger entries that are **Open**.</span></span>  

4. <span data-ttu-id="60dff-117">Sélectionnez l'écriture comptable appropriée, puis choisissez l'action **Définir ID lettrage**.</span><span class="sxs-lookup"><span data-stu-id="60dff-117">Select the relevant general ledger entry, and then choose the **Set Applies-to ID** action.</span></span>  

    <span data-ttu-id="60dff-118">Le champ **ID lettrage** est mis à jour avec l'ID utilisateur.</span><span class="sxs-lookup"><span data-stu-id="60dff-118">The **Applies-to ID** field is updated with the user ID.</span></span> <span data-ttu-id="60dff-119">Le montant restant est affiché dans le champ **Solde** de la page **Lettrer écritures comptables**.</span><span class="sxs-lookup"><span data-stu-id="60dff-119">The remaining amount is displayed in the **Balance** field on the **Apply General Ledger Entries** page.</span></span>  
5. <span data-ttu-id="60dff-120">Sélectionnez l'action **Valider le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="60dff-120">Choose the **Post Application** action.</span></span>  

    <span data-ttu-id="60dff-121">Vous pouvez valider le lettrage même si le solde est égal à 0.</span><span class="sxs-lookup"><span data-stu-id="60dff-121">You can post the application even if the balance amount is equal to 0.</span></span> <span data-ttu-id="60dff-122">Une fois validé, le champ **Montant restant** est affecté comme suit :</span><span class="sxs-lookup"><span data-stu-id="60dff-122">When posted, the **Remaining Amount** field is affected as follows:</span></span>  

    - <span data-ttu-id="60dff-123">Si le **Solde** est égal à 0, le champ **Montant restant** de toutes les écritures comptables est défini sur 0.</span><span class="sxs-lookup"><span data-stu-id="60dff-123">If the **Balance** is equal to 0, then the **Remaining Amount** field on all ledger entries is set to 0.</span></span>  

    - <span data-ttu-id="60dff-124">Si le **Solde** n'est pas égal à 0, le montant du champ **Solde** est transféré vers le champ **Montant restant** pour l'écriture comptable qui a été sélectionnée lors de la validation du lettrage.</span><span class="sxs-lookup"><span data-stu-id="60dff-124">If the **Balance** is not equal to 0, then the amount in the **Balance** field is transferred to the **Remaining Amount** field for the general ledger entry that was selected when you posted the application.</span></span>  

    - <span data-ttu-id="60dff-125">Pour toutes les autres écritures comptables, le champ **Montant restant** est défini sur 0 et les champs **Ouvert**, **N° séquence lettrage final**, **Montant lettrage final** et **Date de clôture** sont mis à jour.</span><span class="sxs-lookup"><span data-stu-id="60dff-125">For all other general ledger entries, the **Remaining Amount** field is set to 0 and the **Open**, **Closed by Entry No.**, **Closed by Amount**, and **Closed at Date** fields are updated.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="60dff-126">Une fois validées, les écritures comptables qui mettent à jour le champ **ID lettrage** sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="60dff-126">When posted, the general ledger entries which update the **Applies-to ID** field are deleted.</span></span>  

6. <span data-ttu-id="60dff-127">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="60dff-127">Choose the **OK** button.</span></span>  

## <a name="to-view-the-applied-general-ledger-entries"></a><span data-ttu-id="60dff-128">Pour afficher les écritures comptables lettrées</span><span class="sxs-lookup"><span data-stu-id="60dff-128">To view the applied general ledger entries</span></span>  

1. <span data-ttu-id="60dff-129">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Historiques des transactions comptabilité**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="60dff-129">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2. <span data-ttu-id="60dff-130">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="60dff-130">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3. <span data-ttu-id="60dff-131">Sélectionnez l'écriture comptable appropriée, puis choisissez l'action **Écritures lettrées**.</span><span class="sxs-lookup"><span data-stu-id="60dff-131">Select the relevant general ledger entry, and then choose the **Applied Entries** action.</span></span>  

    <span data-ttu-id="60dff-132">Vous pouvez afficher toutes les écritures comptables lettrées.</span><span class="sxs-lookup"><span data-stu-id="60dff-132">You can view all the applied general ledger entries.</span></span>  

4. <span data-ttu-id="60dff-133">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="60dff-133">Choose the **OK** button.</span></span>  

## <a name="to-unapply-general-ledger-entries"></a><span data-ttu-id="60dff-134">Pour délettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="60dff-134">To unapply general ledger entries</span></span>  

1. Sélectionnez l'icône :::image type="icon" source="../../../media/ui-search/search_small.png" border="false":::, entrez **Historiques des transactions comptabilité**, puis choisissez le lien associé.  
2. <span data-ttu-id="60dff-136">Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="60dff-136">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3. <span data-ttu-id="60dff-137">Sélectionnez l'écriture comptable que vous souhaitez délettrer, puis choisissez l'action **Annuler le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="60dff-137">Select the general ledger entry that you want to unapply, and then choose the **Undo Application** action.</span></span>  

    <span data-ttu-id="60dff-138">Les écritures comptables lettrées sont delettrées.</span><span class="sxs-lookup"><span data-stu-id="60dff-138">The applied general ledger entries are unapplied.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="60dff-139">Si une écriture est lettrée par plusieurs écritures lettrage, vous devez commencer par délettrer la dernière écriture lettrage.</span><span class="sxs-lookup"><span data-stu-id="60dff-139">If an entry is applied to more than one application entry, you must unapply the latest application entry first.</span></span> <span data-ttu-id="60dff-140">Par défaut, la dernière écriture s'affiche.</span><span class="sxs-lookup"><span data-stu-id="60dff-140">By default, the latest entry is displayed.</span></span>  

4. <span data-ttu-id="60dff-141">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="60dff-141">Choose the **OK** button.</span></span>  
