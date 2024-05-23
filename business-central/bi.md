---
title: Analyses financières
description: 'Business Central vous aider à collecter, analyser et partager les données de votre société pour BI.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '103, 108, 198, 490'
ms.date: 03/27/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Analyses financières

Les entreprises capturent une énorme quantité de données au cours de leurs activités quotidiennes, ce qui soutient une précieuse business intelligence (BI) pour les décideurs :

- Les chiffres de vente
- Ac&hats
- Frais d'exploitation
- Salaires des employés
- Budgets

[!INCLUDE[prod_short](includes/prod_short.md)] contient de nombreuses fonctionnalités pour vous aider à collecter, analyser et partager les données financières de votre société :

- États financiers (pour états financiers et des indicateurs de performance clés)
- Analyse ad hoc sur les listes
- Analyse ad hoc des données dans Excel (en utilisant open dans Excel)
- États financiers intégrés

Chacune de ces fonctionnalités présente ses propres avantages et inconvénients, selon le type d’analyse des données et le rôle de l’utilisateur. Pour en savoir plus, consultez [Analyse, Business Intelligence et Reporting](reports-bi-reporting.md).

Cet article vous présente la possibilité d’utiliser ces fonctionnalités analytiques pour fournir des informations financières.

## Besoins analytiques en finance

Lorsque l’on réfléchit aux besoins d’analyse en finance, il peut être utile d’utiliser un modèle mental basé sur des personnalités décrites à un niveau élevé et leurs différents besoins en matière d’analyse.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration de différents personnages pour l’analyse" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

Les personnes occupant différents rôles ont des besoins différents en matière de données et utilisent les données de différentes manières. Par exemple, les professionnels de la finance interagissent avec les données différemment des professionnels de la vente.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration de la manière dont différentes personnes ont des besoins analytiques différents." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Rôle              | Agrégation de données  | Façons typiques de consommer des données                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|Directeur financier / PDG          | Données performances  | Indicateurs de performance clés <br> Tableaux de bord <br> États financiers           |
|Gestion des finances | Tendances, résumés | États managériaux prédéfinis <br> Analyse ad hoc      | 
|Aide-comptable         | Informations détaillées     | États exploitation prédéfinis <br> Données de tâche à l’écran |

## Indicateurs de performance clés financiers

Un indicateur de performance clé (KPI) est une valeur mesurable qui montre l’efficacité avec laquelle vous atteignez vos objectifs. En finance, les gens utilisent souvent les KPI suivants pour surveiller la santé financière de leur organisation :

- Marge bénéf. brute
- Marge bénéficiaire nette
- Fonds de roulement
- Rapport courant/rapide
- Levier financier, également connu sous le nom de multiplicateur d’équité
- Ratio d’endettement
- Chiffre d’affaires total des actifs
- Retour sur capitaux propres
- Le rendement des actifs

<!-- Not ready to publish yet
For more information, see [Financial KPIs in Business Central](bi-finance-kpis.md) 
-->

## Utilisation États financiers pour produire des états financiers et des indicateurs de performance clés

La fonctionnalité **états financiers** vous donne un aperçu des données financières enregistrées dans votre plan comptable (COA). Configurez les états financiers pour analysent les chiffres de la comptabilité et comparent les écritures comptables et les écritures comptables budget. Les résultats s’affichent dans les graphiques et les états de votre page d’accueil, comme le graphique Trésorerie et les états Comptes de gestion et Bilan.

Les axes jouent un rôle important dans la veille économique. Un axe correspond à des données que vous pouvez ajouter à une écriture en tant que paramètre. Les dimensions vous permettent de regrouper les entrées présentant des caractéristiques similaires afin de les rendre plus faciles à analyser. Par exemple, clients, régions, vos produits et vos vendeurs. Entre autres objectifs, utilisez des axes analytiques à la définition de vues d’analyse et de la création d’états financiers. Pour plus d’informations, consultez [Utiliser les dimensions](finance-dimensions.md).

> [!TIP]
> Pour analyser rapidement les données transactionnelles par dimensions, vous pouvez filtrer les totaux du plan comptable et toutes les entrées de toutes les pages **Entrées** par axes analytiques. Recherchez l’action **Définir le filtre axe**.  

Le tableau suivant décrit une série de tâches dans Financial Reporting et inclut des liens vers les articles qui les décrivent.  

