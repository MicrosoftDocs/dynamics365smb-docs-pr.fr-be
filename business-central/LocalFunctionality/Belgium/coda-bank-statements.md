---
title: Relevés bancaires CODA
description: Le Coded Statement of Account (CODA) est une norme bancaire nationale conçue par l'Association belge des Banques et des Sociétés de Bourse qui vous permet de traitement automatiquement des relevés bancaires électroniques.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 86b2be248c852482ec87e336ddd7ce9249926197
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771493"
---
# <a name="coda-bank-statements"></a>Relevés bancaires CODA
Le Coded Statement of Account (CODA) est une norme bancaire nationale conçue par l'Association belge des Banques et des Sociétés de Bourse qui vous permet de traitement automatiquement des relevés bancaires électroniques.  

Chaque type de transaction d'un relevé CODA se voit attribuer un code unique. [!INCLUDE[prod_short](../../includes/prod_short.md)] utilise ce code pour interpréter les transactions et les lettrer aux écritures comptables correspondantes.  

## <a name="applying-statement-lines"></a>Lettrage des lignes relevé  
Lorsque vous avez importé un relevé CODA, vous pouvez lettrer les lignes relevé à des écritures comptables existantes selon les informations reprises dans la table **Encodage CODA**.  

Si l'encodage CODA de la ligne relevé est introuvable, [!INCLUDE[prod_short](../../includes/prod_short.md)] interrompra le traitement et poursuivra avec la ligne relevé suivante. Si vous sélectionnez le champ **Validation par défaut**, la ligne relevé sera utilisée comme validation par défaut.  

Si l'encodage CODA de la ligne relevé est trouvé, les lignes relevé seront associées aux types de comptes et aux numéros de comptes correspondants suivants :  

- Comptes généraux : si le type de compte est un compte général, la ligne relevé est validée sur le compte général correspondant.  

- Client ou fournisseur : si le type de compte est client ou fournisseur, une écriture comptable client ou fournisseur correspondante est trouvée selon les critères suivants :  

    - Si une écriture comptable est trouvée avec le format standard, elle sera associée à la ligne relevé et le statut lettrage sera défini sur **Lettrée**. Si l'écriture comptable n'est pas au format standard, le numéro de compte bancaire du client ou du fournisseur est utilisé pour retrouver le client ou le fournisseur.  

    - Si aucune écriture comptable avec un montant restant correspondant n'est trouvée, le compte client ou fournisseur est utilisé et le statut lettrage sera défini sur **Lettrée en partie**.  

    - Si le numéro de compte bancaire est utilisé pour trouver le client ou le fournisseur, une écriture comptable correspondant est trouvée en fonction du montant de la ligne relevé. Si le montant est trouvé, la ligne relevé est associée à l'écriture comptable correspondante et le statut lettrage sera défini sur **Lettrée**.  

    - Si le numéro de compte bancaire ne peut pas être utilisé pour trouver le client ou le fournisseur, [!INCLUDE[prod_short](../../includes/prod_short.md)] interrompra le traitement de la ligne actuelle ou utilisera la ligne comme validation par défaut, avant de poursuivre avec la ligne relevé suivante.  

Vous pouvez exécuter le traitement autant de fois que vous le souhaitez. Seules les lignes relevé dont le statut lettrage est vide seront lettrées.  

Lorsque vous avez lettré toutes les lignes relevé à un compte général ou à une écriture comptable client ou fournisseur correspondante, vous pouvez valider les lignes relevé CODA. Pour plus d'informations, voir [Transférer et publier automatiquement des relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).  

## <a name="see-also"></a>Voir aussi  
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Configurer des comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md)   
 [Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Importer des relevés CODA](how-to-import-coda-statements.md)   
 [Lettrer des relevés CODA](how-to-apply-coda-statements.md)   
 [Créer des feuilles financières](how-to-create-financial-journals.md)   
 [Transférer et publier automatiquement des relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md)   
 [Transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]