---
title: "Isabel 6"
description: "L'organisation Isabel a développé une plateforme CIS (Client Isabel Synchronizer) afin que Business Central puisse s'intégrer en toute sécurité à Isabel. CIS gère l'échange de documents depuis ou vers le serveur Isabel."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 67400e424305cc705db5c1bd52a8e4de17ecc5a9
ms.openlocfilehash: 0d58e55c5c22c42b892b1f6a26915d93447b20f9
ms.contentlocale: fr-be
ms.lasthandoff: 11/20/2018

---
# <a name="isabel-6"></a><span data-ttu-id="f3e9c-104">Isabel 6</span><span class="sxs-lookup"><span data-stu-id="f3e9c-104">Isabel 6</span></span>
<span data-ttu-id="f3e9c-105">L'organisation Isabel a développé une plateforme CIS (Client Isabel Synchronizer) qui permet à [!INCLUDE[d365fin](../../includes/d365fin_md.md)] de s'intégrer en toute sécurité à Isabel.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-105">The Isabel organization has developed a Client Isabel Synchronizer (CIS) platform that allows [!INCLUDE[d365fin](../../includes/d365fin_md.md)] to securely integrate with Isabel.</span></span> <span data-ttu-id="f3e9c-106">CIS gère l'échange de documents depuis ou vers le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-106">CIS handles document exchange to and from the Isabel server.</span></span>  

<span data-ttu-id="f3e9c-107">Pour charger ou télécharger des fichiers de banque, vous devez configurer votre environnement pour utiliser Isabel.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-107">To upload or download the bank files, you will have to set up your environment to work with Isabel.</span></span> [!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="f3e9c-108">communique avec le CIS.dll via un encapsulateur COM.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-108">communicates to the CIS.dll through a COM wrapper.</span></span>  

<span data-ttu-id="f3e9c-109">Pour configurer votre système pour utiliser Isabel, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="f3e9c-109">To set up your system to work with Isabel, complete the following:</span></span>  

- <span data-ttu-id="f3e9c-110">Installez les composants de sécurité Isabel.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-110">Install the Isabel security components.</span></span> <span data-ttu-id="f3e9c-111">Pour plus d'informations, voir la zone de téléchargement du [site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323).</span><span class="sxs-lookup"><span data-stu-id="f3e9c-111">For more information, see the download area on the [Isabel website](https://go.microsoft.com/fwlink/?LinkId=210323).</span></span>  

- <span data-ttu-id="f3e9c-112">Installez l'encapsulateur COM fabriqué par l'organisation Isabel.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-112">Install the COM wrapper that is manufactured by the Isabel organization.</span></span> <span data-ttu-id="f3e9c-113">Cet encapsulateur est inclus dans le package Isabel GO 6.20.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-113">This wrapper is included with the Isabel GO 6.20 package.</span></span>  

- <span data-ttu-id="f3e9c-114">Enregistrez l'encapsulateur COM sur votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-114">Register the COM wrapper on your computer.</span></span> <span data-ttu-id="f3e9c-115">À l'invite de commandes, recherchez le CIS.dll puis exécutez la commande **regsvr32 CISComWrapper.dll**.</span><span class="sxs-lookup"><span data-stu-id="f3e9c-115">At the command prompt, locate the CIS.dll and then execute the **regsvr32 CISComWrapper.dll** command.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f3e9c-116">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f3e9c-116">See Also</span></span>  
 <span data-ttu-id="f3e9c-117">[Site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323) </span><span class="sxs-lookup"><span data-stu-id="f3e9c-117">[Isabel website](https://go.microsoft.com/fwlink/?LinkId=210323) </span></span>  
 <span data-ttu-id="f3e9c-118">[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="f3e9c-118">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 [<span data-ttu-id="f3e9c-119">Paramétrer des opérations bancaires électroniques</span><span class="sxs-lookup"><span data-stu-id="f3e9c-119">Set Up Electronic Banking</span></span>](how-to-set-up-electronic-banking.md)

