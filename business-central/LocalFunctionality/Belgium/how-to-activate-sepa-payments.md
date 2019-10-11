---
title: Comment activer les paiements SEPA
description: Pour soumettre les paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: e7e1219c644e7115047af14c6550d41f7d613566
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300276"
---
# <a name="activate-sepa-payments"></a><span data-ttu-id="3ccda-103">Activer des paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="3ccda-103">Activate SEPA Payments</span></span>
<span data-ttu-id="3ccda-104">Pour soumettre les paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA.</span><span class="sxs-lookup"><span data-stu-id="3ccda-104">To submit vendor payments electronically in Single Euro Payments Area (SEPA) ISO 20022 payment format, you must set up prerequisites for enabling SEPA payments.</span></span>  

<span data-ttu-id="3ccda-105">Les procédures suivantes sont consacrées à l'activation d'un paiement SEPA et à la configuration de comptes bancaires fournisseur.</span><span class="sxs-lookup"><span data-stu-id="3ccda-105">The following procedures describe how to enable SEPA payment and set up vendor bank accounts.</span></span>  

## <a name="to-enable-countriesregions-for-sepa"></a><span data-ttu-id="3ccda-106">Pour activer des pays/régions pour SEPA</span><span class="sxs-lookup"><span data-stu-id="3ccda-106">To enable countries/regions for SEPA</span></span>  

1.  <span data-ttu-id="3ccda-107">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Pays/Régions**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="3ccda-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Countries/Regions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="3ccda-108">Choisissez l'action **Modifier la liste**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-108">Choose the **Edit List** action.</span></span>  
3.  <span data-ttu-id="3ccda-109">Activez la case à cocher **SEPA autorisé** pour chaque pays ou région que vous souhaitez activer pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="3ccda-109">Select the **SEPA Allowed** check box for each country or region that you want to enable for SEPA.</span></span>  
4.  <span data-ttu-id="3ccda-110">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-110">Choose the **OK** button.</span></span>  

## <a name="to-enable-bank-accounts-for-sepa"></a><span data-ttu-id="3ccda-111">Pour activer des comptes bancaires pour SEPA</span><span class="sxs-lookup"><span data-stu-id="3ccda-111">To enable bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="3ccda-112">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="3ccda-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="3ccda-113">Sélectionnez le compte bancaire que vous souhaitez activer pour SEPA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-113">Select the bank account that you want to enable for SEPA, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="3ccda-114">Dans le champ **Code pays/région**, sélectionnez le code approprié.</span><span class="sxs-lookup"><span data-stu-id="3ccda-114">In the **Country/Region Code** field, select the appropriate code.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="3ccda-115">Le code pays/région spécifié doit être activé pour SEPA, comme décrit dans la procédure précédente.</span><span class="sxs-lookup"><span data-stu-id="3ccda-115">The specified country/region code must be enabled for SEPA as described in the previous procedure.</span></span>  

4.  <span data-ttu-id="3ccda-116">Entrez une valeur dans le champ **Solde minimum**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-116">Enter a value in the **Min. Balance** field.</span></span>  
5.  <span data-ttu-id="3ccda-117">Dans le champ **Code SWIFT**, entrez un code.</span><span class="sxs-lookup"><span data-stu-id="3ccda-117">In the **SWIFT Code** field, enter a code.</span></span>  
6.  <span data-ttu-id="3ccda-118">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-118">Choose the **OK** button.</span></span>  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a><span data-ttu-id="3ccda-119">Pour configurer des comptes bancaires fournisseur pour SEPA</span><span class="sxs-lookup"><span data-stu-id="3ccda-119">To set up vendor bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="3ccda-120">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Fournisseurs**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="3ccda-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="3ccda-121">Sélectionnez le fournisseur concerné, puis choisissez l'action **Comptes bancaires**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-121">Select the relevant vendor, and then choose the **Bank Accounts** action.</span></span>  
3.  <span data-ttu-id="3ccda-122">Sélectionnez le compte bancaire fournisseur à paramétrer pour SEPA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-122">Select the vendor bank account to set up for SEPA, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="3ccda-123">Dans les champs **IBAN** et **Code SWIFT**, entrez le code international d'identification bancaire de la banque auprès de laquelle le fournisseur a son compte.</span><span class="sxs-lookup"><span data-stu-id="3ccda-123">In the **IBAN** and **SWIFT Code** fields, enter the international bank identifier code of the bank where the vendor has the account.</span></span>  
5.  <span data-ttu-id="3ccda-124">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="3ccda-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3ccda-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3ccda-125">See Also</span></span>  
 <span data-ttu-id="3ccda-126">[Paiements SEPA](sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="3ccda-126">[SEPA Payments](sepa-payments.md) </span></span>  
 <span data-ttu-id="3ccda-127">[Classer les paiements SEPA](how-to-file-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="3ccda-127">[File SEPA Payments](how-to-file-sepa-payments.md) </span></span>  
 <span data-ttu-id="3ccda-128">[Classer les paiements SEPA hors Euro](how-to-file-non-euro-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="3ccda-128">[File Non-Euro SEPA Payments](how-to-file-non-euro-sepa-payments.md) </span></span>  
 [<span data-ttu-id="3ccda-129">Configurer les protocoles d'exportation</span><span class="sxs-lookup"><span data-stu-id="3ccda-129">Set Up Export Protocols</span></span>](how-to-set-up-export-protocols.md)
