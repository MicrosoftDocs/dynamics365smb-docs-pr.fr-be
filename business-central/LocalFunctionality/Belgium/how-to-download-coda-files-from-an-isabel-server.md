---
title: "Procédure : Télécharger des fichiers CODA à partir d'un serveur Isabel"
description: "Les fichiers CODA peuvent être téléchargés manuellement ou en mode assisté."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 3391529dd136311adce3cdca49dcf9917d060e7c
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="download-coda-files-from-an-isabel-server"></a><span data-ttu-id="d37ed-103">Télécharger des fichiers CODA à partir d'un serveur Isabel</span><span class="sxs-lookup"><span data-stu-id="d37ed-103">Download CODA Files from an Isabel Server</span></span>
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

<span data-ttu-id="d37ed-104">Les fichiers CODA peuvent être téléchargés manuellement ou en mode assisté.</span><span class="sxs-lookup"><span data-stu-id="d37ed-104">CODA files can be downloaded manually or in attended mode.</span></span>  

<span data-ttu-id="d37ed-105">Pour télécharger manuellement des fichiers CODA, connectez-vous au serveur Isabel et sélectionnez les fichiers que vous souhaitez télécharger.</span><span class="sxs-lookup"><span data-stu-id="d37ed-105">To manually download CODA files, log  on to the Isabel server and select the files that you want to download.</span></span> <span data-ttu-id="d37ed-106">Les fichiers téléchargés peuvent être importés à partir du tableau **Compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="d37ed-106">The downloaded files can then be imported from the **Bank Account** table.</span></span> <span data-ttu-id="d37ed-107">Pour plus d'informations, reportez-vous à [Importer des relevés CODA](how-to-import-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="d37ed-107">For more information, see [Import CODA Statements](how-to-import-coda-statements.md).</span></span>  

## <a name="to-download-coda-files-in-attended-mode"></a><span data-ttu-id="d37ed-108">Pour télécharger les fichiers CODA en mode assisté</span><span class="sxs-lookup"><span data-stu-id="d37ed-108">To download CODA files in attended mode</span></span>  

1.  <span data-ttu-id="d37ed-109">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="d37ed-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IBS Logs**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d37ed-110">Choisissez l'action **Télécharger**.</span><span class="sxs-lookup"><span data-stu-id="d37ed-110">Choose the **Download** action.</span></span>  
3.  <span data-ttu-id="d37ed-111">Dans la fenêtre **Options de demande de téléchargement IBS**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d37ed-111">In the **IBS Download Request Options** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="d37ed-112">Champ</span><span class="sxs-lookup"><span data-stu-id="d37ed-112">Field</span></span>|<span data-ttu-id="d37ed-113">Description</span><span class="sxs-lookup"><span data-stu-id="d37ed-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="d37ed-114">**Date début**</span><span class="sxs-lookup"><span data-stu-id="d37ed-114">**From Date**</span></span>|<span data-ttu-id="d37ed-115">Spécifiez la date de début du téléchargement.</span><span class="sxs-lookup"><span data-stu-id="d37ed-115">Specify the start date of the download.</span></span>|  
    |<span data-ttu-id="d37ed-116">**Historique cumulé**</span><span class="sxs-lookup"><span data-stu-id="d37ed-116">**To Date**</span></span>|<span data-ttu-id="d37ed-117">Spécifiez la date de fin du téléchargement.</span><span class="sxs-lookup"><span data-stu-id="d37ed-117">Specify the end date of the download.</span></span>|  
    |<span data-ttu-id="d37ed-118">**Format de fichier**</span><span class="sxs-lookup"><span data-stu-id="d37ed-118">**File Format**</span></span>|<span data-ttu-id="d37ed-119">Sélectionnez **Coda** comme format de fichier.</span><span class="sxs-lookup"><span data-stu-id="d37ed-119">Select **Coda** as the file format.</span></span>|  
    |<span data-ttu-id="d37ed-120">**Statut du fichier**</span><span class="sxs-lookup"><span data-stu-id="d37ed-120">**File Status**</span></span>|<span data-ttu-id="d37ed-121">Sélectionnez le statut du fichier du téléchargement.</span><span class="sxs-lookup"><span data-stu-id="d37ed-121">Select the file status of the download.</span></span> <span data-ttu-id="d37ed-122">Les statuts du fichier incluent **Non téléchargé**, **Téléchargé** et **Tout**.</span><span class="sxs-lookup"><span data-stu-id="d37ed-122">File statuses include **Not Downloaded**, **Downloaded**, and **All**.</span></span> <span data-ttu-id="d37ed-123">Généralement, vous devez sélectionner **Non téléchargé**, car vous téléchargez les fichiers CODA qui n'ont pas été téléchargés dans votre système.</span><span class="sxs-lookup"><span data-stu-id="d37ed-123">Typically you will select **Not Downloaded**, because you are downloading the CODA files that have not been downloaded to your system.</span></span>|  

4.  <span data-ttu-id="d37ed-124">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="d37ed-124">Choose the **OK** button.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="d37ed-125">Vous ne pouvez supprimer aucune fichier du serveur Isabel via la fenêtre **Options de demande de téléchargement IBS**.</span><span class="sxs-lookup"><span data-stu-id="d37ed-125">You cannot delete any files from the Isabel server by using the **IBS Download Request Options** window.</span></span> <span data-ttu-id="d37ed-126">Vous devez supprimer manuellement les fichiers en vous connectant au serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="d37ed-126">You must manually delete the files by logging on to the Isabel server.</span></span>  

     <span data-ttu-id="d37ed-127">Après le téléchargement des fichiers CODA, le champ **Statut processus** sera défini sur **Créé** dans la fenêtre **Journaux IBS**.</span><span class="sxs-lookup"><span data-stu-id="d37ed-127">After the CODA files have been downloaded, the **Process Status** field will display **Created** in the **IBS Logs** window.</span></span> <span data-ttu-id="d37ed-128">Vous pouvez vous connecter au serveur Isabel pour récupérer manuellement les fichiers.</span><span class="sxs-lookup"><span data-stu-id="d37ed-128">You can log on to the Isabel server to manually retrieve the files.</span></span> <span data-ttu-id="d37ed-129">Pour plus d'informations, reportez-vous à [Importer des relevés CODA](how-to-import-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="d37ed-129">For more information, see [Import CODA Statements](how-to-import-coda-statements.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="d37ed-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d37ed-130">See Also</span></span>  
[<span data-ttu-id="d37ed-131">Fonctionnalité locale pour la Belgique</span><span class="sxs-lookup"><span data-stu-id="d37ed-131">Belgium Local Functionality</span></span>](belgium-local-functionality.md)

