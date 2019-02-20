---
title: "Téléchargement des fichiers de paiement vers un serveur Isabel"
description: "Les fichiers de paiement peuvent être téléchargés à l'aide de la page Feuilles IBS. Les champs Mode d'intégration du chargement et Mode d'intégration du téléchargement dans la page Paramétrage des opérations bancaires électroniques doivent être définis sur Assisté pour télécharger les fichiers de paiement."
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
ms.sourcegitcommit: 1acac32a417f794801da50c866db2643ea0a4c2d
ms.openlocfilehash: 34ca4afa9714336652ed654194f02e5493a750ee
ms.contentlocale: fr-be
ms.lasthandoff: 01/22/2019

---
# <a name="upload-payment-files-to-an-isabel-server"></a>Télécharger les fichiers de paiement vers un serveur Isabel
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

Les fichiers de paiement peuvent être téléchargés à l'aide de la page **Feuilles IBS**. Les champs **Mode d'intégration du chargement** et **Mode d'intégration du téléchargement** dans la page **Paramétrage des opérations bancaires électroniques** doivent être définis sur **Assisté** pour télécharger les fichiers de paiement.  

> [!NOTE]  
>  Avant de pouvoir télécharger les fichiers de paiement, vous devez être connecté au serveur Isabel.  

## <a name="to-upload-payment-files-in-attended-mode"></a>Pour télécharger les fichiers de paiement en mode assisté  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Feuilles IBS**, puis sélectionnez le lien connexe.  
2.  Choisissez l'action **Obtenir le contrat et l'utilisateur**.  
3.  Après avoir vérifié les fichiers de paiement, un ID utilisateur et un ID contrat s'affichent dans les champs **ID utilisateur IBS** et **ID contrat IBS**.  

    Le champ **Statut du téléchargement** est défini sur **Prêt pour le téléchargement**. S'il existe plusieurs contrats sur le serveur Isabel pour le compte bancaire, le champ **Statut du téléchargement** est défini sur **Un conflit existe**. Sélectionnez le contrat approprié.  

4.  Choisissez l'action **Procéder au téléchargement**. Les fichiers de paiement sont téléchargés sur le serveur Isabel et le champ **Statut du processus** est défini sur **Traité**.  
5.  Poursuivez le traitement des fichiers de paiement en les signant et en les envoyant vers le serveur Isabel.  

## <a name="see-also"></a>Voir aussi  
 [Archiver les écritures journal IBS](how-to-archive-ibs-log-entries.md)

