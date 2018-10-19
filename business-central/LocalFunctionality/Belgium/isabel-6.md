---
title: "Isabel 6"
description: "L'organisation Isabel a développé une plateforme CIS (Client Isabel Synchronizer) qui permet à [!INCLUDE[d365fin](../../includes/d365fin_md.md)] de s'intégrer en toute sécurité à Isabel. CIS gère l'échange de documents depuis ou vers le serveur Isabel."
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
ms.openlocfilehash: 9a9ac84f3a62a4515568aa017ba5fc5d4ed1e450
ms.contentlocale: fr-be
ms.lasthandoff: 09/28/2018

---
# <a name="isabel-6"></a>Isabel 6
L'organisation Isabel a développé une plateforme CIS (Client Isabel Synchronizer) qui permet à [!INCLUDE[d365fin](../../includes/d365fin_md.md)] de s'intégrer en toute sécurité à Isabel. CIS gère l'échange de documents depuis ou vers le serveur Isabel.  

Pour charger ou télécharger des fichiers de banque, vous devez configurer votre environnement pour utiliser Isabel. [!INCLUDE[d365fin](../../includes/d365fin_md.md)] communique avec le CIS.dll via un encapsulateur COM.  

Pour configurer votre système pour utiliser Isabel, procédez comme suit :  

- Installez les composants de sécurité Isabel. Pour plus d'informations, voir la zone de téléchargement du [site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323).  

- Installez l'encapsulateur COM fabriqué par l'organisation Isabel. Cet encapsulateur est inclus dans le package Isabel GO 6.20.  

- Enregistrez l'encapsulateur COM sur votre ordinateur. À l'invite de commandes, recherchez le CIS.dll puis exécutez la commande **regsvr32 CISComWrapper.dll**.  

## <a name="see-also"></a>Voir aussi  
 [Site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323)   
 [Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)   
 [Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)

