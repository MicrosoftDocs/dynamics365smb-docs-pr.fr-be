---
title: Gérer des immobilisations
description: En savoir plus sur la fonctionnalité d’immobilisations et afficher un aperçu de l’utilisation et de la gestion de vos immobilisations.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'machinery, buildings'
ms.search.form: '5604, 5606, 5664, 5601, 5602, 5658, 5603, 5671, 5641, 5629, 5633, 5634, 5649, 5622, 5650'
ms.date: 05/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="manage-fixed-assets"></a>Gérer des immobilisations

Le module Immobilisations dans [!INCLUDE[prod_short](includes/prod_short.md)] offre un aperçu des immobilisations et garantit un amortissement correct. Elle vous aide également de suivre les coûts de maintenance, de gérer les polices d’assurance, de valider les transactions d’immobilisations, et de générer des états et des statistiques variés.

## <a name="what-is-a-fixed-asset"></a>Qu’est-ce qu’une immobilisation ?

Les immobilisations diffèrent des autres articles de votre entrepôt. Une immobilisation, également appelée immobilisation, est une immobilisation corporelle, une usine ou un équipement (PP&E) que vous possédez ou gérez dans l’espoir qu’elle continuera à contribuer à générer des revenus. Un actif est fixe lorsqu’il s’agit d’un article que votre entreprise ne consommera pas, ne vendra pas ou ne convertira pas en espèces au cours de l’année civile suivante. Les immobilisations sont différentes des actifs courants, qui sont en espèces ou devraient être convertis en espèces au cours des 12 prochains mois. Les immobilisations diffèrent également de votre inventaire, car celui-ci est généralement consommé en peu de temps.

## <a name="types-of-fixed-assets"></a>Types d'immobilisations

Les entreprises investissent généralement dans quelques types d’immobilisations. Voici quelques exemples :

- Bâtiments et installations
- Matériel informatique et logiciels
- Meubles et accessoires
- Machine
- Véhicules

## <a name="understanding-fixed-asset-accounting"></a>Comprendre la comptabilité des immobilisations

La comptabilité des immobilisations signifie tenir des registres financiers précis sur vos immobilisations. Ces enregistrements incluent des détails sur les cinq étapes du cycle de vie d’un actif. Après votre achat initial, le cycle de vie de chaque immobilisation comprend au moins trois des étapes suivantes :

- Acquisition : Vous ajoutez une nouvelle immobilisation à vos livres.
- Amortissement : vous enregistrez la baisse de valeur périodique d’un actif, que vous utilisez une méthode d’amortissement pour calculer. Pour en savoir plus, consultez [Calcul Amortissement immo.](LocalFunctionality/India/FA_Depreciation.md).
- Réévaluation : vous enregistrez une évaluation de la juste valeur marchande actuelle d’un actif. Pour en savoir plus, accédez à [Réévaluer des Immobilisations](fa-how-revalue.md).
- Dépréciation : Vous constatez une réduction de valeur due à des événements ou des circonstances.
- Élimination : vous vendez, mettez au rebut ou utilisez d’une autre manière l’élimination d’un actif à la fin de sa durée de vie.

Les audits s’inscrivent également dans les contrôles détaillés des écritures comptables de votre entreprise après la clôture des comptes de l’exercice. Qu’ils soient internes ou externes, les audits sont l’endroit où vous pourriez remarquer des incohérences ou des différences entre vos notes et l’état réel de vos actifs. Les audits favorisent la transparence de vos actifs et de votre comptabilité si vous perdez plus d’argent que prévu.

## <a name="video-overview"></a>Présentation de la vidéo

La vidéo suivante couvre les notions de base des immobilisations :

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4AegS?rel=0]

## <a name="initial-setup-of-fixed-assets"></a>Configuration initiale des immobilisations

Avant de pouvoir gérer les immobilisations, vous devez effectuer les configurations suivantes :

- Valeur par défaut
- Comptabilité immobilisations
- Groupes et types comptabilisation
- Clés de ventilation
- Feuilles immobilisation

Pour en savoir plus, accédez à [Configuration des Immobilisations](fa-setup.md).

## <a name="fixed-assets-analytics"></a>Analyse des immobilisations

