---
title: Test des paiements électroniques
description: Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 1fca14d85e9754b187297c145b6f228d60fb44fb
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379763"
---
# <a name="test-electronic-payments"></a>Tester les paiements électroniques
Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.  

Certaines des informations validées sont les suivantes :  

- Si les numéros des comptes bancaires sont valides.  
- Si les lignes paiement positives sont présentes.  
- Si les paiements nationaux et internationaux sont effectués à partir d'un seul compte bancaire.  
- Si un seul compte bancaire peut être utilisé pour Isabel (Interbanks Standards Association Belgium).  
- Si des lignes de paiement sont en euros pour SEPA (Espace unique de paiement en euros).  
- Si une souche de numéros a été définie pour SEPA.  

Vous pouvez afficher les erreurs sur la page **Exporter/Vérifier les journaux des erreurs**.  

> [!IMPORTANT]  
>  Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.  

## <a name="to-test-payment-journal-lines"></a>Pour tester les lignes feuille paiement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles paiement**, puis sélectionnez le lien associé.  
2.  Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.  
3.  Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.  
4.  Entrez les informations sur les lignes feuille paiement, puis choisissez l'action **Vérifier lignes paiement** pour valider les lignes feuille paiement. La validation réalisée sur les lignes feuille dépend du type de vérification spécifié dans la page **Protocoles d'exportation**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des suggestions de règlement](how-to-generate-payment-suggestions.md)   
 [Imprimer les fichiers de paiement](how-to-print-payment-files.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]