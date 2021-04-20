---
title: Paramétrage de la TVA non déductible
description: Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3798454967217fb3b10d22e2c168ed8c2185722f
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779201"
---
# <a name="set-up-non-deductible-vat"></a>Paramétrer la TVA non déductible
Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA. Par exemple, dans la page **Fiche compte général**, si vous entrez 75 dans le champ **% de TVA non déductible**, 75 % du montant de TVA normal sont considérés comme des frais supplémentaires et sont ajoutés au montant net lors de la validation. Les 25 % restants sont validés en tant que TVA normale.  

> [!NOTE]  
>  Si aucune valeur n'est entrée dans le champ **% de TVA non déductible**, le montant de TVA est déductible à 100 %.  

## <a name="to-set-up-the-non-deductible-vat-percentage"></a>Pour définir le pourcentage de TVA non déductible  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Plan comptable**, puis sélectionnez le lien associé.  
2.  Sélectionnez un compte frais général qui requiert la déduction partielle, puis choisissez l'action **Modifier**.  
3.  Saisissez le montant dans le champ **% de TVA non déductible**.  
4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [TVA belge](belgian-vat.md)   
 [Imprimer les déclarations de TVA périodiques](how-to-print-periodic-vat-reports.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]