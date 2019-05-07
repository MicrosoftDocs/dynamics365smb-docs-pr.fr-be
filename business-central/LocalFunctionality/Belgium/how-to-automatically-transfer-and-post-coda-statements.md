---
title: Comment transférer et valider automatiquement les relevés CODA
description: Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière.
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
ms.openlocfilehash: d249493a9278d462741015cf66c1f3536aa566ba
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2019
ms.locfileid: "912822"
---
# <a name="automatically-transfer-and-post-coda-statements"></a>Transférer et publier automatiquement des relevés CODA
Après avoir appliqué et traité toutes les lignes de relevés CODA, vous pouvez transférer les lignes de relevés CODA vers une feuille financière.  

Après avoir transféré les lignes relevé, vous pouvez valider les lignes vers une feuille comptabilité correspondante. S'il n'existe aucune feuille comptabilité, vous ne pouvez pas transférer les lignes. Vous pouvez créer une feuille pour traiter les relevés CODA. Pour plus d'informations, voir [Créer des feuilles financières](how-to-create-financial-journals.md).  

Vous pouvez aussi transférer et valider manuellement les relevés CODA. Pour plus d'informations, voir [Transférer et publier manuellement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).  

## <a name="to-automatically-transfer-statement-lines"></a>Pour transférer automatiquement les lignes relevé  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.  
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
