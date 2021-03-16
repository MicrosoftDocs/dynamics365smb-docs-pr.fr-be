---
title: Génération des suggestions de domiciliation
description: Après avoir paramétré les domiciliations, vous pouvez commencer à générer des suggestions de domiciliation. Vous pouvez uniquement créer des suggestions de domiciliation pour les clients nationaux.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5432ac680c0b32f7436d407315d3be1eefe2dbac
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379548"
---
# <a name="generate-domiciliation-suggestions"></a><span data-ttu-id="66708-104">Générer des suggestions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="66708-104">Generate Domiciliation Suggestions</span></span>
<span data-ttu-id="66708-105">Après avoir paramétré les domiciliations, vous pouvez commencer à générer des suggestions de domiciliation.</span><span class="sxs-lookup"><span data-stu-id="66708-105">After you have set up domiciliations, you can start generating domiciliation suggestions.</span></span> <span data-ttu-id="66708-106">Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], vous pouvez uniquement créer des suggestions de domiciliation pour les clients nationaux.</span><span class="sxs-lookup"><span data-stu-id="66708-106">In [!INCLUDE[prod_short](../../includes/prod_short.md)], you can create domiciliation suggestions for domestic customers only.</span></span>  

## <a name="to-generate-domiciliation-suggestions"></a><span data-ttu-id="66708-107">Pour générer des suggestions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="66708-107">To generate domiciliation suggestions</span></span>  

1.  <span data-ttu-id="66708-108">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuille domiciliation**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="66708-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Domiciliation Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="66708-109">Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Suggérer des domiciliations**.</span><span class="sxs-lookup"><span data-stu-id="66708-109">In the **Batch Name** field, select the required journal batch, and then choose the **Suggest Domiciliations** action.</span></span>  
3.  <span data-ttu-id="66708-110">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="66708-110">Fill in the fields as displayed in the following table.</span></span>  

    |<span data-ttu-id="66708-111">Champ</span><span class="sxs-lookup"><span data-stu-id="66708-111">Field</span></span>|<span data-ttu-id="66708-112">Désignation</span><span class="sxs-lookup"><span data-stu-id="66708-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="66708-113">**Date d'échéance**</span><span class="sxs-lookup"><span data-stu-id="66708-113">**Due Date**</span></span>|<span data-ttu-id="66708-114">Entrez la date d'échéance à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="66708-114">Enter the due date to be included in the batch job.</span></span> <span data-ttu-id="66708-115">Seules les écritures dont la date d'échéance est antérieure ou identique à cette date sont incluses.</span><span class="sxs-lookup"><span data-stu-id="66708-115">Only entries that have a due date before or on this date will be included.</span></span>|  
    |<span data-ttu-id="66708-116">**Accepter les escomptes**</span><span class="sxs-lookup"><span data-stu-id="66708-116">**Take Payment Discounts**</span></span>|<span data-ttu-id="66708-117">Sélectionnez ce champ si vous souhaitez inclure dans le traitement par lots les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.</span><span class="sxs-lookup"><span data-stu-id="66708-117">Select if you want the batch job to include customer ledger entries for which you can receive a payment discount.</span></span>|  
    |<span data-ttu-id="66708-118">**Date d'escompte**</span><span class="sxs-lookup"><span data-stu-id="66708-118">**Payment Discount Date**</span></span>|<span data-ttu-id="66708-119">Entrez la date qui est utilisée pour calculer l'escompte.</span><span class="sxs-lookup"><span data-stu-id="66708-119">Enter the date that will be used to calculate the payment discount.</span></span>|  
    |<span data-ttu-id="66708-120">**Sélectionner les remboursements possibles**</span><span class="sxs-lookup"><span data-stu-id="66708-120">**Select Possible Refunds**</span></span>|<span data-ttu-id="66708-121">Sélectionnez ce champ si vous souhaitez inclure dans le traitement par lots les remboursements.</span><span class="sxs-lookup"><span data-stu-id="66708-121">Select if you want the batch job to include refunds.</span></span>|  
    |<span data-ttu-id="66708-122">**Date de validation**</span><span class="sxs-lookup"><span data-stu-id="66708-122">**Posting Date**</span></span>|<span data-ttu-id="66708-123">Entrez la date qui s'affiche comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="66708-123">Enter the date that will appear as the posting date on the lines that the batch job inserts in the domiciliation journal.</span></span>|  

4.  <span data-ttu-id="66708-124">Entrez les éventuels critères de filtre supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="66708-124">Enter any additional filter criteria.</span></span>  
5.  <span data-ttu-id="66708-125">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="66708-125">Choose the **OK** button.</span></span>  

<span data-ttu-id="66708-126">Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes correspondant aux filtres.</span><span class="sxs-lookup"><span data-stu-id="66708-126">When the batch job is finished, the domiciliation journal contains all open customer ledger entries that match the filters.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="66708-127">Les suggestions de domiciliation n'incluent que les clients pour lesquels un numéro de domiciliation est configuré.</span><span class="sxs-lookup"><span data-stu-id="66708-127">The domiciliation suggestions will include only customers who have a Domiciliation number set up.</span></span> <span data-ttu-id="66708-128">Pour plus d'informations, voir [Paramétrer les domiciliations](how-to-set-up-domiciliations.md).</span><span class="sxs-lookup"><span data-stu-id="66708-128">For more information, see [Set Up Domiciliations](how-to-set-up-domiciliations.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="66708-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="66708-129">See Also</span></span>  
 <span data-ttu-id="66708-130">[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="66708-130">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="66708-131">[Prélévement à l'aide de la domiciliation](direct-debit-using-domiciliation.md) </span><span class="sxs-lookup"><span data-stu-id="66708-131">[Direct Debit Using Domiciliation](direct-debit-using-domiciliation.md) </span></span>  
 <span data-ttu-id="66708-132">[Paramétrer les domiciliations](how-to-set-up-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="66708-132">[Set Up Domiciliations](how-to-set-up-domiciliations.md) </span></span>  
 <span data-ttu-id="66708-133">[Tester les domiciliations](how-to-test-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="66708-133">[Test Domiciliations](how-to-test-domiciliations.md) </span></span>  
 <span data-ttu-id="66708-134">[Modifier et supprimer des lignes de domiciliation](how-to-edit-and-delete-domiciliation-lines.md) </span><span class="sxs-lookup"><span data-stu-id="66708-134">[Edit and Delete Domiciliation Lines](how-to-edit-and-delete-domiciliation-lines.md) </span></span>  
 [<span data-ttu-id="66708-135">Exporter et valider les domiciliations</span><span class="sxs-lookup"><span data-stu-id="66708-135">Export and Post Domiciliations</span></span>](how-to-export-and-post-domiciliations.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]