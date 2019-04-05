---
title: Isabel 6
description: L'organisation Isabel a développé une plateforme CIS (Client Isabel Synchronizer) afin que Business Central puisse s'intégrer en toute sécurité à Isabel. CIS gère l'échange de documents depuis ou vers le serveur Isabel.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 0d58e55c5c22c42b892b1f6a26915d93447b20f9
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/08/2019
ms.locfileid: "826479"
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
