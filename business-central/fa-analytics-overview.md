---
title: Analyse Immobilisations
description: 'Découvrez comment collecter, analyser et partager des données sur les immobilisations à des fins de business intelligence.'
author: brentholtorf
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '5601, 5600, 5615, 5616, 5617'
ms.date: 04/27/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="fixed-assets-analytics"></a>Analyse Immobilisations

Les entreprises possédant des immobilisations capturent de nombreuses données les concernant au cours de leurs activités quotidiennes. Ces données soutiennent une précieuse business intelligence (BI) pour les gestionnaires d’immobilisations :

- Acquisitions actifs
- Dépréciations d’actifs
- Assurance et réparation
- Budget actif

[!INCLUDE[prod_short](includes/prod_short.md)] fournit de nombreuses fonctionnalités pour vous aider à collecter, analyser et partager les données sur les immobilisations votre société :

- États financiers (pour des états financiers et des indicateurs de performance clés sur comptes Immobilisations)
- Analyse ad hoc sur les listes
- Analyse ad hoc des données dans Excel (en utilisant open dans Excel)
- Outils d'analyse sur les immobilisations intégrés
- États sur les immobilisations intégrés

> [!NOTE]
> L’analyse des immobilisations est un peu différente des autres domaines. Vous devez analyser les données déjà présentes, telles que les acquisitions d’actifs, les dépréciations et les assurances, mais également les données futures, telles que les dépréciations et les mises hors service d’actifs. Pour ce dernier type d’analyse, [!INCLUDE[prod_short](includes/prod_short.md)] dispose de rapports intégrés permettant de calculer ces chiffres.

Chaque fonctionnalités présente ses avantages et inconvénients, selon le type d’analyse des données et le rôle de l’utilisateur. Pour en savoir plus, consultez [Analyse, Business Intelligence et Reporting](reports-bi-reporting.md).

Cet article décrit les façons d’utiliser ces fonctionnalités analytiques pour obtenir des informations sur vos immobilisations.

## <a name="analytics-needs-in-asset-management"></a>Besoins analytiques dans la gestion des actifs

Quand on réfléchit aux besoins d’analyse en gestion des actifs, il peut être utile d’utiliser un modèle basé sur une personne décrites à un niveau élevé des besoins en matière d’analyse.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration de différents personnages pour l’analyse" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

En matière de données, Les personnes occupant différents rôles ont des besoins différents et utilisent les données de différentes manières. Par exemple, les professionnels de la gestion de patrimoine et de la finance interagissent avec les données différemment des professionnels de la vente.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration de la manière dont différentes personnes ont des besoins analytiques différents." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Rôle              | Agrégation de données  | Façons typiques de consommer des données                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|CFO / COO / CEO                 | Données performances  | Indicateurs de performance clés <br> Tableaux de bord <br> États financiers           |
|Gestion des immobilisations / Contrôleur   | Tendances, résumés | États managériaux prédéfinis <br> Analyse ad hoc      | 
|Aide-comptable                      | Informations détaillées     | États exploitation prédéfinis <br> Données de tâche à l’écran |

## <a name="asset-management-kpis"></a>KPI Gestion des immobilisations

Un indicateur de performance clé (KPI) est une valeur mesurable qui montre l’efficacité avec laquelle vous atteignez vos objectifs. En gestion d'actifs, les gens utilisent souvent les KPI suivants pour surveiller l'utilisation des actifs de leur organisation :

- Chiffre d’affaires total des actifs
- Le rendement des actifs

## <a name="use-financial-reporting-to-produce-financial-statements-and-kpis-related-to-fixed-assets"></a>Utilisation États financiers pour produire des états financiers et des indicateurs de performance clés associés à Immobilisations

