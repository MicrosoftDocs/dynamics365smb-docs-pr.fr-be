---
title: Comment exporter et valider des domiciliations
description: "Vous pouvez soumettre des domiciliations à votre banque en exportant les données dans un fichier. Lorsque vous effectuez un export vers un fichier, vous pouvez choisir de valider automatiquement les écritures comptables."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 8bbfbf5c035a65863a1cfc497bfcd18c00518a52
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="export-and-post-domiciliations"></a><span data-ttu-id="cd1eb-104">Exporter et valider les domiciliations</span><span class="sxs-lookup"><span data-stu-id="cd1eb-104">Export and Post Domiciliations</span></span>
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

<span data-ttu-id="cd1eb-105">Vous pouvez envoyer des domiciliations à votre banque en exportant les données vers un fichier.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-105">You can submit domiciliations to your bank by exporting the data to a file.</span></span> <span data-ttu-id="cd1eb-106">Lorsque vous exportez les données dans un fichier, vous pouvez choisir de valider automatiquement les lignes en comptabilité.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-106">When you export to a file, you can choose to automatically post the lines to the general ledger.</span></span>  

<span data-ttu-id="cd1eb-107">Selon la configuration du champ **Format exp. domiciliation européenne SEPA** dans la fenêtre **Fiche compte bancaire**, l'action **Fichier domiciliations** ouvre l'une des pages de requête suivantes :</span><span class="sxs-lookup"><span data-stu-id="cd1eb-107">Depending on setup of the **SEPA Direct Debit Exp. Format** field in the **Bank Account Card** window, the **File Domiciliations** action opens either of these request pages:</span></span>  

- <span data-ttu-id="cd1eb-108">Fenêtre **Créer lignes FS** : pour le format Domiciliation européenne SEPA.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-108">**Create Gen. Jnl. Lines** window – for the SEPA Direct Debit format.</span></span>  
- <span data-ttu-id="cd1eb-109">Fenêtre **Fichier domiciliation** : pour les formats nationaux.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-109">**File Domiciliations** window – for domestic formats.</span></span>  

## <a name="to-export-and-post-domiciliations-in-sepa-format"></a><span data-ttu-id="cd1eb-110">Pour exporter et valider des domiciliations au format SEPA</span><span class="sxs-lookup"><span data-stu-id="cd1eb-110">To export and post domiciliations in SEPA format</span></span>  

1.  <span data-ttu-id="cd1eb-111">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles saisie domiciliation**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Domiciliation Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cd1eb-112">Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Fichier domiciliations**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-112">In the **Batch Name** field, select the required journal batch, and then choose the **File Domiciliations** action.</span></span>  
3.  <span data-ttu-id="cd1eb-113">Dans la fenêtre **Créer lignes FS**, sélectionnez le raccourci **Options**, puis remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-113">In the **Create Gen. Jnl. Lines** window, select the **Options** FastTab, and then fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cd1eb-114">Champ</span><span class="sxs-lookup"><span data-stu-id="cd1eb-114">Field</span></span>|<span data-ttu-id="cd1eb-115">Description</span><span class="sxs-lookup"><span data-stu-id="cd1eb-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cd1eb-116">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-116">**Journal Template Name**</span></span>|<span data-ttu-id="cd1eb-117">Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations seront validées.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-117">Select the general journal template that the domiciliations will be posted from.</span></span>|  
    |<span data-ttu-id="cd1eb-118">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-118">**Journal Batch**</span></span>|<span data-ttu-id="cd1eb-119">Sélectionnez le nom feuille comptabilité à partir duquel les lignes feuille seront transférées.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-119">Select the general journal batch that the journal lines will be transferred from.</span></span>|  
    |<span data-ttu-id="cd1eb-120">**Valider lignes FS**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-120">**Post General Journal Lines**</span></span>|<span data-ttu-id="cd1eb-121">Sélectionnez pour valider en comptabilité.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-121">Select to post to the general ledger.</span></span>|  

