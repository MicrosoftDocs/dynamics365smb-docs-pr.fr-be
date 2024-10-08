---
title: 'Vue d''ensemble Analyses, business intelligence et reporting'
description: 'Fournit une vue d’ensemble de toutes les fonctionnalités analyse, de Business Intelligence et de création de rapports prises en charge dans le produit Business Central.'
author: KennieNP
ms.topic: get-started
ms.devlang: al
ms.search.keywords: feature overview
ms.reviewer: bholtorf
ms.date: 09/22/2022
ms.author: kepontop
ms.service: dynamics-365-business-central
---

# <a name="analytics-business-intelligence-and-reporting-overview"></a>Vue d'ensemble Analyses, business intelligence et reporting

Les petites et moyennes entreprises répondent sur des analyses et des rapports intégrés qu’elles peuvent utiliser prêts à l’emploi pour aider à suivre leur activité. [!INCLUDE[prod_short](includes/prod_short.md)] fournit des rapports et des outils d’analyse qui couvrent les processus commerciaux de base et complexes pour ces organisations. Vous pouvez également effectuer des analyses ad hoc directement depuis votre page d’accueil.  

## <a name="analytics-needs-in-organizations"></a>Besoins analytiques en organisations

Lorsque l’on réfléchit aux besoins d’analyse en organisations, il peut être utile d’utiliser un modèle mental basé sur des personnalités décrites à un niveau élevé et leurs différents besoins en matière d’analyse.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration de différents personnages pour l’analyse" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

Le modèle est basé sur le fait que différents rôles dans une organisation ont des besoins différents en matière de données. Plus un rôle est placé haut dans l’organigramme, plus la personne occupant ce rôle a besoin de données agrégées pour effectuer son travail.

Les rôles ont souvent des méthodes privilégiées pour consommer et analyser les données, des méthodes qui reflètent le niveau d’agrégation des données dont ils ont besoin.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration de la manière dont différentes personnes ont des besoins analytiques différents." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

Utilisez les sections suivantes pour en savoir plus sur les façons de consommer les données de [!INCLUDE[prod_short](includes/prod_short.md)] :

- États financiers
- KPI et tableaux de bord
- Analyse ad hoc
- États

## <a name="using-financial-reports-to-produce-financial-statements-and-kpis"></a>Utilisation États financiers pour produire des états financiers et des indicateurs de performance clés

La fonctionnalité états financiers vous donnent un aperçu des données financières enregistrées dans votre plan comptable (COA). Configurez les états financiers pour analysent les chiffres de la comptabilité et comparent les écritures comptables et les écritures comptables budget.

:::image type="content" source="media/acc_schedule_13_columns.jpg" alt-text="Capture d’écran d’un rapport financiers." lightbox="media/acc_schedule_13_columns.jpg":::

Les axes jouent un rôle important dans la veille économique. Un axe correspond à des données que vous pouvez ajouter à une écriture en tant que paramètre. Les dimensions vous permettent de regrouper les entrées présentant des caractéristiques similaires. Par exemple, groupes clients, régions, vos produits et vendeurs. Les groupes facilitent la récupération des données à des fins d’analyse. Entre autres objectifs, vous utilisez des axes analytiques à la définition de vues d’analyse et de la création d’états financiers. Pour plus d’informations, consultez [Utiliser les dimensions](finance-dimensions.md).

Pour en savoir plus sur les états financiers et les KPI, consultez [Utiliser les états financiers pour produire des états financiers et des KPI](bi.md).

## <a name="using-key-performance-indicators-to-meet-your-business-goals"></a>Utilisation d’indicateurs de performance clés pour répondre aux objectifs de votre entreprise

Un indicateur de performance clé (KPI) est une valeur mesurable qui montre l’efficacité avec laquelle vous atteignez vos objectifs. Considérez les KPI comme le tableau de bord de votre entreprise, un moyen de mesurer si vous atteignez vos objectifs.

L’identification et le suivi des KPI vous permettent de savoir si votre entreprise est sur la bonne voie ou si vous devez changer de cap. Lorsqu’ils sont utilisés correctement, les KPI sont des outils puissants qui vous aident à :

- Surveiller la santé financière de l’entreprise.
- Mesurer les progrès par rapport aux objectifs stratégiques.
- Repérez les problèmes dès le début.
- Apportez des ajustements opportuns aux tactiques.
- Motiver les membres de l’équipe.
- Prendre de meilleures décisions, plus rapidement.

Pour en savoir plus sur les KIP, alle zà [Utilisation d’indicateurs de performance clés pour répondre aux objectifs de votre entreprise](./analytics-about-kpis.md)

## <a name="ad-hoc-data-analysis"></a>Analyse de données ad hoc

Vous souhaiterez peut-être simplement vérifier si les chiffres s’additionnent correctement, confirmer ou infirmer rapidement une hypothèse sur l’entreprise, ou peut-être rechercher des anomalies dans vos données financières. Pour les analyses ad hoc, il se peut que vous ne disposiez pas d’un rapport intégré permettant de répondre à vos questions. Pour les analyses ad hoc, utilisez ces deux fonctionnalités :

- Analyses des données sur les pages de listes comptables
- Ouvrir dans Excel

La fonction d’analyse des données vous permet d’ouvrir presque toutes page de liste, telle que les Écritures comptables, les écritures du grand livre, d’entrer en mode analyse, puis de regrouper, filtrer et faire pivoter les données comme bon vous semble. 

:::image type="content" source="media/data-analysis-gl-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures G/L." lightbox="media/data-analysis-gl-entries.png":::

De la même manière, vous pouvez utiliser le **Ouvrir dans Excel** action pour ouvrir une page de liste, éventuellement filtrer la liste sur un sous-ensemble de données, puis utiliser Excel pour travailler avec les données. Par exemple, en utilisant des fonctionnalités telles que l’analyse des données, l’analyse de simulation ou la feuille de prévision.