La fonctionnalité **Financial Reporting** vous donne un aperçu des données financières enregistrées dans votre plan comptable (COA). Configurez les états financiers pour analysent les chiffres de la comptabilité et comparent les écritures comptables et les écritures comptables budget. Spécifiquement pour la gestion des actifs, vous pouvez configurer des rapports financiers sur les comptes du comptabilité (G/L) que vous utilisez pour suivre les validations de Immobilisations.

Les axes jouent un rôle important dans la veille économique. Un axe correspond à des données que vous pouvez ajouter à une écriture en tant que paramètre. Les axes vous permettent de regrouper des écritures dotées de caractéristiques similaires, telles que les clients, les produits et les commerciaux, et de récupérer facilement ces groupes à des fins d’analyse. Entre autres objectifs, vous utilisez des axes analytiques à la définition de vues d’analyse et de la création d’états financiers. Pour plus d’informations, consultez [Utiliser les dimensions](finance-dimensions.md).

Pour en savoir plus sur les états financiers, accédez à [Préparer les états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md).

## <a name="finance-reporting-across-business-units-or-legal-entities-related-to-fixed-assets"></a>États financiers entre les divisions ou les entités juridiques (associé à Immobilisations)

Certaines organisations utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans plusieurs centres de profit ou entités juridiques. D’autres utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans les filiales qui rendre compte aux organisations mères. [!INCLUDE [prod_short](includes/prod_short.md)] fournit aux comptables des outils qui les aident à transférer les écritures comptables de deux ou plusieurs sociétés (filiales) dans une société consolidée. Spécifiquement pour la gestion des actifs, vous souhaiterez peut-être consolider les écritures comptabilité pour vos comptes Immobilisations pour suivre les KPI de actifs dans les unités commerciales ou les entités juridiques.

Pour en savoir plus, reportez-vous à [Consolidation de la société](finance-consolidated-company-reporting.md).

## <a name="ad-hoc-analysis-of-fixed-assets-data"></a>Analyse ad hoc des données Immobilisations

Parfois, il suffit de vérifier si les chiffres s’additionnent correctement ou de confirmer rapidement un chiffre. Les fonctionnalités suivantes sont idéales pour les analyses ad hoc :

- Analyses des données sur les pages de listes comptables
- Ouvrir dans Excel

La fonction d’analyse des données vous permet d’ouvrir presque toutes page de liste, telle que les **Écritures comptables**, les **écritures comptables immobilisation**, d’entrer en mode analyse, puis de regrouper, filtrer et faire pivoter les données comme bon vous semble.

:::image type="content" source="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png" alt-text="Exemple de comment effectuer une analyse de données sur la page Écritures comptables immobilisation pour voir la valeur d’un actif." lightbox="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png":::

De la même manière, vous pouvez utiliser le **Ouvrir dans Excel** action pour ouvrir une page de liste pour les écritures comptables, éventuellement filtrer la liste sur un sous-ensemble de données, puis utiliser Excel pour travailler avec les données. Par exemple, en utilisant des fonctionnalités telles que l’analyse des données, l’analyse de simulation ou la feuille de prévision.

<!-- :::image type="content" source="media/open-in-excel-gl-entries.png" alt-text="Example of how to do data analysis on the G/L entries data using Excel." lightbox="media/open-in-excel-gl-entries.png"::: -->

> [!TIP]
> Si vous configuré OneDrive pour les fonctionnalités système, le classeur Excel s’ouvre dans votre navigateur à l’aide d’Excel pour le Web. 

Pour plus d’informations sur la manière d’effectuer une analyse ad hoc sur la comptables immobilisation, voir [Analyse ad hoc sur les données Immobilisations](ad-hoc-analysis-fa.md).


## <a name="built-in-reports-for-fixed-assets"></a>États intégrés sur les immobilisations

[!INCLUDE [prod_short](includes/prod_short.md)] comprend plusieurs rapports, fonctions de traçage et outils incorporés qui aident les auditeurs ou contrôleurs chargés de rendre compte sur les Immobilisations.

