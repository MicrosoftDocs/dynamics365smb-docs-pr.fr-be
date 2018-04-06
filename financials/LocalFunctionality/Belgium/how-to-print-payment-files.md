---
title: Comment imprimer les fichiers paiement
description: "Après avoir imprimé un test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier paiement."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: a7305fe72c7bbc35b8e164f12e3fe341b489d80c
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="print-payment-files"></a><span data-ttu-id="03e80-103">Imprimer des fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="03e80-103">Print Payment Files</span></span>
<span data-ttu-id="03e80-104">Après avoir imprimé un rapport test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.</span><span class="sxs-lookup"><span data-stu-id="03e80-104">After you have printed a test report and corrected all errors, you can print the payment journal lines to a payment file.</span></span>  

<span data-ttu-id="03e80-105">Un fichier paiement contient des paiements nationaux, internationaux, SEPA ou SEPA non libellés en Euro.</span><span class="sxs-lookup"><span data-stu-id="03e80-105">A payment file contains either domestic, international, SEPA, or non-euro SEPA payments.</span></span> <span data-ttu-id="03e80-106">Le fichier peut être envoyé à une banque sur disquette, par un modem ou via Isabel (Interbanks Standards Association Belgium).</span><span class="sxs-lookup"><span data-stu-id="03e80-106">The file can be sent to a bank either on disk, by modem, or via Interbanks Standards Association Belgium (Isabel).</span></span> <span data-ttu-id="03e80-107">Vous ne pouvez créer qu'un fichier par date de validation et par code devise.</span><span class="sxs-lookup"><span data-stu-id="03e80-107">You can only create one file for each posting date and each currency code.</span></span> <span data-ttu-id="03e80-108">Lorsque vous exportez les paiements dans un fichier, une note d'accompagnement est imprimée et peut aussi être envoyée à la banque.</span><span class="sxs-lookup"><span data-stu-id="03e80-108">When you export the payments to a file, an accompanying note is printed, which can also be sent to the bank.</span></span>  

<span data-ttu-id="03e80-109">Dans la feuille paiement, le champ **Statut** des lignes exportées sera défini sur **Validé**.</span><span class="sxs-lookup"><span data-stu-id="03e80-109">In the payment journal, the **Status** field on the exported lines will be set to **Posted**.</span></span>  

## <a name="to-print-a-payment-file"></a><span data-ttu-id="03e80-110">Pour imprimer un fichier paiement</span><span class="sxs-lookup"><span data-stu-id="03e80-110">To print a payment file</span></span>  

1.  <span data-ttu-id="03e80-111">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille paiement**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="03e80-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="03e80-112">Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="03e80-112">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="03e80-113">Champ</span><span class="sxs-lookup"><span data-stu-id="03e80-113">Field</span></span>|<span data-ttu-id="03e80-114">Description</span><span class="sxs-lookup"><span data-stu-id="03e80-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="03e80-115">**Nom de la feuille**</span><span class="sxs-lookup"><span data-stu-id="03e80-115">**Batch Name**</span></span>|<span data-ttu-id="03e80-116">Spécifiez le nom de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="03e80-116">Specify the batch name of the payment journal.</span></span>|  
    |<span data-ttu-id="03e80-117">**Compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="03e80-117">**Bank Account**</span></span>|<span data-ttu-id="03e80-118">Spécifiez le compte bancaire de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="03e80-118">Specify the bank account of the payment journal.</span></span>|  
    |<span data-ttu-id="03e80-119">**Protocole d'exportation**</span><span class="sxs-lookup"><span data-stu-id="03e80-119">**Export Protocol**</span></span>|<span data-ttu-id="03e80-120">Spécifiez le code du protocole d'exportation de la ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="03e80-120">Specify the export protocol code of the payment journal line.</span></span> <span data-ttu-id="03e80-121">Exportez des protocoles qui contrôlent le fichier de paiement qui sera généré dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="03e80-121">Export protocols control which payment file will be generated in the payment journal.</span></span><br /><br /> <span data-ttu-id="03e80-122">Vous pouvez avoir plusieurs formats d'exportation différents dans un seul lot, comme les formats national, international, SEPA, ou un ensemble des trois.</span><span class="sxs-lookup"><span data-stu-id="03e80-122">You can have a mixture of export formats in a single batch, such as domestic, international, SEPA, or a combination of these.</span></span> <span data-ttu-id="03e80-123">Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un format ou protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="03e80-123">However, when exporting the payment lines to a file, you can only use one export format, or export protocol.</span></span> <span data-ttu-id="03e80-124">**Note :**  En définissant le protocole d'exportation, vous définissez également le type de validation qui sera effectuée dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="03e80-124">**Note:**  By defining the export protocol, you also define the type of validation that will be performed in the payment journal.</span></span>|  

3.  <span data-ttu-id="03e80-125">Choisissez l'action **Vérifier les lignes de paiement**.</span><span class="sxs-lookup"><span data-stu-id="03e80-125">Choose the **Check Payment Lines** action.</span></span>

    <span data-ttu-id="03e80-126">La fenêtre **Exporter les journaux d'erreur de chèque** affiche les erreurs éventuelles qui pourraient exister.</span><span class="sxs-lookup"><span data-stu-id="03e80-126">The **Export Check Error Logs** window displays any errors that may exist.</span></span> <span data-ttu-id="03e80-127">S'il y a des erreurs, vous devez les corriger avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="03e80-127">If there are errors, you must fix the errors before you can continue.</span></span>

4. <span data-ttu-id="03e80-128">S'il n'y a pas d'erreur, choisissez l'action **Exporter les lignes de paiement**.</span><span class="sxs-lookup"><span data-stu-id="03e80-128">If there are no errors, choose the **Export Payment Lines** action.</span></span>  

    <span data-ttu-id="03e80-129">L'état que vous avez spécifié dans le champ **ID impression test** des **Modèles FS paiements EB** s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="03e80-129">The report that you specified in the **Test Report ID** field in the **EB Payment Journal Templates** will open.</span></span>  

5.  <span data-ttu-id="03e80-130">Cliquez sur le bouton **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="03e80-130">Choose the **Print** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="03e80-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="03e80-131">See Also</span></span>  
 <span data-ttu-id="03e80-132">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-132">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="03e80-133">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-133">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="03e80-134">[Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-134">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 <span data-ttu-id="03e80-135">[Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-135">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="03e80-136">[Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-136">[Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="03e80-137">[Générer des propositions de paiement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-137">[Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 <span data-ttu-id="03e80-138">[Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-138">[Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="03e80-139">[Tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="03e80-139">[Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 [<span data-ttu-id="03e80-140">Gérer les lignes paiement électronique</span><span class="sxs-lookup"><span data-stu-id="03e80-140">Manage Electronic Payment Lines</span></span>](how-to-manage-electronic-payment-lines.md)

