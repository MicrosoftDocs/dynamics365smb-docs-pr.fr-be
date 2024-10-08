---
title: Analyses dans achats
description: "Business\_Central contient un de nombreuses fonctionnalités pour vous aider à collecter, analyser et partager des données précieuses pour BI et la prise de décision dans l'organisation achats."
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '9306, 9307, 518, 29'
ms.date: 04/29/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="analytics-in-purchasing"></a>Analyses dans achats

Les entreprises capturent des lots de données au cours de leurs activités quotidiennes, ce qui soutient une précieuse BI pour les gestionnaires d'achats :

- Demandes de prix
- Commandes achat
- Factures achat

[!INCLUDE[prod_short](includes/prod_short.md)] fournit de nombreuses fonctionnalités pour vous aider à collecter, analyser et partager les données d'achat de votre société :

- Analyse ad hoc sur les listes
- Analyse ad hoc des données dans Excel (en utilisant open dans Excel)
- États de vente intégrés

Chacune de ces fonctionnalités présente ses avantages et inconvénients, selon le type d’analyse des données et le rôle de l’utilisateur. Pour en savoir plus, consultez [Analyse, Business Intelligence et Reporting](reports-bi-reporting.md).

Cet article vous présente comment d’utiliser ces fonctionnalités analytiques pour obtenir des informations achats.

## <a name="analytics-needs-in-purchasing"></a>Besoins analytiques en achats

Lorsque l’on réfléchit aux besoins d’analyse en achats, il peut être utile d’utiliser un modèle basé sur une personne décrites à un niveau élevé des différents besoins en matière d’analyse.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration de différents personnages pour l’analyse" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

Les personnes occupant différents rôles ont des besoins différents en matière de données et utilisent les données de différentes manières. Par exemple, les professionnels de la gestion de patrimoine et de la finance interagissent avec les données différemment des professionnels de la vente.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration de la manière dont différentes personnes ont des besoins analytiques différents." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Rôle              | Agrégation de données  | Façons typiques de consommer des données                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|COO / CSO / CFO / CEO    | Données performances  | Indicateurs de performance clés <br> Tableaux de bord <br> États financiers           |
|gestionnaire des achats.      | Tendances, résumés | États managériaux prédéfinis <br> Analyse ad hoc      | 
|Chargé d’achat / Agent d’achat | Informations détaillées     | États exploitation prédéfinis <br> Données de tâche à l’écran |

<!-- 
## <a name="purchasing-kpis"></a>Purchasing KPIs

A key performance indicator (KPI) is a measurable value that shows how effectively you’re meeting your goals. In purchasing management, people often use the following KPIs to monitor their organization's purchasing performance:

- TODO  
-->

## <a name="use-financial-reporting-to-produce-financial-statements-and-kpis-related-to-purchasing"></a>Utilisation États financiers pour produire des états financiers et des indicateurs de performance clés (associés à achats)

La fonctionnalité **Financial Reporting** vous donne un aperçu des données financières enregistrées dans votre plan comptable (COA). Configurez les états financiers pour analysent les chiffres de la comptabilité et comparent les écritures comptables et les écritures comptables budget. Spécifiquement pour les achats, vous pouvez configurer des rapports financiers sur les comptes du comptabilité (G/L) que vous utilisez pour suivre les validations d’achat.

Les axes jouent un rôle important dans la veille économique. Un axe correspond à des données que vous pouvez ajouter à une écriture en tant que paramètre. Les axes vous permettent de regrouper des écritures dotées de caractéristiques similaires, telles que les clients, les régions et les produits et de récupérer facilement ces groupes à des fins d’analyse. Entre autres objectifs, utilisez des axes analytiques à la définition de vues d’analyse et de la création d’états financiers. Pour plus d’informations, consultez [Utiliser les dimensions](finance-dimensions.md).

Pour en savoir plus sur les états financiers, accédez à [Préparer des états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md).

## <a name="finance-reporting-across-business-units-or-legal-entities-related-to-purchasing"></a>États financiers entre les divisions ou les entités juridiques (associé à achats)

Certaines organisations utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans plusieurs centres de profit ou entités juridiques. D’autres utilisent [!INCLUDE [prod_short](includes/prod_short.md)] dans les filiales qui rendre compte aux organisations mères. [!INCLUDE [prod_short](includes/prod_short.md)] fournit aux comptables des outils qui les aident à transférer les écritures comptables de deux ou plusieurs sociétés (filiales) dans une société consolidée. Spécifiquement pour la gestion des achats, vous souhaiterez peut-être consolider les écritures comptabilité pour vos comptes d’achats afin de suivre les KPI de vente dans les unités commerciales ou les entités juridiques.

Pour en savoir plus, reportez-vous à [Consolidation de la société](finance-consolidated-company-reporting.md).

## <a name="ad-hoc-analysis-of-purchasing-data"></a>Analyse ad hoc des données achats

Parfois, il suffit de vérifier si les chiffres s’additionnent correctement ou de confirmer rapidement un chiffre. Les fonctionnalités suivantes sont idéales pour les analyses ad hoc :

- Analyses des données sur les pages de listes comptables
- Ouvrir dans Excel

