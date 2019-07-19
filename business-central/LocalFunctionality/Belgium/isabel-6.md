---
title: Isabel 6
description: L'organisation Isabel a développé une plateforme CIS (Client Isabel Synchronizer) afin que Business Central puisse s'intégrer en toute sécurité à Isabel. CIS gère l'échange de documents depuis ou vers le serveur Isabel.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: belgium-local-functionality
ms.openlocfilehash: a0501d6ad8410d3666ac7e7f3fa8597e48990518
ms.sourcegitcommit: e8abfb78e13f3c29035087b09d7930f2950ab7a3
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 07/01/2019
ms.locfileid: "1717632"
---
# <a name="isabel-6"></a>Isabel 6
L'organisation Isabel a développé une plateforme CIS (Client Isabel Synchronizer) qui permet à [!INCLUDE[d365fin](../../includes/d365fin_md.md)] de s'intégrer en toute sécurité à Isabel. CIS gère l'échange de documents depuis ou vers le serveur Isabel.  

Pour charger ou télécharger des fichiers de banque, vous devez configurer votre environnement pour utiliser Isabel. [!INCLUDE[d365fin](../../includes/d365fin_md.md)] communique avec le fichier CIS.dll via un encapsulateur COM.  

Pour configurer votre système pour utiliser Isabel, procédez comme suit :  

- Installez les composants de sécurité Isabel. Pour plus d'informations, voir la zone de téléchargement du [site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323).  

- Installez l'encapsulateur COM fabriqué par l'organisation Isabel. Cet encapsulateur est inclus dans le package Isabel GO 6.20.  

- Enregistrez l'encapsulateur COM sur votre ordinateur. À l'invite de commandes, recherchez le fichier CIS.dll puis exécutez la commande **regsvr32 CISComWrapper.dll**.  

## <a name="see-also"></a>Voir aussi  
 [Site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323)   
 [Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)   
 [Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)
