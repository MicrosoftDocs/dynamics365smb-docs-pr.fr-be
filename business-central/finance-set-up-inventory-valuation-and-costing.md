---
title: Configuration de l’évaluation du stock | Microsoft Docs
description: Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 2194a29247b6ec3c2ee87dfbfe6631f433d0514e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783735"
---
# <a name="setting-up-inventory-valuation-and-costing"></a>Configuration de l’évaluation du stock

Pour vous assurer que les coûts ajustés sont enregistrés correctement, vous devez configurer plusieurs champs et pages avant de commencer à effectuer des transactions article. En règle générale, les entreprises choisissent une méthode de calcul des coûts spécifique et l’appliquent aux articles en stock, par exemple, pour les aider à suivre la valeur des articles en stock.  

> [!TIP]
> Pour une introduction aux coûts en [!INCLUDE [prod_short](includes/prod_short.md)], voir [À propos de l’évaluation des coûts de stock](finance-learn-about-costing.md).

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.

|**Pour**|**Voir**|  
|------------|-------------|
|Spécifiez un mode évaluation stock par défaut de l’entreprise pour régir la manière dont son coût entrant est utilisé pour évaluer la valeur du stock et le coût des biens vendus.|[Définir des informations générales relatives aux stocks](inventory-how-setup-general.md)|  
|Spécifiez un mode évaluation des articles individuels s’ils nécessitent un mode évaluation stock différent.|[Enregistrer de nouveaux articles](inventory-how-register-new-items.md)|  
|S’assurer que les coûts sont automatiquement validés dans la comptabilité lorsqu’un mouvement de stock est validé.|Champ **Compta. coûts automatique** sur la page **Paramètres stock**|  
|S’assurer que les coûts prévus sont validés dans la comptabilité afin de visualiser, à partir des comptes généraux en attente, une estimation des montants dus et du coût des articles échangés avant qu’ils ne soient effectivement facturés.|Champ **Compta. coûts prévus** sur la page **Paramètres stock**|  
|Configurer le système afin d’ajuster automatiquement toute modification des coûts chaque fois que vous validez des mouvements de stock.|[Ajuster coûts et prix article](inventory-how-adjust-item-costs.md)|  
|Définir si le coût moyen doit être calculé uniquement par article ou par article pour chaque point de stock et pour chaque variante de l’article.|Champ **Type calcul coût moyen** sur la page **Paramètres stock**|  
|Sélectionnez la période que l’application doit utiliser pour calculer le coût moyen pondéré des articles qui utilisent la méthode évaluation stock Moyen.|Champ **Période coût moyen** sur la page **Paramètres stock**|  
|Définir des périodes inventaire pour contrôler la valeur du stock dans le temps en refusant d’accorder la validation de transactions lorsque les périodes inventaire sont clôturées.|[Utiliser les périodes inventaire](finance-how-to-work-with-inventory-periods.md)|  
|S’assurer que les retours vente sont rapprochés des transactions sortantes afin de préserver la valeur du stock.|Champ **Coût retour identique obligatoire** sur la page **Ventes**|  
|S’assurer que les retours achat sont rapprochés des transactions entrantes afin de préserver la valeur du stock.|Champ **Coût retour identique obligatoire** sur la page **Achats**|
|Configurer les règles d’arrondi à appliquer lors de l’ajustement ou de la proposition des prix article et lors de l’ajustement ou de la proposition des coûts standard.|Page **Mode arrondi**|  

## <a name="see-also"></a>Voir aussi

[Gestion des coûts ajustés](finance-manage-inventory-costs.md)  
[Définir des informations générales relatives aux stocks](inventory-how-setup-general.md)  
[Rapprocher les coûts ajustés avec la comptabilité](finance-how-to-post-inventory-costs-to-the-general-ledger.md)  
[Pratiques de configuration recommandées : mode évaluation stock](setup-best-practices-costing-method.md)  
[Détails de conception : Évaluation stock](design-details-inventory-costing.md)  
[Détails de conception : Modifier le mode évaluation stock pour les articles](design-details-changing-costing-methods.md)  
[Utilisation de Business Central](ui-work-product.md)  
[Finances](finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]