Cette section décrit les outils analytiques que vous pouvez utiliser pour obtenir des informations dans vos données sur vos Immobilisations.

| Pour... | Voir |
| --- | --- |
| Découvrez les fonctionnalités d’analyse des données sur les immobilisations. | [Vue d’ensemble de l’analyse des immobilisations](fa-analytics-overview.md) |
| Effectuez une analyse ad hoc des données Immobilisations directement sur les pages de liste et les requêtes. | [Analyse ad hoc des données Immobilisations](ad-hoc-analysis-fa.md) |
| Explorez états intégrés sur les immobilisations. | [États sur les immobilisations intégrés](fa-reports.md) |
| Surveillance des coûts de maintenance. | [Surveillance des coûts de maintenance](fa-how-maintain.md#monitor-maintenance-costs)|
| Surveillance des couvertures d’assurance. | [Surveillance des couvertures d’assurance](fa-how-insure.md#to-monitor-insurance-coverage) |
| Afficher des écritures comptables cession. | [Affichage des écritures comptables cession](fa-how-dispose-retire.md#to-view-disposal-ledger-entries) |
| Visualiser des valeurs de cession prévues. | [Affichage des valeurs de cession prévues](fa-how-manage-budgets.md#to-view-projected-disposal-values) |

## <a name="register-fixed-assets"></a>Enregistrer Immobilisations

Pour chaque immobilisation, vous devez créer une fiche contenant des informations les concernant. Par exemple, vous pouvez paramétrer les bâtiments ou le matériel de production en tant qu'actifs principale avec une liste de composants. Vous pouvez regrouper les actifs de différentes manières par exemple, par classe, par département ou par emplacement. Puis, vous pouvez acquérir, maintenir et commercialiser les immobilisations. Vous pouvez également paramétrer des immobilisations budgétées. La budgétisation vous permet par exemple d’inclure dans des états des acquisitions et des ventes anticipées.

| À  | Voir |
| --- | --- |
| Gérer les budgets d’immobilisations, budgéter les coûts d’acquisition, les cessions d’immobilisations et l’amortissement. |[Gestion des budgets pour les immobilisations](fa-how-manage-budgets.md) |
| Créer des immobilisations, affecter des méthodes d'amortissement, valider des acquisitions et des valeurs résiduelles et imprimer les listes d'immobilisations. |[Acquisition des immobilisations](fa-how-acquire.md) |

## <a name="set-up-depreciations-for-your-fixed-assets"></a>Configurer les Amortissement des immobilisations

Pour suivre des amortissements d’immobilisations et d'autres transactions financières pour les immobilisations, vous configurez une, voire plusieurs lois d’amortissements pour chacune. Voici quelques étapes pour amortir les actifs :

1. Exécuter un état qui calculer l'amortissement périodique.
1. Renseignez une feuille avec les écritures résultant.
1. Validez la feuille.

[!INCLUDE[prod_short](includes/prod_short.md)] prend en charge plusieurs méthodes d’amortissement. Pour en savoir plus, consultez [Méthodes amortissement](fa-depreciation-methods.md). Vous pouvez configurer plusieurs lois d’amortissement pour chaque immobilisation à différentes fins, telles qu’une pour la déclaration fiscale, et une autre pour les états internes.

| À  | Voir |
| --- | --- |
| En savoir plus sur les différentes méthodes d’amortissement des immobilisations. |[Méthodes d’amortissement](fa-depreciation-methods.md) |
| Calculer l’amortissement, valider l’amortissement et analyser l’amortissement dans les états sur les immobilisations. |[Amortissement des immobilisations](fa-how-depreciate-amortize.md) |
| Afficher les valeurs comptables d’amortissement modifiées. | [Affichage des valeurs de la loi d’amortissement modifiées](fa-how-trans-split-combine.md#to-view-changed-depreciation-book-values-due-to-fixed-asset-reclassification) |
| Enregistrer les transactions immobilisation manuellement sur la page **Feuille compta. immo.** ou sur la page **Feuille immo.**, selon que les transactions sont destinées pour des rapports financiers ou pour la gestion interne. | [Configuration des amortissements](fa-how-setup-depreciation.md) |

## <a name="fixed-assets-maintenance-and-insurance"></a>Entretien et assurance des immobilisations

Enregistrer des coûts de maintenance et la date de la prochaine visite d'entretien pour chaque actif. Le suivi des frais de maintenance peut être utile dans le cadre de l’élaboration du budget et de la prise de décisions concernant le remplacement éventuel d’une immobilisation. Vous pouvez rattacher chaque immobilisation à une ou plusieurs polices d’assurance et vérifier que les primes des polices correspondent à la valeur des actifs.

| À  | Voir |
| --- | --- |
| Enregistrer les visites de service, valider les coûts de maintenance et surveiller les coûts de maintenance. |[Mise à jour des immobilisations](fa-how-maintain.md) |
| Surveillance des coûts de maintenance. | [Surveillance des coûts de maintenance](fa-how-maintain.md#monitor-maintenance-costs)|
| Mettre à jour les informations d’assurance, valider les coûts d’acquisition vers les polices d’assurance, modifier la couverture assurance, visualiser les statistiques assurance et répertorier les polices d’assurance. |[Assurance des immobilisations](fa-how-insure.md) |
| Surveillance des couvertures d’assurance. | [Surveillance des couvertures d’assurance](fa-how-insure.md#to-monitor-insurance-coverage) |

## <a name="reclassify-transfer-split-upcombine-adjust-value-write-down-and-dispose-fixed-assets"></a>Reclasser, transférer, diviser/regrouper, ajuster la valeur, déprécier et céder des immobilisations

| À  | Voir |
| --- | --- |
| Reclasser les immobilisations, les transférer vers d'autres emplacements, les diviser ou les combiner. |[Transférer, fractionner ou regrouper les immobilisations](fa-how-trans-split-combine.md) |
| Ajuster les valeurs des immobilisations, valider les réévaluations et les transactions de dépréciation. |[Réévaluation des immobilisations](fa-how-revalue.md) |
| Valider les transactions de cession, visualiser les écritures comptables cession et valider les cessions partielles. |[Cession ou annulation des immobilisations](fa-how-dispose-retire.md) |
| Afficher des écritures comptables cession. | [Affichage des écritures comptables cession](fa-how-dispose-retire.md#to-view-disposal-ledger-entries) |
| Visualiser des valeurs de cession prévues. | [Affichage des valeurs de cession prévues](fa-how-manage-budgets.md#to-view-projected-disposal-values) |

## <a name="tips-for-improving-your-fixed-asset-accounting"></a>Conseils pour améliorer votre comptabilité des immobilisations

Il existe quelques éléments que vous pouvez mettre en œuvre dans votre stratégie comptable pour les immobilisations et qui peuvent vous aider à maximiser vos revenus.

- Établir un seuil de capitalisation. Lorsque vous achetez un article, déterminez un montant fixe pour la capitalisation. Le montant permet de garantir la cohérence de vos livres comptables et permet à vous et à votre équipe de repérer plus facilement les erreurs comptables.
- Réévaluer le cycle de vie des équipements. Il est important d’estimer correctement la durée pendant laquelle vous pouvez utiliser vos immobilisations aux fins prévues à l’origine. Étant donné que la comptabilité et l’amortissement reposent sur des estimations précises du cycle de vie, réévaluez-les si nécessaire, car cela peut changer au fil du temps.
- Marquez vos actifs. Il est essentiel de suivre et d’étiqueter vos actifs tout au long de leur cycle de vie, car de nombreux facteurs peuvent affecter leur valeur. L’étiquetage permet de suivre vos objets tout au long des étapes de leur cycle de vie, de prévenir le vol, d’éliminer les erreurs de placement et de prendre en charge les statistiques financières.
- Automatisez les informations avec un logiciel de comptabilité des immobilisations. L’automatisation des activités manuelles pour suivre vos données avec un logiciel de comptabilité des immobilisations facilite la réalisation des processus. La protection par mot de passe peut contribuer à fournir un accès uniquement aux personnes qui en ont besoin et qui sont formées à cet effet.

## <a name="see-also"></a>Voir aussi

[Paramétrage d’immobilisations](fa-setup.md)  
[Vue d’ensemble de l’analyse des immobilisations](fa-analytics-overview.md)  
[Vue d’ensemble de Finance](finance.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Modification des fonctionnalités affichées](ui-experiences.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
