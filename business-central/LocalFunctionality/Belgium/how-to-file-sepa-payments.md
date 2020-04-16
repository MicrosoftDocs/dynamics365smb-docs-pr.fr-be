---
title: Effectuer des paiements SEPA
description: Dans Business Central, vous pouvez utiliser les virements SEPA pour effectuer des paiements SEPA auprès de la banque.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: f740f082f6ac6aa7157f0ef491937c35eeffee6b
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/01/2020
ms.locfileid: "3180893"
---
# <a name="file-sepa-payments"></a><span data-ttu-id="1990d-103">Effectuer des paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="1990d-103">File SEPA Payments</span></span>
<span data-ttu-id="1990d-104">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez utiliser les virements SEPA pour effectuer des paiements SEPA auprès de la banque.</span><span class="sxs-lookup"><span data-stu-id="1990d-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use Single Euro Payments Area (SEPA) credit transfers to file SEPA payments with the bank.</span></span>  

<span data-ttu-id="1990d-105">SEPA unifie les modes de paiement dans les pays/régions européens participants, ce qui rend les paiements internationaux aussi faciles à traiter que les paiements nationaux.</span><span class="sxs-lookup"><span data-stu-id="1990d-105">SEPA unifies payment methods in participating European countries/regions, which makes international payments as easy to process as domestic payments.</span></span> <span data-ttu-id="1990d-106">Les citoyens et sociétés européens peuvent effectuer et recevoir des règlements en euros, à l'intérieur ou l'extérieur des frontières nationales, avec les mêmes conditions, droits, et obligations de base, quel que soit leur emplacement.</span><span class="sxs-lookup"><span data-stu-id="1990d-106">European citizens and companies can make and receive payments in euros, whether within or across national borders, with the same basic conditions, rights, and obligations, regardless of location.</span></span>  

<span data-ttu-id="1990d-107">Avant de pouvoir effectuer un paiement SEPA, vous devez effectuer les tâches d'administration suivantes :</span><span class="sxs-lookup"><span data-stu-id="1990d-107">Before you can file a SEPA payment, you must complete the following administration tasks:</span></span>  

- <span data-ttu-id="1990d-108">Paramétrez un nouveau protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="1990d-108">Set up a new export protocol.</span></span>
- <span data-ttu-id="1990d-109">Dans la table **Pays/région**, sélectionnez le champ **SEPA autorisé** pour chaque pays appartenant à la zone AEE.</span><span class="sxs-lookup"><span data-stu-id="1990d-109">In the **Country/Region** table, select the **SEPA Allowed** field for each country that belongs to the EEA zone.</span></span>  
- <span data-ttu-id="1990d-110">Vérifiez que le champ **Devise euro** dans la table **Paramètres comptabilité** correspond à la devise dans les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="1990d-110">Verify that the **Currency Euro** field in the **General Ledger Setup** table corresponds with the currency in the payment lines.</span></span>  
- <span data-ttu-id="1990d-111">Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient l'IBAN et le code SWIFT.</span><span class="sxs-lookup"><span data-stu-id="1990d-111">Verify that the vendor’s **Preferred Bank Account** field in the **Vendor** table contains the IBAN and SWIFT code.</span></span>  

## <a name="to-file-a-sepa-payment"></a><span data-ttu-id="1990d-112">Pour effectuer un paiement SEPA</span><span class="sxs-lookup"><span data-stu-id="1990d-112">To file a SEPA payment</span></span>  

1.  <span data-ttu-id="1990d-113">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Classer les paiements SEPA**, puis choisissez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="1990d-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **File SEPA Payments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="1990d-114">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="1990d-114">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="1990d-115">Champ</span><span class="sxs-lookup"><span data-stu-id="1990d-115">Field</span></span>|<span data-ttu-id="1990d-116">Désignation</span><span class="sxs-lookup"><span data-stu-id="1990d-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1990d-117">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="1990d-117">**Journal Template Name**</span></span>|<span data-ttu-id="1990d-118">Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="1990d-118">Specify the general journal template for the SEPA payment report.</span></span>|  
    |<span data-ttu-id="1990d-119">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="1990d-119">**Journal Batch**</span></span>|<span data-ttu-id="1990d-120">Spécifiez la feuille comptabilité pour l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="1990d-120">Specify the general journal batch for the SEPA payment report.</span></span>|  
    |<span data-ttu-id="1990d-121">**Valider les lignes feuille comptabilité**</span><span class="sxs-lookup"><span data-stu-id="1990d-121">**Post General Journal Lines**</span></span>|<span data-ttu-id="1990d-122">Spécifiez si vous souhaitez transférer les lignes paiement vers la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="1990d-122">Specify if you want to transfer the payment lines to the general ledger.</span></span>|  
    |<span data-ttu-id="1990d-123">**Inclure axes**</span><span class="sxs-lookup"><span data-stu-id="1990d-123">**Include Dimensions**</span></span>|<span data-ttu-id="1990d-124">Saisissez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="1990d-124">Enter the dimensions that you want to include in the SEPA payment report.</span></span> <span data-ttu-id="1990d-125">L'option n'est disponible que si le champ **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="1990d-125">The option is available only if the **Summarize Gen. Jnl. Lines** field on the **Electronic Banking Setup** page is selected.</span></span>|  
    |<span data-ttu-id="1990d-126">**Date d'exécution**</span><span class="sxs-lookup"><span data-stu-id="1990d-126">**Execution Date**</span></span>|<span data-ttu-id="1990d-127">Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date comptabilisation sur les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="1990d-127">Enter an execution date if you want an execution date that differs from the posting date on the payment lines.</span></span>|  
    |<span data-ttu-id="1990d-128">**Emplacement**</span><span class="sxs-lookup"><span data-stu-id="1990d-128">**File Name**</span></span>|<span data-ttu-id="1990d-129">Entrez le nom du fichier, y compris le lecteur et le dossier, dans lequel vous souhaitez imprimer l'état.</span><span class="sxs-lookup"><span data-stu-id="1990d-129">Enter the name of the file, including the drive and folder, to which you want to print the report.</span></span>|  

3.  <span data-ttu-id="1990d-130">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="1990d-130">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1990d-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1990d-131">See Also</span></span>  
 <span data-ttu-id="1990d-132">[Paramétrer les protocoles d'exportation](how-to-set-up-export-protocols.md) </span><span class="sxs-lookup"><span data-stu-id="1990d-132">[Set Up Export Protocols](how-to-set-up-export-protocols.md) </span></span>  
 <span data-ttu-id="1990d-133">[Classer les paiements SEPA hors Euro](how-to-file-non-euro-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="1990d-133">[File Non-Euro SEPA Payments](how-to-file-non-euro-sepa-payments.md) </span></span>  
 [<span data-ttu-id="1990d-134">Activer les règlements SEPA</span><span class="sxs-lookup"><span data-stu-id="1990d-134">Activate SEPA Payments</span></span>](how-to-activate-sepa-payments.md)