| À | Voir |
| --- | --- |
| Créer de nouveaux états financiers pour définir les déclarations financières aux fins de reporting ou pour les afficher comme graphiques.| [Préparer des états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md)|
| Utilisez des comptes statistiques pour compléter les informations dans les états financiers. Les comptes statistiques vous permettent d’ajouter des mesures basées sur des données non transactionnelles. Vous pouvez ajouter les données non transactionnelles sous forme d’unités basées sur des chiffres, telles que l’effectif des employés, la superficie en pieds carrés ou le nombre de clients ayant des comptes en retard. | [Analyse des données avec les comptes statistiques](bi-use-statistical-accounts.md) |
| Apprenez à configurer un nouveau rapport financier à travers des exemples. | [Procédure pas-à-pas : utilisation des états financiers pour créer de prévisions de trésorerie](walkthrough-making-cash-flow-forecasts-by-using-account-schedules.md) |
| Analyser vos performances financières en définissant des KPI (Indicateurs de performances clés) basés sur les états financiers, que vous publiez ensuite comme services Web. Les KPI des états financiers publiés peuvent être affichés sur un site Web ou être importés dans Microsoft Excel à l’aide des services Web OData. |[Configuration et publication des services Web KPI sur la base d’états financiers](bi-how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules.md) |
| Configurer des vues pour analyser des données à l’aide d’axes.|[Analyse des données par axe analytique](bi-how-analyze-data-dimension.md)|
| Créer de nouveaux rapports d'analyse pour les ventes, les achats et le stock, et configurer des modèles d'analyse. |[Création d’états d’analyse](bi-how-create-analysis-views-reports.md)|

## États financiers entre les divisions ou les entités juridiques

Certaines organisations utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans plusieurs centres de profit ou entités juridiques. D’autres utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans les filiales qui doivent rendre compte aux organisations mères. [!INCLUDE [prod_short](includes/prod_short.md)] fournit aux comptables des outils qui les aident à transférer les écritures comptables de deux ou plusieurs sociétés (filiales) dans une société consolidée.  

Pour en savoir plus, reportez-vous à [Consolidation de la société](finance-consolidated-company-reporting.md).

## Analyse ad hoc des données financières

Parfois, il suffit de vérifier si les chiffres s’additionnent correctement ou de confirmer rapidement un chiffre. Les fonctionnalités suivantes sont idéales pour les analyses ad hoc :

- Analyses des données sur les pages de listes comptables
- Ouvrir dans Excel

La fonction d’analyse des données vous permet d’ouvrir presque une page de liste, telle que les Écritures comptables, les écritures du grand livre des immobilisations, les écritures du grand livre des chèques ou les écritures du grand livre des comptes bancaires, d’entrer en mode analyse, puis de regrouper, filtrer et faire pivoter les données comme bon vous semble. .

:::image type="content" source="media/data-analysis-gl-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures G/L." lightbox="media/data-analysis-gl-entries.png":::

De la même manière, vous pouvez utiliser le **Ouvrir dans Excel** action pour ouvrir une page de liste pour les écritures comptables, éventuellement filtrer la liste sur un sous-ensemble de données, puis utiliser Excel pour travailler avec les données. Par exemple, en utilisant des fonctionnalités telles que l’analyse des données, l’analyse de simulation ou la feuille de prévision.

:::image type="content" source="media/open-in-excel-gl-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures G/L avec Excel." lightbox="media/open-in-excel-gl-entries.png":::

> [!TIP]
> Si vous configuré OneDrive pour les fonctionnalités système, le classeur Excel s’ouvre dans votre navigateur à l’aide d’Excel pour le Web. 


Pour plus d’informations sur la manière d’effectuer une analyse ad hoc sur les grands livres, voir [Analyse ad hoc sur les données financières](ad-hoc-analysis-finance.md). 

## États intégrés pour la finance

[!INCLUDE [prod_short](includes/prod_short.md)] comprend plusieurs rapports, fonctions de traçage et outils incorporés qui aident les auditeurs ou contrôleurs chargés de rendre compte au service financier.

