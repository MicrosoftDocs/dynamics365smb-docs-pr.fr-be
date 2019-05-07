---
title: Effectuer des paiements SEPA
description: Dans Business Central, vous pouvez utiliser les virements SEPA pour effectuer des paiements SEPA auprès de la banque.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: e24b63e60bbaea99a8c093ac556288aef7ced9c8
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2019
ms.locfileid: "913746"
---
# <a name="file-sepa-payments"></a><span data-ttu-id="3ce45-103">Effectuer des paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="3ce45-103">File SEPA Payments</span></span>
<span data-ttu-id="3ce45-104">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez utiliser les virements SEPA pour effectuer des paiements SEPA auprès de la banque.</span><span class="sxs-lookup"><span data-stu-id="3ce45-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use Single Euro Payments Area (SEPA) credit transfers to file SEPA payments with the bank.</span></span>  

<span data-ttu-id="3ce45-105">SEPA unifie les modes de paiement dans les pays/régions européens participants, ce qui rend les paiements internationaux aussi faciles à traiter que les paiements nationaux.</span><span class="sxs-lookup"><span data-stu-id="3ce45-105">SEPA unifies payment methods in participating European countries/regions, which makes international payments as easy to process as domestic payments.</span></span> <span data-ttu-id="3ce45-106">Les citoyens et sociétés européens peuvent effectuer et recevoir des règlements en euros, à l'intérieur ou l'extérieur des frontières nationales, avec les mêmes conditions, droits, et obligations de base, quel que soit leur emplacement.</span><span class="sxs-lookup"><span data-stu-id="3ce45-106">European citizens and companies can make and receive payments in euros, whether within or across national borders, with the same basic conditions, rights, and obligations, regardless of location.</span></span>  

<span data-ttu-id="3ce45-107">Avant de pouvoir effectuer un paiement SEPA, vous devez effectuer les tâches d'administration suivantes :</span><span class="sxs-lookup"><span data-stu-id="3ce45-107">Before you can file a SEPA payment you must complete the following administration tasks:</span></span>  

- <span data-ttu-id="3ce45-108">Paramétrez un nouveau protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="3ce45-108">Set up a new export protocol.</span></span> <span data-ttu-id="3ce45-109">Pour plus d'informations, voir Protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="3ce45-109">For more information, see Export Protocol.</span></span>  
- <span data-ttu-id="3ce45-110">Dans la table **Pays/région**, sélectionnez le champ **SEPA autorisé** pour chaque pays appartenant à la zone AEE.</span><span class="sxs-lookup"><span data-stu-id="3ce45-110">In the **Country/Region** table, select the **SEPA Allowed** field for each country that belongs to the EEA zone.</span></span>  
- <span data-ttu-id="3ce45-111">Vérifiez que le champ **Devise euro** dans la table **Paramètres comptabilité** correspond à la devise dans les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="3ce45-111">Verify that the **Currency Euro** field in the **General Ledger Setup** table corresponds with the currency in the payment lines.</span></span>  
- <span data-ttu-id="3ce45-112">Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient l'IBAN et le code SWIFT.</span><span class="sxs-lookup"><span data-stu-id="3ce45-112">Verify that the vendor’s **Preferred Bank Account** field in the **Vendor** table contains the IBAN and SWIFT code.</span></span>  

## <a name="to-file-a-sepa-payment"></a><span data-ttu-id="3ce45-113">Pour effectuer un paiement SEPA</span><span class="sxs-lookup"><span data-stu-id="3ce45-113">To file a SEPA payment</span></span>  

1.  <span data-ttu-id="3ce45-114">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Effectuer des paiements SEPA**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="3ce45-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **File SEPA Payments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="3ce45-115">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="3ce45-115">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="3ce45-116">Champ</span><span class="sxs-lookup"><span data-stu-id="3ce45-116">Field</span></span>|<span data-ttu-id="3ce45-117">Désignation</span><span class="sxs-lookup"><span data-stu-id="3ce45-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="3ce45-118">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="3ce45-118">**Journal Template Name**</span></span>|<span data-ttu-id="3ce45-119">Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="3ce45-119">Specify the general journal template for the SEPA payment report.</span></span>|  
    |<span data-ttu-id="3ce45-120">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="3ce45-120">**Journal Batch**</span></span>|<span data-ttu-id="3ce45-121">Spécifiez la feuille comptabilité pour l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="3ce45-121">Specify the general journal batch for the SEPA payment report.</span></span>|  
    |<span data-ttu-id="3ce45-122">**Valider les lignes feuille comptabilité**</span><span class="sxs-lookup"><span data-stu-id="3ce45-122">**Post General Journal Lines**</span></span>|<span data-ttu-id="3ce45-123">Spécifiez si vous souhaitez transférer les lignes paiement vers la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="3ce45-123">Specify if you want to transfer the payment lines to the general ledger.</span></span>|  
    |<span data-ttu-id="3ce45-124">**Inclure axes**</span><span class="sxs-lookup"><span data-stu-id="3ce45-124">**Include Dimensions**</span></span>|<span data-ttu-id="3ce45-125">Saisissez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="3ce45-125">Enter the dimensions that you want to include in the SEPA payment report.</span></span> <span data-ttu-id="3ce45-126">L'option n'est disponible que si le champ **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="3ce45-126">The option is only available if the **Summarize Gen. Jnl. Lines** field on the **Electronic Banking Setup** page is selected.</span></span>|  
    |<span data-ttu-id="3ce45-127">**Date d'exécution**</span><span class="sxs-lookup"><span data-stu-id="3ce45-127">**Execution Date**</span></span>|<span data-ttu-id="3ce45-128">Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date comptabilisation sur les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="3ce45-128">Enter an execution date if you want an execution date that differs from the posting date on the payment lines.</span></span>|  
    |<span data-ttu-id="3ce45-129">**Emplacement**</span><span class="sxs-lookup"><span data-stu-id="3ce45-129">**File Name**</span></span>|<span data-ttu-id="3ce45-130">Entrez le nom du fichier, y compris le lecteur et le dossier, dans lequel vous souhaitez imprimer l'état.</span><span class="sxs-lookup"><span data-stu-id="3ce45-130">Enter the name of the file, including the drive and folder, to which you want to print the report.</span></span>|  

3.  <span data-ttu-id="3ce45-131">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="3ce45-131">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3ce45-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3ce45-132">See Also</span></span>  
 <span data-ttu-id="3ce45-133">[Paramétrer les protocoles d'exportation](how-to-set-up-export-protocols.md) </span><span class="sxs-lookup"><span data-stu-id="3ce45-133">[Set Up Export Protocols](how-to-set-up-export-protocols.md) </span></span>  
 <span data-ttu-id="3ce45-134">[Effectuer des paiements SEPA hors euro](how-to-file-non-euro-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="3ce45-134">[File Non-Euro SEPA Payments](how-to-file-non-euro-sepa-payments.md) </span></span>  
 [<span data-ttu-id="3ce45-135">Activer les règlements SEPA</span><span class="sxs-lookup"><span data-stu-id="3ce45-135">Activate SEPA Payments</span></span>](how-to-activate-sepa-payments.md)