4.  <span data-ttu-id="cd1eb-122">Cliquez sur le bouton **OK** pour exporter le fichier.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-122">Choose the **OK** button to export the file.</span></span>  
5.  <span data-ttu-id="cd1eb-123">Sélectionnez un emplacement adéquat depuis lequel vous téléchargez le fichier pour l'envoyer à votre banque, puis sélectionnez **Sauvegarder**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-123">Choose an appropriate location from where you upload the file to your bank, and then choose **Save**.</span></span>  
6.  <span data-ttu-id="cd1eb-124">Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-124">Choose the **Yes** button to automatically post the domiciliation journal lines.</span></span>  

    <span data-ttu-id="cd1eb-125">Si vous n'avez pas activé la case à cocher **Valider lignes FS**, vous devrez valider les domiciliations manuellement en comptabilité.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-125">If you did not select the **Post General Journal Lines** check box, you will have to post the domiciliations manually in the general journal.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="cd1eb-126">Après avoir validé les domiciliations en comptabilité, supprimez les domiciliations validées dans la fenêtre **Feuille de domiciliation**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-126">After you have posted domiciliations in the general journal, delete the posted domiciliations in the **Domiciliation Journal** window.</span></span> <span data-ttu-id="cd1eb-127">Pour ce faire, sélectionnez toutes les lignes dont le statut est **Validé**, puis cliquez sur le bouton **Supprimer**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-127">To do this, select all lines with status **Posted**, and then choose the **Delete** button.</span></span>  

## <a name="to-export-and-post-domiciliations-in-isabel-format"></a><span data-ttu-id="cd1eb-128">Pour exporter et valider des domiciliations au format Isabel</span><span class="sxs-lookup"><span data-stu-id="cd1eb-128">To export and post domiciliations in Isabel format</span></span>  

1.  <span data-ttu-id="cd1eb-129">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles saisie domiciliation**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-129">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Domiciliation Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cd1eb-130">Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Fichier domiciliations**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-130">In the **Batch Name** field, select the required journal batch, and then choose the **File Domiciliations** action.</span></span>  
3.  <span data-ttu-id="cd1eb-131">Dans la fenêtre **Fichier domiciliations**, sélectionnez le raccourci **Options**, puis remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-131">In the **File Domiciliations** window, select the **Options** FastTab, and then fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cd1eb-132">Champ</span><span class="sxs-lookup"><span data-stu-id="cd1eb-132">Field</span></span>|<span data-ttu-id="cd1eb-133">Description</span><span class="sxs-lookup"><span data-stu-id="cd1eb-133">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cd1eb-134">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-134">**Journal Template Name**</span></span>|<span data-ttu-id="cd1eb-135">Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations seront validées.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-135">Select the general journal template that the domiciliations will be posted from.</span></span>|  
    |<span data-ttu-id="cd1eb-136">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-136">**Journal Batch**</span></span>|<span data-ttu-id="cd1eb-137">Sélectionnez le nom feuille comptabilité à partir duquel les lignes feuille seront transférées.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-137">Select the general journal batch that the journal lines will be transferred from.</span></span>|  
    |<span data-ttu-id="cd1eb-138">**Valider lignes FS**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-138">**Post General Journal Lines**</span></span>|<span data-ttu-id="cd1eb-139">Sélectionnez pour valider en comptabilité.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-139">Select to post to the general ledger.</span></span>|  
    |<span data-ttu-id="cd1eb-140">**Date pivot**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-140">**Pivot Date**</span></span>|<span data-ttu-id="cd1eb-141">Entrez une date pivot si vous souhaitez que la date soit différente de la date de validation sur les lignes domiciliation.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-141">Enter a pivot date if you want a date that differs from the posting date on the domiciliation lines.</span></span> <span data-ttu-id="cd1eb-142">La date entrée écrasera la date de validation sur les lignes feuille sélectionnées.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-142">The date entered will overwrite the posting date on the selected journal lines.</span></span>|  
    |<span data-ttu-id="cd1eb-143">**N° d'immatriculation**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-143">**Inscription No.**</span></span>|<span data-ttu-id="cd1eb-144">Entrez le numéro d'inscription figurant sur la déclaration intracommunautaire (disquette).</span><span class="sxs-lookup"><span data-stu-id="cd1eb-144">Enter the inscription number that is on the intra-community declaration disk.</span></span> <span data-ttu-id="cd1eb-145">Le numéro est inclus dans le fichier et la note d'accompagnement.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-145">The number is included in the file and on the accompanying note.</span></span>|  
    |<span data-ttu-id="cd1eb-146">**Nom du fichier**</span><span class="sxs-lookup"><span data-stu-id="cd1eb-146">**File Name**</span></span>|<span data-ttu-id="cd1eb-147">Entrez le nom du fichier d'exportation que vous créez.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-147">Enter the name of the export file that you are creating.</span></span>|  

