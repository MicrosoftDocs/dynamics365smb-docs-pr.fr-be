---
title: 'Transférer et publier automatiquement des relevés CODA [BE]'
description: 'Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.form: 2000040
ms.date: 12/06/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="automatically-transfer-and-post-coda-statements-in-the-belgian-version"></a>Transférer et publier automatiquement des relevés CODA dans la version belge

Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière.  

Après avoir transféré les lignes relevé, vous pouvez valider les lignes vers une feuille comptabilité correspondante. S'il n'existe aucune feuille comptabilité, vous ne pouvez pas transférer les lignes. Vous pouvez créer une feuille pour traiter les relevés CODA. Pour plus d'informations, voir [Créer des feuilles financières](how-to-create-financial-journals.md).  

Vous pouvez aussi transférer et valider manuellement les relevés CODA. Pour plus d'informations, voir [Transférer et publier manuellement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).  

## <a name="to-automatically-transfer-statement-lines"></a>Pour transférer automatiquement les lignes relevé

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Comptes bancaires**, puis choisissez le lien associé.  
2.  Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.  
3.  Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.  
4.  Choisissez l'action **Transférer à FS**.  
5.  Cliquez sur le bouton **Oui**.  

Le traitement par lots transfère à présent les lignes relevé CODA à la feuille financière.  

Après avoir transféré les lignes relevé vers la feuille, vous pouvez valider les lignes relevé vers la feuille financière correspondante.  

## <a name="see-also"></a>Voir aussi
 [Relevés bancaires CODA](coda-bank-statements.md)   
 [Importer les relevés CODA](how-to-import-coda-statements.md)   
 [Lettrer les relevés CODA](how-to-apply-coda-statements.md)   
 [Créer des feuilles financières](how-to-create-financial-journals.md)   
 [Transférer et publier manuellement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
