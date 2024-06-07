---
title: Assembler au projet
description: Apprenez à utiliser l’assemblage sur commande pour un projet.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'project management, task'
ms.search.form: '88, 275, 276, 1001, 1002, 1003, 1004, 1005, 1006, 1007, 1020'
ms.date: 08/03/2022
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="assemble-to-project"></a>Assembler au projet

Assembler selon le projet vous aide à améliorer la gestion des stocks en assemblant sur commande uniquement lorsque cela est nécessaire.

Lorsque vous choisissez un article à assembler pour commande sur une ligne planification de projet, [!INCLUDE [prod_short](includes/prod_short.md)] crée un ordre d’assemblage. L’ordre d’assemblage est basé sur la ligne planning projet et ses lignes sont basées sur la nomenclature d’assemblage de l’article. Pour en savoir plus sur les nomenclatures d’élément d’assemblage, consultez [Utilisation des nomenclatures d’assemblage](assembly-how-work-assembly-boms.md). La quantité de composants sur la nomenclature d’assemblage est multipliée par la quantité commandée. La page **Lignes Assembler pour commande** affiche des détails sur les lignes de commande d’assemblage liées. Les détails peuvent vous aider à personnaliser l’élément d’assemblage. Comme pour les ventes, vous ne pouvez pas valider directement les ordres d’assemblage liés. Pour en savoir plus sur les ordres d'assemblage, consultez [Vente d’articles en stock dans des flux à assembler pour commande](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md).

Les ordres d’assemblage sont réservés aux projets, et [!INCLUDE [prod_short](includes/prod_short.md)] synchronise le suivi des articles entre les lignes de planification du projet et l’ordre d’assemblage.

## <a name="integrate-with-warehouse-management"></a>Intégrer la Warehouse Management

Assembler au projet s’intègre aux fonctionnalités Warehouse Management pour faciliter l’assemblage et l’expédition. Le processus permet également de garantir que le flux depuis l’assemblage du projet jusqu’à la livraison se déroule sans problème dans les processus internes de l’entrepôt. Pour en savoir plus sur les flux d’entrepôt internes pour les projets, rendez-vous sur [Flux pour la production, l’assemblage et les projets](design-details-internal-warehouse-flows.md#flows-to-and-from-assembly-in-a-basic-warehouse-configuration).

Le tableau suivant décrit les configurations d’entrepôt qui s’assemblent pour commander des supports.

|Configuration  |Désignation  |
|---------|---------|
|**Pas de manutention d’entrepôt**|Utilisez un journal de projet pour publier une utilisation totale ou partielle. La production et la consommation des composants sont automatiquement enregistrées pour l’ordre d’assemblage.         |
|**Prélèvement de stock**|Utilisez un prélèvement stock pour publier une utilisation totale ou partielle. La production et la consommation des composants sont automatiquement enregistrées pour l’ordre d’assemblage.          |
|**Prélèvement entrepôt**|Créez et enregistrez les prélèvements en entrepôt pour les composants, puis utilisez un journal de projet pour publier leur utilisation. [!INCLUDE [prod_short](includes/prod_short.md)] vérifie si les composants d’assemblage consommés ont été prélevés. La production et la consommation des composants sont automatiquement enregistrées pour l’ordre d’assemblage.         |

## <a name="known-limitations"></a>Limitations connues

Cette section décrit les limitations connues pour l’assemblage dans le projet.

* Le champ **Quantité à assembler pour commander** n’est pas disponible pour les projets clôturés.
* Pour les scénarios de prélèvement en entrepôt, la **Quantité à assembler pour commander** peut être nulle ou égale à la quantité. Vous ne pouvez pas mélanger l’assemblage sur commande et l’assemblage pour stock sur une ligne de planification de projet. Vous devez créer des lignes de planification de projet distinctes.
* L’assemblage sur commande n’affecte pas les parties facturables d’un projet. Un assemblage est inclus sur les factures de vente, mais pas ses composants. Vous ne pouvez pas modifier le champ **Quantité à assembler pour commander** pour les lignes facturables.
* La planification des commandes et la feuille de travail de planification ne sont pas affectées car le projet constitue l’entrée de la planification. Le moteur de planification considère l’assemblage comme une demande.
* Vous ne pouvez pas saisir une quantité négative dans le champ **Quantité à assembler pour commander** .
* Vous ne pouvez pas annuler un assemblage.

## <a name="see-also"></a>Voir aussi

[Gestion de projets](projects-manage-projects.md)  
[Gestion nomenclature d’assemblage](assembly-assemble-items.md)  
[Création des projets](projects-how-create-jobs.md)
