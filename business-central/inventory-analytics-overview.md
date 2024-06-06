---
title: Analyse du stock
description: "Business\_Central contient un de nombreuses fonctionnalités pour vous aider à collecter, analyser et partager des données précieuses de votre stock pour BI et la prise de décision dans l'organisation."
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 05/03/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="inventory-analytics"></a>Analyse du stock

Les entreprises capturent des lots de données au cours de leurs activités quotidiennes, ce qui soutient une précieuse BI pour les gestionnaires stock :

- Expédition des marchandises lorsque les commandes sont exécutées.
- Réceptions des articles lorsque les bons de commande sont exécutés.
- Déplacement des articles entre magasins.

[!INCLUDE[prod_short](includes/prod_short.md)] fournit de nombreuses fonctionnalités pour vous aider à collecter, analyser et partager les données stock de votre société :

- Analyse ad hoc sur les listes
- Analyse ad hoc des données dans Excel (en utilisant Ouvrir dans Excel)
- Outils d’analyse des stock intégrés
- États intégrés pour la stock

Chacune de ces fonctionnalités présente ses avantages et inconvénients, selon le type d’analyse des données et le rôle de l’utilisateur. Pour en savoir plus, consultez [Analyse, Business Intelligence et Reporting](reports-bi-reporting.md).

Cet article vous présente comment d’utiliser ces fonctionnalités analytiques pour obtenir des informations stock.

## <a name="analytics-needs-in-inventory"></a>Besoins analytiques en stock

Lorsque l’on réfléchit aux besoins d’analyse en gestion des stock, il peut être utile d’utiliser un modèle basé sur une personne décrites à un niveau élevé des différents besoins en matière d’analyse.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration de différents personnages pour l’analyse" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

Les personnes occupant différents rôles ont des besoins différents en matière de données et utilisent les données de différentes manières. Par exemple, les professionnels de la gestion de patrimoine et de la finance interagissent avec les données différemment des professionnels de la vente.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration de la manière dont différentes personnes ont des besoins analytiques différents." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Rôle              | Agrégation de données  | Façons typiques de consommer des données                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|CFO / CFO / CEO    | Données performances  | KPI, tableaux de bord, rapports financiers           |
|Gestionnaire d’inventaire  | Tendances, résumés | Rapports de gestion intégrés, analyse ad hoc      | 
|Magasinier   | Informations détaillées     | Rapports opérationnels intégrés, données de tâches à l’écran |

<!-- 
## <a name="inventory-kpis"></a>Inventory KPIs

A key performance indicator (KPI) is a measurable value that shows how effectively you’re meeting your goals. In inventory management, people often use the following KPIs to monitor their organization's sales performance:

- TODO  
-->

## <a name="use-financial-reporting-to-produce-financial-statements-and-kpis-related-to-inventory"></a>Utilisation États financiers pour produire des états financiers et des indicateurs de performance clés (associés à stock)

La fonctionnalité **Financial Reporting** vous donne un aperçu des données financières enregistrées dans votre plan comptable (COA). Configurez les états financiers pour analysent les chiffres de la comptabilité et comparent les écritures comptables et les écritures comptables budget. Spécifiquement pour la gestion des stock, vous pouvez configurer des rapports financiers sur les comptes du comptabilité (G/L) que vous utilisez pour suivre les validations de stock.

Les axes jouent un rôle important dans la veille économique. Un axe correspond à des données que vous ajouter à une écriture en tant que paramètre. Les axes vous permettent de regrouper des écritures dotées de caractéristiques similaires, telles que les clients, les régions, les produits et les commerciaux. Entre autres objectifs, utilisez des axes analytiques à la définition de vues d’analyse et de la création d’états financiers. Pour plus d’informations, consultez [Utiliser les dimensions](finance-dimensions.md).

Pour en savoir plus sur les états financiers, accédez à [Préparer des états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md).

## <a name="finance-reporting-across-business-units-or-legal-entities-related-to-inventory"></a>États financiers entre les divisions ou les entités juridiques (associé à stock)

Certaines organisations utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans plusieurs centres de profit ou entités juridiques. D’autres utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans les filiales qui rendre compte aux organisations mères. [!INCLUDE [prod_short](includes/prod_short.md)] fournit aux comptables des outils qui les aident à transférer les écritures comptables de deux ou plusieurs sociétés (filiales) dans une société consolidée. Spécifiquement pour la gestion des stock, vous souhaiterez peut-être consolider les écritures comptabilité pour vos comptes stock pour suivre les KPI de vente dans les unités commerciales ou les entités juridiques.

Pour en savoir plus, reportez-vous à [Consolidation de la société](finance-consolidated-company-reporting.md).

## <a name="ad-hoc-analysis-of-inventory-data"></a>Analyse ad hoc des données stock

Parfois, il suffit de vérifier si les chiffres s’additionnent correctement ou de confirmer rapidement un chiffre. Les fonctionnalités suivantes sont idéales pour les analyses ad hoc :

- Analyses des données sur les pages de listes comptables
- Ouvrir dans Excel

La fonction d’analyse des données vous permet d’ouvrir presque toutes page de liste, telle que les **Écritures comptables article** d’entrer en mode analyse, puis de regrouper, filtrer et faire pivoter les données comme bon vous semble.

:::image type="content" source="media/data-analysis-inventory-dead-stock.png" alt-text="Exemple de comment effectuer une analyse des données de stock ancien sur la page des écritures comptables articles" lightbox="media/data-analysis-inventory-dead-stock.png":::

