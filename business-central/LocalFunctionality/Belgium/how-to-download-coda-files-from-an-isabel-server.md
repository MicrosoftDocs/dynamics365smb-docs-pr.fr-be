---
title: "Procédure : Télécharger des fichiers CODA à partir d'un serveur Isabel"
description: "Les fichiers CODA peuvent être téléchargés manuellement ou en mode assisté."
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
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 3391529dd136311adce3cdca49dcf9917d060e7c
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="download-coda-files-from-an-isabel-server"></a>Télécharger des fichiers CODA à partir d'un serveur Isabel
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

Les fichiers CODA peuvent être téléchargés manuellement ou en mode assisté.  

Pour télécharger manuellement des fichiers CODA, connectez-vous au serveur Isabel et sélectionnez les fichiers que vous souhaitez télécharger. Les fichiers téléchargés peuvent être importés à partir du tableau **Compte bancaire**. Pour plus d'informations, reportez-vous à [Importer des relevés CODA](how-to-import-coda-statements.md).  

## <a name="to-download-coda-files-in-attended-mode"></a>Pour télécharger les fichiers CODA en mode assisté  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.  
2.  Choisissez l'action **Télécharger**.  
3.  Dans la fenêtre **Options de demande de téléchargement IBS**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Date début**|Spécifiez la date de début du téléchargement.|  
    |**Historique cumulé**|Spécifiez la date de fin du téléchargement.|  
    |**Format de fichier**|Sélectionnez **Coda** comme format de fichier.|  
    |**Statut du fichier**|Sélectionnez le statut du fichier du téléchargement. Les statuts du fichier incluent **Non téléchargé**, **Téléchargé** et **Tout**. Généralement, vous devez sélectionner **Non téléchargé**, car vous téléchargez les fichiers CODA qui n'ont pas été téléchargés dans votre système.|  

4.  Cliquez sur le bouton **OK**.  

    > [!NOTE]  
    >  Vous ne pouvez supprimer aucune fichier du serveur Isabel via la fenêtre **Options de demande de téléchargement IBS**. Vous devez supprimer manuellement les fichiers en vous connectant au serveur Isabel.  

     Après le téléchargement des fichiers CODA, le champ **Statut processus** sera défini sur **Créé** dans la fenêtre **Journaux IBS**. Vous pouvez vous connecter au serveur Isabel pour récupérer manuellement les fichiers. Pour plus d'informations, reportez-vous à [Importer des relevés CODA](how-to-import-coda-statements.md).  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)

