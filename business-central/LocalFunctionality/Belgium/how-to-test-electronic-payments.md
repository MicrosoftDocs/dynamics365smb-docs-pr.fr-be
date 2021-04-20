---
title: Tester les paiements électroniques dans la version belge
description: Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: d978afd9acc11bd574af42bc93d265a509568334
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779192"
---
# <a name="test-electronic-payments"></a><span data-ttu-id="a27bc-103">Tester les paiements électroniques</span><span class="sxs-lookup"><span data-stu-id="a27bc-103">Test Electronic Payments</span></span>

<span data-ttu-id="a27bc-104">Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.</span><span class="sxs-lookup"><span data-stu-id="a27bc-104">After you have set up electronic banking and generated payment suggestions, you can test the payment journal lines for errors before posting them.</span></span>  

<span data-ttu-id="a27bc-105">Certaines des informations validées sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="a27bc-105">Some of the information that is validated includes:</span></span>  

- <span data-ttu-id="a27bc-106">Si les numéros des comptes bancaires sont valides.</span><span class="sxs-lookup"><span data-stu-id="a27bc-106">Whether bank account numbers are valid.</span></span>  
- <span data-ttu-id="a27bc-107">Si les lignes paiement positives sont présentes.</span><span class="sxs-lookup"><span data-stu-id="a27bc-107">Whether positive payment lines are present.</span></span>  
- <span data-ttu-id="a27bc-108">Si les paiements nationaux et internationaux sont effectués à partir d'un seul compte bancaire.</span><span class="sxs-lookup"><span data-stu-id="a27bc-108">Whether domestic and international payments are made from only one bank account.</span></span>  
- <span data-ttu-id="a27bc-109">Si un seul compte bancaire peut être utilisé pour Isabel (Interbanks Standards Association Belgium).</span><span class="sxs-lookup"><span data-stu-id="a27bc-109">Whether only one bank account can be used for Interbanks Standards Association Belgium (Isabel).</span></span>  
- <span data-ttu-id="a27bc-110">Si des lignes de paiement sont en euros pour SEPA (Espace unique de paiement en euros).</span><span class="sxs-lookup"><span data-stu-id="a27bc-110">Whether payment lines are in euro for Single Euro Payments Area (SEPA).</span></span>  
- <span data-ttu-id="a27bc-111">Si une souche de numéros a été définie pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="a27bc-111">Whether a number series has been defined for SEPA.</span></span>  

<span data-ttu-id="a27bc-112">Vous pouvez afficher les erreurs sur la page **Exporter/Vérifier les journaux des erreurs**.</span><span class="sxs-lookup"><span data-stu-id="a27bc-112">You can view any errors on the **Export Check Error Logs** page.</span></span>  

> [!IMPORTANT]  
> <span data-ttu-id="a27bc-113">Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.</span><span class="sxs-lookup"><span data-stu-id="a27bc-113">You have to correct all errors before you can post the lines.</span></span>  

## <a name="to-test-payment-journal-lines"></a><span data-ttu-id="a27bc-114">Pour tester les lignes feuille paiement</span><span class="sxs-lookup"><span data-stu-id="a27bc-114">To test payment journal lines</span></span>  

1. <span data-ttu-id="a27bc-115">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles paiement**, puis sélectionnez le lien pour ouvrir la page **Feuilles paiement EB**.</span><span class="sxs-lookup"><span data-stu-id="a27bc-115">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the link to open the **EB Payment Journals** page.</span></span>  
2. <span data-ttu-id="a27bc-116">Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.</span><span class="sxs-lookup"><span data-stu-id="a27bc-116">In the **Batch Name** field, select the required journal batch.</span></span>  
3. <span data-ttu-id="a27bc-117">Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="a27bc-117">In the **Export Protocol** field, select the export protocol.</span></span>  
4. <span data-ttu-id="a27bc-118">Entrez les informations sur les lignes feuille paiement, puis choisissez l'action **Vérifier lignes paiement** pour valider les lignes feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="a27bc-118">Enter the payment journal line information, and then choose the **Check Payment Lines** action to validate the payment journal lines.</span></span> <span data-ttu-id="a27bc-119">La validation réalisée sur les lignes feuille dépend du type de vérification spécifié dans la page **Protocoles d'exportation**.</span><span class="sxs-lookup"><span data-stu-id="a27bc-119">The validation that is performed on the journal lines depends on the type of check that is specified on the **Export Protocols** page.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a27bc-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a27bc-120">See Also</span></span>  

[<span data-ttu-id="a27bc-121">Créer des modèles et des lots de feuilles paiement</span><span class="sxs-lookup"><span data-stu-id="a27bc-121">Create Payment Journal Templates and Batches</span></span>](how-to-create-payment-journal-templates-and-batches.md)  
[<span data-ttu-id="a27bc-122">Paiements électroniques belges</span><span class="sxs-lookup"><span data-stu-id="a27bc-122">Belgian Electronic Payments</span></span>](belgian-electronic-payments.md)  
[<span data-ttu-id="a27bc-123">Paramétrer les fournisseurs pour des suggestions de règlement automatique</span><span class="sxs-lookup"><span data-stu-id="a27bc-123">Set Up Vendors for Automatic Payment Suggestions</span></span>](how-to-set-up-vendors-for-automatic-payment-suggestions.md)  
[<span data-ttu-id="a27bc-124">Proposer paiements fournisseur</span><span class="sxs-lookup"><span data-stu-id="a27bc-124">Suggest Vendor Payments</span></span>](../../payables-how-suggest-vendor-payments.md)  
[<span data-ttu-id="a27bc-125">Imprimer les fichiers de paiement</span><span class="sxs-lookup"><span data-stu-id="a27bc-125">Print Payment Files</span></span>](how-to-print-payment-files.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
