---
title: Générer des suggestions de règlement [BE]
description: Après avoir configuré les opérations bancaires électroniques, vous pouvez commencer à générer des suggestions de règlement. Pour cela, utilisez la feuille paiement.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 256
ms.date: 06/17/2021
ms.author: edupont
ms.openlocfilehash: ea4d0844d4b915f5e97d3bb7da5fef67a3444e9d
ms.sourcegitcommit: 6d48c1f601ed22b6b0358311baf63c073ab75e64
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/01/2022
ms.locfileid: "8366309"
---
# <a name="generate-payment-suggestions-in-the-belgian-version"></a>Générer des suggestions de règlement dans la version belge
Après avoir configuré les opérations bancaires électroniques, vous pouvez commencer à générer des suggestions de règlement. Pour cela, utilisez la feuille paiement.  

## <a name="to-generate-payment-suggestions"></a>Pour générer des suggestions de règlement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles paiement**, puis choisissez le lien associé.  
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
 [Gérer les lignes de paiement électronique](/dynamics365/business-central/LocalFunctionality/Belgium/belgian-electronic-payments)   
 [Imprimer les fichiers de paiement](how-to-print-payment-files.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]