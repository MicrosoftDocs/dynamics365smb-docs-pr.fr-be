---
title: Génération des suggestions de règlement
description: Après avoir configuré les opérations bancaires électroniques, vous pouvez commencer à générer des suggestions de règlement. Pour cela, utilisez la feuille paiement.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 31804146cca328c7a3155bf2f310b96864135c1a
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379545"
---
# <a name="generate-payment-suggestions"></a>Générer des suggestions de règlement
Après avoir configuré les opérations bancaires électroniques, vous pouvez commencer à générer des suggestions de règlement. Pour cela, utilisez la feuille paiement.  

## <a name="to-generate-payment-suggestions"></a>Pour générer des suggestions de règlement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles paiement**, puis sélectionnez le lien associé.  
2.  Sélectionnez la feuille appropriée, puis choisissez l'action **Proposer paiements fournisseur**.  
3.  Sur la page **Proposer paiements fournisseur**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Dernière date d'échéance**|Entrez la dernière date d'échéance qui peut s'afficher sur les écritures comptables fournisseur à inclure dans le traitement par lots.|  
    |**Accepter les avoirs**|Sélectionnez ce champ pour inclure les avoirs en attente pour les fournisseurs. Les avoirs sont soustraits du montant dû. Lorsque vous sélectionnez des avoirs, la date d'échéance n'est pas utilisée.|  
    |**Accepter les escomptes**|Sélectionnez ce champ pour inclure les écritures comptables fournisseur pour lesquelles vous pouvez obtenir un escompte.|  
    |**Date d'escompte**|Entrez la date qui est utilisée pour calculer un escompte.|  
    |**Montant disponible**|S'il y a un montant maximal disponible pour les paiements, vous pouvez le saisir ici. Le traitement par lots crée ensuite une suggestion de paiement sur la base de ce montant et de la priorité des fournisseurs.|  
    |**Date de validation**|Saisissez la date qui s'affiche comme date comptabilisation sur les lignes que le traitement par lots insère dans la feuille paiements.|  

4.  Entrez les critères de filtre.  
5.  Pour démarrer le traitement par lots, cliquez sur le bouton **OK**.  

Lorsque le traitement par lots est terminé, la feuille paiement contient toutes les écritures comptables fournisseur correspondant aux filtres.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Gérer les lignes de paiement électronique](how-to-manage-electronic-payment-lines.md)   
 [Imprimer les fichiers de paiement](how-to-print-payment-files.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]