La fonction **d’analyse des données** vous permet d’ouvrir presque toutes page de liste, telle que les **Commande achat**, **factures achats validées**, **Écritures comptables fournisseur** ou **les écritures comptables**, d’entrer en mode analyse, puis de regrouper, filtrer et faire pivoter les données comme bon vous semble.

:::image type="content" source="media/data-analysis-vendor-ledger-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures comptables" lightbox="media/data-analysis-vendor-ledger-entries.png":::

De la même manière, vous pouvez utiliser le **Ouvrir dans Excel** action pour ouvrir une page de liste, filtrer la liste sur un sous-ensemble de données, puis utiliser Excel pour travailler avec les données. Par exemple, en utilisant des fonctionnalités telles que l’analyse des données, l’analyse de simulation ou la feuille de prévision.

:::image type="content" source="media/open-in-excel-vendor-ledger-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures comptables avec Excel." lightbox="media/open-in-excel-vendor-ledger-entries.png":::

> [!TIP]
> Si vous configuré OneDrive pour les fonctionnalités système, le classeur Excel s’ouvre dans votre navigateur.

Pour en savoir plus sur la manière d’effectuer une analyse ad hoc des données d’achat, accédez à [Analyse ad hoc des données d’achat](ad-hoc-analysis-purchasing.md).

## <a name="built-in-reports-for-purchasing"></a>États intégrés pour l'achat

[!INCLUDE [prod_short](includes/prod_short.md)] comprend plusieurs rapports intégrés, fonctions de traçage et outils pour aider les organisations d’achat à créer des rapports sur leurs données.

Pour obtenir un aperçu des rapports disponibles, choisir sur **Tous les rapports** en haut de votre page d’accueil. Cette Action ouvre l’explorateur de rôles, qui est filtré selon les fonctionnalités du **Rapport et analyse** option. Pour en savoir plus, voir [Recherche de rapports avec l’explorateur de rôles](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-purchasing.png" alt-text="Exemple de rapports sur le centre de rôle XXX." lightbox="media/report-explorer-purchasing.png":::

<!-- Built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel. -->

Pour en savoir plus sur les rapports pertinents pour les achats, accédez aux [Rapports d’achat intégrés](purchase-reports.md).

## <a name="on-screen-purchasing-analytics"></a>Analyse des achats à l’écran

[!INCLUDE [prod_short](includes/prod_short.md)] comporte plusieurs pages qui vous donnent des aperçus des achats et des tâches à accomplir. Voici un exemple pour commencer :

- [Afficher la disponibilité des articles](inventory-how-availability-overview.md)  
- [Calculer les dates des achats](purchasing-date-calculation-for-purchases.md)
- [Affichage des écritures comptables d’achat](purchasing-how-record-purchases.md#viewing-ledger-entries)


### <a name="show-purchasing-related-general-ledger-entries-and-balances-from-the-chart-of-accounts-page"></a>Afficher les écritures comptables et les soldes liés aux achats à partir de la page Plan comptable

La page Plan comptable affiche tous les comptes du grand livre avec des chiffres agrégés comptabilisé dans le grand livre. À partir de cette page, vous pouvez faire des choses comme :  

- Afficher les états qui affichent les écritures comptables et les soldes.  
- Vérifier la liste des groupes comptabilisation pour ce compte.
- Afficher les soldes débit et crédit d’un seul compte.

Spécifiquement pour les achats, vous pouvez créer une vue sur la page Plan comptable qui affiche uniquement les comptes que vous utilisez pour valider les écritures d’achat.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Exemple de la façon dont la page Plan comptable affiche des informations financières" lightbox="media/chart-of-accounts-page.png":::

Pour en savoir plus, allez à [Familiarisation avec le plan comptable](finance-general-ledger.md#the-chart-of-accounts).

### <a name="analyze-data-by-dimensions-related-to-purchasing"></a>Analyse des données par axe analytique (lié aux achats)

Les axes analytiques sont des valeurs qui permettent de catégoriser les écritures afin de pouvoir les suivre et les analyser sur les documents, tels que les commandes achat. Ils peuvent par exemple indiquer de quel projet ou département provient une écriture.  

Au lieu de configurer des comptes généraux distincts pour chaque service ou Emplacement, vous pouvez utiliser les axes analytiques comme base d’analyse et éviter d’avoir à créer une structure de plan comptable compliqué.

Pour plus d’informations, consultez [Analyse des données par axe analytique](bi-how-analyze-data-dimension.md).

## <a name="see-also"></a>Voir aussi

[Consolidation de la société](finance-consolidated-company-reporting.md)  
[Préparer des états financiers avec des données financières et des catégories de compte](bi-how-work-account-schedule.md)  
[Gestion des états financiers entre les divisions ou les entités juridiques](finance-consolidated-company-reporting.md)  
[Analyse ad hoc des données achats](ad-hoc-analysis-purchasing.md)  
[États achats intégrés](purchase-reports.md)  
[Comprendre du plan comptable](finance-general-ledger.md#the-chart-of-accounts)  
[Analyse des données par axe analytique](bi-how-analyze-data-dimension.md)  
[Vue d'ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
