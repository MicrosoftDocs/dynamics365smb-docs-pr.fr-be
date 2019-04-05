---
title: Procédure d'exportation des déclarations tierces intracommunautaires
description: En Belgique, un déclarant tiers doit renseigner la déclaration D.E.B (Intrastat). Le déclarant tiers doit être une personne ou une société externe.
services: project-madeira
documentationcenter: ''
author: sorenfriisalexandersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/30/2018
ms.author: soalex
ms.openlocfilehash: acb6c589ad748d7e98e71acef9cc0d6e62fc53d3
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/08/2019
ms.locfileid: "826499"
---
# <a name="export-intrastat-third-party-declarations"></a>Exporter les déclarations tierces intracommunautaires
En Belgique, un déclarant tiers doit renseigner la déclaration D.E.B (Intrastat). Le déclarant tiers doit être une personne ou une société externe. 

## <a name="to-export-the-third-party-declaration"></a>Pour exporter la déclaration tierce  
Avant d'exporter le fichier, il est conseillé d'afficher un aperçu de l'état. Pour plus d'informations, voir [Imprimer l'état du formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md).  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Feuille intracomm.**, puis sélectionnez le lien connexe.  
2.  Choisissez l'action **Créer fichier**.  
3.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Déclaration Nihil**|Sélectionnez ce champ si vous n'avez aucune transaction commerciale avec des pays/régions de l'Union européenne (UE) et que vous souhaitez envoyer une déclaration vide.|  
    |**Informations de contrepartie**|Activez ce champ pour inclure des informations de contrepartie dans le fichier de déclaration d'échanges de biens intracommunautaires (nouvelle exigence à partir de 2019). La déclaration de contrepartie ajoutée au fichier est issue du **Code pays/région origine** et de l'**ID partenaire** de la Feuille intracomm.|  
    |**N° entreprise/N° id. intracomm.**|Entrez le numéro d'entreprise ou d'enregistrement de TVA.|  
    
4.  Choisissez le bouton **OK**.  

Ensuite, envoyez la déclaration au portail OneGate.  

## <a name="see-also"></a>Voir aussi  
 [États intracommunautaires belges](belgian-intrastat-reporting.md)   
 [Paramétrer des types de déclarations](how-to-set-up-declaration-types.md)   
 [Paramétrer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md)   
 [Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md)   
 [Imprimer l'état du formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md)
