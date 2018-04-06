---
title: Comment activer les paiements SEPA
description: "Pour envoyer les paiements des fournisseurs par voie électronique au format de paiement ISO 20022 de l'Espace unique de paiement en euros (SEPA), vous devez définir les prérequis pour l'activation des paiements SEPA."
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
ms.openlocfilehash: 3f53a511b47702726d0142d24e9a4fb7159200c9
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="activate-sepa-payments"></a><span data-ttu-id="14291-103">Activer des paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="14291-103">Activate SEPA Payments</span></span>
<span data-ttu-id="14291-104">Pour envoyer les paiements des fournisseurs par voie électronique au format de paiement ISO 20022 de l'Espace unique de paiement en euros (SEPA), vous devez définir les prérequis pour l'activation des paiements SEPA.</span><span class="sxs-lookup"><span data-stu-id="14291-104">To submit vendor payments electronically in Single Euro Payments Area (SEPA) ISO 20022 payment format, you must set up prerequisites for enabling SEPA payments.</span></span>  

<span data-ttu-id="14291-105">Les procédures suivantes sont consacrées à l'activation d'un paiement SEPA et à la configuration de comptes bancaires fournisseur.</span><span class="sxs-lookup"><span data-stu-id="14291-105">In the following procedures describe how to enable SEPA payment and set up vendor bank accounts.</span></span>  

## <a name="to-enable-countriesregions-for-sepa"></a><span data-ttu-id="14291-106">Pour activer des pays/régions pour SEPA</span><span class="sxs-lookup"><span data-stu-id="14291-106">To enable countries/regions for SEPA</span></span>  

1.  <span data-ttu-id="14291-107">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Pays/Régions**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="14291-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Countries/Regions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="14291-108">Choisissez l'action **Modifier la liste**.</span><span class="sxs-lookup"><span data-stu-id="14291-108">Choose the **Edit List** action.</span></span>  
3.  <span data-ttu-id="14291-109">Activez la case à cocher **SEPA autorisé** pour chaque pays ou région que vous souhaitez activer pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="14291-109">Select the **SEPA Allowed** check box for each country or region that you want to enable for SEPA.</span></span>  
4.  <span data-ttu-id="14291-110">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="14291-110">Choose the **OK** button.</span></span>  

## <a name="to-enable-bank-accounts-for-sepa"></a><span data-ttu-id="14291-111">Pour activer des comptes bancaires pour SEPA</span><span class="sxs-lookup"><span data-stu-id="14291-111">To enable bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="14291-112">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="14291-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="14291-113">Sélectionnez le compte bancaire que vous souhaitez activer pour SEPA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="14291-113">Select the bank account that you want to enable for SEPA, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="14291-114">Dans le raccourci **Général**, dans le champ **Pays/Région**, sélectionnez le code adéquat.</span><span class="sxs-lookup"><span data-stu-id="14291-114">On the **General** FastTab, in the **Country/Region Code** field, select the appropriate code.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="14291-115">Le code pays/région spécifié doit être activé pour SEPA, comme décrit dans la procédure précédente.</span><span class="sxs-lookup"><span data-stu-id="14291-115">The specified country/region code must be enabled for SEPA as described in the previous procedure.</span></span>  

4.  <span data-ttu-id="14291-116">Entrez une valeur dans le champ **Solde minimum**.</span><span class="sxs-lookup"><span data-stu-id="14291-116">Enter a value in the **Min. Balance** field.</span></span>  
5.  <span data-ttu-id="14291-117">Dans le raccourci **Transfert**, dans le champs **Code SWIFT**, entrez un code.</span><span class="sxs-lookup"><span data-stu-id="14291-117">On the **Transfer** FastTab, in the **SWIFT Code** field, enter a code.</span></span>  
6.  <span data-ttu-id="14291-118">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="14291-118">Choose the **OK** button.</span></span>  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a><span data-ttu-id="14291-119">Pour configurer des comptes bancaires fournisseur pour SEPA</span><span class="sxs-lookup"><span data-stu-id="14291-119">To set up vendor bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="14291-120">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Fournisseurs**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="14291-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="14291-121">Sélectionnez le fournisseur concerné, puis choisissez l'action **Comptes bancaires**.</span><span class="sxs-lookup"><span data-stu-id="14291-121">Select the relevant vendor, and then choose the **Bank Accounts** action.</span></span>  
3.  <span data-ttu-id="14291-122">Sélectionnez le compte bancaire fournisseur à paramétrer pour SEPA, puis choisissez **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="14291-122">Select the vendor bank account to set up for SEPA, and then choose the **Edit**.</span></span>  
4.  <span data-ttu-id="14291-123">Dans le raccourci **Transfert**, dans les champs **N° compte bancaire international** et **Code SWIFT**, entrez le code d'identification bancaire international de la banque où le fournisseur a ouvert le compte.</span><span class="sxs-lookup"><span data-stu-id="14291-123">On the **Transfer** FastTab, in the **IBAN** and **SWIFT Code** fields, enter the international bank identifier code of the bank where the vendor has the account.</span></span>  
5.  <span data-ttu-id="14291-124">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="14291-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="14291-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="14291-125">See Also</span></span>  
 <span data-ttu-id="14291-126">[Paiements SEPA](sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="14291-126">[SEPA Payments](sepa-payments.md) </span></span>  
 <span data-ttu-id="14291-127">[Classer les paiements SEPA](how-to-file-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="14291-127">[File SEPA Payments](how-to-file-sepa-payments.md) </span></span>  
 <span data-ttu-id="14291-128">[Classer les paiements SEPA hors Euro](how-to-file-non-euro-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="14291-128">[File Non-Euro SEPA Payments](how-to-file-non-euro-sepa-payments.md) </span></span>  
 [<span data-ttu-id="14291-129">Configurer les protocoles d'exportation</span><span class="sxs-lookup"><span data-stu-id="14291-129">Set Up Export Protocols</span></span>](how-to-set-up-export-protocols.md)

