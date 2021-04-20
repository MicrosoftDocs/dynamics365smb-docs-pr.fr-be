---
title: Imprimer les fichiers de paiement dans la version belge
description: Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement dans la version belge de Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a2536af3bc33354a782a840c4320cc61a217af7a
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779222"
---
# <a name="print-payment-files"></a><span data-ttu-id="01dc4-103">Imprimer les fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="01dc4-103">Print Payment Files</span></span>

<span data-ttu-id="01dc4-104">Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.</span><span class="sxs-lookup"><span data-stu-id="01dc4-104">After you have printed a test report and corrected all errors, you can print the payment journal lines to a payment file.</span></span>  

<span data-ttu-id="01dc4-105">Un fichier de paiement contient les paiements nationaux, internationaux, SEPA ou SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="01dc4-105">A payment file contains either domestic, international, SEPA, or non-euro SEPA payments.</span></span> <span data-ttu-id="01dc4-106">Ce fichier peut être envoyé à une banque sur disque, par modem ou via le serveur Isabel (Interbanks Standards Association Belgium).</span><span class="sxs-lookup"><span data-stu-id="01dc4-106">The file can be sent to a bank either on disk, by modem, or via Interbanks Standards Association Belgium (Isabel).</span></span> <span data-ttu-id="01dc4-107">Vous ne pouvez créer qu'un seul fichier pour chaque date comptabilisation et chaque code devise.</span><span class="sxs-lookup"><span data-stu-id="01dc4-107">You can create only one file for each posting date and each currency code.</span></span> <span data-ttu-id="01dc4-108">Lorsque vous exportez les paiements dans un fichier, une note associée est imprimée, qui peut également être envoyée à la banque.</span><span class="sxs-lookup"><span data-stu-id="01dc4-108">When you export the payments to a file, an accompanying note is printed, which can also be sent to the bank.</span></span>  

<span data-ttu-id="01dc4-109">Dans la feuille paiement, le champ **Statut** sur les lignes exportées est défini sur **Validé**.</span><span class="sxs-lookup"><span data-stu-id="01dc4-109">In the payment journal, the **Status** field on the exported lines will be set to **Posted**.</span></span>  

## <a name="to-print-a-payment-file"></a><span data-ttu-id="01dc4-110">Pour imprimer un fichier de paiement</span><span class="sxs-lookup"><span data-stu-id="01dc4-110">To print a payment file</span></span>  

1. <span data-ttu-id="01dc4-111">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuille paiement**, puis sélectionnez le lien pour ouvrir la page **Feuille paiement EB**.</span><span class="sxs-lookup"><span data-stu-id="01dc4-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journal**, and then choose the link to open the **EB Payment Journal** page.</span></span>  
2. <span data-ttu-id="01dc4-112">Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.</span><span class="sxs-lookup"><span data-stu-id="01dc4-112">In the **Batch Name** field, select the required journal batch.</span></span>  
3. <span data-ttu-id="01dc4-113">Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="01dc4-113">In the **Export Protocol** field, select the export protocol.</span></span>  

    <span data-ttu-id="01dc4-114">Les protocoles d'exportation contrôlent le fichier de paiement généré dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="01dc4-114">Export protocols control which payment file will be generated in the payment journal.</span></span> <span data-ttu-id="01dc4-115">Vous pouvez combiner plusieurs formats d'exportation dans un même traitement par lots, par exemple national, international, SEPA ou une combinaison de ceux-ci.</span><span class="sxs-lookup"><span data-stu-id="01dc4-115">You can have a mixture of export formats in a single batch, such as domestic, international, SEPA, or a combination of these.</span></span> <span data-ttu-id="01dc4-116">Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un seul format d'exportation ou protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="01dc4-116">However, when exporting the payment lines to a file, you can use only one export format, or export protocol.</span></span>  

    > [!NOTE]
    > <span data-ttu-id="01dc4-117">En définissant le protocole d'exportation, vous définissez également le type de validation qui est exécuté dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="01dc4-117">By defining the export protocol, you also define the type of validation that will be performed in the payment journal.</span></span>
4. <span data-ttu-id="01dc4-118">Entrez les informations ligne feuille paiement, puis choisissez l'action **Vérifier lignes paiement**.</span><span class="sxs-lookup"><span data-stu-id="01dc4-118">Enter the payment journal line information, and then choose the **Check Payment Lines** action.</span></span>

    <span data-ttu-id="01dc4-119">La page **Exporter/Vérifier les journaux des erreurs** affiche les erreurs éventuelles.</span><span class="sxs-lookup"><span data-stu-id="01dc4-119">The **Export Check Error Logs** page displays any errors that exist.</span></span> <span data-ttu-id="01dc4-120">S'il existe des erreurs, vous devez les corriger avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="01dc4-120">If there are errors, you must fix them before you can continue.</span></span>

5. <span data-ttu-id="01dc4-121">S'il n'existe aucune erreur, choisissez l'action **Exporter lignes paiement**.</span><span class="sxs-lookup"><span data-stu-id="01dc4-121">If there are no errors, choose the **Export Payment Lines** action.</span></span>  

    <span data-ttu-id="01dc4-122">L'état que vous avez spécifié dans le champ **ID impression test** de la page **Modèles feuille paiement EB** s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="01dc4-122">The report that you specified in the **Test Report ID** field in the **EB Payment Journal Templates** will open.</span></span>  

6. <span data-ttu-id="01dc4-123">Cliquez sur le bouton **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="01dc4-123">Choose the **Print** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="01dc4-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="01dc4-124">See Also</span></span>

[<span data-ttu-id="01dc4-125">Opérations bancaires électroniques, Belgique</span><span class="sxs-lookup"><span data-stu-id="01dc4-125">Belgian Electronic Banking</span></span>](belgian-electronic-banking.md)  
[<span data-ttu-id="01dc4-126">Paiements électroniques belges</span><span class="sxs-lookup"><span data-stu-id="01dc4-126">Belgian Electronic Payments</span></span>](belgian-electronic-payments.md)  
[<span data-ttu-id="01dc4-127">Paramétrer les fournisseurs pour des suggestions de règlement automatique</span><span class="sxs-lookup"><span data-stu-id="01dc4-127">Set Up Vendors for Automatic Payment Suggestions</span></span>](how-to-set-up-vendors-for-automatic-payment-suggestions.md)  
[<span data-ttu-id="01dc4-128">Proposer paiements fournisseur</span><span class="sxs-lookup"><span data-stu-id="01dc4-128">Suggest Vendor Payments</span></span>](../../payables-how-suggest-vendor-payments.md)  
[<span data-ttu-id="01dc4-129">Créer des modèles et des lots de feuilles paiement</span><span class="sxs-lookup"><span data-stu-id="01dc4-129">Create Payment Journal Templates and Batches</span></span>](how-to-create-payment-journal-templates-and-batches.md)  
[<span data-ttu-id="01dc4-130">Tester les paiements électroniques</span><span class="sxs-lookup"><span data-stu-id="01dc4-130">Test Electronic Payments</span></span>](how-to-test-electronic-payments.md)  
