---
title: 'Paramétrer des types de déclarations [BE]'
description: 'Dans Business Central, il existe deux types de déclaration dans la version belge, la déclaration simplifiée et la déclaration étendue.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 06/17/2021
ms.author: bholtorf
---
# <a name="set-up-declaration-types-in-the-belgian-version"></a>Paramétrer des types de déclarations dans la version belge

[!INCLUDE[intrastat-2022w2](../../includes/intrastat-2022w2.md)]

Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], il existe deux types de déclarations :  

- Déclaration simplifiée  
- Déclaration étendue  

Le type de déclaration dépend de la quantité de biens expédiés ou reçus. Pour déterminer le type de déclaration à utiliser, visitez le site Web de la [Banque Nationale de Belgique](https://aka.ms/BelgianNationalBank).  

Lorsque vous utilisez la déclaration étendue, vous devez également configurer un Incoterm dans la déclaration intracommunautaire pour chaque méthode de livraison. Si vous ne voyez pas le champ **Incoterm dans la déclaration D.E.B.** de la page **Conditions de livraison**, vous devrez peut-être personnaliser la page et ajouter le champ.

## <a name="to-set-up-declaration-types"></a>Pour paramétrer des types de déclarations

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Paramètres comptabilité**, puis choisissez le lien associé.  
2. Activez la case à cocher **Déclaration D.E.B. simplifiée** pour configurer un type de déclaration simplifiée. Effacez ce champ pour utiliser la déclaration étendue.  
3. Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi

[États intracommunautaires belges](belgian-intrastat-reporting.md)  
[Paramétrer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md)  
[Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md)  
[Exporter les déclarations tierces intracommunautaires](how-to-export-intrastat-third-party-declararations.md)  
[Imprimer l'état Formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md)  
[Paramétrer les états intracommunautaires](../../finance-how-setup-report-intrastat.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
