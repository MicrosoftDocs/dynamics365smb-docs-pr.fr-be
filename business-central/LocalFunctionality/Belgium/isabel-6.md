---
title: Isabel 6
description: "L'organisation Isabel a développé une plateforme appelée Client Isabel Synchronizer (CIS), qui permet l'intégration sécurisée de [!INCLUDE[d365fin](../../includes/d365fin_md.md)] avec Isabel. CIS traite les échanges de documents depuis et vers le serveur Isabel."
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
ms.openlocfilehash: c11f7d19fdcaef78a97db9e9da6ed7c420c365a9
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="isabel-6"></a><span data-ttu-id="30e23-104">Isabel 6</span><span class="sxs-lookup"><span data-stu-id="30e23-104">Isabel 6</span></span>
<span data-ttu-id="30e23-105">L'organisation Isabel a développé une plateforme appelée Client Isabel Synchronizer (CIS), qui permet l'intégration sécurisée de [!INCLUDE[d365fin](../../includes/d365fin_md.md)] avec Isabel.</span><span class="sxs-lookup"><span data-stu-id="30e23-105">The Isabel organization has developed a Client Isabel Synchronizer (CIS) platform that allows [!INCLUDE[d365fin](../../includes/d365fin_md.md)] to securely integrate with Isabel.</span></span> <span data-ttu-id="30e23-106">CIS traite les échanges de documents depuis et vers le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="30e23-106">CIS handles document exchange to and from the Isabel server.</span></span>  

<span data-ttu-id="30e23-107">Pour télécharger les fichiers bancaires depuis ou vers le serveur, vous devez configurer votre environnement pour qu'il fonctionne avec Isabel.</span><span class="sxs-lookup"><span data-stu-id="30e23-107">To upload or download the bank files, you will have to set up your environment to work with Isabel.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)]<span data-ttu-id="30e23-108"> communique au serveur CIS.dll via une fonction wrapper COM.</span><span class="sxs-lookup"><span data-stu-id="30e23-108"> communicates to the CIS.dll through a COM wrapper.</span></span>  

<span data-ttu-id="30e23-109">Pour configurer votre système afin qu'il fonctionne avec Isabel, suivez les étapes ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="30e23-109">To set up your system to work with Isabel, complete the following:</span></span>  

- <span data-ttu-id="30e23-110">Installez les composants de sécurité d'Isabel.</span><span class="sxs-lookup"><span data-stu-id="30e23-110">Install the Isabel security components.</span></span> <span data-ttu-id="30e23-111">Pour en savoir plus, consultez la section consacrée au téléchargement sur le [site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323).</span><span class="sxs-lookup"><span data-stu-id="30e23-111">For more information, see the download area on the [Isabel website](http://go.microsoft.com/fwlink/?LinkId=210323).</span></span>  

- <span data-ttu-id="30e23-112">Installez la fonction wrapper COM conçue par l'organisation Isabel.</span><span class="sxs-lookup"><span data-stu-id="30e23-112">Install the COM wrapper that is manufactured by the Isabel organization.</span></span> <span data-ttu-id="30e23-113">Cette fonction wrapper est incluse dans le package d'Isabel GO 6.20.</span><span class="sxs-lookup"><span data-stu-id="30e23-113">This wrapper is included with the Isabel GO 6.20 package.</span></span>  

- <span data-ttu-id="30e23-114">Enregistrez la fonction wrapper COM sur votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="30e23-114">Register the COM wrapper on your computer.</span></span> <span data-ttu-id="30e23-115">Lors de l'invite de commandes, trouvez le fichier intitulé CIS.dll, puis exécutez la commande **regsvr32 CISComWrapper.dll**.</span><span class="sxs-lookup"><span data-stu-id="30e23-115">At the command prompt, locate the CIS.dll and then execute the **regsvr32 CISComWrapper.dll** command.</span></span>  

## <a name="see-also"></a><span data-ttu-id="30e23-116">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="30e23-116">See Also</span></span>  
 <span data-ttu-id="30e23-117">[Site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323) </span><span class="sxs-lookup"><span data-stu-id="30e23-117">[Isabel website](http://go.microsoft.com/fwlink/?LinkId=210323) </span></span>  
 <span data-ttu-id="30e23-118">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="30e23-118">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 [<span data-ttu-id="30e23-119">Configurer des opérations bancaires électroniques</span><span class="sxs-lookup"><span data-stu-id="30e23-119">Set Up Electronic Banking</span></span>](how-to-set-up-electronic-banking.md)

