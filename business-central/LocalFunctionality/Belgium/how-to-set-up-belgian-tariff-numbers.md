---
title: 'Paramétrer les nomenclatures produits belges [BE]'
description: "Les autorités douanières et fiscales belges ont établi un code article à 8\_chiffres pour diverses nomenclatures produits."
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.form: 310
ms.date: 06/17/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="set-up-belgian-tariff-numbers-in-the-belgian-version"></a>Paramétrer les nomenclatures produits belges dans la version belge

Les autorités douanières et fiscales belges ont établi un code article à 8 chiffres pour diverses nomenclatures produits.  

## <a name="to-set-up-tariff-numbers"></a>Pour paramétrer les nomenclatures produits

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Nomenclatures produits**, puis choisissez le lien associé.  
2. Sélectionnez l'action **Nouveau**.  
3. Dans la page **Nomenclatures produits**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Facteur de conversion**|Entrez le facteur de conversion pour la nomenclature produit. Le facteur de conversion est le facteur par lequel vous devez multiplier l'unité article pour obtenir l'unité imposée par la D.E.B. Le facteur de conversion peut être utilisé lorsque l'unité article diffère de l'unité imposée par la D.E.B. Le champ est disponible lorsque le champ **Unités supplémentaires** est sélectionné.|  
    |**Unité**|Entrez l'unité de mesure pour la nomenclature produit. Le champ est disponible lorsque le champ **Unités supplémentaires** est sélectionné.|  
    |**Poids obligatoire**|Sélectionnez ce champ pour afficher le poids des articles.|  

4. Choisissez le bouton **OK**.  
  
## <a name="see-also"></a>Voir aussi

 [États intracommunautaires belges](belgian-intrastat-reporting.md)   
 [Paramétrer des types de déclarations](how-to-set-up-declaration-types.md)   
 [Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md)   
 [Exporter les déclarations de tiers intracomm.](how-to-export-intrastat-third-party-declararations.md)   
 [Imprimer l'état Formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