4.  <span data-ttu-id="cd1eb-148">Cliquez sur le bouton **Imprimer** pour exporter les domiciliations, puis imprimez la note d'accompagnement, ou cliquez sur le bouton **Aperçu** pour la consulter à l'écran.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-148">Choose the **Print** button to export the domiciliations and print the accompanying note, or choose the **Preview** button to view it on the screen.</span></span> <span data-ttu-id="cd1eb-149">Si vous ne souhaitez pas exporter le fichier pour l'instant, cliquez sur le bouton **Annuler**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-149">If you do not want to export the file now, choose the **Cancel** button.</span></span>  
5.  <span data-ttu-id="cd1eb-150">Cliquez sur le bouton **OK** pour envoyer l'état à l'imprimante.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-150">Choose the **OK** button to send the report to the printer.</span></span>  
6.  <span data-ttu-id="cd1eb-151">Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-151">Choose the **Yes** button to automatically post the domiciliation journal lines.</span></span>  

    <span data-ttu-id="cd1eb-152">Si vous n'avez pas activé la case à cocher **Valider lignes FS**, vous devrez valider les domiciliations manuellement en comptabilité.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-152">If you did not select the **Post General Journal Lines** check box, you will have to post the domiciliations manually in the general journal.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="cd1eb-153">Après avoir validé les domiciliations en comptabilité, supprimez les domiciliations validées dans la fenêtre **Feuille de domiciliation**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-153">After you have posted domiciliations in the general journal, delete the posted domiciliations in the **Domiciliation Journal** window.</span></span> <span data-ttu-id="cd1eb-154">Pour cela, sélectionnez toutes les lignes ayant le statut **Validée**, puis choisissez le bouton **Supprimer**.</span><span class="sxs-lookup"><span data-stu-id="cd1eb-154">To do this, select all lines with status **Posted**, and then choose the **Delete** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cd1eb-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cd1eb-155">See Also</span></span>  
 <span data-ttu-id="cd1eb-156">[Prélèvements bancaires avec domiciliation](direct-debit-using-domiciliation.md) </span><span class="sxs-lookup"><span data-stu-id="cd1eb-156">[Direct Debit Using Domiciliation](direct-debit-using-domiciliation.md) </span></span>  
 <span data-ttu-id="cd1eb-157">[Paramétrer les domiciliations](how-to-set-up-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="cd1eb-157">[Set Up Domiciliations](how-to-set-up-domiciliations.md) </span></span>  
 <span data-ttu-id="cd1eb-158">[Générer les propositions de domiciliation](how-to-generate-domiciliation-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="cd1eb-158">[Generate Domiciliation Suggestions](how-to-generate-domiciliation-suggestions.md) </span></span>  
 <span data-ttu-id="cd1eb-159">[Tester les domiciliations](how-to-test-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="cd1eb-159">[Test Domiciliations](how-to-test-domiciliations.md) </span></span>  
 [<span data-ttu-id="cd1eb-160">Modifier et supprimer des lignes de domiciliation</span><span class="sxs-lookup"><span data-stu-id="cd1eb-160">Edit and Delete Domiciliation Lines</span></span>](how-to-edit-and-delete-domiciliation-lines.md)

