---
title: "Paramétrage de la TVA non déductible"
description: "Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: fd0fd5d1b7aa15d2d5249278a00b6350f953a777
ms.contentlocale: fr-be
ms.lasthandoff: 11/26/2018

---
# <a name="set-up-non-deductible-vat"></a>Paramétrer la TVA non déductible
Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses pouvant être partiellement déclarées comme TVA. Par exemple, dans la page **Fiche compte général**, si vous entrez 75 % dans le champ **% de TVA non déductible**, 75 % du montant de TVA normal sont considérés comme des frais supplémentaires et sont ajoutés au montant net lors de la validation. Les 25 % restants sont validés en tant que TVA normale.  

> [!NOTE]  
>  Si aucune valeur n'est entrée dans le champ **% de TVA non déductible**, le montant de TVA est déductible à 100 %.  

## <a name="to-set-up-the-non-deductible-vat-percentage"></a>Pour définir le pourcentage de TVA non déductible  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.  
2.  Sélectionnez un compte frais général qui requiert la déduction partielle, puis choisissez l'action **Modifier**.  
3.  Dans le raccourci **Validation**, entrez le montant dans le champ **% de TVA non déductible**.  
4.  Choisissez le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [TVA belge](belgian-vat.md)   
 [Imprimer les déclarations de TVA périodiques](how-to-print-periodic-vat-reports.md)

