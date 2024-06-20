---
title: 'Paramétrer des opérations bancaires électroniques [BE]'
description: 'Avec les opérations bancaires électroniques, vous pouvez effectuer des paiements électroniques à des fournisseurs et clients nationaux, internationaux, SEPA et SEPA non euro.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.form: 11308
ms.date: 11/24/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="set-up-electronic-banking-in-the-belgian-version"></a>Paramétrer des opérations bancaires électroniques dans la version belge

Avec les opérations bancaires électroniques, vous pouvez effectuer des paiements électroniques à des fournisseurs et clients nationaux, internationaux, SEPA et SEPA non euro. Avant de pouvoir les opérations bancaires électroniques, vous devez définir les informations suivantes :  

- Paramétrage des opérations bancaires électroniques.  
- Codes IBLC/BLWI - Pour plus d'informations, voir [Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md).  

## <a name="to-set-up-electronic-banking"></a>Pour paramétrer les opérations bancaires électroniques

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Paramétrage des opérations bancaires électroniques**, puis choisissez le lien associé.  
2.  Dans la page **Paramétrage des opérations bancaires électroniques**, renseignez les champs comme indiqué dans le tableau suivant.   

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Totaliser lignes feuille compta.**|Sélectionnez pour indiquer si vous souhaitez regrouper les lignes feuille paiement pour chaque fournisseur.|  
    |**Limiter les textes du message de paiement**|Sélectionnez pour indiquer si vous souhaitez tronquer les longs messages de paiement. Les messages sont tronqués s'ils sont supérieurs à 106 caractères pour les paiements nationaux et inférieurs à 140 caractères pour les paiements internationaux.|  
 
3.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi
 [Site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323)   
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des suggestions de règlement](how-to-generate-payment-suggestions.md)   
 [Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)     
 [Imprimer les fichiers de paiement](how-to-print-payment-files.md)    
 [Résumé des lignes règlement et des lignes feuille comptabilité](summarizing-payment-lines-and-general-journal-lines.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
