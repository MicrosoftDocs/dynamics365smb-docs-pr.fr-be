---
title: Gestion nomenclature d’assemblage
description: Découvrez comment fournir des produits aux clients en combinant des composants dans des processus simples sans utiliser de fonctions de fabrication.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 04/26/2024
ms.custom: bap-template
ms.search.keywords: 'kit, kitting'
ms.search.form: '900, 901, 902, 903, 904, 907, 910, 916, 920, 921, 922, 923, 940, 941, 942, 930, 931, 932, 914, 915, 905'
ms.service: dynamics-365-business-central
---
# <a name="assembly-management"></a>Gestion nomenclature d’assemblage

Les entreprises peuvent fournir des produits aux clients en combinant des composants sans utiliser de fonctions de fabrication. Les fonctions d’assemblage d’articles s’intègrent aux fonctions associées telles que les ventes, la planification, les réservations et l’entreposage.  

Un élément d’assemblage est un article pouvant être vendu et contenant une nomenclature d’élément d’assemblage. Pour en savoir plus sur les nomenclatures d’élément d’assemblage, consultez [Utilisation des nomenclatures d’assemblage](assembly-how-work-assembly-boms.md).

Les ordres d’assemblage sont des ordres internes, tout comme les ordres de fabrication. Utilisez les ordres d’assemblage pour gérer le processus d’assemblage et pour lier les besoins de vente aux activités entrepôt. Les ordres d’assemblage impliquent à la fois la production et la consommation lors de la validation. Les en-têtes d’ordre d’assemblage sont similaires aux lignes feuille production. Les lignes d’ordre d’assemblage sont similaires aux lignes feuille consommation.  

Vous pouvez utiliser une stratégie de stock juste à temps et personnaliser les produits pour répondre aux demandes des clients. Les ordres d’assemblage peuvent être automatiquement créés et liés lorsque vous créez une ligne de commande vente. Le lien entre la demande de vente et l’approvisionnement d’assemblage ouvre plusieurs opportunités lorsque vous traitez des commandes vente :

* Personnaliser les éléments d’assemblage à la volée.
* Promettre des dates de livraison en fonction de la disponibilité des composants.
* Valider la production et l’expédition de l’article assemblé directement à partir de sa commande vente.

Pour en savoir plus sur la vente d’articles assemblés, consultez [Vente d’articles à assembler pour commande](assembly-how-to-sell-items-assembled-to-order.md).  

Les lignes des commandes vente peuvent contenir des articles à prélever dans le stock et des articles à assembler pour la commande. Les quantités assemblées pour commande ont priorité sur les quantités en stock dans le cas d’une expédition partielle. Pour en savoir plus sur la vente d’articles de stock et d’assemblage, consultez [Scénarios de combinaison](assembly-assemble-to-order-or-assemble-to-stock.md#combination-scenarios).  

Lorsqu’une quantité assemblée pour commande est prête à être expédiée, un magasinier peut valider un prélèvement stock pour les lignes de commande vente. La validation d’un prélèvement stock fait deux choses :

* Crée un mouvement de stock pour les composants
* Valide le résultat d’assemblage et l’expédition de la commande vente.

Pour en savoir plus sur les prélèvements stock et les articles de l’assemblage pour commande, consultez [Traitement des articles à assembler pour commande dans des prélèvements stock](warehouse-how-to-pick-items-with-inventory-picks.md#handling-assemble-to-order-items-with-inventory-picks).

Le tableau suivant décrit une série de tâches et inclut des liens vers les articles qui les décrivent.

|**Pour**|**Voir**|  
|------------|-------------|  
|Découvrez plus d’informations sur l’assemblage d’articles pour les commandes vente et le stockage.|[Description des processus Assembler pour commande et Assembler pour stock](assembly-assemble-to-order-or-assemble-to-stock.md)|
|Utilisez les fiches magasin et les paramètres stock pour définir le flux des articles vers et depuis l’assemblage.|[Configuration des entrepôts de base avec les zones d’opérations](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)|
|Établissez un devis pour un article d’assemblage personnalisé, puis convertissez le devis en vente lorsque le client l’accepte.|[Établissement d’un devis de vente Assembler pour commande](assembly-how-to-quote-an-assemble-to-order-sale.md)|
|Combinez des composants pour créer un article pour une commande ou pour le stock.|[Assemblage des articles](assembly-how-to-assemble-items.md)|  
|Vendez les éléments d’assemblage qui ne sont pas disponibles actuellement en créant un ordre d’assemblage associé pour fournir la quantité totale ou partielle de la commande vente.|[Vente d’articles à assembler pour commande](assembly-how-to-sell-items-assembled-to-order.md)|
|Si des articles à assembler pour commande sont déjà en stock, vous pouvez déduire cette quantité de l’ordre d’assemblage et la réserver dans le stock.|[Vente d’articles en stock dans des flux d’assemblage pour commande](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md)|  
|Lorsque les éléments d’assemblage ne sont pas en stock, utilisez un ordre d’assemblage pour fournir tout ou partie de la quantité.|[Vente simultanée d’articles à assembler pour commande et d’articles en stock](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md)|
|Créez des éléments d’assemblage personnalisés pour les commandes cadres ouvertes avant de créer les commandes vente.|[Création de commandes cadres d’assemblage](assembly-how-to-create-blanket-assembly-orders.md)|
|Annulez un ordre d’assemblage validé, par exemple parce que la facture a été validée avec des erreurs.|[Validation de l’annulation d’assemblage](assembly-how-to-undo-assembly-posting.md)|
|Apprenez à utiliser les nomenclatures d’assemblage et leurs différences avec les nomenclatures de production.|[Utilisation des nomenclatures d’élément d’assemblage](assembly-how-work-assembly-boms.md)|
|Découvrez plus d’informations sur la validation de la consommation de l’assemblage et de la production, et sur la manière dont [!INCLUDE [prod_short](includes/prod_short.md)] répartit les coûts des articles et des ressources dans la comptabilité.|[Détails de conception : validation d’ordre d’assemblage](design-details-assembly-order-posting.md)|  

## <a name="see-also"></a>Voir aussi

[Utilisation des nomenclatures](inventory-how-work-BOMs.md)  
[Stock](inventory-manage-inventory.md)  
[Vue d’ensemble de la gestion des entrepôts](design-details-warehouse-management.md)
[Vue d’ensemble de la gestion des entrepôts](design-details-supply-planning.md)  
<!-- [Walkthrough: Planning Supplies Manually](walkthrough-planning-supplies-manually.md)   -->
<!-- [Walkthrough: Selling, Assembling, and Shipping Kits](walkthrough-selling-assembling-and-shipping-kits.md)   -->
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