De la même manière, vous pouvez utiliser le **Ouvrir dans Excel** action pour ouvrir une page de liste, éventuellement filtrer la liste sur un sous-ensemble de données, puis utiliser Excel pour travailler avec les données. Par exemple, en utilisant des fonctionnalités telles que l’analyse des données, l’analyse de simulation ou la feuille de prévision.

<!-- :::image type="content" source="media/open-in-excel-item-ledger-entries.png" alt-text="Example of how to do data analysis on the Item Ledger Entries data using Excel." lightbox="media/open-in-excel-item-ledger-entries.png"::: -->

> [!TIP]
> Si vous configuré OneDrive pour les fonctionnalités système, le classeur Excel s’ouvre dans votre navigateur.

Pour en savoir plus sur la manière d’effectuer une analyse ad hoc des données de stock, accédez à [Analyse ad hoc des données de stock](ad-hoc-analysis-inventory.md).

## <a name="built-in-reports-for-inventory"></a>États intégrés pour stock

[!INCLUDE [prod_short](includes/prod_short.md)] comprend plusieurs rapports intégrés, fonctions de traçage et outils pour aider les organisations stock à créer des rapports sur leurs données.

Pour obtenir un aperçu des rapports disponibles, choisir sur **Tous les rapports** de votre page d’accueil. Cette Action ouvre l’explorateur de rapport, qui est filtré selon les fonctionnalités du **Rapport et analyse** option. Sous l’en-tête **Ventes et marketing** , choisissez **Explorer**. Pour en savoir plus, voir [Recherche de rapports avec l’explorateur de rôles](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-sales.png" alt-text="Exemple de rapports sur le centre de rôle ventes." lightbox="media/report-explorer-sales.png":::

<!-- The built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel. -->

Pour en savoir plus sur les rapports pertinents pour les stock, accédez aux [Rapports stock et Entrepôt intégrés](inventory-WMS-reports.md).

## <a name="on-screen-inventory-analytics"></a>Analyse des stock à l’écran

[!INCLUDE [prod_short](includes/prod_short.md)] comporte plusieurs pages qui vous donnent des aperçus des stocks et des tâches à accomplir. Voici des exemple pour commencer :

- [Afficher la disponibilité des articles](inventory-how-availability-overview.md)
- [Suivi des articles avec les numéros de lot, de série et de paquet](inventory-how-work-item-tracking.md)
- [Traçabilité : articles suivis](inventory-how-to-trace-item-tracked-items.md)
- [Audit du rapprochement entre la comptabilité des stocks et la comptabilité générale](finance-how-to-post-inventory-costs-to-the-general-ledger.md#to-audit-the-reconciliation-between-the-inventory-ledger-and-the-general-ledger)
- [Affichage d’articles transbordés dans une feuille expédition ou une feuille prélèvement](warehouse-how-to-cross-dock-items.md#to-view-cross-docked-items-in-a-shipment-or-pick-worksheet)

Le module de vente comprend également des pages d’analyse liées à l’inventaire :

- [Calcul des dates promesse commande](sales-how-to-calculate-order-promising-dates.md)
- [Calculer la dates de livraison des Commandes ventes](sales-date-calculation-for-sales.md)
- [Suivi des paquets](sales-how-track-packages.md)

### <a name="show-inventory-related-general-ledger-entries-and-balances-from-the-chart-of-accounts-page"></a>Afficher les écritures comptables et les soldes liés aux stock à partir de la page Plan comptable

La page **Plan comptable** affiche tous les comptes du grand livre avec des chiffres agrégés comptabilisé dans le grand livre. À partir de cette page, vous pouvez faire des choses comme :  

- Afficher les états qui affichent les écritures comptables et les soldes.  
- Vérifier la liste des groupes comptabilisation pour ce compte.
- Afficher les soldes débit et crédit d’un seul compte.

Spécifiquement pour les gestion stock, vous pouvez créer une vue sur la page Plan comptable qui affiche uniquement les comptes que vous utilisez pour valider les écritures stock.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Exemple de la façon dont la page Plan comptable affiche des informations financières" lightbox="media/chart-of-accounts-page.png":::

Pour en savoir plus, allez à [Familiarisation avec le plan comptable](finance-general-ledger.md#the-chart-of-accounts).

### <a name="analyze-inventory-data-by-dimensions"></a>Analyse des données stock par axe analytique

Les axes analytiques sont des valeurs qui permettent de catégoriser les écritures afin de pouvoir les suivre et les analyser sur les documents, tels que les commandes vente. Ils peuvent par exemple indiquer de quel projet ou département provient une écriture.  

Au lieu de configurer des comptes généraux distincts pour chaque service ou Emplacement, vous pouvez utiliser les axes analytiques comme base d’analyse et éviter d’avoir à créer une structure de plan comptable compliqué.

Pour plus d’informations, consultez [Analyse des données par axe analytique](bi-how-analyze-data-dimension.md).

## <a name="see-also"></a>Voir aussi

[Consolidation de la société](finance-consolidated-company-reporting.md)   
[Préparer des états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md)  
[Gestion des états financiers entre les divisions ou les entités juridiques](finance-consolidated-company-reporting.md)  
[Analyse ad hoc des données de stock](ad-hoc-analysis-inventory.md)  
[États de stock et d’entrepôt intégrés](inventory-WMS-reports.md)  
[Comprendre du plan comptable](finance-general-ledger.md#the-chart-of-accounts)  
[Analyse des données par axe analytique](bi-how-analyze-data-dimension.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)   
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
