---
title: Isabel 6
description: "L'organisation Isabel a développé une plateforme Client Isabel Synchronizer (CIS) qui permet à [!INCLUDE[d365fin](../../includes/d365fin_md.md)] de s'intégrer en toute sécurité à Isabel. CIS gère l'échange de documents vers et depuis le serveur Isabel."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: f06394c4a2aa1dc7f1df1d6e1a1339e81a1a8d1f
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="isabel-6"></a>Isabel 6
L'organisation Isabel a développé une plateforme appelée Client Isabel Synchronizer (CIS), qui permet l'intégration sécurisée de [!INCLUDE[d365fin](../../includes/d365fin_md.md)] avec Isabel. CIS traite les échanges de documents depuis et vers le serveur Isabel.  

Pour télécharger les fichiers bancaires depuis ou vers le serveur, vous devez configurer votre environnement pour qu'il fonctionne avec Isabel. [!INCLUDE[d365fin](../../includes/d365fin_md.md)] communique au serveur CIS.dll via une fonction wrapper COM.  

Pour configurer votre système afin qu'il fonctionne avec Isabel, suivez les étapes ci-dessous :  

- Installez les composants de sécurité d'Isabel. Pour en savoir plus, consultez la section consacrée au téléchargement sur le [site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323).  

- Installez la fonction wrapper COM conçue par l'organisation Isabel. Cette fonction wrapper est incluse dans le package d'Isabel GO 6.20.  

- Enregistrez la fonction wrapper COM sur votre ordinateur. À l'invite de commandes, localisez le fichier CIS.dll, puis exécutez la commande **regsvr32 CISComWrapper.dll**.  

## <a name="see-also"></a>Voir aussi  
 [Site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323)   
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)

