---
title: Test des paiements électroniques
description: Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 9edf27caaea179b1a8fb62dcc34e2e7fe097a157
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/08/2019
ms.locfileid: "826438"
---
# <a name="test-electronic-payments"></a>Tester les paiements électroniques
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'eventuelles erreurs avant de les valider.  

Certaines des informations validées sont les suivantes :  

- Les numéros des comptes bancaires sont valides.  
- Les lignes paiement positives sont présentes.  
- Si les paiements nationaux et internationaux sont effectués à partir d'un seul compte bancaire.  
- Si un seul compte bancaire peut être utilisé pour Isabel.  
- Si les lignes paiement sont en euro pour SEPA.  
- Si une souche de numéros a été définie pour SEPA.  

Vous pouvez afficher les erreurs sur la page **Exporter/Vérifier les journaux des erreurs**.  

> [!IMPORTANT]  
>  Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.  

## <a name="to-test-payment-journal-lines"></a>Pour tester les lignes feuille paiement  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles paiement**, puis sélectionnez le lien connexe.  
2.  Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.  
3.  Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.  
4.  Entrez les informations sur les lignes feuille paiement, puis choisissez l'action **Vérifier lignes paiement** pour valider les lignes feuille paiement. La validation réalisée sur les lignes feuille dépend du type de vérification spécifié dans la page **Protocoles d'exportation**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des suggestions de règlement](how-to-generate-payment-suggestions.md)   
 [Imprimer les fichiers de paiement](how-to-print-payment-files.md)
