---
title: "Comment lettrer les relevés CODA"
description: "Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la fenêtre **Fiche compte bancaire**. Le statut du lettrage sur chaque ligne est vide car les montants du relevé n'ont pas été appliqués aux écritures comptables ouvertes."
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
ms.openlocfilehash: 01d764627f26ea40ec6d6a6b102cb6e367a0cb76
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="apply-coda-statements"></a>Lettrer des relevés CODA
Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la fenêtre **Fiche compte bancaire**. Le statut lettrage de chaque ligne sera vide, car les montants du relevé n'ont pas été lettrés à des écritures comptables en attente.  

Les montants du relevé peuvent être lettrés à des écritures comptables en attente des manières suivantes :  

-   Lettrage manuel des lignes relevé CODA.  
-   Lettrage automatique des montants du relevé CODA aux écritures comptables et comptes adéquats. Le traitement automatique des lignes relevé CODA est recommandé.  

## <a name="to-manually-apply-the-coda-statement-lines"></a>Pour lettrer manuellement les lignes relevé CODA  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.  
3.  Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.  
4.  Dans le raccourci **Lignes relevé CODA**, pour chaque ligne relevé, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**N° compte**|Entrez le numéro du compte général, la banque, le client, le fournisseur ou l'immobilisation auquel la ligne relevé compte bancaire est liée.|  
    |**Description**|[!INCLUDE[d365fin](../../includes/d365fin_md.md)] récupère automatiquement la description à partir du fichier CODA importé, mais vous pouvez modifier le contenu de ce champ.|  

5.  Cliquez sur le bouton **OK**.  

## <a name="to-automatically-apply-the-coda-statement-lines"></a>Pour lettrer automatiquement les lignes relevé CODA  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.  
3.  Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.  
4.  Choisissez l'action **Valider lignes relevé CODA**.  
5.  Remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Validation par défaut**|Définissez si vous souhaitez que le traitement par lots valide les montants du relevé qui ne peuvent pas être liés à des écritures comptables existantes. Pour plus d'informations, voir Encodage CODA.|  
    |**Imprimer liste**|Sélectionnez l'option d'impression d'une liste des montants du relevé qui ne peuvent pas être liés automatiquement.|  

6.  Cliquez sur le bouton **OK**.  

    Lorsque vous démarrez le traitement par lots, les montants relevés sont appliqués aux écritures comptables existantes selon les codes transaction. Pour plus d'informations, reportez vous à [Configuration de comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md).  

## <a name="see-also"></a>Voir aussi  
 [Relevés bancaires CODA](coda-bank-statements.md)   
 [Configurer des comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md)   
 [Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Importer des relevés CODA](how-to-import-coda-statements.md)   
 [Créer des feuilles financières](how-to-create-financial-journals.md)   
 [Transférer et publier automatiquement des relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md)   
 [Transférer et publier manuellement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md)

