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
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 47d255e1217eca08d073400ea92adaf012d76c71
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676600"
---
# <a name="activate-sepa-payments"></a><span data-ttu-id="61f29-103">Activer des paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="61f29-103">Activate SEPA Payments</span></span>
<span data-ttu-id="61f29-104">Pour soumettre les paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA.</span><span class="sxs-lookup"><span data-stu-id="61f29-104">To submit vendor payments electronically in Single Euro Payments Area (SEPA) ISO 20022 payment format, you must set up prerequisites for enabling SEPA payments.</span></span>  

<span data-ttu-id="61f29-105">Les procédures suivantes sont consacrées à l'activation d'un paiement SEPA et à la configuration de comptes bancaires fournisseur.</span><span class="sxs-lookup"><span data-stu-id="61f29-105">The following procedures describe how to enable SEPA payment and set up vendor bank accounts.</span></span>  

## <a name="to-enable-countriesregions-for-sepa"></a><span data-ttu-id="61f29-106">Pour activer des pays/régions pour SEPA</span><span class="sxs-lookup"><span data-stu-id="61f29-106">To enable countries/regions for SEPA</span></span>  

1.  <span data-ttu-id="61f29-107">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Pays/Régions**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="61f29-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="61f29-108">Choisissez l'action **Modifier la liste**.</span><span class="sxs-lookup"><span data-stu-id="61f29-108">Choose the **Edit List** action.</span></span>  
3.  <span data-ttu-id="61f29-109">Activez la case à cocher **SEPA autorisé** pour chaque pays ou région que vous souhaitez activer pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="61f29-109">Select the **SEPA Allowed** check box for each country or region that you want to enable for SEPA.</span></span>  
4.  <span data-ttu-id="61f29-110">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="61f29-110">Choose the **OK** button.</span></span>  

## <a name="to-enable-bank-accounts-for-sepa"></a><span data-ttu-id="61f29-111">Pour activer des comptes bancaires pour SEPA</span><span class="sxs-lookup"><span data-stu-id="61f29-111">To enable bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="61f29-112">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Comptes bancaires**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="61f29-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="61f29-113">Sélectionnez le compte bancaire que vous souhaitez activer pour SEPA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="61f29-113">Select the bank account that you want to enable for SEPA, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="61f29-114">Dans le champ **Code pays/région**, sélectionnez le code approprié.</span><span class="sxs-lookup"><span data-stu-id="61f29-114">In the **Country/Region Code** field, select the appropriate code.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="61f29-115">Le code pays/région spécifié doit être activé pour SEPA, comme décrit dans la procédure précédente.</span><span class="sxs-lookup"><span data-stu-id="61f29-115">The specified country/region code must be enabled for SEPA as described in the previous procedure.</span></span>  

4.  <span data-ttu-id="61f29-116">Entrez une valeur dans le champ **Solde minimum**.</span><span class="sxs-lookup"><span data-stu-id="61f29-116">Enter a value in the **Min. Balance** field.</span></span>  
5.  <span data-ttu-id="61f29-117">Dans le champ **Code SWIFT**, entrez un code.</span><span class="sxs-lookup"><span data-stu-id="61f29-117">In the **SWIFT Code** field, enter a code.</span></span>  
6.  <span data-ttu-id="61f29-118">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="61f29-118">Choose the **OK** button.</span></span>  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a><span data-ttu-id="61f29-119">Pour configurer des comptes bancaires fournisseur pour SEPA</span><span class="sxs-lookup"><span data-stu-id="61f29-119">To set up vendor bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="61f29-120">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Fournisseurs**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="61f29-120">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="61f29-121">Sélectionnez le fournisseur concerné, puis choisissez l'action **Comptes bancaires**.</span><span class="sxs-lookup"><span data-stu-id="61f29-121">Select the relevant vendor, and then choose the **Bank Accounts** action.</span></span>  
3.  <span data-ttu-id="61f29-122">Sélectionnez le compte bancaire fournisseur à paramétrer pour SEPA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="61f29-122">Select the vendor bank account to set up for SEPA, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="61f29-123">Dans les champs **IBAN** et **Code SWIFT**, entrez le code international d'identification bancaire de la banque auprès de laquelle le fournisseur a son compte.</span><span class="sxs-lookup"><span data-stu-id="61f29-123">In the **IBAN** and **SWIFT Code** fields, enter the international bank identifier code of the bank where the vendor has the account.</span></span>  
5.  <span data-ttu-id="61f29-124">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="61f29-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="61f29-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="61f29-125">See Also</span></span>  
 <span data-ttu-id="61f29-126">[Paiements SEPA](sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="61f29-126">[SEPA Payments](sepa-payments.md) </span></span>  
 <span data-ttu-id="61f29-127">[Classer les paiements SEPA](how-to-file-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="61f29-127">[File SEPA Payments](how-to-file-sepa-payments.md) </span></span>  
 <span data-ttu-id="61f29-128">[Classer les paiements SEPA hors Euro](how-to-file-non-euro-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="61f29-128">[File Non-Euro SEPA Payments](how-to-file-non-euro-sepa-payments.md) </span></span>  
 [<span data-ttu-id="61f29-129">Configurer les protocoles d'exportation</span><span class="sxs-lookup"><span data-stu-id="61f29-129">Set Up Export Protocols</span></span>](how-to-set-up-export-protocols.md)
