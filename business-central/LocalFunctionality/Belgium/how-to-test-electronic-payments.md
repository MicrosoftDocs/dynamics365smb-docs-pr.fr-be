---
title: Test des paiements électroniques
description: Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.
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
ms.openlocfilehash: fae1e4edb37f64983e76f0a5d7158000f057d161
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237747"
---
# <a name="test-electronic-payments"></a><span data-ttu-id="caac3-103">Tester les paiements électroniques</span><span class="sxs-lookup"><span data-stu-id="caac3-103">Test Electronic Payments</span></span>
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

<span data-ttu-id="caac3-104">Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.</span><span class="sxs-lookup"><span data-stu-id="caac3-104">After you have set up electronic banking and generated payment suggestions, you can test the payment journal lines for errors before posting them.</span></span>  

<span data-ttu-id="caac3-105">Certaines des informations validées sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="caac3-105">Some of the information that is validated includes:</span></span>  

- <span data-ttu-id="caac3-106">Les numéros des comptes bancaires sont valides.</span><span class="sxs-lookup"><span data-stu-id="caac3-106">Bank accounts numbers are valid.</span></span>  
- <span data-ttu-id="caac3-107">Les lignes paiement positives sont présentes.</span><span class="sxs-lookup"><span data-stu-id="caac3-107">Positive payment lines are present.</span></span>  
- <span data-ttu-id="caac3-108">Si les paiements nationaux et internationaux sont effectués à partir d'un seul compte bancaire.</span><span class="sxs-lookup"><span data-stu-id="caac3-108">If domestic and international payments are made from only one bank account.</span></span>  
- <span data-ttu-id="caac3-109">Si un seul compte bancaire peut être utilisé pour Isabel.</span><span class="sxs-lookup"><span data-stu-id="caac3-109">If only one bank account can be used for Isabel.</span></span>  
- <span data-ttu-id="caac3-110">Si les lignes paiement sont en euro pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="caac3-110">If payment lines are in Euro for SEPA.</span></span>  
- <span data-ttu-id="caac3-111">Si une souche de numéros a été définie pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="caac3-111">If a number series has been defined for SEPA.</span></span>  

<span data-ttu-id="caac3-112">Vous pouvez afficher les erreurs sur la page **Exporter/Vérifier les journaux des erreurs**.</span><span class="sxs-lookup"><span data-stu-id="caac3-112">You can view any errors on the **Export Check Error Logs** page.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="caac3-113">Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.</span><span class="sxs-lookup"><span data-stu-id="caac3-113">You have to correct all errors before you can post the lines.</span></span>  

## <a name="to-test-payment-journal-lines"></a><span data-ttu-id="caac3-114">Pour tester les lignes feuille paiement</span><span class="sxs-lookup"><span data-stu-id="caac3-114">To test payment journal lines</span></span>  

1.  <span data-ttu-id="caac3-115">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles paiement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="caac3-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="caac3-116">Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.</span><span class="sxs-lookup"><span data-stu-id="caac3-116">In the **Batch Name** field, select the required journal batch.</span></span>  
3.  <span data-ttu-id="caac3-117">Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="caac3-117">In the **Export Protocol** field, select the export protocol.</span></span>  
4.  <span data-ttu-id="caac3-118">Entrez les informations sur les lignes feuille paiement, puis choisissez l'action **Vérifier lignes paiement** pour valider les lignes feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="caac3-118">Enter the payment journal line information, and then choose the **Check Payment Lines** action to validate the payment journal lines.</span></span> <span data-ttu-id="caac3-119">La validation réalisée sur les lignes feuille dépend du type de vérification spécifié dans la page **Protocoles d'exportation**.</span><span class="sxs-lookup"><span data-stu-id="caac3-119">The validation that is performed on the journal lines depends on the type of check that is specified on the **Export Protocols** page.</span></span>  

## <a name="see-also"></a><span data-ttu-id="caac3-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="caac3-120">See Also</span></span>  
 <span data-ttu-id="caac3-121">[Paiements électroniques, Belgique](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="caac3-121">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="caac3-122">[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="caac3-122">[Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="caac3-123">[Générer des suggestions de règlement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="caac3-123">[Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 [<span data-ttu-id="caac3-124">Imprimer les fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="caac3-124">Print Payment Files</span></span>](how-to-print-payment-files.md)
