---
title: "Comment lettrer les relevés CODA"
description: "Après l'importation d'un relevé CODA, vous pouvez accéder aux lignes relevé à partir de la fenêtre **Fiche compte bancaire**. Le statut lettrage de chaque ligne sera vide, car les montants du relevé n'ont pas été lettrés à des écritures comptables en attente."
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
ms.openlocfilehash: 0da7a0a08aeeebe5316c089538482780d82cb5d3
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="apply-coda-statements"></a><span data-ttu-id="d3eb7-104">Lettrer des relevés CODA</span><span class="sxs-lookup"><span data-stu-id="d3eb7-104">Apply CODA Statements</span></span>
<span data-ttu-id="d3eb7-105">Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la fenêtre **Fiche compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-105">After a CODA statement has been imported, the statement lines can be accessed from the **Bank Account Card** window.</span></span> <span data-ttu-id="d3eb7-106">Le statut lettrage de chaque ligne sera vide, car les montants du relevé n'ont pas été lettrés à des écritures comptables en attente.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-106">The application status on each line will be blank because the statement amounts have not been applied to outstanding ledger entries.</span></span>  

<span data-ttu-id="d3eb7-107">Les montants du relevé peuvent être lettrés à des écritures comptables en attente des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="d3eb7-107">Statement amounts can be applied to outstanding ledger entries by:</span></span>  

-   <span data-ttu-id="d3eb7-108">Lettrage manuel des lignes relevé CODA.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-108">Manually applying CODA statement lines.</span></span>  
-   <span data-ttu-id="d3eb7-109">Lettrage automatique des montants du relevé CODA aux écritures comptables et comptes adéquats.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-109">Automatically applying CODA statement amounts to the appropriate ledger entries and accounts.</span></span> <span data-ttu-id="d3eb7-110">Le traitement automatique des lignes relevé CODA est recommandé.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-110">Automatic processing of CODA statement lines is recommended.</span></span>  

## <a name="to-manually-apply-the-coda-statement-lines"></a><span data-ttu-id="d3eb7-111">Pour lettrer manuellement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="d3eb7-111">To manually apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="d3eb7-112">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d3eb7-113">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-113">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="d3eb7-114">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-114">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="d3eb7-115">Dans le raccourci **Lignes relevé CODA**, pour chaque ligne relevé, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-115">In the **CODA Statement Lines** FastTab, for each statement line, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="d3eb7-116">Champ</span><span class="sxs-lookup"><span data-stu-id="d3eb7-116">Field</span></span>|<span data-ttu-id="d3eb7-117">Description</span><span class="sxs-lookup"><span data-stu-id="d3eb7-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="d3eb7-118">**N° compte**</span><span class="sxs-lookup"><span data-stu-id="d3eb7-118">**Account No.**</span></span>|<span data-ttu-id="d3eb7-119">Entrez le numéro du compte général, la banque, le client, le fournisseur ou l'immobilisation auquel la ligne relevé compte bancaire est liée.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-119">Enter the number of the general ledger account, bank, customer, vendor, or fixed asset, which the bank account statement line is linked to.</span></span>|  
    |<span data-ttu-id="d3eb7-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3eb7-120">**Description**</span></span>|[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="d3eb7-121">récupère automatiquement la description à partir du fichier CODA importé, mais vous pouvez modifier le contenu de ce champ.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-121"> automatically retrieves the description from the imported CODA file, but you can modify the contents of this field.</span></span>|  

5.  <span data-ttu-id="d3eb7-122">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-122">Choose the **OK** button.</span></span>  

## <a name="to-automatically-apply-the-coda-statement-lines"></a><span data-ttu-id="d3eb7-123">Pour lettrer automatiquement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="d3eb7-123">To automatically apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="d3eb7-124">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d3eb7-125">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-125">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="d3eb7-126">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-126">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="d3eb7-127">Choisissez l'action **Valider lignes relevé CODA**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-127">Choose the **Process CODA Statement Lines** action.</span></span>  
5.  <span data-ttu-id="d3eb7-128">Remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-128">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="d3eb7-129">Champ</span><span class="sxs-lookup"><span data-stu-id="d3eb7-129">Field</span></span>|<span data-ttu-id="d3eb7-130">Description</span><span class="sxs-lookup"><span data-stu-id="d3eb7-130">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="d3eb7-131">**Validation par défaut**</span><span class="sxs-lookup"><span data-stu-id="d3eb7-131">**Default Posting**</span></span>|<span data-ttu-id="d3eb7-132">Définissez si vous souhaitez que le traitement par lots valide les montants du relevé qui ne peuvent pas être liés à des écritures comptables existantes.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-132">Select if you want the batch job to post statement amounts that cannot be linked to existing ledger entries.</span></span> <span data-ttu-id="d3eb7-133">Pour plus d'informations, voir Encodage CODA.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-133">For more information, see Transaction Coding.</span></span>|  
    |<span data-ttu-id="d3eb7-134">**Imprimer liste**</span><span class="sxs-lookup"><span data-stu-id="d3eb7-134">**Print List**</span></span>|<span data-ttu-id="d3eb7-135">Sélectionnez l'option d'impression d'une liste des montants du relevé qui ne peuvent pas être liés automatiquement.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-135">Select to print a list of statement amounts that cannot be linked automatically.</span></span>|  

6.  <span data-ttu-id="d3eb7-136">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-136">Choose the **OK** button.</span></span>  

    <span data-ttu-id="d3eb7-137">Lorsque vous commencez le traitements par lots, les montants du relevé seront lettrés à des écritures comptables existantes selon les codes transaction.</span><span class="sxs-lookup"><span data-stu-id="d3eb7-137">When you start the batch job, statement amounts will be applied to existing ledger entries based on the transaction codes.</span></span> <span data-ttu-id="d3eb7-138">Pour plus d'informations, reportez vous à [Configuration de comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md).</span><span class="sxs-lookup"><span data-stu-id="d3eb7-138">For more information, see [Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="d3eb7-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3eb7-139">See Also</span></span>  
 <span data-ttu-id="d3eb7-140">[Relevés bancaires CODA](coda-bank-statements.md) </span><span class="sxs-lookup"><span data-stu-id="d3eb7-140">[CODA Bank Statements](coda-bank-statements.md) </span></span>  
 <span data-ttu-id="d3eb7-141">[Configurer des comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md) </span><span class="sxs-lookup"><span data-stu-id="d3eb7-141">[Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md) </span></span>  
 <span data-ttu-id="d3eb7-142">[Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="d3eb7-142">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="d3eb7-143">[Importer des relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="d3eb7-143">[Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="d3eb7-144">[Créer des feuilles financières](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="d3eb7-144">[Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 <span data-ttu-id="d3eb7-145">[Transférer et publier automatiquement des relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="d3eb7-145">[Automatically Transfer and Post CODA Statements](how-to-automatically-transfer-and-post-coda-statements.md) </span></span>  
 [<span data-ttu-id="d3eb7-146">Transférer et publier manuellement des relevés CODA</span><span class="sxs-lookup"><span data-stu-id="d3eb7-146">Manually Transfer and Post CODA Statements</span></span>](how-to-manually-transfer-and-post-coda-statements.md)

