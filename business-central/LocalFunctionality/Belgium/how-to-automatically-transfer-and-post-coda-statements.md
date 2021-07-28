---
title: Comment transférer et valider automatiquement les relevés CODA [BE]
description: Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/17/2021
ms.author: edupont
ms.openlocfilehash: 370b96acf0ce9fed9f04f6b2cae391980586318b
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 07/08/2021
ms.locfileid: "6437201"
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

Le traitement par lots transfèrera à présent les lignes relevé CODA à la feuille financière.  

Après avoir transféré les lignes relevé vers la feuille, vous pouvez valider les lignes relevé vers la feuille financière correspondante.  

## <a name="see-also"></a>Voir aussi  
 [Relevés bancaires CODA](coda-bank-statements.md)   
 [Importer des relevés CODA](how-to-import-coda-statements.md)   
 [Lettrer des relevés CODA](how-to-apply-coda-statements.md)   
 [Créer des feuilles financières](how-to-create-financial-journals.md)   
 [Transférer et publier manuellement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]