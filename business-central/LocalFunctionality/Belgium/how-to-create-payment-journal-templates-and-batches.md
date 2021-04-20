---
title: Création de modèles et de lots de feuilles paiement
description: Dans la version belge de Business Central, les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à celle des autres types de feuille.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1cbfb5a74c54a39ab3ed2bc11b7f4c3eca5964bd
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775008"
---
# <a name="create-payment-journal-templates-and-batches"></a>Créer des modèles et des lots de feuilles paiement
Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à celle des autres types de feuille. Toutefois, la feuille paiement contient des champs qui sont propres au traitement des paiements. Avant de commencer à générer des suggestions de paiement, vous devez paramétrer un modèle feuille paiement et une feuille paiement.  

Si vous affectez un compte bancaire au modèle feuille paiement, le compte bancaire est inséré sur toutes les feuilles paiement et lignes feuille paiement qui sont créées à l'aide de ce modèle. En spécifiant un compte bancaire pour le modèle feuille, vous pouvez réduire le temps nécessaire pour vérifier les suggestions de paiement.  

## <a name="to-create-a-payment-journal-template"></a>Pour créer un modèle feuille paiement  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Modèles feuille paiement**, puis sélectionnez le lien associé.  
2. Sélectionnez l'action **Nouveau**.  
3. Sur la page **Modèles feuille paiement EB**, renseignez les champs.  

    [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

    > [!IMPORTANT]
    > Si les champs **ID page** et **ID impression test** ne sont pas affichés, vous devez les ajouter via la personnalisation. Vous devez compléter les champs pour pouvoir continuer. Pour plus d'informations, voir [Personnaliser votre espace de travail](../../ui-personalization-user.md).
4. Répétez l'étape 2 pour chaque modèle supplémentaire.

5. Cliquez sur le bouton **OK**.  

## <a name="to-add-payment-journal-batches-to-the-journal-template"></a>Pour ajouter des feuilles paiement au modèle feuille  

1.  Dans la page **Modèles feuille paiement**, choisissez l'action **Feuilles**.  
2.  Dans la page **Feuilles paiement**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom**|Entrez un nom unique pour la feuille.<br /><br /> **REMARQUE :** pour que le nom feuille soit mis à jour numériquement, ajoutez un nombre au nom feuille. Par exemple, le nom FEUILLE1 augmente d'un numéro à chaque validation, vous aurez donc FEUILLE2, FEUILLE3, etc.|  
    |**Description**|Entrez une description pour la feuille.|  
    |**Code motif**|Spécifiez éventuellement le code motif qui est associé à cette feuille.|  
    |**Statut**|Spécifie le statut de la feuille.|

Vous pouvez ensuite tester la configuration. Pour plus d'informations, voir [Tester les paiements électroniques](how-to-test-electronic-payments.md).  

3.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
 [Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]