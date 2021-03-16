---
title: Exportation et validation des domiciliations
description: Vous pouvez soumettre des domiciliations à votre banque en exportant les données dans un fichier. Lorsque vous exportez les données dans un fichier, vous pouvez choisir de valider automatiquement les lignes dans la comptabilité.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: e8f61320be95fd6787251a79384f1492686a3e63
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379563"
---
# <a name="export-and-post-domiciliations"></a><span data-ttu-id="ffc9a-104">Exporter et valider les domiciliations</span><span class="sxs-lookup"><span data-stu-id="ffc9a-104">Export and Post Domiciliations</span></span>
<span data-ttu-id="ffc9a-105">Vous pouvez soumettre des domiciliations à votre banque en exportant les données dans un fichier.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-105">You can submit domiciliations to your bank by exporting the data to a file.</span></span> <span data-ttu-id="ffc9a-106">Lorsque vous exportez les données dans un fichier, vous pouvez choisir de valider automatiquement les lignes dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-106">When you export to a file, you can choose to automatically post the lines to the general ledger.</span></span>  

<span data-ttu-id="ffc9a-107">Selon le paramétrage du champ **Format exp. prélèvement SEPA** dans la page **Fiche compte bancaire**, l'action **Domiciliations de fichier** ouvre l'une des pages de demande suivantes :</span><span class="sxs-lookup"><span data-stu-id="ffc9a-107">Depending on setup of the **SEPA Direct Debit Exp. Format** field on the **Bank Account Card** page, the **File Domiciliations** action opens either of these request pages:</span></span>  

- <span data-ttu-id="ffc9a-108">Page **Créer des lignes feuille comptabilité** – pour le format de prélèvement SEPA.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-108">**Create Gen. Jnl. Lines** page – for the SEPA Direct Debit format.</span></span>  
- <span data-ttu-id="ffc9a-109">Page **Domiciliations de fichier** – pour les formats nationaux.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-109">**File Domiciliations** page – for domestic formats.</span></span>  

## <a name="to-export-and-post-domiciliations-in-sepa-format"></a><span data-ttu-id="ffc9a-110">Pour exporter et valider les domiciliations au format SEPA</span><span class="sxs-lookup"><span data-stu-id="ffc9a-110">To export and post domiciliations in SEPA format</span></span>  

1.  <span data-ttu-id="ffc9a-111">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles domiciliation**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Domiciliation Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ffc9a-112">Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Domiciliations de fichier**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-112">In the **Batch Name** field, select the required journal batch, and then choose the **File Domiciliations** action.</span></span>  
3.  <span data-ttu-id="ffc9a-113">Sur la page **Créer des lignes feuille comptabilité**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-113">On the **Create Gen. Jnl. Lines** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="ffc9a-114">Champ</span><span class="sxs-lookup"><span data-stu-id="ffc9a-114">Field</span></span>|<span data-ttu-id="ffc9a-115">Désignation</span><span class="sxs-lookup"><span data-stu-id="ffc9a-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="ffc9a-116">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-116">**Journal Template Name**</span></span>|<span data-ttu-id="ffc9a-117">Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations sont validées.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-117">Select the general journal template that the domiciliations will be posted from.</span></span>|  
    |<span data-ttu-id="ffc9a-118">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-118">**Journal Batch**</span></span>|<span data-ttu-id="ffc9a-119">Sélectionnez la feuille comptabilité à partir de laquelle les lignes feuille sont transférées.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-119">Select the general journal batch that the journal lines will be transferred from.</span></span>|  
    |<span data-ttu-id="ffc9a-120">**Valider les lignes feuille comptabilité**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-120">**Post General Journal Lines**</span></span>|<span data-ttu-id="ffc9a-121">Sélectionnez ce champ pour valider les lignes feuille dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-121">Select to post to the general ledger.</span></span>|  

