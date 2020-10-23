---
title: Impression des fichiers de paiement
description: Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3910523325ac8ef5d6341b09c4bbe55863b90809
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 10/01/2020
ms.locfileid: "3913985"
---
# <a name="print-payment-files"></a>Imprimer les fichiers de paiement
Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.  

Un fichier de paiement contient les paiements nationaux, internationaux, SEPA ou SEPA hors euro. Ce fichier peut être envoyé à une banque sur disque, par modem ou via le serveur Isabel (Interbanks Standards Association Belgium). Vous ne pouvez créer qu'un seul fichier pour chaque date comptabilisation et chaque code devise. Lorsque vous exportez les paiements dans un fichier, une note associée est imprimée, qui peut également être envoyée à la banque.  

Dans la feuille paiement, le champ **Statut** sur les lignes exportées est défini sur **Validé**.  

## <a name="to-print-a-payment-file"></a>Pour imprimer un fichier de paiement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuille paiement**, puis sélectionnez le lien associé.  
2.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom de la feuille**|Spécifiez le nom de la feuille paiement.|  
    |**Compte bancaire**|Spécifiez le compte bancaire de la feuille paiement.|  
    |**Protocole d'exportation**|Spécifiez le code du protocole d'exportation de la ligne feuille paiement. Les protocoles d'exportation contrôlent le fichier de paiement généré dans la feuille paiement.<br /><br /> Vous pouvez combiner plusieurs formats d'exportation dans un même traitement par lots, par exemple national, international, SEPA ou une combinaison de ceux-ci. Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un seul format d'exportation ou protocole d'exportation. **Remarque :** en définissant le protocole d'exportation, vous définissez également le type de validation qui est exécuté dans la feuille paiement.|  

3.  Choisissez l'action **Vérifier lignes paiement**.

    La page **Exporter/Vérifier les journaux des erreurs** affiche les erreurs éventuelles. S'il existe des erreurs, vous devez les corriger avant de continuer.

4. S'il n'existe aucune erreur, choisissez l'action **Exporter lignes paiement**.  

    L'état que vous avez spécifié dans le champ **ID impression test** de la page **Modèles feuille paiement EB** s'ouvre.  

5.  Cliquez sur le bouton **Imprimer**.  

## <a name="see-also"></a>Voir aussi  
 [Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)   
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
 [Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des suggestions de règlement](how-to-generate-payment-suggestions.md)   
 [Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Gérer les lignes de paiement électronique](how-to-manage-electronic-payment-lines.md)
