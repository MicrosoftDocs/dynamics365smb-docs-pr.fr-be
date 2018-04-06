---
title: "Récapitulatif des lignes paiements et des lignes feuille comptabilité"
description: "Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)] gère plusieurs types de transactions de la même manière."
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
ms.openlocfilehash: 9d481dd75aa9ea24f89be99949d3d0a188b2fdf6
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="summarizing-payment-lines-and-general-journal-lines"></a><span data-ttu-id="1b8c2-103">Résumer les lignes de paiement et feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="1b8c2-103">Summarizing Payment Lines and General Journal Lines</span></span>
<span data-ttu-id="1b8c2-104">[!INCLUDE[d365fin](../../includes/d365fin_md.md)] traite les différents types de transactions de la même manière :</span><span class="sxs-lookup"><span data-stu-id="1b8c2-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] handles the following types of transactions in the same way:</span></span>  

- <span data-ttu-id="1b8c2-105">Paiements intérieurs</span><span class="sxs-lookup"><span data-stu-id="1b8c2-105">Domestic payments</span></span>  
- <span data-ttu-id="1b8c2-106">Paiements étrangers</span><span class="sxs-lookup"><span data-stu-id="1b8c2-106">International payments</span></span>  
- <span data-ttu-id="1b8c2-107">Paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="1b8c2-107">SEPA payments</span></span>  
- <span data-ttu-id="1b8c2-108">Paiements SEPA non libellés en Euro</span><span class="sxs-lookup"><span data-stu-id="1b8c2-108">Non-euro SEPA payments</span></span>  

## <a name="how-payment-journal-lines-are-transferred-to-the-general-journal"></a><span data-ttu-id="1b8c2-109">Comment les lignes feuille paiement sont transférées dans la feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="1b8c2-109">How Payment Journal Lines are Transferred to the General Journal</span></span>  
<span data-ttu-id="1b8c2-110">Lorsque vous exportez les lignes feuille paiement dans un fichier, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] transfère les lignes feuille paiement dans la feuille comptabilité spécifiée.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-110">When you export the payment journal lines to a file, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] transfers the payment journal lines to the specified general journal.</span></span> <span data-ttu-id="1b8c2-111">Par défaut, une ligne feuille comptabilité est créée pour chaque ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-111">By default, a general journal line is created for each payment journal line.</span></span>  

<span data-ttu-id="1b8c2-112">Les deux champs suivants dans la fenêtre **Configuration de la banque électronique** affectent la manière dont sont résumées les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-112">The following two fields in the **Electronic Banking Setup** window affect how the payment lines are summarized:</span></span>  

- <span data-ttu-id="1b8c2-113">**Résumer lignes FS**</span><span class="sxs-lookup"><span data-stu-id="1b8c2-113">**Summarize Gen. Jnl. Lines**</span></span>  
- <span data-ttu-id="1b8c2-114">**Couper comm. de paiement**</span><span class="sxs-lookup"><span data-stu-id="1b8c2-114">**Cut off Payment Message Texts**</span></span>  

<span data-ttu-id="1b8c2-115">Si vous avez sélectionné la case à cocher **Résumer lignes FS** dans la fenêtre **Configuration de la banque électronique**, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] résume toutes les lignes feuille paiement pour un fournisseur spécifique sur une ligne feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-115">If you have selected the **Summarize Gen. Jnl. Lines** check box in the **Electronic Banking Setup** window, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] summarizes all payment journal lines for a specific vendor into one general journal line.</span></span> <span data-ttu-id="1b8c2-116">La description générale « Paiement %1 », où %1 est le numéro du fournisseur, est utilisée pour la description de la ligne feuille résumée.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-116">The general description "Payment %1," where %1 is the vendor number, is used for the summarized journal line description.</span></span> <span data-ttu-id="1b8c2-117">Une ligne paiement et une ligne feuille comptabilité distinctes sont créées pour traiter :</span><span class="sxs-lookup"><span data-stu-id="1b8c2-117">A separate payment line and a separate general journal line are created to handle:</span></span>  

- <span data-ttu-id="1b8c2-118">Les lignes feuille paiement qui contiennent des paiements partiels, avec les champs **Paiement partiel** et **Ligne individuelle** sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-118">Payment journal lines that contain partial payments, with both the **Partial Payment** and the **Separate Line** fields selected.</span></span>  

- <span data-ttu-id="1b8c2-119">Les lignes feuille paiement qui contiennent une communication structurée (a réussi le test MOD97), qui définit **Communication structurée** sur True dans la feuille bancaire électronique.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-119">Payment journal lines that contain a standard format message (that is, passes the MOD97 test), which sets **Standard Format Message** to True in the electronic banking journal.</span></span>  

