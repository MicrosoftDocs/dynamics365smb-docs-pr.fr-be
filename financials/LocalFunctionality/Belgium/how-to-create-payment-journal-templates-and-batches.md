---
title: "Procédure : Créer des modèles et des lots de feuille paiement"
description: "Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à la structure des autres types de feuille."
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
ms.openlocfilehash: 02a1b3a9226abdd1278dab5fb43566243cd85172
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="create-payment-journal-templates-and-batches"></a>Créer des modèles et des lots de feuille paiement
Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est semblable à celle des autres types de feuilles. Toutefois, la feuille paiement contient des champs spécifiques au traitement des paiements. Avant de pouvoir commencer à générer des propositions de paiement, vous devez configurer un modèle feuille paiement et un nom feuille paiement.  

Si vous attribuez un compte bancaire au modèle feuille paiement, le compte bancaire sera inséré dans tous les noms feuille paiement et toutes les lignes feuille paiement créés à l'aide de ce modèle. En indiquant un compte bancaire pour le modèle feuille, vous pouvez réduire le délai de vérification des propositions de paiement.  

## <a name="to-create-a-payment-journal-template"></a>Pour créer un modèle feuille paiement  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Modèles FS paiements**, puis sélectionnez le lien correspondant.  
2.  Choisissez l'action **Nouveau**.  
3.  Dans la fenêtre **Modèles FS paiements EB**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom**|Entrez le nom unique du modèle feuille paiement que vous créez.|  
    |**Description**|Entrez une description du modèle feuille paiement.|  
    |**Compte bancaire**|Sélectionnez le compte bancaire qui sera utilisé lorsque vous créerez une proposition de paiement.|  
    |**Code motif**|Sélectionnez le code motif qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille. Si vous souhaitez utiliser un autre code motif sur une ligne feuille, vous pouvez le modifier manuellement.|  
    |**Code journal**|Sélectionnez le code source qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille.|  

4.  Cliquez sur le bouton **OK**.  

## <a name="to-add-payment-journal-batches-to-the-journal-template"></a>Pour ajouter des noms feuille paiement au modèle feuille  

1.  Dans la fenêtre **Modèles FS paiements**, choisissez l'action **Noms feuilles**.  
2.  Dans la fenêtre **Nom FS paiements**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez un nom de modèle feuille pour le nom feuille paiement.|  
    |**Nom**|Entrez un nom unique pour le nom feuille.<br /><br /> **NOTE :** pour que le nom feuille se mette à jour de façon numérique, ajoutez un numéro dans le nom feuille. Par exemple, à chaque validation, le nom KBC1 sera mis à jour en KBC2, KBC3, etc.|  
    |**Description**|Entrez une description pour le nom feuille.|  
    |**Code motif**|Spécifie le code motif lié à ce nom feuille.|  
    |**Statut**|Indique le statut du lot.|  

3.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
 [Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)

