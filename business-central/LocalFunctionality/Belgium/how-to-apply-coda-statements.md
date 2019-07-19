---
title: Lettrage des relevés CODA
description: Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la page Fiche compte bancaire. Le statut de lettrage sur chaque ligne est vide, car les montants du relevé n'ont pas été lettrés aux écritures comptables ouvertes.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 780fa9f5cbe2d9c0a79f8f61d9a7aafeb211b733
ms.sourcegitcommit: 5b6dd8d881c0eb65ece6936a94dfda3185574335
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/28/2019
ms.locfileid: "1710949"
---
# <a name="apply-coda-statements"></a>Lettrer les relevés CODA
Une fois qu'un relevé CODA a été importé, les lignes relevé sont accessibles à partir de la page **Fiche compte bancaire**. Le statut de lettrage sur chaque ligne est vide, car les montants du relevé n'ont pas été lettrés aux écritures comptables ouvertes.  

Les montants du relevé peuvent être lettrés aux écritures comptables ouvertes comme suit :  

-   En lettrant manuellement les lignes relevé CODA.  
-   En lettrant automatiquement les montants du relevé CODA aux écritures comptables et aux comptes appropriés. Le traitement automatique des lignes relevé CODA est recommandé.  

## <a name="to-manually-apply-the-coda-statement-lines"></a>Pour lettrer manuellement les lignes relevé CODA  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien connexe.  
2.  Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.  
3.  Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.  
4.  Pour chaque ligne relevé, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**N° compte**|Entrez le numéro du compte général, de la banque, du client, du fournisseur ou de l'immobilisation, auquel la ligne relevé du compte bancaire est associée.|  
    |**Description**|[!INCLUDE[d365fin](../../includes/d365fin_md.md)] récupère automatiquement la description à partir du fichier CODA importé, mais vous pouvez modifier le contenu de ce champ.|  

5.  Choisissez le bouton **OK**.  

## <a name="to-automatically-apply-the-coda-statement-lines"></a>Pour lettrer automatiquement les lignes relevé CODA  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien connexe.  
2.  Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.  
3.  Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.  
4.  Choisissez l'action **Traiter les lignes relevé CODA**.  
5.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Comptabilisation par défaut**|Sélectionnez ce champ si vous souhaitez que le traitement par lots valide les montants du relevé qui ne peuvent pas être associés aux écritures comptables existantes.|  
    |**Imprimer liste**|Sélectionnez ce champ pour imprimer la liste des montants du relevé qui ne peuvent pas être associés automatiquement.|  

6.  Choisissez le bouton **OK**.  

    Lorsque vous démarrez le traitement par lots, les montants du relevé sont lettrés aux écritures comptables existantes en fonction des codes transaction. Pour plus d'informations, voir [Paramétrer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md).

## <a name="see-also"></a>Voir aussi  
 [Relevés bancaires CODA](coda-bank-statements.md)   
 [Paramétrer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md)   
 [Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Importer les relevés CODA](how-to-import-coda-statements.md)   
 [Créer des journaux financiers](how-to-create-financial-journals.md)   
 [Transférer et valider automatiquement les relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md)   
 [Transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md)
