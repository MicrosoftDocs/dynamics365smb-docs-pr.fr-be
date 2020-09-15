---
title: Paramétrage des nomenclatures produits belges
description: Les autorités douanières et fiscales belges ont établi un code article à 8 chiffres pour diverses nomenclatures produits.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: df49775ffa64d024bd015897acb11b5e15bc272c
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778441"
---
# <a name="set-up-belgian-tariff-numbers"></a>Paramétrer les nomenclatures produits belges
Les autorités douanières et fiscales belges ont établi un code article à 8 chiffres pour diverses nomenclatures produits.  

### <a name="to-set-up-tariff-numbers"></a>Pour paramétrer les nomenclatures produits  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Nomenclatures produits**, puis sélectionnez le lien associé.  
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
 [Exporter les déclarations de tiers intracomm.](how-to-export-intrastat-third-party-declararations.md)   
 [Imprimer l'état Formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md)
