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
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 728d5c10bdb98ae16ffe1139343c6fe86d34199e
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676612"
---
# <a name="print-payment-files"></a><span data-ttu-id="9ef96-103">Imprimer les fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="9ef96-103">Print Payment Files</span></span>
<span data-ttu-id="9ef96-104">Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.</span><span class="sxs-lookup"><span data-stu-id="9ef96-104">After you have printed a test report and corrected all errors, you can print the payment journal lines to a payment file.</span></span>  

<span data-ttu-id="9ef96-105">Un fichier de paiement contient les paiements nationaux, internationaux, SEPA ou SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="9ef96-105">A payment file contains either domestic, international, SEPA, or non-euro SEPA payments.</span></span> <span data-ttu-id="9ef96-106">Ce fichier peut être envoyé à une banque sur disque, par modem ou via le serveur Isabel (Interbanks Standards Association Belgium).</span><span class="sxs-lookup"><span data-stu-id="9ef96-106">The file can be sent to a bank either on disk, by modem, or via Interbanks Standards Association Belgium (Isabel).</span></span> <span data-ttu-id="9ef96-107">Vous ne pouvez créer qu'un seul fichier pour chaque date comptabilisation et chaque code devise.</span><span class="sxs-lookup"><span data-stu-id="9ef96-107">You can create only one file for each posting date and each currency code.</span></span> <span data-ttu-id="9ef96-108">Lorsque vous exportez les paiements dans un fichier, une note associée est imprimée, qui peut également être envoyée à la banque.</span><span class="sxs-lookup"><span data-stu-id="9ef96-108">When you export the payments to a file, an accompanying note is printed, which can also be sent to the bank.</span></span>  

<span data-ttu-id="9ef96-109">Dans la feuille paiement, le champ **Statut** sur les lignes exportées est défini sur **Validé**.</span><span class="sxs-lookup"><span data-stu-id="9ef96-109">In the payment journal, the **Status** field on the exported lines will be set to **Posted**.</span></span>  

## <a name="to-print-a-payment-file"></a><span data-ttu-id="9ef96-110">Pour imprimer un fichier de paiement</span><span class="sxs-lookup"><span data-stu-id="9ef96-110">To print a payment file</span></span>  

1.  <span data-ttu-id="9ef96-111">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuille paiement**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="9ef96-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9ef96-112">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="9ef96-112">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="9ef96-113">Champ</span><span class="sxs-lookup"><span data-stu-id="9ef96-113">Field</span></span>|<span data-ttu-id="9ef96-114">Désignation</span><span class="sxs-lookup"><span data-stu-id="9ef96-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="9ef96-115">**Nom de la feuille**</span><span class="sxs-lookup"><span data-stu-id="9ef96-115">**Batch Name**</span></span>|<span data-ttu-id="9ef96-116">Spécifiez le nom de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9ef96-116">Specify the batch name of the payment journal.</span></span>|  
    |<span data-ttu-id="9ef96-117">**Compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="9ef96-117">**Bank Account**</span></span>|<span data-ttu-id="9ef96-118">Spécifiez le compte bancaire de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9ef96-118">Specify the bank account of the payment journal.</span></span>|  
    |<span data-ttu-id="9ef96-119">**Protocole d'exportation**</span><span class="sxs-lookup"><span data-stu-id="9ef96-119">**Export Protocol**</span></span>|<span data-ttu-id="9ef96-120">Spécifiez le code du protocole d'exportation de la ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9ef96-120">Specify the export protocol code of the payment journal line.</span></span> <span data-ttu-id="9ef96-121">Les protocoles d'exportation contrôlent le fichier de paiement généré dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9ef96-121">Export protocols control which payment file will be generated in the payment journal.</span></span><br /><br /> <span data-ttu-id="9ef96-122">Vous pouvez combiner plusieurs formats d'exportation dans un même traitement par lots, par exemple national, international, SEPA ou une combinaison de ceux-ci.</span><span class="sxs-lookup"><span data-stu-id="9ef96-122">You can have a mixture of export formats in a single batch, such as domestic, international, SEPA, or a combination of these.</span></span> <span data-ttu-id="9ef96-123">Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un seul format d'exportation ou protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="9ef96-123">However, when exporting the payment lines to a file, you can use only one export format, or export protocol.</span></span> <span data-ttu-id="9ef96-124">**Remarque :** en définissant le protocole d'exportation, vous définissez également le type de validation qui est exécuté dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9ef96-124">**Note:**  By defining the export protocol, you also define the type of validation that will be performed in the payment journal.</span></span>|  

3.  <span data-ttu-id="9ef96-125">Choisissez l'action **Vérifier lignes paiement**.</span><span class="sxs-lookup"><span data-stu-id="9ef96-125">Choose the **Check Payment Lines** action.</span></span>

    <span data-ttu-id="9ef96-126">La page **Exporter/Vérifier les journaux des erreurs** affiche les erreurs éventuelles.</span><span class="sxs-lookup"><span data-stu-id="9ef96-126">The **Export Check Error Logs** page displays any errors that exist.</span></span> <span data-ttu-id="9ef96-127">S'il existe des erreurs, vous devez les corriger avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="9ef96-127">If there are errors, you must fix them before you can continue.</span></span>

4. <span data-ttu-id="9ef96-128">S'il n'existe aucune erreur, choisissez l'action **Exporter lignes paiement**.</span><span class="sxs-lookup"><span data-stu-id="9ef96-128">If there are no errors, choose the **Export Payment Lines** action.</span></span>  

    <span data-ttu-id="9ef96-129">L'état que vous avez spécifié dans le champ **ID impression test** de la page **Modèles feuille paiement EB** s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="9ef96-129">The report that you specified in the **Test Report ID** field in the **EB Payment Journal Templates** will open.</span></span>  

5.  <span data-ttu-id="9ef96-130">Cliquez sur le bouton **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="9ef96-130">Choose the **Print** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9ef96-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9ef96-131">See Also</span></span>  
 <span data-ttu-id="9ef96-132">[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-132">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="9ef96-133">[Paiements électroniques, Belgique](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-133">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="9ef96-134">[Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-134">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 <span data-ttu-id="9ef96-135">[Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-135">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="9ef96-136">[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-136">[Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="9ef96-137">[Générer des suggestions de règlement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-137">[Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 <span data-ttu-id="9ef96-138">[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-138">[Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="9ef96-139">[Tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="9ef96-139">[Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 [<span data-ttu-id="9ef96-140">Gérer les lignes de paiement électronique</span><span class="sxs-lookup"><span data-stu-id="9ef96-140">Manage Electronic Payment Lines</span></span>](how-to-manage-electronic-payment-lines.md)
