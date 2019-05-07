---
title: Lettrage des relevés CODA
description: Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la page Fiche compte bancaire. Le statut de lettrage sur chaque ligne est vide, car les montants du relevé n'ont pas été lettrés aux écritures comptables ouvertes.
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
ms.openlocfilehash: 2b4a1da4a92cdd10301c14c15384737af51d902f
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2019
ms.locfileid: "921817"
---
# <a name="apply-coda-statements"></a><span data-ttu-id="b2cb5-104">Lettrer les relevés CODA</span><span class="sxs-lookup"><span data-stu-id="b2cb5-104">Apply CODA Statements</span></span>
<span data-ttu-id="b2cb5-105">Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la page **Fiche compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-105">After a CODA statement has been imported, the statement lines can be accessed from the **Bank Account Card** page.</span></span> <span data-ttu-id="b2cb5-106">Le statut de lettrage sur chaque ligne est vide, car les montants du relevé n'ont pas été lettrés aux écritures comptables ouvertes.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-106">The application status on each line will be blank because the statement amounts have not been applied to outstanding ledger entries.</span></span>  

<span data-ttu-id="b2cb5-107">Les montants du relevé peuvent être lettrés aux écritures comptables ouvertes comme suit :</span><span class="sxs-lookup"><span data-stu-id="b2cb5-107">Statement amounts can be applied to outstanding ledger entries by:</span></span>  

-   <span data-ttu-id="b2cb5-108">En lettrant manuellement les lignes relevé CODA.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-108">Manually applying CODA statement lines.</span></span>  
-   <span data-ttu-id="b2cb5-109">En lettrant automatiquement les montants du relevé CODA aux écritures comptables et aux comptes appropriés.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-109">Automatically applying CODA statement amounts to the appropriate ledger entries and accounts.</span></span> <span data-ttu-id="b2cb5-110">Le traitement automatique des lignes relevé CODA est recommandé.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-110">Automatic processing of CODA statement lines is recommended.</span></span>  

## <a name="to-manually-apply-the-coda-statement-lines"></a><span data-ttu-id="b2cb5-111">Pour lettrer manuellement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="b2cb5-111">To manually apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="b2cb5-112">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b2cb5-113">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-113">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="b2cb5-114">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-114">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="b2cb5-115">Dans le raccourci **Lignes relevé CODA**, pour chaque ligne relevé, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-115">In the **CODA Statement Lines** FastTab, for each statement line, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="b2cb5-116">Champ</span><span class="sxs-lookup"><span data-stu-id="b2cb5-116">Field</span></span>|<span data-ttu-id="b2cb5-117">Désignation</span><span class="sxs-lookup"><span data-stu-id="b2cb5-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="b2cb5-118">**N° compte**</span><span class="sxs-lookup"><span data-stu-id="b2cb5-118">**Account No.**</span></span>|<span data-ttu-id="b2cb5-119">Entrez le numéro du compte général, de la banque, du client, du fournisseur ou de l'immobilisation, auquel la ligne relevé du compte bancaire est associée.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-119">Enter the number of the general ledger account, bank, customer, vendor, or fixed asset, which the bank account statement line is linked to.</span></span>|  
    |<span data-ttu-id="b2cb5-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="b2cb5-120">**Description**</span></span>|[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="b2cb5-121">récupère automatiquement la description à partir du fichier CODA importé, mais vous pouvez modifier le contenu de ce champ.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-121">automatically retrieves the description from the imported CODA file, but you can modify the contents of this field.</span></span>|  

5.  <span data-ttu-id="b2cb5-122">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-122">Choose the **OK** button.</span></span>  

## <a name="to-automatically-apply-the-coda-statement-lines"></a><span data-ttu-id="b2cb5-123">Pour lettrer automatiquement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="b2cb5-123">To automatically apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="b2cb5-124">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b2cb5-125">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-125">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="b2cb5-126">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-126">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="b2cb5-127">Choisissez l'action **Traiter les lignes relevé CODA**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-127">Choose the **Process CODA Statement Lines** action.</span></span>  
5.  <span data-ttu-id="b2cb5-128">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-128">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="b2cb5-129">Champ</span><span class="sxs-lookup"><span data-stu-id="b2cb5-129">Field</span></span>|<span data-ttu-id="b2cb5-130">Désignation</span><span class="sxs-lookup"><span data-stu-id="b2cb5-130">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="b2cb5-131">**Comptabilisation par défaut**</span><span class="sxs-lookup"><span data-stu-id="b2cb5-131">**Default Posting**</span></span>|<span data-ttu-id="b2cb5-132">Sélectionnez ce champ si vous souhaitez que le traitement par lots valide les montants du relevé qui ne peuvent pas être associés aux écritures comptables existantes.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-132">Select if you want the batch job to post statement amounts that cannot be linked to existing ledger entries.</span></span> <span data-ttu-id="b2cb5-133">Pour plus d'informations, voir Codage des transactions.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-133">For more information, see Transaction Coding.</span></span>|  
    |<span data-ttu-id="b2cb5-134">**Imprimer liste**</span><span class="sxs-lookup"><span data-stu-id="b2cb5-134">**Print List**</span></span>|<span data-ttu-id="b2cb5-135">Sélectionnez ce champ pour imprimer la liste des montants du relevé qui ne peuvent pas être associés automatiquement.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-135">Select to print a list of statement amounts that cannot be linked automatically.</span></span>|  

6.  <span data-ttu-id="b2cb5-136">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-136">Choose the **OK** button.</span></span>  

    <span data-ttu-id="b2cb5-137">Lorsque vous démarrez le traitement par lots, les montants du relevé sont lettrés aux écritures comptables existantes en fonction des codes transaction.</span><span class="sxs-lookup"><span data-stu-id="b2cb5-137">When you start the batch job, statement amounts will be applied to existing ledger entries based on the transaction codes.</span></span> <span data-ttu-id="b2cb5-138">Pour plus d'informations, voir [Paramétrer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md).</span><span class="sxs-lookup"><span data-stu-id="b2cb5-138">For more information, see [Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="b2cb5-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b2cb5-139">See Also</span></span>  
 <span data-ttu-id="b2cb5-140">[Relevés bancaires CODA](coda-bank-statements.md) </span><span class="sxs-lookup"><span data-stu-id="b2cb5-140">[CODA Bank Statements](coda-bank-statements.md) </span></span>  
 <span data-ttu-id="b2cb5-141">[Paramétrer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md) </span><span class="sxs-lookup"><span data-stu-id="b2cb5-141">[Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md) </span></span>  
 <span data-ttu-id="b2cb5-142">[Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="b2cb5-142">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="b2cb5-143">[Importer les relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="b2cb5-143">[Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="b2cb5-144">[Créer des journaux financiers](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="b2cb5-144">[Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 <span data-ttu-id="b2cb5-145">[Transférer et valider automatiquement les relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="b2cb5-145">[Automatically Transfer and Post CODA Statements](how-to-automatically-transfer-and-post-coda-statements.md) </span></span>  
 [<span data-ttu-id="b2cb5-146">Transférer et valider manuellement les relevés CODA</span><span class="sxs-lookup"><span data-stu-id="b2cb5-146">Manually Transfer and Post CODA Statements</span></span>](how-to-manually-transfer-and-post-coda-statements.md)
