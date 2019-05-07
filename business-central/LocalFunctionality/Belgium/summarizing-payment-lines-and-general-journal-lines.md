---
title: Résumé des lignes règlement et des lignes feuille comptabilité
description: Business Central totalise les lignes règlement et les lignes feuille.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 482578e4b37921802e3d3295086b7d5dc9e794b4
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2019
ms.locfileid: "917232"
---
# <a name="summarizing-payment-lines-and-general-journal-lines"></a><span data-ttu-id="75ccd-103">Résumé des lignes règlement et des lignes feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="75ccd-103">Summarizing Payment Lines and General Journal Lines</span></span>
<span data-ttu-id="75ccd-104">Business Central totalise les lignes règlement et les lignes feuille pour les types de paiements suivants :</span><span class="sxs-lookup"><span data-stu-id="75ccd-104">Business Central summarizes payment lines and journal line across the following types of payments:</span></span>  

- <span data-ttu-id="75ccd-105">Paiements nationaux</span><span class="sxs-lookup"><span data-stu-id="75ccd-105">Domestic payments</span></span>  
- <span data-ttu-id="75ccd-106">Paiements internationaux</span><span class="sxs-lookup"><span data-stu-id="75ccd-106">International payments</span></span>  
- <span data-ttu-id="75ccd-107">Paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="75ccd-107">SEPA payments</span></span>  
- <span data-ttu-id="75ccd-108">Paiements SEPA hors euro</span><span class="sxs-lookup"><span data-stu-id="75ccd-108">Non-euro SEPA payments</span></span>  

## <a name="how-payment-journal-lines-are-transferred-to-the-general-journal"></a><span data-ttu-id="75ccd-109">Transfert des lignes feuille paiement vers la feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="75ccd-109">How Payment Journal Lines are Transferred to the General Journal</span></span>  
<span data-ttu-id="75ccd-110">Lorsque vous exportez les lignes feuille paiement vers un fichier, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] transfère les lignes feuille paiement vers la feuille comptabilité spécifiée.</span><span class="sxs-lookup"><span data-stu-id="75ccd-110">When you export the payment journal lines to a file, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] transfers the payment journal lines to the specified general journal.</span></span> <span data-ttu-id="75ccd-111">Par défaut, une ligne feuille comptabilité est créée pour chaque ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="75ccd-111">By default, a general journal line is created for each payment journal line.</span></span>  

<span data-ttu-id="75ccd-112">Les deux champs suivants de la page **Paramétrage des opérations bancaires électroniques** affectent la manière dont les lignes paiement sont totalisées :</span><span class="sxs-lookup"><span data-stu-id="75ccd-112">The following two fields on the **Electronic Banking Setup** page affect how the payment lines are summarized:</span></span>  

- <span data-ttu-id="75ccd-113">**Totaliser lignes feuille compta.**</span><span class="sxs-lookup"><span data-stu-id="75ccd-113">**Summarize Gen. Jnl. Lines**</span></span>  
- <span data-ttu-id="75ccd-114">**Limiter les textes du message de paiement**</span><span class="sxs-lookup"><span data-stu-id="75ccd-114">**Cut off Payment Message Texts**</span></span>  

<span data-ttu-id="75ccd-115">Si vous avez activé la case à cocher **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques**, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] totalise toutes les lignes feuille paiement d'un fournisseur spécifique en une ligne feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="75ccd-115">If you have selected the **Summarize Gen. Jnl. Lines** check box on the **Electronic Banking Setup** page, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] summarizes all payment journal lines for a specific vendor into one general journal line.</span></span> <span data-ttu-id="75ccd-116">La description générale « Paiement %1 », où %1 correspond au numéro de fournisseur, est utilisée pour la description de la ligne feuille totalisée.</span><span class="sxs-lookup"><span data-stu-id="75ccd-116">The general description "Payment %1," where %1 is the vendor number, is used for the summarized journal line description.</span></span> <span data-ttu-id="75ccd-117">Une ligne paiement distincte et une ligne feuille comptabilité distincte sont créées pour gérer :</span><span class="sxs-lookup"><span data-stu-id="75ccd-117">A separate payment line and a separate general journal line are created to handle:</span></span>  

- <span data-ttu-id="75ccd-118">Les lignes feuille paiement contenant des paiements partiels, avec les champs **Paiement partiel** et **Ligne distincte** sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="75ccd-118">Payment journal lines that contain partial payments, with both the **Partial Payment** and the **Separate Line** fields selected.</span></span>  