Pour obtenir un aperçu des rapports disponibles, vous pouvez choisir sur **Tous les rapports** dans le volet supérieur de votre page d’accueil. Cette Action ouvre l’explorateur de rôles, qui est filtré selon les fonctionnalités du **Rapport et analyse** option. Pour en savoir plus, voir [Recherche de rapports avec l’explorateur de rôles](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-finance.png" alt-text="Exemple de rapports sur le centre de rôle finance." lightbox="media/report-explorer-finance.png":::

Les rapports intégrés sont disponibles en deux versions :

- Conçu pour l’impression (pdf).
- Conçu pour l’analyse dans Excel.

Pour plus d’informations, consultez ces aperçus pour les rapports pertinents pour la finance.

- [États financiers Excel intégrés](finance-analyze-excel.md)
- [États financiers clés intégrés](finance-reports.md)
- [États sur les immobilisations intégrés](fa-reports.md)
- [États des comptes clients intégrés](receivables-reports.md)
- [États des comptes fournisseurs intégrés](payables-reports.md)

<!-- TODO: add when we have these articles
* [Built-in Cost Accounting reports](cost-accounting-reports.md) 
* [Built-in Cash Management reports](cost-accounting-reports.md) 
* [Built-in Tax and VAT reports](tax-and-vat-reports.md) 
-->

## Pages de tâches financières à l’écran

[!INCLUDE [prod_short](includes/prod_short.md)] comporte plusieurs pages qui vous donnent des aperçus des finances et des tâches à accomplir.

### Afficher les écritures et les soldes du grand livre à partir de la page Plan comptable

La page Plan comptable affiche tous les comptes du grand livre avec des chiffres agrégés comptabilisé dans le grand livre. À partir de cette page, vous pouvez faire des choses comme :  

- Afficher les états qui affichent les écritures comptables et les soldes.  
- Vérifier la liste des groupes comptabilisation pour ce compte.
- Afficher les soldes débit et crédit d’un seul compte.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Exemple de la façon dont la page Plan comptable affiche des informations financières" lightbox="media/chart-of-accounts-page.png":::

Pour en savoir plus, allez à [Familiarisation avec le plan comptable](finance-general-ledger.md#the-chart-of-accounts).

### Afficher les montants réels comparés aux montants budgétés pour tous les comptes et pour plusieurs périodes

Lors de la collecte, l’analyse, et le partage des données de votre société, vous voyez les montants réels comparés aux montants budgétés de tous les comptes et pour plusieurs périodes. Sur la page **Plan comptable** faites la comparaison, choisissez l’action **Réalisé/Budget par compte**.

Pour en savoir plus, voir [Analyser les montants réalisés et les montants budgétés](bi-how-analyze-actual-versus-budget.md).

### Analyse des données par axe analytique

Les axes analytiques sont des valeurs qui permettent de catégoriser les écritures afin de pouvoir les suivre et les analyser sur les documents, tels que les commandes vente. Ils peuvent par exemple indiquer de quel projet ou département provient une écriture.  

Au lieu de configurer des comptes généraux distincts pour chaque service et projet, vous pouvez utiliser les axes analytiques comme base d’analyse et éviter d’avoir à créer une structure de plan comptable compliqué.

En analyse financière, un axe correspond à des données que vous ajoutez à une écriture comptable comme une sorte de marqueur. Ces données permettent de regrouper des écritures comptables dotées de caractéristiques similaires, telles que les clients, les régions, les produits et les commerciaux, et de récupérer facilement ces groupes à des fins d'analyse. Vous pouvez utiliser les axes sur des écritures de feuilles, de documents et de budgets. Pour plus d’informations, reportez vous à [Analyser des données par axe analytique](bi-how-analyze-data-dimension.md)

### Analyse de trésorerie

Dans page d’accueil Comptable, sous **Performances financières**, Cycle trésorerie, Trésorerie et Revenus et dépenses, les graphiques offrent des méthodes pour analyser la trésorerie :

- Vérifier les chiffres pour une période à l’aide du curseur de la chronologie.
- Filtrez le graphique en sélectionnant la source dans la légende.
- Modifiez la durée de la période, ou accédez à la période précédente ou suivante, en choisissant les options du menu déroulant Performances financières.

:::image type="content" source="media/cashflow-accountant-rolecentre.png" alt-text="Exemple de l’apparence des visuels de flux de trésorerie sur le centre de rôle du comptable" lightbox="media/cashflow-accountant-rolecentre.png":::

Pour vérifier la prévision, outre les écritures de prévision, vous pouvez également consulter la feuille d’activité de trésorerie. Par exemple, vous pouvez voir comment les prévisions :

- Gère les ventes et les achats confirmés.
- Retire les dépenses et ajoute les recettes.
- Ignore les commandes ventes et les commandes achats en double.

Pour en savoir plus, accédez à [Analyse de la trésorerie dans votre société](finance-analyze-cash-flow.md).

## Voir aussi

[Gestion des états financiers entre les divisions ou les entités juridiques](finance-consolidated-company-reporting.md)  
<!-- [Financial KPIs in Business Central](bi-finance-kpis.md)    -->
[Préparer des états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md)  
[Analyse ad hoc sur données financières](ad-hoc-analysis-finance.md)   
[Comprendre du plan comptable](finance-general-ledger.md#the-chart-of-accounts)  
[États financiers Excel intégrés](finance-analyze-excel.md)  
[États financiers clés intégrés](finance-reports.md)  
[États sur les immobilisations intégrés](fa-reports.md)  
[États des comptes clients intégrés](receivables-reports.md)  
[États des comptes fournisseurs intégrés](payables-reports.md)  
[Vue d’ensemble de Finances](finance.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)   
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
