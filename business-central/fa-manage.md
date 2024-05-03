---
title: Gérer les immobilisations (contient une vidéo)
description: En savoir plus sur la fonctionnalité d’immobilisations et afficher un aperçu de l’utilisation et de la gestion de vos immobilisations.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: conceptual
ms.search.keywords: 'machinery, buildings'
ms.search.form: '5604, 5606, 5664, 5601, 5602, 5658, 5603, 5671, 5641, 5629, 5633, 5634, 5649, 5622, 5650'
ms.date: 03/25/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="manage-fixed-assets"></a>Gérer des immobilisations

Le module Immobilisations dans [!INCLUDE[prod_short](includes/prod_short.md)] offre un aperçu des immobilisations et garantit un amortissement périodique correct. Elle vous permet également de connaître les coûts de maintenance, de gérer les polices d’assurance, de valider les transactions d’immobilisations, et de générer des états et des statistiques variés.

## <a name="video-overview"></a>Présentation de la vidéo

La vidéo suivante couvre les notions de base des immobilisations :

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4AegS?rel=0]

## <a name="fixed-assets-overview"></a>Vue d’ensemble des immobilisations

Pour chaque immobilisation, vous devez créer une fiche contenant des informations la concernant. Vous pouvez configurer des bâtiments ou un équipement de production en tant qu’actif principal avec une liste de composants et vous pouvez les regrouper de différentes façons, comme par catégorie, département ou emplacement. Puis, vous pouvez commencer à acquérir, maintenir et commercialiser les immobilisations. Vous pouvez également paramétrer des immobilisations budgétées. La budgétisation vous permet par exemple d’inclure dans des états des acquisitions et des ventes anticipées.

> [!IMPORTANT]
> Avant de pouvoir gérer les immobilisations, vous devez effectuer les configurations suivantes :
>
> * Valeur par défaut
> * Comptabilité immobilisations
> * Groupes comptabilisation
> * Clés de ventilation
> * Feuilles immobilisation
>
> Pour plus d’informations, reportez-vous à [Paramétrage d’immobilisations](fa-setup.md).

Pour suivre des amortissements d’immobilisations et d'autres transactions financières pour les immobilisations, vous configurez une, voire plusieurs lois d’amortissements pour chacune. L’amortissement est effectué en exécutant un état afin de calculer l’amortissement périodique et compléter une feuille avec les écritures résultantes, puis valider la feuille. [!INCLUDE[prod_short](includes/prod_short.md)] prend en charge plusieurs méthodes d’amortissement. Pour en savoir plus, voir [Méthodes d’amortissement](fa-depreciation-methods.md). Vous pouvez configurer plusieurs lois d’amortissement par immobilisation à différentes fins, telles qu’une pour la déclaration fiscale, et une autre pour les états internes.

Pour chaque immobilisation, vous pouvez enregistrer des coûts de maintenance et la date de la prochaine visite d'entretien. Le suivi des frais de maintenance peut être utile dans le cadre de l’élaboration du budget et de la prise de décisions concernant le remplacement éventuel d’une immobilisation.

Vous pouvez rattacher chaque immobilisation à une ou plusieurs polices d’assurance et vérifier que les primes des polices correspondent à la valeur des actifs.

> [!NOTE]  
> Vous pouvez enregistrer les transactions immobilisation sur la page **Feuille compta. immo.** ou sur la page **Feuille immo.**, selon que les transactions sont destinées pour des rapports financiers ou pour la gestion interne. L’aide pour les immobilisations décrit uniquement la procédure d’utilisation de la page **Feuille compta. immo.**. Pour en savoir plus, voir [Configurer l’amortissement d’immobilisation](fa-how-setup-depreciation.md).

## <a name="how-to-use-fixed-assets"></a>Utilisation des immobilisations

Le tableau suivant décrit une série de tâches et inclut des liens vers les articles qui les décrivent.

| À  | Voir |
| --- | --- |
| Paramétrez les conditions préalables de la fonctionnalité des immobilisations (en définissant les valeurs par défaut, la comptabilité des immobilisations, les groupes comptabilisation, les clés de ventilation, les feuilles et les types de validation). | [Paramétrage d’immobilisations](fa-setup.md)|
| Créer des immobilisations, affecter des méthodes d'amortissement, valider des acquisitions et des valeurs résiduelles et imprimer les listes d'immobilisations. |[Acquérir des immobilisations](fa-how-acquire.md) |
| Enregistrer les visites de service, valider les coûts de maintenance et surveiller les coûts de maintenance. |[Mettre à jour des immobilisations](fa-how-maintain.md) |
| Mettre à jour les informations d’assurance, valider les coûts d’acquisition vers les polices d’assurance, modifier la couverture assurance, visualiser les statistiques assurance et répertorier les polices d’assurance. |[Assurer les immobilisations](fa-how-insure.md) |
| Reclasser les immobilisations, les transférer vers d’autres emplacements, les diviser ou les combiner. |[Transférer, fractionner ou regrouper les immobilisations](fa-how-trans-split-combine.md) |
| Ajuster les valeurs des immobilisations, valider les réévaluations et les transactions de dépréciation. |[Réévaluer les immobilisations](fa-how-revalue.md) |
| Calculer l’amortissement, valider l’amortissement et analyser l’amortissement dans les états sur les immobilisations. |[Amortissement des immobilisations](fa-how-depreciate-amortize.md) |
| En savoir plus sur les différentes méthodes d’amortissement des immobilisations. |[Méthodes d’amortissement](fa-depreciation-methods.md) |
| Valider les transactions de cession, visualiser les écritures comptables cession et valider les cessions partielles. |[Céder ou annuler des immobilisations](fa-how-dispose-retire.md) |
| Gérer les budgets d’immobilisations, budgéter les coûts d’acquisition, les cessions d’immobilisations et l’amortissement. |[Gestion des budgets pour les immobilisations](fa-how-manage-budgets.md) |
| Apprenez-en davantage sur les fonctionnalités intégrées de reporting et d’analyse pour les immobilisations. | [États et analyses des immobilisations](fa-reports.md) |

## <a name="see-also"></a>Voir aussi

[Paramétrage d’immobilisations](fa-setup.md)  
[Vue d’ensemble de Finances](finance.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Modification des fonctionnalités affichées](ui-experiences.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]
