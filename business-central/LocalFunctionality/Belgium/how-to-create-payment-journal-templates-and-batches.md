---
title: Création de modèles et de lots de feuilles paiement
description: Dans la version belge de Business Central, les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à celle des autres types de feuille.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1cbfb5a74c54a39ab3ed2bc11b7f4c3eca5964bd
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775008"
---
# <a name="create-payment-journal-templates-and-batches"></a><span data-ttu-id="30358-104">Créer des modèles et des lots de feuilles paiement</span><span class="sxs-lookup"><span data-stu-id="30358-104">Create Payment Journal Templates and Batches</span></span>
<span data-ttu-id="30358-105">Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], les suggestions de paiement sont générées et validées dans les feuilles paiement.</span><span class="sxs-lookup"><span data-stu-id="30358-105">In [!INCLUDE[prod_short](../../includes/prod_short.md)], payment suggestions are generated and posted in payment journals.</span></span> <span data-ttu-id="30358-106">La structure de la feuille paiement est similaire à celle des autres types de feuille.</span><span class="sxs-lookup"><span data-stu-id="30358-106">The structure of the payment journal is similar to the structure of other journal types.</span></span> <span data-ttu-id="30358-107">Toutefois, la feuille paiement contient des champs qui sont propres au traitement des paiements.</span><span class="sxs-lookup"><span data-stu-id="30358-107">However, the payment journal contains some fields that are specific for processing payments.</span></span> <span data-ttu-id="30358-108">Avant de commencer à générer des suggestions de paiement, vous devez paramétrer un modèle feuille paiement et une feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="30358-108">Before you can start generating payment suggestions, you have to set up a payment journal template and a payment journal batch.</span></span>  

<span data-ttu-id="30358-109">Si vous affectez un compte bancaire au modèle feuille paiement, le compte bancaire est inséré sur toutes les feuilles paiement et lignes feuille paiement qui sont créées à l'aide de ce modèle.</span><span class="sxs-lookup"><span data-stu-id="30358-109">If you assign a bank account to the payment journal template, the bank account will be inserted on all payment journal batches and payment journal lines that are created by using this template.</span></span> <span data-ttu-id="30358-110">En spécifiant un compte bancaire pour le modèle feuille, vous pouvez réduire le temps nécessaire pour vérifier les suggestions de paiement.</span><span class="sxs-lookup"><span data-stu-id="30358-110">By specifying a bank account for the journal template, you can reduce the time that is required for checking the payment suggestions.</span></span>  

## <a name="to-create-a-payment-journal-template"></a><span data-ttu-id="30358-111">Pour créer un modèle feuille paiement</span><span class="sxs-lookup"><span data-stu-id="30358-111">To create a payment journal template</span></span>  

