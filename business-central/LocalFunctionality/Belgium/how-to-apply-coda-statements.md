---
title: Lettrage des relevés CODA
description: Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la page Fiche compte bancaire. Le statut de lettrage sur chaque ligne est vide, car les montants du relevé n'ont pas été lettrés aux écritures comptables ouvertes.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 9df39e10efd1c5a040e1f5a7c162d32b41066971
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379578"
---
# <a name="apply-coda-statements"></a><span data-ttu-id="5abcb-104">Lettrer les relevés CODA</span><span class="sxs-lookup"><span data-stu-id="5abcb-104">Apply CODA Statements</span></span>
<span data-ttu-id="5abcb-105">Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la page **Fiche compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-105">After a CODA statement has been imported, the statement lines can be accessed from the **Bank Account Card** page.</span></span> <span data-ttu-id="5abcb-106">Le statut de lettrage sur chaque ligne est vide, car les montants du relevé n'ont pas été lettrés aux écritures comptables ouvertes.</span><span class="sxs-lookup"><span data-stu-id="5abcb-106">The application status on each line will be blank because the statement amounts have not been applied to outstanding ledger entries.</span></span>  

<span data-ttu-id="5abcb-107">Les montants du relevé peuvent être lettrés aux écritures comptables ouvertes comme suit :</span><span class="sxs-lookup"><span data-stu-id="5abcb-107">Statement amounts can be applied to outstanding ledger entries by:</span></span>  

-   <span data-ttu-id="5abcb-108">En lettrant manuellement les lignes relevé CODA.</span><span class="sxs-lookup"><span data-stu-id="5abcb-108">Manually applying CODA statement lines.</span></span>  
-   <span data-ttu-id="5abcb-109">En lettrant automatiquement les montants du relevé CODA aux écritures comptables et aux comptes appropriés.</span><span class="sxs-lookup"><span data-stu-id="5abcb-109">Automatically applying CODA statement amounts to the appropriate ledger entries and accounts.</span></span> <span data-ttu-id="5abcb-110">Le traitement automatique des lignes relevé CODA est recommandé.</span><span class="sxs-lookup"><span data-stu-id="5abcb-110">Automatic processing of CODA statement lines is recommended.</span></span>  

## <a name="to-manually-apply-the-coda-statement-lines"></a><span data-ttu-id="5abcb-111">Pour lettrer manuellement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="5abcb-111">To manually apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="5abcb-112">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Comptes bancaires**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="5abcb-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5abcb-113">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-113">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="5abcb-114">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-114">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="5abcb-115">Pour chaque ligne relevé, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5abcb-115">For each statement line, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5abcb-116">Champ</span><span class="sxs-lookup"><span data-stu-id="5abcb-116">Field</span></span>|<span data-ttu-id="5abcb-117">Désignation</span><span class="sxs-lookup"><span data-stu-id="5abcb-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5abcb-118">**N° compte**</span><span class="sxs-lookup"><span data-stu-id="5abcb-118">**Account No.**</span></span>|<span data-ttu-id="5abcb-119">Entrez le numéro du compte général, de la banque, du client, du fournisseur ou de l'immobilisation, auquel la ligne relevé du compte bancaire est associée.</span><span class="sxs-lookup"><span data-stu-id="5abcb-119">Enter the number of the general ledger account, bank, customer, vendor, or fixed asset that the bank account statement line is linked to.</span></span>|  
    |<span data-ttu-id="5abcb-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="5abcb-120">**Description**</span></span>|[!INCLUDE[prod_short](../../includes/prod_short.md)] <span data-ttu-id="5abcb-121">récupère automatiquement la description à partir du fichier CODA importé, mais vous pouvez modifier le contenu de ce champ.</span><span class="sxs-lookup"><span data-stu-id="5abcb-121">automatically retrieves the description from the imported CODA file, but you can modify the contents of this field.</span></span>|  

5.  <span data-ttu-id="5abcb-122">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-122">Choose the **OK** button.</span></span>  

## <a name="to-automatically-apply-the-coda-statement-lines"></a><span data-ttu-id="5abcb-123">Pour lettrer automatiquement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="5abcb-123">To automatically apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="5abcb-124">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Comptes bancaires**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="5abcb-124">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5abcb-125">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-125">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="5abcb-126">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-126">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="5abcb-127">Choisissez l'action **Traiter les lignes relevé CODA**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-127">Choose the **Process CODA Statement Lines** action.</span></span>  
5.  <span data-ttu-id="5abcb-128">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5abcb-128">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5abcb-129">Champ</span><span class="sxs-lookup"><span data-stu-id="5abcb-129">Field</span></span>|<span data-ttu-id="5abcb-130">Désignation</span><span class="sxs-lookup"><span data-stu-id="5abcb-130">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5abcb-131">**Comptabilisation par défaut**</span><span class="sxs-lookup"><span data-stu-id="5abcb-131">**Default Posting**</span></span>|<span data-ttu-id="5abcb-132">Sélectionnez ce champ si vous souhaitez que le traitement par lots valide les montants du relevé qui ne peuvent pas être associés aux écritures comptables existantes.</span><span class="sxs-lookup"><span data-stu-id="5abcb-132">Select if you want the batch job to post statement amounts that cannot be linked to existing ledger entries.</span></span>|  
    |<span data-ttu-id="5abcb-133">**Imprimer liste**</span><span class="sxs-lookup"><span data-stu-id="5abcb-133">**Print List**</span></span>|<span data-ttu-id="5abcb-134">Sélectionnez ce champ pour imprimer la liste des montants du relevé qui ne peuvent pas être associés automatiquement.</span><span class="sxs-lookup"><span data-stu-id="5abcb-134">Select to print a list of statement amounts that cannot be linked automatically.</span></span>|  

6.  <span data-ttu-id="5abcb-135">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="5abcb-135">Choose the **OK** button.</span></span>  

    <span data-ttu-id="5abcb-136">Lorsque vous démarrez le traitement par lots, les montants du relevé sont lettrés aux écritures comptables existantes en fonction des codes transaction.</span><span class="sxs-lookup"><span data-stu-id="5abcb-136">When you start the batch job, statement amounts will be applied to existing ledger entries based on the transaction codes.</span></span> <span data-ttu-id="5abcb-137">Pour plus d'informations, voir [Paramétrer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md).</span><span class="sxs-lookup"><span data-stu-id="5abcb-137">For more information, see [Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="5abcb-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5abcb-138">See Also</span></span>  
 <span data-ttu-id="5abcb-139">[Relevés bancaires CODA](coda-bank-statements.md) </span><span class="sxs-lookup"><span data-stu-id="5abcb-139">[CODA Bank Statements](coda-bank-statements.md) </span></span>  
 <span data-ttu-id="5abcb-140">[Paramétrer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md) </span><span class="sxs-lookup"><span data-stu-id="5abcb-140">[Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md) </span></span>  
 <span data-ttu-id="5abcb-141">[Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="5abcb-141">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="5abcb-142">[Importer les relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="5abcb-142">[Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="5abcb-143">[Créer des journaux financiers](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="5abcb-143">[Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 <span data-ttu-id="5abcb-144">[Transférer et publier automatiquement des relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="5abcb-144">[Automatically Transfer and Post CODA Statements](how-to-automatically-transfer-and-post-coda-statements.md) </span></span>  
 [<span data-ttu-id="5abcb-145">Transférer et publier manuellement des relevés CODA</span><span class="sxs-lookup"><span data-stu-id="5abcb-145">Manually Transfer and Post CODA Statements</span></span>](how-to-manually-transfer-and-post-coda-statements.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]