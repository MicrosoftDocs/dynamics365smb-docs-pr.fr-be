---
title: "Comment générer des propositions de paiement"
description: "Après avoir créé des transactions bancaires électroniques, vous pouvez commencer à générer des propositions de paiement. Pour cela, utilisez une feuille paiement."
redirect_url: belgian-electronic-payments
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 1c7a748f48cb36b30851795119a072ab6d77c961
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="generate-payment-suggestions"></a>Générer des propositions de paiement
Après avoir créé des transactions bancaires électroniques, vous pouvez commencer à générer des propositions de paiement. Vous pouvez le faire dans la feuille paiement.  

## <a name="to-generate-payment-suggestions"></a>Pour générer des propositions de paiement  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles paiement**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez la feuille adéquate, puis choisissez l'action **Proposer paiements fournisseur**.  
3.  Dans la fenêtre **Proposer paiements fournisseur**, dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Dern. date d'échéance**|Entrez la dernière date d'échéance qui peut apparaître sur les écritures comptables fournisseur à inclure dans le traitement par lots.|  
    |**Tenir compte des avoirs**|Sélectionnez pour inclure les avoirs restants pour les fournisseurs. Les avoirs seront soustraits du montant dû. Lorsque vous sélectionnez des avoirs, la date d'échéance n'est pas utilisée.|  
    |**Obtenir escomptes**|Sélectionnez pour inclure les écritures comptables fournisseur pour lesquelles vous pouvez obtenir un escompte.|  
    |**Date d'escompte**|Entrez la date qui sera utilisée pour calculer un escompte.|  
    |**Montant disponible**|S'il y a un montant maximal disponible pour les paiements, vous pouvez l'entrer ici. Le traitement par lots créera alors une proposition de paiement basée sur ce montant et la priorité des fournisseurs.|  
    |**Date comptabilisation**|Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille paiement.|  

4.  Dans le raccourci **Fournisseur**, entrez les critères de filtre.  
5.  Cliquez sur le bouton **OK** pour démarrer le traitement par lots.  

Une fois le traitement par lots terminé, la feuille paiement contient toutes les écritures comptables fournisseur qui correspondent aux filtres.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md)   
 [Imprimer des fichiers de paiement](how-to-print-payment-files.md)