Pour obtenir un aperçu des rapports disponibles, choisir sur **Tous les rapports** en haut de votre page d’accueil. Cette Action ouvre la page l’explorateur de rôles, qui est filtré selon les fonctionnalités du **Rapport et analyse** option. Pour rechercher des rapports relatifs aux immobilisations, dans le champ **Rechercher** , saisissez **immobilisations**. Pour en savoir plus, voir [Recherche de rapports avec l’explorateur de rôles](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-fixed-assets.png" alt-text="Exemple de rapports sur le centre de rôle finance." lightbox="media/report-explorer-fixed-assets.png":::

<!-- Built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel. -->

Pour plus d’informations sur les rapports pertinents pour les immobilisations, consultez [Rapports intégrés sur les immobilisations](fa-reports.md).

## <a name="on-screen-fixed-assets-analytics"></a>Analyses des immobilisations à l'écran

[!INCLUDE [prod_short](includes/prod_short.md)] comporte plusieurs pages qui vous donnent des aperçus des Immobilisations et des tâches à accomplir. Voici des exemple pour commencer :

- [Calculer l’amortissement, valider l’amortissement et analyser l’amortissement](fa-how-depreciate-amortize.md)
- [Surveillance des coûts de maintenance](fa-how-maintain.md#to-monitor-maintenance-costs)
- [Surveillance des couvertures d’assurance](fa-how-insure.md#to-monitor-insurance-coverage)
- [Affichage des valeurs de la loi d’amortissement modifiées](fa-how-trans-split-combine.md#to-view-changed-depreciation-book-values-due-to-fixed-asset-reclassification)
- [Affichage des écritures comptables cession](fa-how-dispose-retire.md#to-view-disposal-ledger-entries)
- [Affichage des valeurs de cession prévues](fa-how-manage-budgets.md#to-view-projected-disposal-values)

### <a name="show-fixed-asset-general-ledger-entries-and-balances-from-the-chart-of-accounts-page"></a>Afficher les écritures comptables immobilisations à partir de la page Plan comptable

La page Plan comptable affiche tous les comptes du grand livre avec des chiffres agrégés dans la comptabilité. À partir de cette page, vous pouvez faire des choses comme :  

- Afficher les états qui affichent les écritures comptables et les soldes.  
- Vérifier la liste des groupes comptabilisation pour ce compte.
- Afficher les soldes débit et crédit d’un seul compte.

Spécifiquement pour les Immobilisations, vous pouvez créer une vue sur la page Plan comptable qui affiche uniquement les comptes que vous utilisez pour valider les écritures Immobilisations.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Exemple de la façon dont la page Plan comptable affiche des informations financières" lightbox="media/chart-of-accounts-page.png":::

Pour en savoir plus, allez à [Familiarisation avec le plan comptable](finance-general-ledger.md#the-chart-of-accounts).

### <a name="analyze-data-by-dimensions-related-to-fixed-assets"></a>Analyse des données par axe analytique (lié aux Immobilisations)

Les axes analytiques sont des valeurs qui permettent de catégoriser les écritures afin de pouvoir les suivre et les analyser sur les documents, tels que les feuilles immo. Les Axes analytiques peuvent, Par exemple, indiquer le service ou le Magasin dont est issue une écriture.  

Au lieu de configurer des comptes généraux distincts pour chaque service ou Emplacement, vous pouvez utiliser les axes analytiques comme base d’analyse et éviter d’avoir à créer une structure de plan comptable compliqué.

Pour plus d’informations, consultez [Analyse des données par axe analytique](bi-how-analyze-data-dimension.md)

## <a name="see-also"></a>Voir aussi

[Gestion des états financiers entre les divisions ou les entités juridiques](finance-consolidated-company-reporting.md)  
[Préparer des états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md)  
[Comprendre du plan comptable](finance-general-ledger.md#the-chart-of-accounts)  
[Analyse ad hoc des données Immobilisations](ad-hoc-analysis-fa.md)   
[États sur les immobilisations intégrés](fa-reports.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
