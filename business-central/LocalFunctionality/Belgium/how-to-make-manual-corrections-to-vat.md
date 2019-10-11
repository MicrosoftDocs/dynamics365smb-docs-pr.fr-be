---
title: Corrections manuelles de la TVA
description: Vous pouvez apporter des corrections à des écritures TVA validées sans valider la correction dans les écritures TVA ou comptables. Cela est utile si vous devez modifier le total des montants TVA des lignes vente ou achat sans modifier la base de TVA. Par exemple, vous pouvez corriger manuellement la TVA si vous recevez une facture d'un fournisseur qui n'a pas calculé correctement la TVA.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: cff41ae9faf2867ac91bc216bb7fc29c9fa10da3
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300254"
---
# <a name="make-manual-corrections-to-vat"></a>Corrections manuelles de la TVA
Vous pouvez apporter des corrections à des écritures TVA validées sans valider la correction dans les écritures TVA ou comptables. Cela est utile si vous devez modifier le total des montants TVA des lignes vente ou achat sans modifier la base de TVA. Par exemple, vous pouvez corriger manuellement la TVA si vous recevez une facture d'un fournisseur qui n'a pas calculé correctement la TVA.  

## <a name="to-make-manual-corrections-to-vat"></a>Pour apporter des corrections manuelles à la TVA  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Aperçu déclaration TVA**, puis sélectionnez le lien connexe.  
2.  Sélectionnez la ligne qui doit être corrigée. Vous pouvez corriger la TVA pour le **Type** de ligne **Lignes** et **TVA**.  
3.  Pour effectuer la correction, sélectionnez le champ **Montant de la correction**. La page **Liste des corrections TVA manuelles** s'ouvre.  
4.  Choisissez l'action **Modifier la liste**. Dans la page **Liste des corrections TVA manuelles**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date de validation**|Entrez la date de validation de la correction TVA.|  
    |**Montant**|Entrez le montant de la correction TVA. Vous devez entrer le montant de la correction, et non le nouveau montant. Par exemple, si le montant est 1 000 et devrait être 1 200, entrez 200.|  
    |**Montant DR**|Ce champ affiche le montant de la correction TVA en devise report.<br /><br /> Le champ est automatiquement calculé, selon le contenu du champ **Montant** et le taux de change actuel.|  

5.  Choisissez le bouton **OK**.  
6.  Actualisez la page **Aperçu déclaration TVA** pour visualiser vos corrections.  
7.  Pour afficher un état associé à l'aperçu des informations TVA, choisissez l'une des actions suivantes :  

    |Action|Désignation|  
    |------------|---------------------------------------|  
    |**État détaillé**|Ouvre l'état **Déclaration TVA**. Pour plus d'informations, voir Déclaration TVA.|  
    |**Formulaire/Déclaration Intervat**|Ouvre l'état **TVA - Formulaire**.<br /><br /> L'état **Formulaire/Déclaration Intervat** est basé sur le modèle déclaration TVA défini dans les paramètres comptabilité. Par conséquent, il peut exporter des données différentes de celles affichées dans la page **Aperçu déclaration TVA**.|  
    |**État Résumé déclaration**|Ouvre l'état **Résumé déclaration de TVA**.|  

## <a name="see-also"></a>Voir aussi  
 [TVA belge](belgian-vat.md)   
 [Imprimer les déclarations de TVA périodiques](how-to-print-periodic-vat-reports.md)   
 [Configurer la TVA non déductible](how-to-set-up-non-deductible-vat.md)
