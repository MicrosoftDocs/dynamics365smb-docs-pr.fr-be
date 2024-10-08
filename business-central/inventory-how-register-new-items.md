---
title: Créer des fiches article pour des biens ou des services
description: Vous créez des fiches article pour les services que vous vendez en heures et pour les produits physiques. Les exemples incluent les éléments d’assemblage et les produits finis que vous vendez à partir de votre inventaire.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'item, finished good, component, raw material, assembly item, item substitution'
ms.search.form: '30, 5717, 31, 32, 346, 9091, 5718, 5716, 5720, 1384, 1383, 35, 5404, 1378, 5719'
ms.date: 05/24/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# Enregistrement des nouveaux articles

Les articles, parmi d’autres produits, constituent la base de votre entreprise, les biens ou les services que vous commercialisez. Chaque article doit être enregistré en tant que fiche article.

* **Inventaire** spécifie que l’article est une unité physique que vous gérez et suivez dans l’inventaire.
* **Hors inventaire** sont des unités physiques que vous ne gérez pas ou ne suivez pas dans l’inventaire.
* **Service** les articles sont une unité de temps de travail, généralement utilisée dans la gestion des services.

Pour en savoir plus sur ces types d'articles, accédez à [À propos des types d’articles](inventory-about-item-types.md).

> [!TIP]
> Il existe également des articles de catalogue, qui sont similaires aux articles hors stock dans la mesure où ce sont des articles que vous proposez aux clients mais que vous ne gérez pas tant que vous ne les vendez pas. Pour en savoir plus, consultez [Utiliser les articles catalogue](inventory-how-work-nonstock-items.md).  

## Fournisseurs principaux et alternatifs

Si vous achetez le même article chez plusieurs fournisseurs, vous pouvez lier ces fournisseurs à la article. Utilisez le **Vendeurs** action sur le **Carte d’article** page pour ouvrir le **Catalogue des fournisseurs d’articles** page. La page affiche les fournisseurs auprès desquels vous achetez l’article, afin que vous puissiez facilement créer ou sélectionner un autre fournisseur lorsque vous créez un bon de commande.

## Utiliser modèles article

