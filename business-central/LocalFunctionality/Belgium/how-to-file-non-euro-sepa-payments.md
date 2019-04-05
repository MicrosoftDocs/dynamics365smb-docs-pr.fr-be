---
title: Effectuer des paiements SEPA hors euro
description: Dans la version belge de Business Central, vous pouvez effectuer des paiements SEPA hors euros auprès de la banque. Cela est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas SEPA et pour les devises autres que l'euro.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: d8da10aae616dd14e34b34492af312bcf1227495
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/08/2019
ms.locfileid: "826515"
---
# <a name="file-non-euro-sepa-payments"></a><span data-ttu-id="c528a-104">Effectuer des paiements SEPA hors euro</span><span class="sxs-lookup"><span data-stu-id="c528a-104">File Non-Euro SEPA Payments</span></span>
<span data-ttu-id="c528a-105">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez effectuer des paiements SEPA hors euro auprès de la banque.</span><span class="sxs-lookup"><span data-stu-id="c528a-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can file non-euro SEPA payments with the bank.</span></span> <span data-ttu-id="c528a-106">Cela est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas SEPA et pour les devises autres que l'euro.</span><span class="sxs-lookup"><span data-stu-id="c528a-106">This is useful when you make payments to other countries that do not use SEPA and for currencies other than the euro.</span></span>  

<span data-ttu-id="c528a-107">Avant de pouvoir effectuer un paiement SEPA hors euro, vous devez effectuer les tâches d'administration suivantes :</span><span class="sxs-lookup"><span data-stu-id="c528a-107">Before you can file a non-euro SEPA payment you must complete the following administration tasks:</span></span>  

- <span data-ttu-id="c528a-108">Paramétrez un nouveau protocole d'exportation pour un paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="c528a-108">Set up a new export protocol for a non-euro SEPA.</span></span> <span data-ttu-id="c528a-109">Pour plus d'informations, voir Protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="c528a-109">For more information, see Export Protocol.</span></span>  
- <span data-ttu-id="c528a-110">Dans la table **Pays/région**, désactivez le champ **SEPA autorisé** pour chaque pays appartenant à la zone AEE.</span><span class="sxs-lookup"><span data-stu-id="c528a-110">In the **Country/Region** table, clear the **SEPA Allowed** field for each country that belongs to the EEA zone.</span></span>  
- <span data-ttu-id="c528a-111">Vérifiez que le champ **Devise euro** dans la table **Paramètres comptabilité** n'est pas en euro.</span><span class="sxs-lookup"><span data-stu-id="c528a-111">Verify that the **Currency Euro** field in the **General Ledger Setup** table is not in euro currency.</span></span>  
- <span data-ttu-id="c528a-112">Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient l'IBAN et le code SWIFT.</span><span class="sxs-lookup"><span data-stu-id="c528a-112">Verify that the vendor’s **Preferred Bank Account** field in the **Vendor** table contains the IBAN and SWIFT code.</span></span>  

## <a name="to-file-a-non-euro-sepa-payment"></a><span data-ttu-id="c528a-113">Pour effectuer un paiement SEPA hors euro</span><span class="sxs-lookup"><span data-stu-id="c528a-113">To file a non-euro SEPA payment</span></span>  

1.  <span data-ttu-id="c528a-114">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Effectuer des paiements SEPA hors euro**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="c528a-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **File Non Euro SEPA Payments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c528a-115">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="c528a-115">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="c528a-116">Champ</span><span class="sxs-lookup"><span data-stu-id="c528a-116">Field</span></span>|<span data-ttu-id="c528a-117">Désignation</span><span class="sxs-lookup"><span data-stu-id="c528a-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="c528a-118">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="c528a-118">**Journal Template Name**</span></span>|<span data-ttu-id="c528a-119">Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="c528a-119">Specify the general journal template for the non-euro SEPA payment report.</span></span>|  
    |<span data-ttu-id="c528a-120">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="c528a-120">**Journal Batch**</span></span>|<span data-ttu-id="c528a-121">Spécifiez la feuille comptabilité pour l'état de paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="c528a-121">Specify the general journal batch for the non-euro SEPA payment report.</span></span>|  
    |<span data-ttu-id="c528a-122">**Valider les lignes feuille comptabilité**</span><span class="sxs-lookup"><span data-stu-id="c528a-122">**Post General Journal Lines**</span></span>|<span data-ttu-id="c528a-123">Spécifiez si vous souhaitez transférer les lignes paiement vers la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="c528a-123">Specify if you want to transfer the payment lines to the general ledger.</span></span>|  
    |<span data-ttu-id="c528a-124">**Inclure axes**</span><span class="sxs-lookup"><span data-stu-id="c528a-124">**Include Dimensions**</span></span>|<span data-ttu-id="c528a-125">Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="c528a-125">Enter the dimensions that you want to include in the non-euro SEPA payment report.</span></span> <span data-ttu-id="c528a-126">L'option n'est disponible que si le champ **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="c528a-126">The option is only available if the **Summarize Gen. Jnl. Lines** field on the **Electronic Banking Setup** page is selected.</span></span>|  
    |<span data-ttu-id="c528a-127">**Date d'exécution**</span><span class="sxs-lookup"><span data-stu-id="c528a-127">**Execution Date**</span></span>|<span data-ttu-id="c528a-128">Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date comptabilisation sur les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="c528a-128">Enter an execution date if you want an execution date that differs from the posting date on the payment lines.</span></span>|  
    |<span data-ttu-id="c528a-129">**Emplacement**</span><span class="sxs-lookup"><span data-stu-id="c528a-129">**File Name**</span></span>|<span data-ttu-id="c528a-130">Entrez le nom du fichier, y compris le lecteur et le dossier, dans lequel vous souhaitez imprimer l'état.</span><span class="sxs-lookup"><span data-stu-id="c528a-130">Enter the name of the file, including the drive and folder, to which you want to print the report.</span></span>|  

3.  <span data-ttu-id="c528a-131">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="c528a-131">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c528a-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c528a-132">See Also</span></span>  
 <span data-ttu-id="c528a-133">[Remplir les paiements SEPA](how-to-file-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="c528a-133">[File SEPA Payments](how-to-file-sepa-payments.md) </span></span>  
 <span data-ttu-id="c528a-134">[Activer les règlements SEPA](how-to-activate-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="c528a-134">[Activate SEPA Payments](how-to-activate-sepa-payments.md) </span></span>  
 [<span data-ttu-id="c528a-135">Paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="c528a-135">SEPA Payments</span></span>](sepa-payments.md)
