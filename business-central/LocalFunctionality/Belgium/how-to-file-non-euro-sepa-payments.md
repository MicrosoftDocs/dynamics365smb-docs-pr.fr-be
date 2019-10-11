---
title: Effectuer des paiements SEPA hors euro
description: Dans la version belge de Business Central, vous pouvez effectuer des paiements SEPA hors euros auprès de la banque. Cela est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas SEPA et pour les devises autres que l'euro.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: f2dfd5a28404c6c346daa8f11694a781303aa2b9
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300262"
---
# <a name="file-non-euro-sepa-payments"></a><span data-ttu-id="476c6-104">Effectuer des paiements SEPA hors euro</span><span class="sxs-lookup"><span data-stu-id="476c6-104">File Non-Euro SEPA Payments</span></span>
<span data-ttu-id="476c6-105">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez effectuer des paiements SEPA hors euro auprès de la banque.</span><span class="sxs-lookup"><span data-stu-id="476c6-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can file non-euro SEPA payments with the bank.</span></span> <span data-ttu-id="476c6-106">Cela est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas SEPA et pour les devises autres que l'euro.</span><span class="sxs-lookup"><span data-stu-id="476c6-106">This is useful when you make payments to other countries that do not use SEPA and for currencies other than the euro.</span></span>  

<span data-ttu-id="476c6-107">Avant de pouvoir effectuer un paiement SEPA hors euro, vous devez effectuer les tâches d'administration suivantes :</span><span class="sxs-lookup"><span data-stu-id="476c6-107">Before you can file a non-euro SEPA payment you must complete the following administration tasks:</span></span>  

- <span data-ttu-id="476c6-108">Paramétrez un nouveau protocole d'exportation pour un paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="476c6-108">Set up a new export protocol for a non-euro SEPA.</span></span>  
- <span data-ttu-id="476c6-109">Dans la table **Pays/région**, désactivez le champ **SEPA autorisé** pour chaque pays appartenant à la zone AEE.</span><span class="sxs-lookup"><span data-stu-id="476c6-109">In the **Country/Region** table, clear the **SEPA Allowed** field for each country that belongs to the EEA zone.</span></span>  
- <span data-ttu-id="476c6-110">Vérifiez que le champ **Devise euro** dans la table **Paramètres comptabilité** n'est pas en euro.</span><span class="sxs-lookup"><span data-stu-id="476c6-110">Verify that the **Currency Euro** field in the **General Ledger Setup** table is not in euro currency.</span></span>  
- <span data-ttu-id="476c6-111">Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient l'IBAN et le code SWIFT.</span><span class="sxs-lookup"><span data-stu-id="476c6-111">Verify that the vendor’s **Preferred Bank Account** field in the **Vendor** table contains the IBAN and SWIFT code.</span></span>  

## <a name="to-file-a-non-euro-sepa-payment"></a><span data-ttu-id="476c6-112">Pour effectuer un paiement SEPA hors euro</span><span class="sxs-lookup"><span data-stu-id="476c6-112">To file a non-euro SEPA payment</span></span>  

1.  <span data-ttu-id="476c6-113">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Effectuer des paiements SEPA hors euro**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="476c6-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **File Non Euro SEPA Payments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="476c6-114">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="476c6-114">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="476c6-115">Champ</span><span class="sxs-lookup"><span data-stu-id="476c6-115">Field</span></span>|<span data-ttu-id="476c6-116">Désignation</span><span class="sxs-lookup"><span data-stu-id="476c6-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="476c6-117">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="476c6-117">**Journal Template Name**</span></span>|<span data-ttu-id="476c6-118">Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="476c6-118">Specify the general journal template for the non-euro SEPA payment report.</span></span>|  
    |<span data-ttu-id="476c6-119">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="476c6-119">**Journal Batch**</span></span>|<span data-ttu-id="476c6-120">Spécifiez la feuille comptabilité pour l'état de paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="476c6-120">Specify the general journal batch for the non-euro SEPA payment report.</span></span>|  
    |<span data-ttu-id="476c6-121">**Valider les lignes feuille comptabilité**</span><span class="sxs-lookup"><span data-stu-id="476c6-121">**Post General Journal Lines**</span></span>|<span data-ttu-id="476c6-122">Spécifiez si vous souhaitez transférer les lignes paiement vers la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="476c6-122">Specify if you want to transfer the payment lines to the general ledger.</span></span>|  
    |<span data-ttu-id="476c6-123">**Inclure axes**</span><span class="sxs-lookup"><span data-stu-id="476c6-123">**Include Dimensions**</span></span>|<span data-ttu-id="476c6-124">Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA hors euro.</span><span class="sxs-lookup"><span data-stu-id="476c6-124">Enter the dimensions that you want to include in the non-euro SEPA payment report.</span></span> <span data-ttu-id="476c6-125">L'option n'est disponible que si le champ **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="476c6-125">The option is available only if the **Summarize Gen. Jnl. Lines** field on the **Electronic Banking Setup** page is selected.</span></span>|  
    |<span data-ttu-id="476c6-126">**Date d'exécution**</span><span class="sxs-lookup"><span data-stu-id="476c6-126">**Execution Date**</span></span>|<span data-ttu-id="476c6-127">Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date comptabilisation sur les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="476c6-127">Enter an execution date if you want an execution date that differs from the posting date on the payment lines.</span></span>|  
    |<span data-ttu-id="476c6-128">**Emplacement**</span><span class="sxs-lookup"><span data-stu-id="476c6-128">**File Name**</span></span>|<span data-ttu-id="476c6-129">Entrez le nom du fichier, y compris le lecteur et le dossier, dans lequel vous souhaitez imprimer l'état.</span><span class="sxs-lookup"><span data-stu-id="476c6-129">Enter the name of the file, including the drive and folder, to which you want to print the report.</span></span>|  

3.  <span data-ttu-id="476c6-130">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="476c6-130">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="476c6-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="476c6-131">See Also</span></span>  
 <span data-ttu-id="476c6-132">[Remplir les paiements SEPA](how-to-file-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="476c6-132">[File SEPA Payments](how-to-file-sepa-payments.md) </span></span>  
 <span data-ttu-id="476c6-133">[Activer les règlements SEPA](how-to-activate-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="476c6-133">[Activate SEPA Payments](how-to-activate-sepa-payments.md) </span></span>  
 [<span data-ttu-id="476c6-134">Paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="476c6-134">SEPA Payments</span></span>](sepa-payments.md)
