---
title: "Comment tester les paiements électroniques"
description: "Après avoir configuré la banque électronique et généré des propositions de paiement, vous pouvez tester les lignes feuille paiement pour repérer les éventuelles erreurs avant de valider les lignes."
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
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: 668ab15d26ffa3f28b658f315d88108b2174a623
ms.contentlocale: fr-be
ms.lasthandoff: 04/16/2018

---
# <a name="test-electronic-payments"></a><span data-ttu-id="80284-103">Tester les paiements électroniques</span><span class="sxs-lookup"><span data-stu-id="80284-103">Test Electronic Payments</span></span>
> [!Note]
> [!INCLUDE [onprem_only](../../includes/onprem_only_md.md)]

<span data-ttu-id="80284-104">Après avoir créé des transactions bancaires électroniques et des propositions de paiement générées, vous pouvez tester les lignes feuille paiement pour les erreurs avant de les valider.</span><span class="sxs-lookup"><span data-stu-id="80284-104">After you have set up electronic banking and generated payment suggestions, you can test the payment journal lines for errors before posting them.</span></span>  

<span data-ttu-id="80284-105">Les informations validées incluent notamment :</span><span class="sxs-lookup"><span data-stu-id="80284-105">Some of the information that is validated includes:</span></span>  

- <span data-ttu-id="80284-106">Les numéros de comptes bancaires sont valides.</span><span class="sxs-lookup"><span data-stu-id="80284-106">Bank accounts numbers are valid.</span></span>  
- <span data-ttu-id="80284-107">Il y a des lignes paiement positives.</span><span class="sxs-lookup"><span data-stu-id="80284-107">Positive payment lines are present.</span></span>  
- <span data-ttu-id="80284-108">Si les paiements nationaux et internationaux sont effectués depuis un seul compte bancaire.</span><span class="sxs-lookup"><span data-stu-id="80284-108">If domestic and international payments are made from only one bank account.</span></span>  
- <span data-ttu-id="80284-109">Si un seul compte bancaire peut être utilisé pour Isabel.</span><span class="sxs-lookup"><span data-stu-id="80284-109">If only one bank account can be used for Isabel.</span></span>  
- <span data-ttu-id="80284-110">Si les lignes paiement sont en Euro pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="80284-110">If payment lines are in Euro for SEPA.</span></span>  
- <span data-ttu-id="80284-111">Si une souche de numéros a été définie pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="80284-111">If a number series has been defined for SEPA.</span></span>  

<span data-ttu-id="80284-112">Vous pouvez consulter les éventuelles erreurs dans la fenêtre **Exporter les journaux d'erreur de chèque**.</span><span class="sxs-lookup"><span data-stu-id="80284-112">You can view any errors in the **Export Check Error Logs** window.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="80284-113">Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.</span><span class="sxs-lookup"><span data-stu-id="80284-113">You have to correct all errors before you can post the lines.</span></span>  

## <a name="to-test-payment-journal-lines"></a><span data-ttu-id="80284-114">Pour tester les lignes feuille paiement</span><span class="sxs-lookup"><span data-stu-id="80284-114">To test payment journal lines</span></span>  

1.  <span data-ttu-id="80284-115">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles paiement**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="80284-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="80284-116">Dans le champ **Nom feuille**, sélectionnez la feuille concernée.</span><span class="sxs-lookup"><span data-stu-id="80284-116">In the **Batch Name** field, select the required journal batch.</span></span>  
3.  <span data-ttu-id="80284-117">Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="80284-117">In the **Export Protocol** field, select the export protocol.</span></span>  
4.  <span data-ttu-id="80284-118">Entrez les informations ligne feuille paiement, puis choisissez l'action **Vérifier les lignes de paiement** pour valider les lignes feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="80284-118">Enter the payment journal line information, and then choose the **Check Payment Lines** action to validate the payment journal lines.</span></span> <span data-ttu-id="80284-119">La validation effectuée sur les lignes feuille dépend du type de contrôle indiqué dans la fenêtre **Protocoles d'exportation**.</span><span class="sxs-lookup"><span data-stu-id="80284-119">The validation that is performed on the journal lines depends on the type of check that is specified in the **Export Protocols** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="80284-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="80284-120">See Also</span></span>  
 <span data-ttu-id="80284-121">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="80284-121">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="80284-122">[Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="80284-122">[Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="80284-123">[Générer des propositions de paiement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="80284-123">[Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 [<span data-ttu-id="80284-124">Imprimer des fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="80284-124">Print Payment Files</span></span>](how-to-print-payment-files.md)

