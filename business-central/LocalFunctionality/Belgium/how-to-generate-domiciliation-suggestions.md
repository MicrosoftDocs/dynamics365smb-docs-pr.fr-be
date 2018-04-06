---
title: "Comment générer des propositions de domiciliation"
description: "Après avoir créé des domiciliations, vous pouvez commencer à générer des propositions de domiciliation. Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous ne pouvez créer que des suggestions de domiciliation pour les clients nationaux."
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
ms.openlocfilehash: bf633fb5a142a59ea54e5cac0552cabecb015e9d
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="generate-domiciliation-suggestions"></a>Générer les propositions de domiciliation
Après avoir créé des domiciliations, vous pouvez commencer à générer des propositions de domiciliation. Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux.  

## <a name="to-generate-domiciliation-suggestions"></a>Pour générer des propositions de domiciliation  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille saisie domiciliation**, puis sélectionnez le lien correspondant.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Proposer domiciliations**.  
3.  Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Date besoin**|Entrez la date d'échéance à inclure dans le traitement par lots. Seules les écritures ayant une date d'échéance antérieure ou identique à cette date seront incluses.|  
    |**Obtenir escomptes**|Sélectionnez si vous souhaitez que le traitement par lots comprenne les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.|  
    |**Date d'escompte**|Entrez la date qui sera utilisée pour calculer l'escompte.|  
    |**Inclure remboursements poss.**|Sélectionnez si vous souhaitez que le traitement par lots inclue les remboursements.|  
    |**Date comptabilisation**|Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.|  

4.  Dans le raccourci **Client**, entrez les éventuels critères de filtre supplémentaires.  
5.  Cliquez sur le bouton **OK**.  

Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes qui correspondent aux filtres.  

> [!NOTE]  
>  Les suggestions de domiciliation ne concernent que les clients disposant d'un numéro de domiciliation. Pour plus d'informations, reportez-vous à [Paramétrer les domiciliations](how-to-set-up-domiciliations.md).  

## <a name="see-also"></a>Voir aussi  
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Prélèvements bancaires avec domiciliation](direct-debit-using-domiciliation.md)   
 [Paramétrer les domiciliations](how-to-set-up-domiciliations.md)   
 [Tester les domiciliations](how-to-test-domiciliations.md)   
 [Modifier et supprimer des lignes de domiciliation](how-to-edit-and-delete-domiciliation-lines.md)   
 [Exporter et valider les domiciliations](how-to-export-and-post-domiciliations.md)