## <a name="example-1"></a><span data-ttu-id="1b8c2-120">Exemple 1</span><span class="sxs-lookup"><span data-stu-id="1b8c2-120">Example 1</span></span>  
<span data-ttu-id="1b8c2-121">Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-121">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)]<span data-ttu-id="1b8c2-122"> crée :</span><span class="sxs-lookup"><span data-stu-id="1b8c2-122"> creates:</span></span>  

- <span data-ttu-id="1b8c2-123">Une ligne paiement combinée dans un fichier XML qui contient une communication concaténée.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-123">One combined payment line in a XML file that has a concatenated payment message.</span></span> <span data-ttu-id="1b8c2-124">Un espace blanc est le délimiteur.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-124">White space is the delimiter.</span></span>  
- <span data-ttu-id="1b8c2-125">Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-125">One payment line in the general journal with a generic description that ../../includes the vendor name.</span></span>  

## <a name="example-2"></a><span data-ttu-id="1b8c2-126">Exemple 2</span><span class="sxs-lookup"><span data-stu-id="1b8c2-126">Example 2</span></span>  
<span data-ttu-id="1b8c2-127">Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-127">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> <span data-ttu-id="1b8c2-128">La case à cocher **Couper comm. de paiement** est désélectionnée, et les lignes paiement SEPA et SEPA non libellées en Euro combinées dépassent 140 caractères dans la communication.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-128">The **Cut off Payment Message Texts** check box is cleared, and combined SEPA and non-euro SEPA payment lines exceed 140 characters in payment message.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)]<span data-ttu-id="1b8c2-129"> crée :</span><span class="sxs-lookup"><span data-stu-id="1b8c2-129"> creates:</span></span>  

- <span data-ttu-id="1b8c2-130">Deux lignes paiement combinées dans un fichier XML.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-130">Two combined payment lines in a XML file.</span></span> <span data-ttu-id="1b8c2-131">La première ligne paiement contient les premières communications concaténées.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-131">The first payment line contains the first concatenated payment messages.</span></span> <span data-ttu-id="1b8c2-132">La deuxième ligne paiement contient la communication de la troisième ligne.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-132">The second payment line contains the payment message from the third line.</span></span>  

- <span data-ttu-id="1b8c2-133">Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-133">One payment line in the general journal with a generic description that ../../includes the vendor name.</span></span>  

## <a name="example-3"></a><span data-ttu-id="1b8c2-134">Exemple 3</span><span class="sxs-lookup"><span data-stu-id="1b8c2-134">Example 3</span></span>  
<span data-ttu-id="1b8c2-135">Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-135">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> <span data-ttu-id="1b8c2-136">La case à cocher **Couper comm. de paiement** est également sélectionnée, et les lignes paiement SEPA et SEPA non libellées en Euro combinées dépassent 140 caractères dans la communication.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-136">The **Cut off Payment Message Texts** check box is also selected and combined SEPA and non-SEPA payment lines exceed 140 characters in payment message.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)]<span data-ttu-id="1b8c2-137"> crée :</span><span class="sxs-lookup"><span data-stu-id="1b8c2-137"> creates:</span></span>  

- <span data-ttu-id="1b8c2-138">Une ligne paiement combinée dans un fichier XML qui contient deux communications concaténées.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-138">One combined payment line in a XML file that has two concatenated payment messages.</span></span> <span data-ttu-id="1b8c2-139">Des points de suspension (...) sont utilisés pour indiquer que le message est tronqué.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-139">An ellipsis (…) is used to indicate that the message is truncated.</span></span>  

- <span data-ttu-id="1b8c2-140">Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-140">One payment line in the general journal with a generic description that includes the vendor name.</span></span>  

<span data-ttu-id="1b8c2-141">Basés sur la structure XML, les paiements sont résumés par numéro de compte, numéro compte bancaire bénéficiaire et numéro compte bancaire. Le filtre compte bancaire peut être vide.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-141">Based on the XML structure, the payments are summarized per account number and beneficiary bank account no and bank account no. The bank account filter can be empty.</span></span>  

<span data-ttu-id="1b8c2-142">Le code EndToEndId dans le message SEPA est prélevé de la communication et peut être tronqué à la longueur maximale de 45 caractères.</span><span class="sxs-lookup"><span data-stu-id="1b8c2-142">The EndToEndId in the SEPA message is taken from the payment message and can be truncated to the maximum length of 45 characters.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1b8c2-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1b8c2-143">See Also</span></span>  
 <span data-ttu-id="1b8c2-144">[Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="1b8c2-144">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 [<span data-ttu-id="1b8c2-145">Paramétrage de Finance</span><span class="sxs-lookup"><span data-stu-id="1b8c2-145">Setting Up Finance</span></span>](../../finance-setup-finance.md)  
 [<span data-ttu-id="1b8c2-146">Enregistrer des achats</span><span class="sxs-lookup"><span data-stu-id="1b8c2-146">Record Purchases</span></span>](../../purchasing-how-record-purchases.md) 

