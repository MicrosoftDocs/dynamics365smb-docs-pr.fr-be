---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 08/26/2020
ms.author: edupont
ms.openlocfilehash: 432d0d4457ecf36427452b699dcf3b9c51d5a006
ms.sourcegitcommit: 3e2eab6920e96596cb4b3c61e590a8c577e8b630
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 08/27/2020
ms.locfileid: "3731360"
---
<span data-ttu-id="ca8e3-101">Pour soumettre des paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA dans votre société.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-101">To submit vendor payments electronically in Single Euro Payments Area (SEPA) ISO 20022 payment format, you must set up prerequisites for enabling SEPA payments in your company.</span></span>  

<span data-ttu-id="ca8e3-102">Les procédures suivantes décrivent comment paramétrer des paiements SEPA et comment modifier la configuration pour des fournisseurs spécifiques.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-102">The following procedures describe how to set up SEPA payments, including how to modify the setup for specific vendors.</span></span>  

## <a name="to-enable-countriesregions-for-sepa"></a><span data-ttu-id="ca8e3-103">Pour activer des pays/régions pour SEPA</span><span class="sxs-lookup"><span data-stu-id="ca8e3-103">To enable countries/regions for SEPA</span></span>  

1. <span data-ttu-id="ca8e3-104">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Pays/Régions**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-104">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ca8e3-105">Choisissez l'action **Modifier la liste**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-105">Choose the **Edit List** action.</span></span>  
3. <span data-ttu-id="ca8e3-106">Activez la case à cocher **SEPA autorisé** pour chaque pays ou région que vous souhaitez activer pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-106">Select the **SEPA Allowed** check box for each country or region that you want to enable for SEPA.</span></span>  
4. <span data-ttu-id="ca8e3-107">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-107">Choose the **OK** button.</span></span>  

## <a name="to-enable-bank-accounts-for-sepa"></a><span data-ttu-id="ca8e3-108">Pour activer des comptes bancaires pour SEPA</span><span class="sxs-lookup"><span data-stu-id="ca8e3-108">To enable bank accounts for SEPA</span></span>  

1. <span data-ttu-id="ca8e3-109">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Comptes bancaires**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-109">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ca8e3-110">Sélectionnez le compte bancaire que vous souhaitez activer pour SEPA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-110">Select the bank account that you want to enable for SEPA, and then choose the **Edit** action.</span></span>  
3. <span data-ttu-id="ca8e3-111">Dans le raccourci **Général**, dans le champ **Pays/Région**, sélectionnez le code adéquat.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-111">On the **General** FastTab, in the **Country/Region Code** field, select the appropriate code.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="ca8e3-112">Le code pays/région spécifié doit être activé pour SEPA, comme décrit dans la procédure précédente.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-112">The specified country/region code must be enabled for SEPA as described in the previous procedure.</span></span>  

4. <span data-ttu-id="ca8e3-113">Entrez une valeur dans le champ **Solde minimum**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-113">Enter a value in the **Min. Balance** field.</span></span>  
5. <span data-ttu-id="ca8e3-114">Dans le raccourci **Transfert**, dans le champs **Code SWIFT**, entrez un code.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-114">On the **Transfer** FastTab, in the **SWIFT Code** field, enter a code.</span></span>  
6. <span data-ttu-id="ca8e3-115">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-115">Choose the **OK** button.</span></span>  

## <a name="to-set-up-a-sepa-iso-20022-export-protocol"></a><span data-ttu-id="ca8e3-116">Pour paramétrer un protocole d'exportation SEPA ISO 20022</span><span class="sxs-lookup"><span data-stu-id="ca8e3-116">To set up a SEPA ISO 20022 export protocol</span></span>  

1. <span data-ttu-id="ca8e3-117">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Protocoles d'exportation**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-117">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Export Protocols**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ca8e3-118">Sur la page **Protocoles d'exportation**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-118">On the **Export Protocols** page, choose the **New** action.</span></span>  
3. <span data-ttu-id="ca8e3-119">Renseignez les champs.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-119">Fill in the fields.</span></span> [!INCLUDE [tooltip-inline-tip_md](../../../includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="ca8e3-120">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-120">Choose the **OK** button.</span></span>  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a><span data-ttu-id="ca8e3-121">Pour configurer des comptes bancaires fournisseur pour SEPA</span><span class="sxs-lookup"><span data-stu-id="ca8e3-121">To set up vendor bank accounts for SEPA</span></span>  

1. <span data-ttu-id="ca8e3-122">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Fournisseurs**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-122">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ca8e3-123">Sélectionnez le fournisseur concerné, puis choisissez l'action **Comptes bancaires**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-123">Select the relevant vendor, and then choose the **Bank Accounts** action.</span></span>  
3. <span data-ttu-id="ca8e3-124">Sélectionnez le compte bancaire fournisseur à paramétrer pour SEPA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-124">Select the vendor bank account to set up for SEPA, and then choose the **Edit** action.</span></span>  
4. <span data-ttu-id="ca8e3-125">Dans le raccourci **Transfert**, dans les champs **IBAN** et **Code SWIFT**, entrez le code international d'identification bancaire ou la banque auprès de laquelle le fournisseur a son compte.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-125">On the **Transfer** FastTab, in the **IBAN** and **SWIFT Code** fields, enter the international bank identifier code of the bank where the vendor has the account.</span></span>  
5. <span data-ttu-id="ca8e3-126">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ca8e3-126">Choose the **OK** button.</span></span>  