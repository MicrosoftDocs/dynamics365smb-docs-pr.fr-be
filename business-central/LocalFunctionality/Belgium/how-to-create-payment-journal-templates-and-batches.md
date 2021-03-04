---
title: Création de modèles et de lots de feuilles paiement
description: Dans la version belge de Business Central, les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à celle des autres types de feuille.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 790c226770f7d67cc24aed97ab0491a98f8d4539
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749727"
---
# <a name="create-payment-journal-templates-and-batches"></a>Créer des modèles et des lots de feuilles paiement
Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à celle des autres types de feuille. Toutefois, la feuille paiement contient des champs qui sont propres au traitement des paiements. Avant de commencer à générer des suggestions de paiement, vous devez paramétrer un modèle feuille paiement et une feuille paiement.  

Si vous affectez un compte bancaire au modèle feuille paiement, le compte bancaire est inséré sur toutes les feuilles paiement et lignes feuille paiement qui sont créées à l'aide de ce modèle. En spécifiant un compte bancaire pour le modèle feuille, vous pouvez réduire le temps nécessaire pour vérifier les suggestions de paiement.  

## <a name="to-create-a-payment-journal-template"></a>Pour créer un modèle feuille paiement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Modèles feuille paiement**, puis sélectionnez le lien associé.  
2.  Sélectionnez l'action **Nouveau**.  
3.  Dans la page **Modèles feuille paiement EB**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom**|Entrez le nom unique du modèle feuille paiement que vous créez.|  
    |**Description**|Entrez une description du modèle feuille paiement.|  
    |**Compte bancaire**|Sélectionnez le compte bancaire qui est utilisé pour créer une suggestion de paiement.|  
    |**Code motif**|Sélectionnez le code motif qui est utilisé sur toutes les feuilles et lignes feuille créées à l'aide du modèle feuille. Si vous souhaitez utiliser un code motif différent sur une ligne feuille, vous pouvez le modifier manuellement.|  
    |**Code source**|Sélectionnez le code source qui est utilisé sur toutes les feuilles et lignes feuille créées à l'aide du modèle feuille.|  

4.  Choisissez le bouton **OK**.  

## <a name="to-add-payment-journal-batches-to-the-journal-template"></a>Pour ajouter des feuilles paiement au modèle feuille  

1.  Dans la page **Modèles feuille paiement**, choisissez l'action **Feuilles**.  
2.  Dans la page **Feuilles paiement**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez un nom de modèle feuille pour la feuille paiement.|  
    |**Nom**|Entrez un nom unique pour la feuille.<br /><br /> **REMARQUE :** pour que le nom feuille soit mis à jour numériquement, ajoutez un nombre au nom feuille. Par exemple, le nom FEUILLE1 augmente d'un numéro à chaque validation, vous aurez donc FEUILLE2, FEUILLE3, etc.|  
    |**Description**|Entrez une description pour la feuille.|  
    |**Code motif**|Spécifie le code motif qui est associé à cette feuille.|  
    |**Statut**|Spécifie le statut de la feuille.|  

3.  Choisissez le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
 [Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]