---
title: TVA belge
description: Les améliorations belges de la fonction de déclaration de TVA vous permettent d'imprimer des détails sur les transactions TVA.
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
ms.openlocfilehash: 4af7598e12720d18a6212c841443e1f577787ac0
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778696"
---
# <a name="belgian-vat"></a>TVA belge
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] comprend des améliorations belges à la fonction de déclaration de TVA qui vous permet d'imprimer les détails de transaction TVA. Vous devez envoyer les états suivants aux autorités fiscales belges :  

-   Déclaration mensuelle/trimestrielle - Cet état permet de créer des déclarations de TVA mensuelles ou trimestrielles, en fonction des revenus de votre société.  

-   Listing TVA annuel (sur papier/disquette) - Cet état permet de déclarer annuellement tous les montants facturés pour les biens et les services à toutes les sociétés belges avec un numéro de TVA enregistré.  

-   Listing TVA-VIES (sur papier/disquette) - Cet état permet de déclarer les ventes de marchandises à d'autres pays.  

Vous êtes également tenu de fournir un relevé imprimé détaillant les transactions TVA aux autorités fiscales belges. Pour plus d'informations, voir Déclaration TVA.  

## <a name="non-deductible-vat"></a>TVA non déductible  
 En Belgique, la TVA peut être entièrement ou partiellement déductible. Des dépenses comme les frais de représentation ou les achats de voitures ne sont que partiellement déductibles et la transaction doit spécifier quel pourcentage de la TVA est non déductible. Par exemple, vous créez un compte général pour les immobilisations comme les voitures, et un autre compte pour les frais de représentation. Pour chaque compte, vous spécifiez quel pourcentage de la TVA déclarée est non déductible en définissant le champ **Pourcentage TVA non déductible**. Ensuite, lorsque vous validez une transaction, la TVA déductible sera validée sur le compte TVA correspondant, et la TVA non déductible sera ajoutée au montant de base et validée sur le même compte que les immobilisations corporelles et incorporelles.  

 Pour les immobilisations, la TVA non déductible est amortie simplement comme le coût d'acquisition de base de l'immobilisation. Vous devez paramétrer des groupes comptabilisation immobilisation distincts pour chaque pourcentage de TVA non déductible, étant donné que chaque groupe comptabilisation immobilisation est validé sur un compte général où le champ **Pourcentage TVA non déductible** spécifie quel pourcentage de TVA doit être validé sur le même compte que l'immobilisation.  

 Si vous sélectionnez le champ **TVA non déductible comprise** dans une ligne déclaration TVA, la TVA non déductible est incluse dans le montant TVA. L'état **Calculer et valider décl. TVA** ajoute la partie non déductible de ce montant aux champs **Montant TVA non déductible** et **Montant TVA devise origine non déductible** dans les écritures TVA résultantes.  

## <a name="see-also"></a>Voir aussi  
 [Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)   
 [Imprimer des états TVA périodiques](how-to-print-periodic-vat-reports.md)   
 [Configurer la TVA non déductible](how-to-set-up-non-deductible-vat.md)
