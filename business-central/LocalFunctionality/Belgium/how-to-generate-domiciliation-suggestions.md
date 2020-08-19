---
title: Génération des suggestions de domiciliation
description: Après avoir paramétré les domiciliations, vous pouvez commencer à générer des suggestions de domiciliation. Vous pouvez uniquement créer des suggestions de domiciliation pour les clients nationaux.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: f58b94bb0254c19aaf06dbdde621ed88567ad3a0
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 08/10/2020
ms.locfileid: "3677169"
---
# <a name="generate-domiciliation-suggestions"></a>Générer des suggestions de domiciliation
Après avoir paramétré les domiciliations, vous pouvez commencer à générer des suggestions de domiciliation. Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez uniquement créer des suggestions de domiciliation pour les clients nationaux.  

## <a name="to-generate-domiciliation-suggestions"></a>Pour générer des suggestions de domiciliation  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuille domiciliation**, puis sélectionnez le lien associé.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Suggérer des domiciliations**.  
3.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date d'échéance**|Entrez la date d'échéance à inclure dans le traitement par lots. Seules les écritures dont la date d'échéance est antérieure ou identique à cette date sont incluses.|  
    |**Accepter les escomptes**|Sélectionnez ce champ si vous souhaitez inclure dans le traitement par lots les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.|  
    |**Date d'escompte**|Entrez la date qui est utilisée pour calculer l'escompte.|  
    |**Sélectionner les remboursements possibles**|Sélectionnez ce champ si vous souhaitez inclure dans le traitement par lots les remboursements.|  
    |**Date de validation**|Entrez la date qui s'affiche comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.|  

4.  Entrez les éventuels critères de filtre supplémentaires.  
5.  Cliquez sur le bouton **OK**.  

Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes correspondant aux filtres.  

> [!NOTE]  
>  Les suggestions de domiciliation n'incluent que les clients pour lesquels un numéro de domiciliation est configuré. Pour plus d'informations, voir [Paramétrer les domiciliations](how-to-set-up-domiciliations.md).  

## <a name="see-also"></a>Voir aussi  
 [Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)   
 [Prélévement à l'aide de la domiciliation](direct-debit-using-domiciliation.md)   
 [Paramétrer les domiciliations](how-to-set-up-domiciliations.md)   
 [Tester les domiciliations](how-to-test-domiciliations.md)   
 [Modifier et supprimer des lignes de domiciliation](how-to-edit-and-delete-domiciliation-lines.md)   
 [Exporter et valider les domiciliations](how-to-export-and-post-domiciliations.md)
