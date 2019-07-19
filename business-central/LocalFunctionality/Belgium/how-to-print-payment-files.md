---
title: Impression des fichiers de paiement
description: Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.
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
ms.openlocfilehash: 853daf678f818ee19d86b663ad2915c0090cd794
ms.sourcegitcommit: 5b6dd8d881c0eb65ece6936a94dfda3185574335
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/28/2019
ms.locfileid: "1711026"
---
# <a name="print-payment-files"></a><span data-ttu-id="1ebf5-103">Imprimer les fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="1ebf5-103">Print Payment Files</span></span>
<span data-ttu-id="1ebf5-104">Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-104">After you have printed a test report and corrected all errors, you can print the payment journal lines to a payment file.</span></span>  

<span data-ttu-id="1ebf5-105">Un fichier de paiement contient les paiements nationaux, internationaux, SEPA ou SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-105">A payment file contains either domestic, international, SEPA, or non-euro SEPA payments.</span></span> <span data-ttu-id="1ebf5-106">Ce fichier peut être envoyé à une banque sur disque, par modem ou via le serveur Isabel (Interbanks Standards Association Belgium).</span><span class="sxs-lookup"><span data-stu-id="1ebf5-106">The file can be sent to a bank either on disk, by modem, or via Interbanks Standards Association Belgium (Isabel).</span></span> <span data-ttu-id="1ebf5-107">Vous ne pouvez créer qu'un seul fichier pour chaque date comptabilisation et chaque code devise.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-107">You can create only one file for each posting date and each currency code.</span></span> <span data-ttu-id="1ebf5-108">Lorsque vous exportez les paiements dans un fichier, une note associée est imprimée, qui peut également être envoyée à la banque.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-108">When you export the payments to a file, an accompanying note is printed, which can also be sent to the bank.</span></span>  

<span data-ttu-id="1ebf5-109">Dans la feuille paiement, le champ **Statut** sur les lignes exportées est défini sur **Validé**.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-109">In the payment journal, the **Status** field on the exported lines will be set to **Posted**.</span></span>  

## <a name="to-print-a-payment-file"></a><span data-ttu-id="1ebf5-110">Pour imprimer un fichier de paiement</span><span class="sxs-lookup"><span data-stu-id="1ebf5-110">To print a payment file</span></span>  

1.  <span data-ttu-id="1ebf5-111">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille paiement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="1ebf5-112">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-112">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="1ebf5-113">Champ</span><span class="sxs-lookup"><span data-stu-id="1ebf5-113">Field</span></span>|<span data-ttu-id="1ebf5-114">Désignation</span><span class="sxs-lookup"><span data-stu-id="1ebf5-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1ebf5-115">**Nom de la feuille**</span><span class="sxs-lookup"><span data-stu-id="1ebf5-115">**Batch Name**</span></span>|<span data-ttu-id="1ebf5-116">Spécifiez le nom de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-116">Specify the batch name of the payment journal.</span></span>|  
    |<span data-ttu-id="1ebf5-117">**Compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="1ebf5-117">**Bank Account**</span></span>|<span data-ttu-id="1ebf5-118">Spécifiez le compte bancaire de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-118">Specify the bank account of the payment journal.</span></span>|  
    |<span data-ttu-id="1ebf5-119">**Protocole d'exportation**</span><span class="sxs-lookup"><span data-stu-id="1ebf5-119">**Export Protocol**</span></span>|<span data-ttu-id="1ebf5-120">Spécifiez le code du protocole d'exportation de la ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-120">Specify the export protocol code of the payment journal line.</span></span> <span data-ttu-id="1ebf5-121">Les protocoles d'exportation contrôlent le fichier de paiement généré dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-121">Export protocols control which payment file will be generated in the payment journal.</span></span><br /><br /> <span data-ttu-id="1ebf5-122">Vous pouvez combiner plusieurs formats d'exportation dans un même traitement par lots, par exemple national, international, SEPA ou une combinaison de ceux-ci.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-122">You can have a mixture of export formats in a single batch, such as domestic, international, SEPA, or a combination of these.</span></span> <span data-ttu-id="1ebf5-123">Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un seul format d'exportation ou protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-123">However, when exporting the payment lines to a file, you can use only one export format, or export protocol.</span></span> <span data-ttu-id="1ebf5-124">**Remarque :** en définissant le protocole d'exportation, vous définissez également le type de validation qui est exécuté dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-124">**Note:**  By defining the export protocol, you also define the type of validation that will be performed in the payment journal.</span></span>|  

3.  <span data-ttu-id="1ebf5-125">Choisissez l'action **Vérifier lignes paiement**.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-125">Choose the **Check Payment Lines** action.</span></span>

    <span data-ttu-id="1ebf5-126">La page **Exporter/Vérifier les journaux des erreurs** affiche les erreurs éventuelles.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-126">The **Export Check Error Logs** page displays any errors that exist.</span></span> <span data-ttu-id="1ebf5-127">S'il existe des erreurs, vous devez les corriger avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-127">If there are errors, you must fix them before you can continue.</span></span>

4. <span data-ttu-id="1ebf5-128">S'il n'existe aucune erreur, choisissez l'action **Exporter lignes paiement**.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-128">If there are no errors, choose the **Export Payment Lines** action.</span></span>  

    <span data-ttu-id="1ebf5-129">L'état que vous avez spécifié dans le champ **ID impression test** de la page **Modèles feuille paiement EB** s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-129">The report that you specified in the **Test Report ID** field in the **EB Payment Journal Templates** will open.</span></span>  

5.  <span data-ttu-id="1ebf5-130">Cliquez sur le bouton **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="1ebf5-130">Choose the **Print** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1ebf5-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1ebf5-131">See Also</span></span>  
 <span data-ttu-id="1ebf5-132">[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-132">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="1ebf5-133">[Paiements électroniques, Belgique](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-133">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="1ebf5-134">[Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-134">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 <span data-ttu-id="1ebf5-135">[Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-135">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="1ebf5-136">[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-136">[Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="1ebf5-137">[Générer des suggestions de règlement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-137">[Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 <span data-ttu-id="1ebf5-138">[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-138">[Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="1ebf5-139">[Tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="1ebf5-139">[Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 [<span data-ttu-id="1ebf5-140">Gérer les lignes de paiement électronique</span><span class="sxs-lookup"><span data-stu-id="1ebf5-140">Manage Electronic Payment Lines</span></span>](how-to-manage-electronic-payment-lines.md)
