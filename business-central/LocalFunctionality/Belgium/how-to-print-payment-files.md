---
title: Comment imprimer les fichiers paiement
description: "Après avoir imprimé un rapport test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 7fb0ddd7f635f20d61163b0bfae950c9aa065230
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="print-payment-files"></a>Imprimer des fichiers de paiement
Après avoir imprimé un rapport test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement.  

Un fichier paiement contient des paiements nationaux, internationaux, SEPA ou SEPA non libellés en Euro. Le fichier peut être envoyé à une banque sur disquette, par un modem ou via Isabel (Interbanks Standards Association Belgium). Vous ne pouvez créer qu'un fichier par date de validation et par code devise. Lorsque vous exportez les paiements dans un fichier, une note d'accompagnement est imprimée et peut aussi être envoyée à la banque.  

Dans la feuille paiement, le champ **Statut** des lignes exportées sera défini sur **Validé**.  

## <a name="to-print-a-payment-file"></a>Pour imprimer un fichier paiement  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille paiement**, puis sélectionnez le lien correspondant.  
2.  Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom de la feuille**|Spécifiez le nom de la feuille paiement.|  
    |**Compte bancaire**|Spécifiez le compte bancaire de la feuille paiement.|  
    |**Protocole d'exportation**|Spécifiez le code du protocole d'exportation de la ligne feuille paiement. Exportez des protocoles qui contrôlent le fichier de paiement qui sera généré dans la feuille paiement.<br /><br /> Vous pouvez avoir plusieurs formats d'exportation différents dans un seul lot, comme les formats national, international, SEPA, ou un ensemble des trois. Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un format ou protocole d'exportation. **Note :**  En définissant le protocole d'exportation, vous définissez également le type de validation qui sera effectuée dans la feuille paiement.|  

3.  Choisissez l'action **Vérifier les lignes de paiement**.

    La fenêtre **Exporter les journaux d'erreur de chèque** affiche les erreurs éventuelles qui pourraient exister. S'il y a des erreurs, vous devez les corriger avant de continuer.

4. S'il n'y a pas d'erreur, choisissez l'action **Exporter les lignes de paiement**.  

    L'état que vous avez spécifié dans le champ **ID impression test** des **Modèles FS paiements EB** s'ouvre.  

5.  Cliquez sur le bouton **Imprimer**.  

## <a name="see-also"></a>Voir aussi  
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
 [Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des propositions de paiement](how-to-generate-payment-suggestions.md)   
 [Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md)

