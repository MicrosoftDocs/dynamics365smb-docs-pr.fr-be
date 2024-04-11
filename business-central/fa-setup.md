---
title: Configurer des immobilisations
description: 'En savoir plus sur la série de tâches que vous devez effectuer pour configurer les immobilisations, telles que les machines ou les bâtiments.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: conceptual
ms.search.keywords: 'machinery, buildings'
ms.search.form: '5607,'
ms.date: 03/25/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# Paramétrage d’immobilisations

Avant de pouvoir utiliser les immobilisations, vous devez définir les éléments suivants :  

* Amortir des immobilisations.  
* La manière dont vous enregistrez les coûts acquisition, amortissements et d’autres valeurs dans le grand livre.  
* En option, comment enregistrer l’assurance et l’entretien des immobilisations.

Les sections de cet article renvoient à des informations supplémentaires sur la configuration des immobilisations. Une fois la configuration terminée, vous pouvez commencer à travailler avec des immobilisations. Pour en savoir plus, voir [Utiliser des immobilisations](fa-manage.md).  

> [!NOTE]  
> Vous pouvez enregistrer les transactions immobilisation sur les pages **Feuille compta. immo.** ou **Feuille immo.**, selon que les transactions sont destinées pour des rapports financiers ou pour la gestion interne. L’article d'aide pour les immobilisations décrit uniquement la procédure d’utilisation de la page **Feuille compta. immo.**.  

Lorsque vous activez une activité immobilisation dans la section **Intégration compta.** sur la page **Fiche loi d’amortissement**, la page **Feuille compta. immo.** sera utilisée pour valider les transactions pour l’activité.

## Tâches de configuration obligatoire

Le tableau suivant contient une séquence de tâches pour configurer les immobilisations et des liens vers des articles connexes.

| À | Voir |
|---|---|
| Configurer les comptes généraux par défaut, les clés de ventilation, les modèles feuille et les lots pour la validation des immobilisations et configurer les catégories et sous-catégories d’immobilisation, telles que Corporelles et Incorporelles. |[Configurer des informations générales pour les immobilisations](fa-how-setup-general.md) |
| Créer des lois d’amortissement, définir différentes méthodes d’amortissement, procéder à l’intégration en comptabilité et activer la duplication d’écritures dans plusieurs lois d’amortissement. |[Configuration des amortissements](fa-how-setup-depreciation.md) |

## Tâches de configuration facultatives (assurance, maintenance et méthodes d’amortissement définies par l’utilisateur)

Le tableau suivant contient une séquence de tâches facultative pour configurer les immobilisations, notamment les assurances, la gestion, et les Méthode amortissement et des liens vers des articles connexes. 

| À | Voir |
|---|---|
| Activer l’assurance des immobilisations, configurer les informations générales d’assurance, une fiche assurance par police et préparer les feuilles pour valider les coûts d’assurance. |[Configurer une assurance immobilisation](fa-how-setup-insurance.md) |
| Activer la maintenance des immobilisations, configurer les informations générales propres à la maintenance, configurer les comptes de validation de la maintenance et définir les types de travaux de maintenance. |[Configuration de la maintenance des immobilisations](fa-how-setup-maintenance.md) |
| Découvrez comment appliquer des méthodes d’amortissement. |[Configuration des méthodes d’amortissement définies par l’utilisateur](fa-how-setup-user-defined-depreciation-method.md) |

## Voir aussi

[Vue d’ensemble des immobilisations](fa-manage.md)  
[Finances](finance.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
