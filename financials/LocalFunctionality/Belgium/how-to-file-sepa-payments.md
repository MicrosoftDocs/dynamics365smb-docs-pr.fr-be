---
title: "Procédure : Classer les paiements SEPA"
description: "Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez classer des paiements SEPA autres qu'en euro auprès de la banque."
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
ms.openlocfilehash: a1faa225b4b75cf9af990dc6a6c78b0e7a9ebe44
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="file-sepa-payments"></a><span data-ttu-id="5b3d9-103">Classer les paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="5b3d9-103">File SEPA Payments</span></span>
<span data-ttu-id="5b3d9-104">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez classer des paiements SEPA autres qu'en euro auprès de la banque.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use Single Euro Payments Area (SEPA) credit transfers to file SEPA payments with the bank.</span></span>  

<span data-ttu-id="5b3d9-105">Le format SEPA unifie les modes de paiement des pays/régions européens participants, ce qui rend les paiements internationaux aussi faciles à traiter que les paiements nationaux.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-105">SEPA unifies payment methods in participating European countries/regions, which makes international payments as easy to process as domestic payments.</span></span> <span data-ttu-id="5b3d9-106">Les citoyens et les sociétés européens peuvent effectuer et recevoir des paiements en euros, dans ou au-delà des frontières nationales, avec les mêmes conditions, droits et obligations de base, quel que soit l'emplacement.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-106">European citizens and companies can make and receive payments in euros, whether within or across national borders, with the same basic conditions, rights, and obligations, regardless of location.</span></span>  

<span data-ttu-id="5b3d9-107">Avant de classer un paiement, vous devez remplir les tâches administratives suivantes :</span><span class="sxs-lookup"><span data-stu-id="5b3d9-107">Before you can file a SEPA payment you must complete the following administration tasks:</span></span>  

- <span data-ttu-id="5b3d9-108">Configurer un nouveau protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-108">Set up a new export protocol.</span></span> <span data-ttu-id="5b3d9-109">Pour plus d'informations, voir Protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-109">For more information, see Export Protocol.</span></span>  
- <span data-ttu-id="5b3d9-110">Dans la table **Pays/Région**, sélectionnez le champ **SEPA autorisé** pour chaque pays appartenant à la zone EEA.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-110">In the **Country/Region** table, select the **SEPA Allowed** field for each country that belongs to the EEA zone.</span></span>  
- <span data-ttu-id="5b3d9-111">Vérifiez que le champ **Devise Euro** de la table **Paramètres comptabilité** correspond à la devise sur les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-111">Verify that the **Currency Euro** field in the **General Ledger Setup** table corresponds with the currency in the payment lines.</span></span>  
- <span data-ttu-id="5b3d9-112">Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient les codes IBAN et SWIFT.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-112">Verify that the vendor’s **Preferred Bank Account** field in the **Vendor** table contains the IBAN and SWIFT code.</span></span>  

## <a name="to-file-a-sepa-payment"></a><span data-ttu-id="5b3d9-113">Pour classer un paiement SEPA</span><span class="sxs-lookup"><span data-stu-id="5b3d9-113">To file a SEPA payment</span></span>  

1.  <span data-ttu-id="5b3d9-114">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Classer les paiements SEPA**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **File SEPA Payments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5b3d9-115">Remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-115">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5b3d9-116">Champ</span><span class="sxs-lookup"><span data-stu-id="5b3d9-116">Field</span></span>|<span data-ttu-id="5b3d9-117">Description</span><span class="sxs-lookup"><span data-stu-id="5b3d9-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5b3d9-118">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="5b3d9-118">**Journal Template Name**</span></span>|<span data-ttu-id="5b3d9-119">Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-119">Specify the general journal template for the SEPA payment report.</span></span>|  
    |<span data-ttu-id="5b3d9-120">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="5b3d9-120">**Journal Batch**</span></span>|<span data-ttu-id="5b3d9-121">Spécifiez le nom feuille comptabilité pour l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-121">Specify the general journal batch for the SEPA payment report.</span></span>|  
    |<span data-ttu-id="5b3d9-122">**Valider lignes FS**</span><span class="sxs-lookup"><span data-stu-id="5b3d9-122">**Post General Journal Lines**</span></span>|<span data-ttu-id="5b3d9-123">Spécifiez si vous souhaitez transférer les lignes de paiement dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-123">Specify if you want to transfer the payment lines to the general ledger.</span></span>|  
    |<span data-ttu-id="5b3d9-124">**Inclure axes**</span><span class="sxs-lookup"><span data-stu-id="5b3d9-124">**Include Dimensions**</span></span>|<span data-ttu-id="5b3d9-125">Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-125">Enter the dimensions that you want to include in the SEPA payment report.</span></span> <span data-ttu-id="5b3d9-126">Cette option est uniquement disponible si le champ **Résumer lignes FS** de la fenêtre **Configuration de la banque électronique** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-126">The option is only available if the **Summarize Gen. Jnl. Lines** field in the **Electronic Banking Setup** window is selected.</span></span>|  
    |<span data-ttu-id="5b3d9-127">**Date d'exécution**</span><span class="sxs-lookup"><span data-stu-id="5b3d9-127">**Execution Date**</span></span>|<span data-ttu-id="5b3d9-128">Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date de validation sur les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-128">Enter an execution date if you want an execution date that differs from the posting date on the payment lines.</span></span>|  
    |<span data-ttu-id="5b3d9-129">**Nom du fichier**</span><span class="sxs-lookup"><span data-stu-id="5b3d9-129">**File Name**</span></span>|<span data-ttu-id="5b3d9-130">Saisissez le nom du fichier, y compris le lecteur et le fichier, relatifs à l'impression de l'état.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-130">Enter the name of the file, including the drive and folder, to which you want to print the report.</span></span>|  

3.  <span data-ttu-id="5b3d9-131">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="5b3d9-131">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5b3d9-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5b3d9-132">See Also</span></span>  
 <span data-ttu-id="5b3d9-133">[Configurer les protocoles d'exportation](how-to-set-up-export-protocols.md) </span><span class="sxs-lookup"><span data-stu-id="5b3d9-133">[Set Up Export Protocols](how-to-set-up-export-protocols.md) </span></span>  
 <span data-ttu-id="5b3d9-134">[Classer les paiements SEPA hors Euro](how-to-file-non-euro-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="5b3d9-134">[File Non-Euro SEPA Payments](how-to-file-non-euro-sepa-payments.md) </span></span>  
 [<span data-ttu-id="5b3d9-135">Activer des paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="5b3d9-135">Activate SEPA Payments</span></span>](how-to-activate-sepa-payments.md)

