---
title: Comment activer les paiements SEPA
description: Pour soumettre les paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 070f9cf19a9e85d8da5b352d319b347b88ddd885
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237713"
---
# <a name="activate-sepa-payments"></a>Activer des paiements SEPA
Pour envoyer les paiements des fournisseurs par voie électronique au format de paiement ISO 20022 de l'Espace unique de paiement en euros (SEPA), vous devez définir les prérequis pour l'activation des paiements SEPA.  

Les procédures suivantes sont consacrées à l'activation d'un paiement SEPA et à la configuration de comptes bancaires fournisseur.  

## <a name="to-enable-countriesregions-for-sepa"></a>Pour activer des pays/régions pour SEPA  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Pays/Régions**, puis sélectionnez le lien correspondant.  
2.  Choisissez l'action **Modifier la liste**.  
3.  Activez la case à cocher **SEPA autorisé** pour chaque pays ou région que vous souhaitez activer pour SEPA.  
4.  Cliquez sur le bouton **OK**.  

## <a name="to-enable-bank-accounts-for-sepa"></a>Pour activer des comptes bancaires pour SEPA  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez le compte bancaire que vous souhaitez activer pour SEPA, puis choisissez l'action **Modifier**.  
3.  Dans le raccourci **Général**, dans le champ **Pays/Région**, sélectionnez le code adéquat.  

    > [!NOTE]  
    >  Le code pays/région spécifié doit être activé pour SEPA, comme décrit dans la procédure précédente.  

4.  Entrez une valeur dans le champ **Solde minimum**.  
5.  Dans le raccourci **Transfert**, dans le champs **Code SWIFT**, entrez un code.  
6.  Cliquez sur le bouton **OK**.  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a>Pour configurer des comptes bancaires fournisseur pour SEPA  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Fournisseurs**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez le fournisseur concerné, puis choisissez l'action **Comptes bancaires**.  
3.  Sélectionnez le compte bancaire fournisseur à paramétrer pour SEPA, puis choisissez **Modifier**.  
4.  Dans le raccourci **Transfert**, dans les champs **IBAN** et **Code SWIFT**, entrez le code international d'identification bancaire ou la banque auprès de laquelle le fournisseur a son compte.  
5.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements SEPA](sepa-payments.md)   
 [Classer les paiements SEPA](how-to-file-sepa-payments.md)   
 [Classer les paiements SEPA hors Euro](how-to-file-non-euro-sepa-payments.md)   
 [Configurer les protocoles d'exportation](how-to-set-up-export-protocols.md)
