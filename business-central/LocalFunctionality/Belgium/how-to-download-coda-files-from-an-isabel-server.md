---
title: Téléchargement des fichiers CODA à partir d'un serveur Isabel
description: Les fichiers CODA peuvent être téléchargés manuellement ou en mode assisté.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: d7b81574cefed5da4b6520733365f689f0aec933
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/08/2019
ms.locfileid: "826502"
---
# <a name="download-coda-files-from-an-isabel-server"></a><span data-ttu-id="bf7b9-103">Télécharger les fichiers CODA à partir d'un serveur Isabel</span><span class="sxs-lookup"><span data-stu-id="bf7b9-103">Download CODA Files from an Isabel Server</span></span>
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

<span data-ttu-id="bf7b9-104">Les fichiers CODA peuvent être téléchargés manuellement ou en mode assisté.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-104">CODA files can be downloaded manually or in attended mode.</span></span>  

<span data-ttu-id="bf7b9-105">Pour télécharger manuellement les fichiers CODA, connectez-vous au serveur Isabel et sélectionnez les fichiers que vous souhaitez télécharger.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-105">To manually download CODA files, log  on to the Isabel server and select the files that you want to download.</span></span> <span data-ttu-id="bf7b9-106">Les fichiers téléchargés peuvent ensuite être importés à partir de la table **Compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-106">The downloaded files can then be imported from the **Bank Account** table.</span></span> <span data-ttu-id="bf7b9-107">Pour plus d'informations, voir [Importer les relevés CODA](how-to-import-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="bf7b9-107">For more information, see [Import CODA Statements](how-to-import-coda-statements.md).</span></span>  

## <a name="to-download-coda-files-in-attended-mode"></a><span data-ttu-id="bf7b9-108">Pour télécharger les fichiers CODA en mode assisté</span><span class="sxs-lookup"><span data-stu-id="bf7b9-108">To download CODA files in attended mode</span></span>  

1.  <span data-ttu-id="bf7b9-109">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Feuilles IBS**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IBS Logs**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bf7b9-110">Choisissez l'action **Télécharger**.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-110">Choose the **Download** action.</span></span>  
3.  <span data-ttu-id="bf7b9-111">Dans la page **Options de demande de téléchargement IBS**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-111">On the **IBS Download Request Options** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="bf7b9-112">Champ</span><span class="sxs-lookup"><span data-stu-id="bf7b9-112">Field</span></span>|<span data-ttu-id="bf7b9-113">Désignation</span><span class="sxs-lookup"><span data-stu-id="bf7b9-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="bf7b9-114">**Date début**</span><span class="sxs-lookup"><span data-stu-id="bf7b9-114">**From Date**</span></span>|<span data-ttu-id="bf7b9-115">Spécifiez la date de début du téléchargement.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-115">Specify the start date of the download.</span></span>|  
    |<span data-ttu-id="bf7b9-116">**Historique cumulé**</span><span class="sxs-lookup"><span data-stu-id="bf7b9-116">**To Date**</span></span>|<span data-ttu-id="bf7b9-117">Spécifiez la date de fin du téléchargement.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-117">Specify the end date of the download.</span></span>|  
    |<span data-ttu-id="bf7b9-118">**Format de fichier**</span><span class="sxs-lookup"><span data-stu-id="bf7b9-118">**File Format**</span></span>|<span data-ttu-id="bf7b9-119">Sélectionnez **Coda** comme format de fichier.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-119">Select **Coda** as the file format.</span></span>|  
    |<span data-ttu-id="bf7b9-120">**Statut du fichier**</span><span class="sxs-lookup"><span data-stu-id="bf7b9-120">**File Status**</span></span>|<span data-ttu-id="bf7b9-121">Sélectionnez le statut du fichier du téléchargement.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-121">Select the file status of the download.</span></span> <span data-ttu-id="bf7b9-122">Les statuts du fichier sont : **Non téléchargé**, **Téléchargé** et **Tous**.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-122">File statuses include **Not Downloaded**, **Downloaded**, and **All**.</span></span> <span data-ttu-id="bf7b9-123">Généralement, vous sélectionnez **Non téléchargé**, car vous téléchargez les fichiers CODA qui n'ont pas été téléchargés dans votre système.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-123">Typically you will select **Not Downloaded**, because you are downloading the CODA files that have not been downloaded to your system.</span></span>|  

4.  <span data-ttu-id="bf7b9-124">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-124">Choose the **OK** button.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="bf7b9-125">Vous ne pouvez pas supprimer des fichiers du serveur Isabel à l'aide de la page **Options de demande de téléchargement IBS**.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-125">You cannot delete any files from the Isabel server by using the **IBS Download Request Options** page.</span></span> <span data-ttu-id="bf7b9-126">Vous devez supprimer manuellement les fichiers en vous connectant au serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-126">You must manually delete the files by logging on to the Isabel server.</span></span>  

     <span data-ttu-id="bf7b9-127">Une fois que les fichiers CODA ont été téléchargés, le champ **Statut du processus** indique **Créé** dans la page **Feuilles IBS**.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-127">After the CODA files have been downloaded, the **Process Status** field will display **Created** on the **IBS Logs** page.</span></span> <span data-ttu-id="bf7b9-128">Vous pouvez vous connecter au serveur Isabel pour récupérer manuellement les fichiers.</span><span class="sxs-lookup"><span data-stu-id="bf7b9-128">You can log on to the Isabel server to manually retrieve the files.</span></span> <span data-ttu-id="bf7b9-129">Pour plus d'informations, voir [Importer les relevés CODA](how-to-import-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="bf7b9-129">For more information, see [Import CODA Statements](how-to-import-coda-statements.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="bf7b9-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bf7b9-130">See Also</span></span>  
[<span data-ttu-id="bf7b9-131">Fonctionnalité locale, Belgique</span><span class="sxs-lookup"><span data-stu-id="bf7b9-131">Belgium Local Functionality</span></span>](belgium-local-functionality.md)
