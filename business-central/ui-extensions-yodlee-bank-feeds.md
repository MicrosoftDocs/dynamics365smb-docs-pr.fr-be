---
title: Rapprochement de paiement avec l’extension Envestnet Yodlee Bank Feeds
description: Décrit l’extension Envestnet Yodlee Bank Feeds, qui établit des liaisons avec les comptes bancaires afin que vous puissiez rapidement rapprocher les paiements.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9bdbcc208429bba15e30bc56cc8a4477312c1cdd
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771248"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a>Extension Envestnet Yodlee Bank Feeds

Pour rapprocher rapidement des paiements effectués sur vos comptes bancaires, le service Envestnet Yodlee Bank Feeds vous permet de lier votre compte bancaire système à votre compte bancaire en ligne. Cela signifie que le dernier relevé bancaire est automatiquement ou manuellement entré dans votre feuille rapprochement, garantissant que vous traitez toujours les derniers paiements avec un risque minimal d’erreurs.

Le service Envestnet Yodlee Bank Feeds n’est pris en charge qu’aux États-Unis et au Canada.

> [!NOTE]
> Le service Envestnet Yodlee Bank Feeds est uniquement pris en charge dans la version en ligne de Business Central. Pour utiliser cette fonctionnalité sur site, vous devez obtenir un compte de cobrand d’Envestnet Yodlee.<br /><br />
> Le service Envestnet Yodlee Bank Feeds n’est pris en charge qu’aux États-Unis et au Canada.
> Seules les banques résidant dans ces pays sont prises en charge, même si des banques d’autres pays peuvent apparaître dans la fenêtre de sélection des banques Envestnet Yodlee Bank Feeds dans [!INCLUDE[prod_short](includes/prod_short.md)].

> [!IMPORTANT]
> En raison de la nouvelle directive sur les services de paiement en Europe (PSD2), après le 14 septembre 2019, vous ne pourrez plus importer automatiquement des relevés bancaires de banques du Royaume-Uni vers [!INCLUDE[prod_short](includes/prod_short.md)]. Nous étudions la possibilité de proposer cette fonctionnalité à l’avenir.

Le service Envestnet Yodlee Bank Feeds offre les avantages suivants :

* Supprime les besoins de saisie manuelle.
* Améliore l’efficacité et la précision lors des rapprochements de paiements.
* Prend en charge un grand nombre de banques.
* Permet de bénéficier d’informations à jour relatives aux transactions bancaires au sein de [!INCLUDE[prod_short](includes/prod_short.md)].
* Prend en charge les flux bancaires manuels comme automatiques.
* Permet la sous-traitance des rapprochements de paiement à un comptable en donnant l’accès aux relevés bancaires.

## <a name="available-bank-feeds"></a>Flux bancaires disponibles
Vous pouvez vérifier si une banque est prise en charge en configurant et en vous connectant au service Envestnet Yodlee Bank Feeds. La banque s’affiche sur la liste si elle est prise en charge par Envestnet Yodlee.

Pour plus d’informations, voir [Configurer le service Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).

## <a name="see-also"></a>Voir aussi
[Personnalisation de [!INCLUDE[prod_short](includes/prod_short.md)] à l’aide des extensions ](ui-extensions.md)    
[Lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]