1. <span data-ttu-id="30358-112">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Modèles feuille paiement**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="30358-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journal Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="30358-113">Sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="30358-113">Choose the **New** action.</span></span>  
3. <span data-ttu-id="30358-114">Sur la page **Modèles feuille paiement EB**, renseignez les champs.</span><span class="sxs-lookup"><span data-stu-id="30358-114">On the **EB Payment Journal Templates** page, fill in the fields.</span></span>  

    [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

    > [!IMPORTANT]
    > <span data-ttu-id="30358-115">Si les champs **ID page** et **ID impression test** ne sont pas affichés, vous devez les ajouter via la personnalisation.</span><span class="sxs-lookup"><span data-stu-id="30358-115">If the **Page ID** and **Test Report ID** fields are not shown, you must add them through personalization.</span></span> <span data-ttu-id="30358-116">Vous devez compléter les champs pour pouvoir continuer.</span><span class="sxs-lookup"><span data-stu-id="30358-116">The fields must be filled in before you continue.</span></span> <span data-ttu-id="30358-117">Pour plus d'informations, voir [Personnaliser votre espace de travail](../../ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="30358-117">For more information, see [Personalize Your Workspace](../../ui-personalization-user.md).</span></span>
4. <span data-ttu-id="30358-118">Répétez l'étape 2 pour chaque modèle supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="30358-118">Repeat step 2 for any additional templates.</span></span>

5. <span data-ttu-id="30358-119">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="30358-119">Choose the **OK** button.</span></span>  

## <a name="to-add-payment-journal-batches-to-the-journal-template"></a><span data-ttu-id="30358-120">Pour ajouter des feuilles paiement au modèle feuille</span><span class="sxs-lookup"><span data-stu-id="30358-120">To add payment journal batches to the journal template</span></span>  

1.  <span data-ttu-id="30358-121">Dans la page **Modèles feuille paiement**, choisissez l'action **Feuilles**.</span><span class="sxs-lookup"><span data-stu-id="30358-121">On the **Payment Journal Templates** page, choose the **Batches** action.</span></span>  
2.  <span data-ttu-id="30358-122">Dans la page **Feuilles paiement**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="30358-122">On the **Paym. Journal Batch** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="30358-123">Champ</span><span class="sxs-lookup"><span data-stu-id="30358-123">Field</span></span>|<span data-ttu-id="30358-124">Description</span><span class="sxs-lookup"><span data-stu-id="30358-124">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="30358-125">**Nom**</span><span class="sxs-lookup"><span data-stu-id="30358-125">**Name**</span></span>|<span data-ttu-id="30358-126">Entrez un nom unique pour la feuille.</span><span class="sxs-lookup"><span data-stu-id="30358-126">Enter a unique name for the journal batch.</span></span><br /><br /> <span data-ttu-id="30358-127">**REMARQUE :** pour que le nom feuille soit mis à jour numériquement, ajoutez un nombre au nom feuille.</span><span class="sxs-lookup"><span data-stu-id="30358-127">**NOTE:** To have the journal name update numerically, include a number in the journal batch name.</span></span> <span data-ttu-id="30358-128">Par exemple, le nom FEUILLE1 augmente d'un numéro à chaque validation, vous aurez donc FEUILLE2, FEUILLE3, etc.</span><span class="sxs-lookup"><span data-stu-id="30358-128">For example, the name KBC1 will increment by one number with every posting to KBC2, KBC3, and so on.</span></span>|  
    |<span data-ttu-id="30358-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="30358-129">**Description**</span></span>|<span data-ttu-id="30358-130">Entrez une description pour la feuille.</span><span class="sxs-lookup"><span data-stu-id="30358-130">Enter a description for the journal batch.</span></span>|  
    |<span data-ttu-id="30358-131">**Code motif**</span><span class="sxs-lookup"><span data-stu-id="30358-131">**Reason Code**</span></span>|<span data-ttu-id="30358-132">Spécifiez éventuellement le code motif qui est associé à cette feuille.</span><span class="sxs-lookup"><span data-stu-id="30358-132">Optionally, specify the reason code that is linked to this journal batch.</span></span>|  
    |<span data-ttu-id="30358-133">**Statut**</span><span class="sxs-lookup"><span data-stu-id="30358-133">**Status**</span></span>|<span data-ttu-id="30358-134">Spécifie le statut de la feuille.</span><span class="sxs-lookup"><span data-stu-id="30358-134">Specifies the status of the batch.</span></span>|

<span data-ttu-id="30358-135">Vous pouvez ensuite tester la configuration.</span><span class="sxs-lookup"><span data-stu-id="30358-135">Next, you can test the configuration.</span></span> <span data-ttu-id="30358-136">Pour plus d'informations, voir [Tester les paiements électroniques](how-to-test-electronic-payments.md).</span><span class="sxs-lookup"><span data-stu-id="30358-136">For more information, see [Test Electronic Payments](how-to-test-electronic-payments.md).</span></span>  

3.  <span data-ttu-id="30358-137">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="30358-137">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="30358-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="30358-138">See Also</span></span>  
 <span data-ttu-id="30358-139">[Paiements électroniques, Belgique](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="30358-139">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="30358-140">[Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="30358-140">[Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 [<span data-ttu-id="30358-141">Paramétrer les codes transaction IBLC-BLWI</span><span class="sxs-lookup"><span data-stu-id="30358-141">Set Up IBLC-BLWI Transaction Codes</span></span>](how-to-set-up-iblc-blwi-transaction-codes.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]