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
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: a895772c1164e5fad2b5de045b15b0b39cfcf015
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237653"
---
# <a name="download-coda-files-from-an-isabel-server"></a>Télécharger les fichiers CODA à partir d'un serveur Isabel
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

Les fichiers CODA peuvent être téléchargés manuellement ou en mode assisté.  

Pour télécharger manuellement les fichiers CODA, connectez-vous au serveur Isabel et sélectionnez les fichiers que vous souhaitez télécharger. Les fichiers téléchargés peuvent ensuite être importés à partir de la table **Compte bancaire**. Pour plus d'informations, voir [Importer les relevés CODA](how-to-import-coda-statements.md).  

## <a name="to-download-coda-files-in-attended-mode"></a>Pour télécharger les fichiers CODA en mode assisté  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Feuilles IBS**, puis sélectionnez le lien connexe.  
2.  Choisissez l'action **Télécharger**.  
3.  Dans la page **Options de demande de téléchargement IBS**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date début**|Spécifiez la date de début du téléchargement.|  
    |**Historique cumulé**|Spécifiez la date de fin du téléchargement.|  
    |**Format de fichier**|Sélectionnez **Coda** comme format de fichier.|  
    |**Statut du fichier**|Sélectionnez le statut du fichier du téléchargement. Les statuts du fichier sont : **Non téléchargé**, **Téléchargé** et **Tous**. Généralement, vous sélectionnez **Non téléchargé**, car vous téléchargez les fichiers CODA qui n'ont pas été téléchargés dans votre système.|  

4.  Choisissez le bouton **OK**.  

    > [!NOTE]  
    >  Vous ne pouvez pas supprimer des fichiers du serveur Isabel à l'aide de la page **Options de demande de téléchargement IBS**. Vous devez supprimer manuellement les fichiers en vous connectant au serveur Isabel.  

     Une fois que les fichiers CODA ont été téléchargés, le champ **Statut du processus** indique **Créé** dans la page **Feuilles IBS**. Vous pouvez vous connecter au serveur Isabel pour récupérer manuellement les fichiers. Pour plus d'informations, voir [Importer les relevés CODA](how-to-import-coda-statements.md).  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale, Belgique](belgium-local-functionality.md)
