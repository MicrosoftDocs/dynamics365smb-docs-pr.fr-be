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
ms.author: edupont
ms.openlocfilehash: 8ada4b29ead380f80309fd1c6f1129623a28d011
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778417"
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