:::image type="content" source="media/open-in-excel-gl-entries.png" alt-text="Exemple de comment effectuer une analyse des données sur la page des écritures G/L avec Excel." lightbox="media/open-in-excel-gl-entries.png":::

> [!TIP]
> Si vous configuré OneDrive pour les fonctionnalités système, le classeur Excel s’ouvre dans votre navigateur à l’aide d’Excel pour le Web.

Pour en savoir plus sur les analyses ad hoc, accédez à [Analyse de données ad hoc](reports-adhoc-analysis.md).

## <a name="reports"></a>États

Un rapport dans [!INCLUDE[prod_short](includes/prod_short.md)] rassemble des informations en fonction d’un ensemble spécifié de critères. Les états organise et présente les informations dans un format facile à lire que vous pouvez utiliser dans Excel, imprimer ou enregistrer sous forme de fichier.  

À titre d’exemple de rapport interactif dans Excel, le rapport ***Agenda des comptes clients** vous permet d’analyser ce que vos clients vous doivent et la date d’échéance des paiements.

:::image type="content" source="media/aged-accounts-receivables-excel.png" alt-text="Exemple de rapport interactif sur les comptes clients chronologiques dans Excel." lightbox="media/aged-accounts-receivables-excel.png":::

Pour les comptes clients anciens, [!INCLUDE[prod_short](includes/prod_short.md)] comprend également un rapport conçu pour l’impression. La possibilité d’imprimer est pratique si vous préférez avoir les données dans un fichier .pdf.

:::image type="content" source="media/aged-accounts-receivables-pdf.png" alt-text="Exemple de rapport sur les comptes clients chronologiques dans PDF." lightbox="media/aged-accounts-receivables-pdf.png":::

[!INCLUDE[prod_short](includes/prod_short.md)] est livré avec plus de 300 rapports intégrés que vous pouvez utiliser pour soutenir vos processus métier avec des informations basées sur les données. Pour obtenir un aperçu rapide de tous les rapports disponibles pour votre rôle, vous pouvez ouvrir l’explorateur de rapports depuis le centre de rôles et toutes les pages de liste et depuis **Dites-moi**.

:::image type="content" source="media/report-explorer-finance.png" alt-text="Exemple de la façon dont l’explorateur de rapports affiche tous les rapports pour un rôle." lightbox="media/report-explorer-finance.png":::

Pour en savoir plus sur l’utilisation de l’explorateur de rapports afin d’afficher tous les rapports intégrés, accédez à [Exploration des rapports par rôle](ui-role-explorer.md).

Le tableau suivant répertorie les articles sur l’utilisation des rapports intégrés dans [!INCLUDE[prod_short](includes/prod_short.md)].

| À  | Voir |
| --- | --- |
| Apprenez à utiliser des rapports (marquer, exécuter, imprimer, planifier et modifier la mise en page). | [Utilisation des rapports dans le travail quotidien](reports-use-reports.md) |
| En savoir plus sur les rapports intégrés disponibles dans [!INCLUDE[prod_short](includes/prod_short.md)]. |[Vue d’ensemble du rapport](reports-available-reports.md)| 
| Utilisez l’Explorateur de rapports pour voir tous les rapports intégrés. | [Explorer les rapports par rôle](ui-role-explorer.md) |

## <a name="external-business-intelligence-and-reporting-tools"></a>Business Intelligence externe et outils de reporting

Si vous préférez, vous pouvez utiliser des outils de BI qui ne sont pas intégrés [!INCLUDE[prod_short](includes/prod_short.md)]. Le tableau suivant fournit des liens vers des conseils et des façons d’utiliser des outils externes.

| À  | Voir |
| --- | --- |
| Utiliser Power BI avec les données Business Central | [Utilisation de Power BI avec Business Central](admin-powerbi.md) |
| Intégrer des outils de veille économique externes avec [!INCLUDE[prod_short](includes/prod_short.md)].| [Outils externes de Business Intelligence](reports-external-analysis.md) |
| Extraction de données vers des entrepôts de données ou des lacs de données| [Comment extraction de données vers des entrepôts de données ou des lacs de données](/dynamics365/business-central/dev-itpro/performance/performance-developer#efficient-extracts-to-data-lakes-or-data-warehouses) |
| Analyser les données Business Central dans Microsoft Fabric| [Introduction à Microsoft Fabric et Business Central](admin-fabric.md) |
| Lire les données métier à partir de Business Central avec API | [Business Central API v2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/) |

## <a name="analytics-by-functional-area"></a>Analyses par domaine fonctionnel

Le contenu de cet article général est également disponible dans des versions spéciales pour de nombreux domaines fonctionnels [!INCLUDE[prod_short](includes/prod_short.md)].

| Utilisation de... | Voir |
| --- | --- |
| Finances | [Analyses financières](bi.md) |
| Vente | [Analyse vente](sales-analytics-overview.md) |
| Achats | [Analyse des achats](purchasing-analytics-overview.md) |
| Gestion des immobilisations | [Analyse des immobilisations](fa-analytics-overview.md) |


## <a name="see-also"></a>Voir aussi

[Utilisation États financiers pour produire des états financiers et des indicateurs de performance clés](bi.md)  
[Utilisation d’indicateurs de performance clés pour répondre aux objectifs de votre entreprise](analytics-about-kpis.md)  
[Analyse de données ad hoc](reports-adhoc-analysis.md)  
[Utilisation des rapports dans le travail quotidien](reports-use-reports.md)  
[Présentation des rapports intégrés](reports-available-reports.md)  
[Explorer les rapports par rôle](ui-role-explorer.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
