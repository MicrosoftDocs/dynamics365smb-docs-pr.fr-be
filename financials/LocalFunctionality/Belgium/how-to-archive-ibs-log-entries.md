---
title: "Comment archiver les écritures journal IBS"
description: "Les lignes journal IBS dont le statut de processus est **Traitées** peuvent être archivées. Les journaux IBS contiennent des informations sur les fichiers de banque électronique créés au cours des transferts par banque électronique via Isabel."
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
ms.openlocfilehash: 9f4f44e0d604fea842f674fbe3c0add2901c3462
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="archive-ibs-log-entries"></a>Archiver les entrées de journal IBS
> [!Note]
> [!INCLUDE [onprem_only](../../includes/onprem_only_md.md)]

Les lignes de journal IBS ayant le statut de processus **Traité** peuvent être archivées. Les journaux IBS contiennent des informations sur les fichiers de banque électronique créés au cours des transferts par banque électronique via Isabel.  

Isabel est un programme logiciel tiers fréquemment utilisé en Belgique pour gérer et transférer des fichiers de banque électronique. Isabel prend actuellement en charge les transactions bancaires telles que les virements SEPA, les ordres bancaires automatisés et les fichiers CODA.  

## <a name="to-archive-an-ibs-log-entry"></a>Pour archiver une écriture journal IBS  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez la ligne que vous souhaitez archiver, puis choisissez l'action **Archiver**.  
3.  Un message vous propose d'archiver les enregistrements de journaux IBS.  
4.  Cliquez sur le bouton **Oui**.  

    > [!NOTE]  
    >  Le champ **Statut processus** de la ligne est maintenant défini sur **Archivé**. Vous pouvez supprimer un enregistrement dont le statut est **Archivé**.  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)