- <span data-ttu-id="75ccd-119">Les lignes feuille paiement contenant un message au format standard (c'est-à-dire, qui a réussi le test MOD97), qui définit le champ **Message au format standard** sur Vrai dans la feuille opérations bancaires électroniques.</span><span class="sxs-lookup"><span data-stu-id="75ccd-119">Payment journal lines that contain a standard format message (that is, passes the MOD97 test), which sets **Standard Format Message** to True in the electronic banking journal.</span></span>  

## <a name="example-1"></a><span data-ttu-id="75ccd-120">Exemple 1</span><span class="sxs-lookup"><span data-stu-id="75ccd-120">Example 1</span></span>  
<span data-ttu-id="75ccd-121">Dans cet exemple, vous exportez les lignes paiement, et la case à cocher **Totaliser lignes feuille compta.** est activée.</span><span class="sxs-lookup"><span data-stu-id="75ccd-121">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="75ccd-122">crée :</span><span class="sxs-lookup"><span data-stu-id="75ccd-122">creates:</span></span>  

- <span data-ttu-id="75ccd-123">Une ligne paiement combinée dans un fichier XML qui contient un message de paiement concaténé.</span><span class="sxs-lookup"><span data-stu-id="75ccd-123">One combined payment line in a XML file that has a concatenated payment message.</span></span> <span data-ttu-id="75ccd-124">L'espace blanc est le séparateur.</span><span class="sxs-lookup"><span data-stu-id="75ccd-124">White space is the delimiter.</span></span>  
- <span data-ttu-id="75ccd-125">Une ligne paiement dans la feuille comptabilité avec une description générique ../../contenant le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="75ccd-125">One payment line in the general journal with a generic description that ../../includes the vendor name.</span></span>  

## <a name="example-2"></a><span data-ttu-id="75ccd-126">Exemple 2</span><span class="sxs-lookup"><span data-stu-id="75ccd-126">Example 2</span></span>  
<span data-ttu-id="75ccd-127">Dans cet exemple, vous exportez les lignes paiement, et la case à cocher **Totaliser lignes feuille compta.** est activée.</span><span class="sxs-lookup"><span data-stu-id="75ccd-127">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> <span data-ttu-id="75ccd-128">La case à cocher **Limiter les textes du message de paiement** est désactivée, et les lignes paiement SEPA et SEPA hors euro combinées dépassent 140 caractères dans le message de paiement.</span><span class="sxs-lookup"><span data-stu-id="75ccd-128">The **Cut off Payment Message Texts** check box is cleared, and combined SEPA and non-euro SEPA payment lines exceed 140 characters in payment message.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="75ccd-129">crée :</span><span class="sxs-lookup"><span data-stu-id="75ccd-129">creates:</span></span>  

- <span data-ttu-id="75ccd-130">Deux lignes paiement combinées dans un fichier XML.</span><span class="sxs-lookup"><span data-stu-id="75ccd-130">Two combined payment lines in a XML file.</span></span> <span data-ttu-id="75ccd-131">La première ligne paiement contient les premiers messages de paiement concaténés.</span><span class="sxs-lookup"><span data-stu-id="75ccd-131">The first payment line contains the first concatenated payment messages.</span></span> <span data-ttu-id="75ccd-132">La deuxième ligne paiement contient le message de paiement de la troisième ligne.</span><span class="sxs-lookup"><span data-stu-id="75ccd-132">The second payment line contains the payment message from the third line.</span></span>  

- <span data-ttu-id="75ccd-133">Une ligne paiement dans la feuille comptabilité avec une description générique ../../contenant le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="75ccd-133">One payment line in the general journal with a generic description that ../../includes the vendor name.</span></span>  

## <a name="example-3"></a><span data-ttu-id="75ccd-134">Exemple 3</span><span class="sxs-lookup"><span data-stu-id="75ccd-134">Example 3</span></span>  
<span data-ttu-id="75ccd-135">Dans cet exemple, vous exportez les lignes paiement, et la case à cocher **Totaliser lignes feuille compta.** est activée.</span><span class="sxs-lookup"><span data-stu-id="75ccd-135">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> <span data-ttu-id="75ccd-136">La case à cocher **Limiter les textes du message de paiement** est également activée, et les lignes paiement SEPA et SEPA hors euro combinées dépassent 140 caractères dans le message de paiement.</span><span class="sxs-lookup"><span data-stu-id="75ccd-136">The **Cut off Payment Message Texts** check box is also selected and combined SEPA and non-SEPA payment lines exceed 140 characters in payment message.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="75ccd-137">crée :</span><span class="sxs-lookup"><span data-stu-id="75ccd-137">creates:</span></span>  

- <span data-ttu-id="75ccd-138">Une ligne paiement combinée dans un fichier XML qui contient deux messages de paiement concaténés.</span><span class="sxs-lookup"><span data-stu-id="75ccd-138">One combined payment line in a XML file that has two concatenated payment messages.</span></span> <span data-ttu-id="75ccd-139">Les points de suspension (…) sont utilisés pour indiquer que le message est tronqué.</span><span class="sxs-lookup"><span data-stu-id="75ccd-139">An ellipsis (…) is used to indicate that the message is truncated.</span></span>  

- <span data-ttu-id="75ccd-140">Une ligne paiement dans la feuille comptabilité avec une description générique contenant le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="75ccd-140">One payment line in the general journal with a generic description that includes the vendor name.</span></span>  

<span data-ttu-id="75ccd-141">Selon la structure XML, les paiements sont totalisés par numéro de compte, numéro de compte bancaire du bénéficiaire et numéro de compte bancaire. Le filtre de compte bancaire peut être vide.</span><span class="sxs-lookup"><span data-stu-id="75ccd-141">Based on the XML structure, the payments are summarized per account number and beneficiary bank account no and bank account no. The bank account filter can be empty.</span></span>  

<span data-ttu-id="75ccd-142">La valeur EndToEndId dans le message SEPA est extraite du message de paiement et peut être tronquée à la longueur maximale de 45 caractères.</span><span class="sxs-lookup"><span data-stu-id="75ccd-142">The EndToEndId in the SEPA message is taken from the payment message and can be truncated to the maximum length of 45 characters.</span></span>  

## <a name="see-also"></a><span data-ttu-id="75ccd-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="75ccd-143">See Also</span></span>  
 <span data-ttu-id="75ccd-144">[Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="75ccd-144">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 [<span data-ttu-id="75ccd-145">Configuration de Finance</span><span class="sxs-lookup"><span data-stu-id="75ccd-145">Setting Up Finance</span></span>](../../finance-setup-finance.md)  
 [<span data-ttu-id="75ccd-146">Enregistrer des achats</span><span class="sxs-lookup"><span data-stu-id="75ccd-146">Record Purchases</span></span>](../../purchasing-how-record-purchases.md)