4.  <span data-ttu-id="ffc9a-122">Cliquez sur le bouton **OK** pour exporter le fichier.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-122">Choose the **OK** button to export the file.</span></span>  
5.  <span data-ttu-id="ffc9a-123">Choisissez un emplacement approprié à partir duquel vous téléchargez le fichier vers votre banque, puis choisissez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-123">Choose an appropriate location from where you upload the file to your bank, and then choose **Save**.</span></span>  
6.  <span data-ttu-id="ffc9a-124">Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-124">Choose the **Yes** button to automatically post the domiciliation journal lines.</span></span>  

    <span data-ttu-id="ffc9a-125">Si vous n'activez pas la case à cocher **Valider les lignes feuille comptabilité**, vous devrez valider les domiciliations manuellement dans la feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-125">If you did not select the **Post General Journal Lines** check box, you will have to post the domiciliations manually in the general journal.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="ffc9a-126">Après avoir validé les domiciliations dans la feuille comptabilité, supprimez les domiciliations validées dans la page **Feuille domiciliation**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-126">After you have posted domiciliations in the general journal, delete the posted domiciliations on the **Domiciliation Journal** page.</span></span> <span data-ttu-id="ffc9a-127">Pour ce faire, sélectionnez toutes les lignes avec le statut **Validé**, puis cliquez sur le bouton **Supprimer**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-127">To do this, select all lines with status **Posted**, and then choose the **Delete** button.</span></span>  

## <a name="to-export-and-post-domiciliations-in-isabel-format"></a><span data-ttu-id="ffc9a-128">Pour exporter et valider les domiciliations au format Isabel</span><span class="sxs-lookup"><span data-stu-id="ffc9a-128">To export and post domiciliations in Isabel format</span></span>  

1.  <span data-ttu-id="ffc9a-129">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles domiciliation**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-129">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Domiciliation Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ffc9a-130">Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Domiciliations de fichier**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-130">In the **Batch Name** field, select the required journal batch, and then choose the **File Domiciliations** action.</span></span>  
3.  <span data-ttu-id="ffc9a-131">Dans la page **Domiciliations de fichier**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-131">On the **File Domiciliations** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="ffc9a-132">Champ</span><span class="sxs-lookup"><span data-stu-id="ffc9a-132">Field</span></span>|<span data-ttu-id="ffc9a-133">Désignation</span><span class="sxs-lookup"><span data-stu-id="ffc9a-133">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="ffc9a-134">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-134">**Journal Template Name**</span></span>|<span data-ttu-id="ffc9a-135">Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations sont validées.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-135">Select the general journal template that the domiciliations will be posted from.</span></span>|  
    |<span data-ttu-id="ffc9a-136">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-136">**Journal Batch**</span></span>|<span data-ttu-id="ffc9a-137">Sélectionnez la feuille comptabilité à partir de laquelle les lignes feuille sont transférées.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-137">Select the general journal batch that the journal lines will be transferred from.</span></span>|  
    |<span data-ttu-id="ffc9a-138">**Valider les lignes feuille comptabilité**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-138">**Post General Journal Lines**</span></span>|<span data-ttu-id="ffc9a-139">Sélectionnez ce champ pour valider les lignes feuille dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-139">Select to post to the general ledger.</span></span>|  
    |<span data-ttu-id="ffc9a-140">**Date pivot**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-140">**Pivot Date**</span></span>|<span data-ttu-id="ffc9a-141">Entrez une date pivot si vous souhaitez que la date soit différente de la date comptabilisation sur les lignes de domiciliation.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-141">Enter a pivot date if you want a date that differs from the posting date on the domiciliation lines.</span></span> <span data-ttu-id="ffc9a-142">La date saisie remplace la date comptabilisation sur les lignes feuille sélectionnées.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-142">The date entered will overwrite the posting date on the selected journal lines.</span></span>|  
    |<span data-ttu-id="ffc9a-143">**N° inscription**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-143">**Inscription No.**</span></span>|<span data-ttu-id="ffc9a-144">Entrez le numéro d'inscription qui figure sur le disque de déclaration intracommunautaire.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-144">Enter the inscription number that is on the intra-community declaration disk.</span></span> <span data-ttu-id="ffc9a-145">Le numéro figure dans le fichier et sur la note jointe.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-145">The number is included in the file and on the accompanying note.</span></span>|  
    |<span data-ttu-id="ffc9a-146">**Emplacement**</span><span class="sxs-lookup"><span data-stu-id="ffc9a-146">**File Name**</span></span>|<span data-ttu-id="ffc9a-147">Entrez le nom du fichier d'exportation que vous créez.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-147">Enter the name of the export file that you are creating.</span></span>|  

