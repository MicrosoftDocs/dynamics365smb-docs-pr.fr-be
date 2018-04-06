---
title: Comment activer les paiements SEPA
description: "Pour envoyer les paiements des fournisseurs par voie électronique au format de paiement ISO 20022 de l'Espace unique de paiement en euros (SEPA), vous devez définir les prérequis pour l'activation des paiements SEPA."
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
ms.openlocfilehash: 3f53a511b47702726d0142d24e9a4fb7159200c9
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

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
4.  Dans le raccourci **Transfert**, dans les champs **N° compte bancaire international** et **Code SWIFT**, entrez le code d'identification bancaire international de la banque où le fournisseur a ouvert le compte.  
5.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements SEPA](sepa-payments.md)   
 [Classer les paiements SEPA](how-to-file-sepa-payments.md)   
 [Classer les paiements SEPA hors Euro](how-to-file-non-euro-sepa-payments.md)   
 [Configurer les protocoles d'exportation](how-to-set-up-export-protocols.md)

