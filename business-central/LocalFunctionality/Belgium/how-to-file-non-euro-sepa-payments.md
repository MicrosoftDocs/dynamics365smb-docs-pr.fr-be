---
title: Effectuer des paiements SEPA hors euro
description: Dans la version belge de Business Central, vous pouvez effectuer des paiements SEPA hors euros auprès de la banque. Cela est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas SEPA et pour les devises autres que l'euro.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: ef7a52a51b52b8fe562d33766794ca110e5309a5
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237789"
---
# <a name="file-non-euro-sepa-payments"></a>Effectuer des paiements SEPA hors euro
Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez effectuer des paiements SEPA hors euro auprès de la banque. Cela est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas SEPA et pour les devises autres que l'euro.  

Avant de pouvoir effectuer un paiement SEPA hors euro, vous devez effectuer les tâches d'administration suivantes :  

- Paramétrez un nouveau protocole d'exportation pour un paiement SEPA hors euro. Pour plus d'informations, voir Protocole d'exportation.  
- Dans la table **Pays/région**, désactivez le champ **SEPA autorisé** pour chaque pays appartenant à la zone AEE.  
- Vérifiez que le champ **Devise euro** dans la table **Paramètres comptabilité** n'est pas en euro.  
- Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient l'IBAN et le code SWIFT.  

## <a name="to-file-a-non-euro-sepa-payment"></a>Pour effectuer un paiement SEPA hors euro  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Effectuer des paiements SEPA hors euro**, puis sélectionnez le lien connexe.  
2.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA hors euro.|  
    |**Feuille**|Spécifiez la feuille comptabilité pour l'état de paiement SEPA hors euro.|  
    |**Valider les lignes feuille comptabilité**|Spécifiez si vous souhaitez transférer les lignes paiement vers la comptabilité.|  
    |**Inclure axes**|Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA hors euro. L'option n'est disponible que si le champ **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques** est sélectionné.|  
    |**Date d'exécution**|Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date comptabilisation sur les lignes paiement.|  
    |**Emplacement**|Entrez le nom du fichier, y compris le lecteur et le dossier, dans lequel vous souhaitez imprimer l'état.|  

3.  Choisissez le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Remplir les paiements SEPA](how-to-file-sepa-payments.md)   
 [Activer les règlements SEPA](how-to-activate-sepa-payments.md)   
 [Paiements SEPA](sepa-payments.md)
