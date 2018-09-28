---
title: "Relevés bancaires CODA"
description: "Le Coded Statement of Account (CODA) est une norme bancaire nationale conçue par l'Association belge des Banques et des Sociétés de Bourse qui vous permet de traitement automatiquement des relevés bancaires électroniques."
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
ms.openlocfilehash: 2b35ff920bc306cfd49fb7dce959a69b582042eb
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="coda-bank-statements"></a><span data-ttu-id="fc041-103">Relevés bancaires CODA</span><span class="sxs-lookup"><span data-stu-id="fc041-103">CODA Bank Statements</span></span>
<span data-ttu-id="fc041-104">Le Coded Statement of Account (CODA) est une norme bancaire nationale conçue par l'Association belge des Banques et des Sociétés de Bourse qui vous permet de traitement automatiquement des relevés bancaires électroniques.</span><span class="sxs-lookup"><span data-stu-id="fc041-104">The Coded Statement of Account (CODA) is a national banking standard, designed by the Belgian Banker's Association, which allows you to automatically process electronic bank statements.</span></span>  

<span data-ttu-id="fc041-105">Chaque type de transaction d'un relevé CODA se voit attribuer un code unique.</span><span class="sxs-lookup"><span data-stu-id="fc041-105">Each type of transaction in a CODA statement is assigned a unique code.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="fc041-106">utilise ce code pour interpréter les transactions et les lettrer aux écritures comptables correspondantes.</span><span class="sxs-lookup"><span data-stu-id="fc041-106"> uses this code to interpret transactions and apply them to the corresponding ledger entries.</span></span>  

## <a name="applying-statement-lines"></a><span data-ttu-id="fc041-107">Lettrage des lignes relevé</span><span class="sxs-lookup"><span data-stu-id="fc041-107">Applying Statement Lines</span></span>  
<span data-ttu-id="fc041-108">Lorsque vous avez importé un relevé CODA, vous pouvez lettrer les lignes relevé à des écritures comptables existantes selon les informations reprises dans la table **Encodage CODA**.</span><span class="sxs-lookup"><span data-stu-id="fc041-108">When you have imported a CODA statement, you can apply the statement lines to existing ledger entries, based on the information in the **Transaction Coding** table.</span></span>  

<span data-ttu-id="fc041-109">Si l'encodage CODA de la ligne relevé est introuvable, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] interrompra le traitement et poursuivra avec la ligne relevé suivante.</span><span class="sxs-lookup"><span data-stu-id="fc041-109">If the transaction coding of the statement line is not found, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] will stop processing and continue with the next statement line.</span></span> <span data-ttu-id="fc041-110">Si vous sélectionnez le champ **Validation par défaut**, la ligne relevé sera utilisée comme validation par défaut.</span><span class="sxs-lookup"><span data-stu-id="fc041-110">If you select the **Default Posting** field, the statement line will be used as a default posting.</span></span>  

<span data-ttu-id="fc041-111">Si l'encodage CODA de la ligne relevé est trouvé, les lignes relevé seront associées aux types de comptes et aux numéros de comptes correspondants suivants :</span><span class="sxs-lookup"><span data-stu-id="fc041-111">If the transaction coding of the statement line is found, the statement lines will be matched to the following account types and corresponding account numbers:</span></span>  

- <span data-ttu-id="fc041-112">Comptes généraux : si le type de compte est un compte général, la ligne relevé est validée sur le compte général correspondant.</span><span class="sxs-lookup"><span data-stu-id="fc041-112">General ledger - If the account type is general ledger account, the statement line is posted on the corresponding general ledger account.</span></span>  

