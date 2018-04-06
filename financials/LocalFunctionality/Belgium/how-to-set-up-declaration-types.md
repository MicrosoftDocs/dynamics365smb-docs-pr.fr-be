---
title: "Procédure : Configurer des types de déclaration"
description: "Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], il existe deux types de déclarations."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/07/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: d1826d0e6037052faec8026f352325a554b4990a
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-declaration-types"></a>Configurer des types de déclaration
Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], il existe deux types de déclarations :  

- Déclaration simplifiée  
- Déclaration étendue  

Le type de déclaration dépend du montant des marchandises expédiées ou reçues. Pour déterminer le type de déclaration à utiliser, visitez le site web [Banque nationale de Belgique](http://go.microsoft.com/fwlink/?LinkId=163064).  

Lorsque vous effectuez une déclaration étendue, vous devez également configurer un incoterme dans la déclaration intracommunautaire pour chaque condition livraison. Si vous ne voyez pas **Incoterme dans la déclaration intracommunautaire** dans la page **Conditions de livraison**, vous devrez peut-être personnaliser la page et ajouter le champ. 

## <a name="to-set-up-declaration-types"></a>Pour définir des types de déclaration  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.  
2.  Sur le raccourci **Général**, sélectionnez la case à cocher **D.E.B. simplifiée** pour configurer un type de déclaration simplifiée. Effacez ce champ pour utiliser la déclaration étendue.  
3.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [État intracommunautaire belge](belgian-intrastat-reporting.md)   
 [Configurer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md)   
 [Configurer les numéros d'établissement intracomm.](how-to-set-up-intrastat-establishment-numbers.md)   
 [Exporter les déclarations de tiers intracomm.](how-to-export-intrastat-third-party-declararations.md)   
 [Imprimer le rapport de formulaire intracomm.](how-to-print-the-intrastat-form-report.md)
