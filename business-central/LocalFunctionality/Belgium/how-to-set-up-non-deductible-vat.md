---
title: Paramétrage de la TVA non déductible
description: Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 6c55566a1d048461d5a02a6f124e1f81d00e70c8
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/01/2020
ms.locfileid: "3180851"
---
# <a name="set-up-non-deductible-vat"></a>Paramétrer la TVA non déductible
Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA. Par exemple, dans la page **Fiche compte général**, si vous entrez 75 dans le champ **% de TVA non déductible**, 75 % du montant de TVA normal sont considérés comme des frais supplémentaires et sont ajoutés au montant net lors de la validation. Les 25 % restants sont validés en tant que TVA normale.  

> [!NOTE]  
>  Si aucune valeur n'est entrée dans le champ **% de TVA non déductible**, le montant de TVA est déductible à 100 %.  

## <a name="to-set-up-the-non-deductible-vat-percentage"></a>Pour définir le pourcentage de TVA non déductible  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Plan comptable**, puis choisissez le lien associé.  
2.  Sélectionnez un compte frais général qui requiert la déduction partielle, puis choisissez l'action **Modifier**.  
3.  Saisissez le montant dans le champ **% de TVA non déductible**.  
4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [TVA belge](belgian-vat.md)   
 [Imprimer les déclarations de TVA périodiques](how-to-print-periodic-vat-reports.md)