Pour réutiliser les paramètres de différents types d’éléments lorsque vous créez de nouveaux éléments, vous pouvez enregistrer les éléments en tant que modèles d’élément. Les modèles d’articles permettent d’accélérer le processus d’ajout de nouveaux articles et d’améliorer la cohérence de vos données d’articles. Lorsque vous enregistrez un nouvel élément, une page apparaît qui vous permet de choisir un modèle. Après avoir choisi un modèle, ses paramètres sont renseignés pour vous sur l’élément que vous créez. Si vous avez un seul modèle article, les nouvelles article utiliseront toujours ce modèle. Pour savoir comment configurer un modèle d’élément, accédez à [Enregistrer une fiche article en tant que modèle d’article](#save-an-item-card-as-an-item-template).

<br/>

## Inclure des éléments dans les nomenclatures

Vous pouvez structurer des hiérarchies comportant un article principal avec des éléments de composants sous-jacents dans les nomenclatures d’assemblage et de production. Pour en savoir plus sur les nomenclatures, consultez [Utilisation des nomenclatures](inventory-how-work-BOMs.md).

## Pour créer une fiche article

La vidéo suivant montre la manière dont un article est paramétrée sur la fiche article. Toutefois, vous pouvez également configurer de nouvelles articles en copiant celles existantes. Pour plus d’informations, aller [Copier des articles existants pour créer de nouveaux articles](inventory-how-copy-items.md).  

> [!Video https://www.microsoft.com/videoplayer/embed/RE47eLx?rel=0]

[!INCLUDE[create_new_item](includes/create_new_item.md)]

> [!NOTE]
> Dans le champ **Mode évaluation stock**, vous configurez la façon dont le coût unitaire de l'article est calculé en estimant le flux d'articles dans votre société. Il existe cinq modes évaluation stock disponibles, selon le type d'article. Pour en savoir plus sur coûts des stocks, accédez à [Détails de conception : Méthodes Évaluation des coûts](design-details-costing-methods.md).
>
> Si vous sélectionnez **Moyenne**, le coût unitaire de l’article est calculé comme le coût unitaire moyen à chaque moment après un achat. Le stock est évalué avec la supposition que tous les stocks sont vendus simultanément. Avec ce paramètre, vous pouvez choisir le champ **Coût unitaire**, sur la page **Aperçu calc. coût moyen** de la fiche article pour afficher des transactions pour calculé le coût moyen.

Vous pouvez utiliser des prix spéciaux ou des remises que vous ou votre fournisseur accordez pour l’article en fonction de certains critères. Par exemple, les critères incluent le client, la quantité minimale de commande ou la date de fin. Configurez les prix spéciaux choisissez les actions **Définir les prix spéciaux** ou **Définir les remises spéciales**. Chaque ligne de la page **Prix de vente**, par exemple, représente un prix spécial. Chaque colonne représente un critère qui doit s’appliquer pour accorder à un client le prix spécial que vous entrez dans le champ **Prix unitaire** de la page **Prix de vente**. Pour plus d’informations sur les prix, voir [Enregistrement des prix de vente, des remises et des accords sur les paiements](sales-how-record-sales-price-discount-payment-agreements.md) ou [Enregistrer les prix d’achat spéciaux et les remises](purchasing-how-record-purchase-price-discount-payment-agreements.md).

### Enregistrer la fiche article en tant que modèle article

1. Sur la page **Fiche article**, sélectionnez l'action **Sauvegarder comme modèle**. La page **Modèle article** affiche la fiche article comme modèle.
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Pour réutiliser des dimensions dans des modèles, choisissez l’action **Associée**, puis choisissez **Élément**, puis **Dimensions**. Les **Dimensions par défaut** de l’élément sélectionné s’ouvrent et affichent tous les codes de dimension configurés pour l’élément.
4. Modifiez ou entrez les codes axe s’appliquant aux nouvelles fiches article créées à l’aide du modèle.
5. Lorsque vous terminez le nouveau modèle article, cliquez sur le bouton **OK**.

Le modèle article est ajouté à la liste des modèles article. Vous pouvez ainsi l'utiliser pour créer des fiches article.

### Articles utilisés dans les ordres de fabrication

Si vous souhaitez enregistrer des articles qui sont ensuite utilisés dans des ordres de fabrication, vous spécifiez le système réappro. comme *Ordre de fabrication* sur le raccourci **Réapprovisionnement**. Pour plus d’informations, voir [À propos des ordres de fabrication](production-about-production-orders.md).  

## Pour configurer plusieurs fournisseurs pour un article

Si vous achetez le même article chez plusieurs fournisseurs, vous devez saisir, pour chacun des fournisseurs de cet article des informations concernant, par exemple, ses prix, ses délais, ses escomptes, etc.  

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Articles**, puis choisissez le lien associé.  
2. Sélectionnez l'article concerné, puis cliquez sur l'action **Modifier**.  
3. Sélectionnez l'action **Fournisseurs**.  
4. Choisissez le **Non.** Champ, puis Sélectionner le fournisseur que vous souhaitez configurer pour l’article.  
5. De manière facultative, renseignez les autres champs.  
6. Répétez les étapes 2 à 5 pour chaque fournisseur auprès de qui vous souhaitez acheter l'article.

Les fournisseurs s’affichent maintenant sur la page **Catalogue fournisseur articles** (que vous ouvrez à partir de la fiche article), de sorte que vous pouvez facilement sélectionner un autre fournisseur.

## Configuration d’articles de substitution

Vous pouvez configurer des articles pour qu’ils aient des substituts, tels que d’autres articles pouvant être utilisés à la place de l’article d’origine.

### Pour affecter le statut de substitut à un article

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Articles**, puis choisissez le lien associé.  
2. Recherchez l’élément concerné, puis choisissez le **Non.** Pour ouvrir l’article carte.  
3. Choisissez l’action **Association**, puis sélectionnez **Article**, puis **Substitutions** pour ouvrir la page **Saisie de substitution d’article**.  
4. Sélectionnez le champ **N° substitut**, puis sélectionnez l’article de substitution dans la liste.
5. Renseignez ou modifiez les autres champs de la page selon vos besoins.

Lorsque la quantité d’articles requis dépasse la quantité disponible en stock, un message apparaît pour vous informer que des articles de substitution sont disponibles.

> [!NOTE]  
> Sachez que les articles de substitution n’entraîneront pas automatiquement le remplacement d’un article par un autre, par exemple lors de la création d’une commande client ou dans une nomenclature. Au lieu de cela, vous serez alerté du fait qu’un substitut est disponible pour vous.

## Catégories, attributs et variantes

[!INCLUDE[inventory_variant](includes/inventory_variant.md)]

En savoir plus sur les variantes dans la section [Gérer les variantes de produits](inventory-item-variants.md).  

## Supprimer de fiches article

Si vous enregistré une transaction pour un article, vous ne pouvez pas supprimer la carte, car les écritures comptables peuvent être nécessaires pour l’évaluation du stock ou l’audit. Pour supprimer des fiches article avec des écritures comptables, contactez le partenaire Microsoft pour le faire via le code.  

## Gérer le stock des entrepôts

Lorsque vous enregistrez un nouvel article, vous verrez des champs liés à la gestion de l’entrepôt, en particulier sur le raccourci **Entrepôt**. Si votre organisation n’utilise pas les fonctionnalités de gestion d’entrepôt dans [!INCLUDE [prod_short](includes/prod_short.md)], vous pouvez alors ignorer ces champs.  

Si votre organisation configure ultérieurement la gestion des entrepôts, nous vous recommandons de vous assurer que chaque article existant possède les bonnes informations dans les différents champs. De cette façon, les processus d’entrepôt peuvent s’exécuter comme prévu. Ces informations peuvent inclure des champs, tels que **Code classe entrepôt** ou **Code modèle rangement**. Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).  

## Planning

Lorsque votre entreprise utilise les processus de planification des approvisionnements dans [!INCLUDE [prod_short](includes/prod_short.md)], vous devez remplir les champs correspondants sur le raccourci **Planification**. Pour une introduction à la zone de planification, voir [Détails de conception : concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md).  

Pour des exemples d’utilisation des champs du raccourci **Planification**, voir [Configurer des recommandations : paramètres de planification](setup-best-practices-planning-parameters.md).  

## Voir aussi

[STOCKS ET EN-COURS](inventory-manage-inventory.md)    
[Configurer les unités de mesure](inventory-how-setup-units-of-measure.md)    
[Gérer les variantes de produits](inventory-item-variants.md)    
[Configurer les rapports Intrastat](finance-how-setup-report-intrastat.md#other-intrastat-configurations)    
[Rapprochez les coûts d’inventaire avec le comptabilité](finance-how-to-post-inventory-costs-to-the-general-ledger.md)    
[Créer une série de nombres](ui-create-number-series.md)    
[Configuration des groupes de publication](finance-posting-groups.md)    
[Achats](purchasing-manage-purchasing.md)    
[Ventes](sales-manage-sales.md)    
[À propos de la fonctionnalité de planification](production-about-planning-functionality.md)    
[Meilleures pratiques de configuration : paramètres de planification](setup-best-practices-planning-parameters.md)    
[Meilleures pratiques de configuration : planification de l’approvisionnement](setup-best-practices-supply-planning.md)    
[Détails de conception : Concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md)    
[Détails de conception : équilibre entre l’offre et la demande](design-details-balancing-demand-and-supply.md)    
[Détails de conception : paramètres de planification](design-details-planning-parameters.md)    
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    


[!INCLUDE[footer-include](includes/footer-banner.md)]
