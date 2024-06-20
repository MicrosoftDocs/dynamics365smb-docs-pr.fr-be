---
title: 'Rendre les modèles feuille obligatoires [BE]'
description: Découvrez comment rendre l'utilisation des modèles feuille obligatoire dans la version belge.
author: altotovi
ms.topic: conceptual
ms.search.keywords: 118
ms.date: 05/24/2022
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="make-journal-templates-mandatory-in-the-belgian-version"></a>Rendre les modèles feuille obligatoires dans la version belge

Vous pouvez utiliser des feuilles pour valider des documents achat et vente et créer d'autres écritures comptables. Les modèles feuille peuvent alors vous aider à structurer différents types d'écritures. Dans la version belge de [!INCLUDE [prod_short](../../includes/prod_short.md)],vous devez spécifier si des modèles feuille sont requis dans la société actuelle.  

## <a name="to-make-journal-templates-required-in-a-company"></a>Pour rendre les modèles feuille obligatoires dans une société

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Paramètres comptabilité**, puis choisissez le lien associé.  
2. Dans le raccourci **Général**, sélectionnez le champ **Nom modèle feuille obligatoire**. Ce champ spécifie si les utilisateurs doivent spécifier un modèle feuille lors qu'ils valident des transactions comptables.  

> [!NOTE]  
> Si le champ **Nom modèle feuille obligatoire** n'est pas sélectionné, [!INCLUDE [prod_short](../../includes/prod_short.md)] n'utilisera pas des noms de modèle dans les écritures et documents validés.

## <a name="use-journal-templates-in-sales-and-purchase-documents"></a>Utiliser des modèles feuille dans des documents achat et vente

Si votre organisation décide d'activer le champ **Nom modèle feuille obligatoire**, vous devez configurer les modèles feuille qui seront utilisés par défaut dans les documents achat et vente.

> [!TIP]  
> Avant de valider une transaction, vous pouvez modifier le nom du modèle suggéré dans le champ **Nom modèle feuille**. De cette façon, les transactions se voient assigner un autre numéro de document, comme défini par le modèle.

### <a name="to-use-journal-templates-in-sales-documents"></a>Pour utiliser des modèles feuille dans des documents vente

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Paramètres ventes**, puis choisissez le lien associé.  
2. Sur le raccourci **Modèles feuille**, choisissez les modèles feuille que vous souhaitez utiliser par défaut pour tous les documents vente.  

### <a name="to-use-journal-templates-in-purchase-documents"></a>Pour utiliser des modèles feuille dans des documents achat

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Paramètres achats**, puis choisissez le lien associé.  
2. Sur le raccourci **Modèles feuille**, choisissez les modèles feuille que vous souhaitez utiliser par défaut pour tous les documents achat.  

## <a name="see-also"></a>Voir aussi

[Créer des feuilles financières dans la version belge](how-to-create-financial-journals.md)  
[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
