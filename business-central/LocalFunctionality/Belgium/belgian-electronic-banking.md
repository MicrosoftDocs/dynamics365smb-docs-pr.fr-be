---
title: Banque électronique belge
description: La banque électronique vous permet d'échanger des données par voie électronique avec des institutions financières belges. Cela garantit une plus grande vitesse de traitement et permet d'éviter les erreurs.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/25/2021
ms.author: edupont
ms.openlocfilehash: 6918790addeb3a3d315e41d537a6d1eefb66f432
ms.sourcegitcommit: e562b45fda20ff88230e086caa6587913eddae26
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/30/2021
ms.locfileid: "6322028"
---
# <a name="belgian-electronic-banking"></a>Banque électronique belge

Dans la version belge de [!INCLUDE [prod_short](../../includes/prod_short.md)], vous pouvez échanger des données avec des institutions financières belges par voie électronique. Cela permet d'accélérer le temps de traitement et d'éviter les erreurs causées par la saisie ou le traitement manuel des données.  

Vous pouvez utiliser la banque électronique pour effectuer les actions suivantes :  

- Envoyer des paiements électroniques.  
- Traiter des relevés bancaires avec CODA.  
- Traiter des domiciliations européennes.  

## <a name="setup"></a>Configuration

Avant de pouvoir traiter des relevés et des paiements électroniques, vous devez configurer la banque électronique sur la page **Paramétrage des opérations bancaires électroniques** comme décrit dans le tableau suivant.

|Champ|Description |
|-----|------------|
|**Totaliser lignes feuille compta.**| Sélectionnez pour indiquer si vous souhaitez regrouper les lignes feuille paiement pour chaque fournisseur.  |
|**Limiter les textes du message de paiement** |Sélectionnez pour indiquer si vous souhaitez tronquer les longs messages de paiement. Les messages seront tronqués si supérieurs à 106 caractères pour les paiements nationaux et inférieurs à 140 caractères pour les paiements internationaux. |

Pour plus d'informations sur l'impact des deux champs sur le mode de transfert des lignes feuille paiement vers la feuille comptabilité, voir [Résumé des lignes règlement et des lignes feuille comptabilité](summarizing-payment-lines-and-general-journal-lines.md).  

## <a name="see-also"></a>Voir aussi

[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)  
[Paiements électroniques belges](belgian-electronic-payments.md)  
[Relevés bancaires CODA](coda-bank-statements.md)  
[Domiciliation européenne](direct-debit-using-domiciliation.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]