4.  <span data-ttu-id="ffc9a-148">Cliquez sur le bouton **Imprimer** pour exporter les domiciliations et imprimer la note jointe, ou cliquez sur le bouton **Aperçu** pour l'afficher à l'écran.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-148">Choose the **Print** button to export the domiciliations and print the accompanying note, or choose the **Preview** button to view it on the screen.</span></span> <span data-ttu-id="ffc9a-149">Si vous ne souhaitez pas exporter le fichier maintenant, cliquez sur le bouton **Annuler**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-149">If you do not want to export the file now, choose the **Cancel** button.</span></span>  
5.  <span data-ttu-id="ffc9a-150">Cliquez sur le bouton **OK** pour envoyer l'état vers l'imprimante.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-150">Choose the **OK** button to send the report to the printer.</span></span>  
6.  <span data-ttu-id="ffc9a-151">Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-151">Choose the **Yes** button to automatically post the domiciliation journal lines.</span></span>  

    <span data-ttu-id="ffc9a-152">Si vous n'activez pas la case à cocher **Valider les lignes feuille comptabilité**, vous devrez valider les domiciliations manuellement dans la feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-152">If you did not select the **Post General Journal Lines** check box, you will have to post the domiciliations manually in the general journal.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="ffc9a-153">Après avoir validé les domiciliations dans la feuille comptabilité, supprimez les domiciliations validées dans la page **Feuille domiciliation**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-153">After you have posted domiciliations in the general journal, delete the posted domiciliations on the **Domiciliation Journal** page.</span></span> <span data-ttu-id="ffc9a-154">Pour ce faire, sélectionnez toutes les lignes avec le statut **Validé**, puis cliquez sur le bouton **Supprimer**.</span><span class="sxs-lookup"><span data-stu-id="ffc9a-154">To do this, select all lines with status **Posted**, and then choose the **Delete** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ffc9a-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ffc9a-155">See Also</span></span>  
 <span data-ttu-id="ffc9a-156">[Prélévement à l'aide de la domiciliation](direct-debit-using-domiciliation.md) </span><span class="sxs-lookup"><span data-stu-id="ffc9a-156">[Direct Debit Using Domiciliation](direct-debit-using-domiciliation.md) </span></span>  
 <span data-ttu-id="ffc9a-157">[Paramétrer les domiciliations](how-to-set-up-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="ffc9a-157">[Set Up Domiciliations](how-to-set-up-domiciliations.md) </span></span>  
 <span data-ttu-id="ffc9a-158">[Générer les propositions de domiciliation](how-to-generate-domiciliation-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="ffc9a-158">[Generate Domiciliation Suggestions](how-to-generate-domiciliation-suggestions.md) </span></span>  
 <span data-ttu-id="ffc9a-159">[Tester les domiciliations](how-to-test-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="ffc9a-159">[Test Domiciliations](how-to-test-domiciliations.md) </span></span>  
 [<span data-ttu-id="ffc9a-160">Modifier et supprimer les lignes domiciliation</span><span class="sxs-lookup"><span data-stu-id="ffc9a-160">Edit and Delete Domiciliation Lines</span></span>](how-to-edit-and-delete-domiciliation-lines.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]