- <span data-ttu-id="fc041-113">Client ou fournisseur : si le type de compte est client ou fournisseur, une écriture comptable client ou fournisseur correspondante est trouvée selon les critères suivants :</span><span class="sxs-lookup"><span data-stu-id="fc041-113">Customer or vendor - If the account type is customer or vendor, a matching customer or vendor ledger entry is found based on the following criteria:</span></span>  

    - <span data-ttu-id="fc041-114">Si une écriture comptable est trouvée avec le format standard, l'écriture comptable sera associée à la ligne relevé et le statut lettrage sera défini sur **Lettrée**.</span><span class="sxs-lookup"><span data-stu-id="fc041-114">If a ledger entry is found using the standard format, the ledger entry will be matched to the statement line and the application status will be set to **Applied**.</span></span> <span data-ttu-id="fc041-115">Si l'écriture comptable n'est pas au format standard, le numéro de compte bancaire du client ou du fournisseur est utilisé pour retrouver le client ou le fournisseur.</span><span class="sxs-lookup"><span data-stu-id="fc041-115">If the ledger entry does not use the standard format, the bank account number of the customer or vendor is used to find the customer or vendor.</span></span>  

    - <span data-ttu-id="fc041-116">Si aucune écriture comptable avec un montant restant correspondant n'est trouvée, le compte client ou fournisseur est utilisé et le statut lettrage sera défini sur **Lettrée en partie**.</span><span class="sxs-lookup"><span data-stu-id="fc041-116">If no ledger entry with a matching remaining amount is found, the customer or vendor account is used and the application status will be set to **Partly Applied**.</span></span>  

    - <span data-ttu-id="fc041-117">Si le numéro de compte bancaire est utilisé pour trouver le client ou le fournisseur, une écriture comptable correspondant est trouvée en fonction du montant de la ligne relevé.</span><span class="sxs-lookup"><span data-stu-id="fc041-117">If the bank account number is used to find the customer or vendor, a matching ledger entry is found based on the amount of the statement line.</span></span> <span data-ttu-id="fc041-118">Si le montant est trouvé, la ligne relevé est associée à l'écriture comptable correspondante et le statut lettrage sera défini sur **Lettrée**.</span><span class="sxs-lookup"><span data-stu-id="fc041-118">If the amount is found, the statement line is matched to the corresponding ledger entry and the application status will be set to **Applied**.</span></span>  

    - <span data-ttu-id="fc041-119">Si le numéro de compte bancaire ne peut pas être utilisé pour trouver le client ou le fournisseur, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] interrompra le traitement de la ligne actuelle ou utilisera la ligne comme validation par défaut, avant de poursuivre avec la ligne relevé suivante.</span><span class="sxs-lookup"><span data-stu-id="fc041-119">If the bank account number cannot be used to find the customer or vendor, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] will either stop processing the current line or use the line as a default posting, before continuing with the next statement line.</span></span>  

<span data-ttu-id="fc041-120">Vous pouvez exécuter le traitement autant de fois que vous le souhaitez.</span><span class="sxs-lookup"><span data-stu-id="fc041-120">You can run the process as many times as you like.</span></span> <span data-ttu-id="fc041-121">Seules les lignes relevé dont le statut lettrage est vide seront lettrées.</span><span class="sxs-lookup"><span data-stu-id="fc041-121">Only statement lines with a blank application status will be applied.</span></span>  

<span data-ttu-id="fc041-122">Lorsque vous avez lettré toutes les lignes relevé à un compte général ou à une écriture comptable client ou fournisseur correspondante, vous pouvez valider les lignes relevé CODA.</span><span class="sxs-lookup"><span data-stu-id="fc041-122">When you have applied all statement lines to a general ledger account or to a matching customer ledger entry or vendor ledger entry, you are ready to post the CODA statement lines.</span></span> <span data-ttu-id="fc041-123">Pour plus d'informations, voir [Transférer et publier automatiquement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="fc041-123">For more information, see [Automatically Transfer and Post CODA Statements](how-to-manually-transfer-and-post-coda-statements.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="fc041-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fc041-124">See Also</span></span>  
 <span data-ttu-id="fc041-125">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="fc041-125">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="fc041-126">[Configurer des comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md) </span><span class="sxs-lookup"><span data-stu-id="fc041-126">[Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md) </span></span>  
 <span data-ttu-id="fc041-127">[Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="fc041-127">[Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="fc041-128">[Importer des relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="fc041-128">[Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="fc041-129">[Lettrer des relevés CODA](how-to-apply-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="fc041-129">[Apply CODA Statements](how-to-apply-coda-statements.md) </span></span>  
 <span data-ttu-id="fc041-130">[Créer des feuilles financières](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="fc041-130">[Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 <span data-ttu-id="fc041-131">[Transférer et publier automatiquement des relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="fc041-131">[Automatically Transfer and Post CODA Statements](how-to-automatically-transfer-and-post-coda-statements.md) </span></span>  
 [<span data-ttu-id="fc041-132">Transférer et publier manuellement des relevés CODA</span><span class="sxs-lookup"><span data-stu-id="fc041-132">Manually Transfer and Post CODA Statements</span></span>](how-to-manually-transfer-and-post-coda-statements.md)

