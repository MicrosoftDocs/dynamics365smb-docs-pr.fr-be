---
title: Effectuer des paiements SEPA
description: "Dans Business Central, vous pouvez utiliser les virements SEPA pour effectuer des paiements SEPA auprès de la banque."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: b645ebee368c9b43961d9fec65e0e82956d10e9c
ms.contentlocale: fr-be
ms.lasthandoff: 11/26/2018

---
# <a name="file-sepa-payments"></a>Effectuer des paiements SEPA
Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez utiliser les virements SEPA pour effectuer des paiements SEPA auprès de la banque.  

SEPA unifie les modes de paiement dans les pays/régions européens participants, ce qui rend les paiements internationaux aussi faciles à traiter que les paiements nationaux. Les citoyens et sociétés européens peuvent effectuer et recevoir des règlements en euros, à l'intérieur ou l'extérieur des frontières nationales, avec les mêmes conditions, droits, et obligations de base, quel que soit leur emplacement.  

Avant de pouvoir effectuer un paiement SEPA, vous devez effectuer les tâches d'administration suivantes :  

- Paramétrez un nouveau protocole d'exportation. Pour plus d'informations, voir Protocole d'exportation.  
- Dans la table **Pays/région**, sélectionnez le champ **SEPA autorisé** pour chaque pays appartenant à la zone AEE.  
- Vérifiez que le champ **Devise euro** dans la table **Paramètres comptabilité** correspond à la devise dans les lignes paiement.  
- Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient l'IBAN et le code SWIFT.  

## <a name="to-file-a-sepa-payment"></a>Pour effectuer un paiement SEPA  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Effectuer des paiements SEPA**, puis sélectionnez le lien connexe.  
2.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA.|  
    |**Feuille**|Spécifiez la feuille comptabilité pour l'état de paiement SEPA.|  
    |**Valider les lignes feuille comptabilité**|Spécifiez si vous souhaitez transférer les lignes paiement vers la comptabilité.|  
    |**Inclure axes**|Saisissez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA. L'option n'est disponible que si le champ **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques** est sélectionné.|  
    |**Date d'exécution**|Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date comptabilisation sur les lignes paiement.|  
    |**Emplacement**|Entrez le nom du fichier, y compris le lecteur et le dossier, dans lequel vous souhaitez imprimer l'état.|  

3.  Choisissez le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paramétrer les protocoles d'exportation](how-to-set-up-export-protocols.md)   
 [Effectuer des paiements SEPA hors euro](how-to-file-non-euro-sepa-payments.md)   
 [Activer les règlements SEPA](how-to-activate-sepa-payments.md)

