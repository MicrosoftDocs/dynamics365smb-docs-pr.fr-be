---
title: "Comment apporter des corrections manuelles à la TVA"
description: "Vous pouvez apporter des corrections à des écritures TVA validées sans valider la correction dans les écritures TVA ou les écritures comptables. Cette option est utile si vous devez apporter une modification aux montants totaux TVA vente ou achat sans modifier la base TVA. Par exemple, vous pouvez corriger manuellement la TVA si vous recevez une facture d'un fournisseur qui a mal calculé la TVA."
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
ms.openlocfilehash: 3feba6afb6327cd274adb43e83ab91a9af864eea
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="make-manual-corrections-to-vat"></a>Effectuer des corrections de TVA manuellement
Vous pouvez apporter des corrections à des écritures TVA validées sans valider la correction dans les écritures TVA ou les écritures comptables. Cette option est utile si vous devez apporter une modification aux montants totaux TVA vente ou achat sans modifier la base TVA. Par exemple, vous pouvez corriger manuellement la TVA si vous recevez une facture d'un fournisseur qui a mal calculé la TVA.  

## <a name="to-make-manual-corrections-to-vat"></a>Pour apporter des corrections manuelles à la TVA  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Aperçu déclaration TVA**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez la ligne qui doit être corrigée. Vous pouvez apporter la correction TVA sur le **Type** de ligne **Total de lignes** et **TVA**.  
3.  Pour apporter la correction, sélectionnez le champ **Montant correction**. La fenêtre **Liste corrections TVA manuelles** s'ouvre.  
4.  Choisissez l'action **Modifier la liste**. Dans la fenêtre **Liste corrections TVA manuelles**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Date comptabilisation**|Entrez la date de validation de la correction TVA.|  
    |**Montant**|Entrez le montant de la correction TVA. Vous devez entrer le montant de la correction, pas le nouveau montant. Par exemple, si le montant est de 1000,00 et doit être de 1200,00, entrez 200,00.|  
    |**Montant DR**|Ce champ affiche le montant de la correction TVA dans la devise report.<br /><br /> Le champ est calculé automatiquement en fonction du contenu du champ **Montant** et du taux de change actuel.|  

5.  Cliquez sur le bouton **OK**.  
6.  Actualisez la fenêtre **Aperçu déclaration TVA** pour voir vos corrections.  
7.  Pour afficher un état lié à l'aperçu des informations sur la TVA, choisissez l'une des actions suivantes :  

    |Action|Description|  
    |------------|---------------------------------------|  
    |**État détaillé**|Ouvre l'état **Déclaration TVA**. Pour plus d'informations, voir Déclaration TVA.|  
    |**Décl. TVA - Formulaire/Intervat**|Ouvre l'état **TVA - Formulaire**. Pour plus d'informations, voir TVA - Formulaire.<br /><br /> L'état **Décl. TVA - Formulaire/Intervat** est basé sur le modèle Déclaration TVA défini dans les paramètres comptabilité. C'est pourquoi il peut exporter des données qui ne sont pas identiques à celles qui s'affichent dans la fenêtre **Aperçu déclaration TVA** window.|  
    |**Décl. TVA - Sommaire : État**|Ouvre l'état **Déclaration TVA - Sommaire**. Pour plus d'informations, voir Déclaration TVA - Sommaire.|  

## <a name="see-also"></a>Voir aussi  
 [TVA belge](belgian-vat.md)   
 [Imprimer des états TVA périodiques](how-to-print-periodic-vat-reports.md)   
 [Configurer la TVA non déductible](how-to-set-up-non-deductible-vat.md)

