---
title: "Comment configurer la TVA non déductible"
description: "Vous pouvez calculer les montants de TVA pour des types spécifiques de dépenses qui peuvent être partiellement déclarés comme soumis à la TVA."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 9bc5416852f31457166a982538093f387c6b4698
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-non-deductible-vat"></a>Configurer la TVA non déductible
Vous pouvez calculer les montants TVA pour les types spécifiques de frais pouvant être partiellement déclarés comme TVA. Par exemple, dans la fenêtre **Fiche compte général**, si vous entrez 75 % dans le champ **% TVA non déductible**, 75 % du montant de TVA habituel seront considérés comme un coût supplémentaire et seront ajoutés au montant net lors de la validation. Les 25 % restants seront validés comme montant de TVA habituel.  

> [!NOTE]  
>  Si aucune valeur n'est entrée dans le champ **% TVA non déductible**, le montant de TVA est 100 % déductible.  

## <a name="to-set-up-the-non-deductible-vat-percentage"></a>Pour configurer le pourcentage de TVA non déductible  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Plan comptable**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez un compte dépenses général qui nécessite la déduction partielle, puis choisissez l'action **Modifier**.  
3.  Dans le raccourci **Validation**, entrez le montant du champ **% TVA non déductible**.  
4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [TVA belge](belgian-vat.md)   
 [Imprimer des états TVA périodiques](how-to-print-periodic-vat-reports.md)

