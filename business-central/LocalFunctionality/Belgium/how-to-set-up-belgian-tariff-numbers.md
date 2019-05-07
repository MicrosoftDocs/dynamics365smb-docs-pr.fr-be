---
title: Paramétrage des nomenclatures produits belges
description: Les autorités douanières et fiscales belges ont établi un code article à 8 unités pour diverses nomenclatures produits.
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
ms.openlocfilehash: 62ffca9d0507e3cadaa79621d0d8a2c45a7af669
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2019
ms.locfileid: "920072"
---
# <a name="set-up-belgian-tariff-numbers"></a>Paramétrer les nomenclatures produits belges
Les autorités douanières et fiscales belges ont établi un code article à 8 unités pour diverses nomenclatures produits.  

### <a name="to-set-up-tariff-numbers"></a>Pour paramétrer les nomenclatures produits  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Nomenclatures produits**, puis sélectionnez le lien connexe.  
2.  Sélectionnez l'action **Nouveau**.  
3.  Dans la page **Nomenclatures produits**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Facteur de conversion**|Entrez le facteur de conversion pour la nomenclature produit. Le facteur de conversion est le facteur par lequel vous devez multiplier l'unité article pour obtenir l'unité imposée par la D.E.B. Le facteur de conversion peut être utilisé lorsque l'unité article diffère de l'unité imposée par la D.E.B. Le champ est disponible lorsque le champ **Unités supplémentaires** est sélectionné.|  
    |**Unité**|Entrez l'unité de mesure pour la nomenclature produit. Le champ est disponible lorsque le champ **Unités supplémentaires** est sélectionné.|  
    |**Poids obligatoire**|Sélectionnez ce champ pour afficher le poids des articles.|  

4.  Choisissez le bouton **OK**.  
  
## <a name="see-also"></a>Voir aussi  
 [États intracommunautaires belges](belgian-intrastat-reporting.md)   
 [Paramétrer des types de déclarations](how-to-set-up-declaration-types.md)   
 [Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md)   
 [Exporter les déclarations tierces intracommunautaires](how-to-export-intrastat-third-party-declararations.md)   
 [Imprimer l'état du formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md)
