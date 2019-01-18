---
title: "Téléchargement des fichiers de paiement vers un serveur Isabel"
description: "Les fichiers de paiement peuvent être téléchargés à l'aide de la page **Feuilles IBS**. Les champs **Mode d'intégration du chargement** et **Mode d'intégration du téléchargement** dans la page **Paramétrage des opérations bancaires électroniques** doivent être définis sur **Assisté** pour télécharger les fichiers de paiement."
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
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 2621f8f73cd00baecbb47c799e9e2adbc0d93bd6
ms.contentlocale: fr-be
ms.lasthandoff: 11/26/2018

---
# <a name="upload-payment-files-to-an-isabel-server"></a><span data-ttu-id="05360-104">Télécharger les fichiers de paiement vers un serveur Isabel</span><span class="sxs-lookup"><span data-stu-id="05360-104">Upload Payment Files to an Isabel Server</span></span>
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

<span data-ttu-id="05360-105">Les fichiers de paiement peuvent être téléchargés à l'aide de la page **Feuilles IBS**.</span><span class="sxs-lookup"><span data-stu-id="05360-105">Payment files can be uploaded using the **IBS Logs** page.</span></span> <span data-ttu-id="05360-106">Les champs **Mode d'intégration du chargement** et **Mode d'intégration du téléchargement** dans la page **Paramétrage des opérations bancaires électroniques** doivent être définis sur **Assisté** pour télécharger les fichiers de paiement.</span><span class="sxs-lookup"><span data-stu-id="05360-106">The **Upload Integration Mode** and **Download Integration Mode** fields on the **Electronic Banking Setup** page must be set to **Attended** to upload payment files.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="05360-107">Avant de pouvoir télécharger les fichiers de paiement, vous devez être connecté au serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="05360-107">Before you can upload payment files you must be logged on to the Isabel server.</span></span>  

## <a name="to-upload-payment-files-in-attended-mode"></a><span data-ttu-id="05360-108">Pour télécharger les fichiers de paiement en mode assisté</span><span class="sxs-lookup"><span data-stu-id="05360-108">To upload payment files in attended mode</span></span>  

1.  <span data-ttu-id="05360-109">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Feuilles IBS**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="05360-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IBS Logs**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="05360-110">Choisissez l'action **Obtenir le contrat et l'utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="05360-110">Choose the **Get Contract and User** action.</span></span>  
3.  <span data-ttu-id="05360-111">Après avoir vérifié les fichiers de paiement, un ID utilisateur et un ID contrat s'affichent dans les champs **ID utilisateur IBS** et **ID contrat IBS**.</span><span class="sxs-lookup"><span data-stu-id="05360-111">After verifying the payment files, a user ID and contract ID will be displayed in the **IBS User ID** and **IBS Contract ID** fields.</span></span>  

    <span data-ttu-id="05360-112">Le champ **Statut du téléchargement** est défini sur **Prêt pour le téléchargement**.</span><span class="sxs-lookup"><span data-stu-id="05360-112">The **Upload Status** field will be set to **Ready for Upload**.</span></span> <span data-ttu-id="05360-113">S'il existe plusieurs contrats sur le serveur Isabel pour le compte bancaire, le champ **Statut du téléchargement** est défini sur **Un conflit existe**.</span><span class="sxs-lookup"><span data-stu-id="05360-113">If more than one contract exists on the Isabel server for the bank account, the **Upload Status** will be set to **Conflict Exists**.</span></span> <span data-ttu-id="05360-114">Sélectionnez le contrat approprié.</span><span class="sxs-lookup"><span data-stu-id="05360-114">Select the correct contract.</span></span>  

4.  <span data-ttu-id="05360-115">Choisissez l'action **Procéder au téléchargement**.</span><span class="sxs-lookup"><span data-stu-id="05360-115">Choose the **Perform Download** action.</span></span> <span data-ttu-id="05360-116">Les fichiers de paiement sont téléchargés sur le serveur Isabel et le champ **Statut du processus** est défini sur **Traité**.</span><span class="sxs-lookup"><span data-stu-id="05360-116">The payment files will be uploaded to the Isabel server and the **Process Status** field will be set to **Processed**.</span></span>  
5.  <span data-ttu-id="05360-117">Poursuivez le traitement des fichiers de paiement en les signant et en les envoyant vers le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="05360-117">Continue processing the payment files by signing and sending the files on the Isabel server.</span></span>  

## <a name="see-also"></a><span data-ttu-id="05360-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05360-118">See Also</span></span>  
 [<span data-ttu-id="05360-119">Archiver les écritures journal IBS</span><span class="sxs-lookup"><span data-stu-id="05360-119">Archive IBS Log Entries</span></span>](how-to-archive-ibs-log-entries.md)

