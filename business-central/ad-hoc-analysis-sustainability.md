---
title: Analyse ad hoc des données de durabilité
description: Découvrez comment utiliser le mode d’analyse des données de durabilité.
author: brentholtorf
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI, sustainability, ESG'
ms.search.form: '6220,'
ms.date: 06/12/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Analyse ad hoc des données de durabilité

Cet article vous apprenez à utiliser fonction **analyse les données** pour analyser des pages de durabilité directement de liste de pages et requêtes. Vous n’avez pas besoin d’exécuter un rapport ou de passer à une autre application, telle qu’Excel. La fonction fournit un moyen interactif et polyvalent de calculer, résumer et examiner les données. Plutôt que d’exécuter des rapports à l’aide d’options et de filtres, vous pouvez ajouter plusieurs onglets qui représentent différentes tâches ou vues sur les données. Quelques exemples sont "Aperçu émissions" ou "Émissions par scope", ou toute autre vue que vous pouvez imaginer. Pour en savoir plus sur l’utilisation de la fonctionnalité **Analyse des données** , accédez à [Analyser la liste et interroger les données avec le mode d’analyse](analysis-mode.md).

Utilisez les pages de liste suivantes pour une analyse ad hoc des données durabilité :

- [Écritures comptables durabilité](https://businesscentral.dynamics.com/?page=6220)

## Scénarios d’analyse ad hoc durabilité

Utilisez la fonctionnalité **Analyse des données** pour une vérification rapide des faits et une analyse ad hoc :

- Si vous ne souhaitez pas générer de rapport.
- S’il n’existe pas de rapport correspondant à votre besoin spécifique.
- Si vous souhaitez effectuer une itération rapide pour avoir une bonne vue d’ensemble sur une partie de votre entreprise.

Les sections suivantes fournissent des exemples de scénarios de durabilité dans [!INCLUDE [prod_short](includes/prod_short.md)].

| Zone | Pour... | Ouvrir cette page en mode analyse | Utiliser ces champs |
| ---- | ----- | ------------------------------- |------------------- |
| [Aperçu des émissions (somme par catégorie)](#example-emission-overview-sum-by-category) | Analysez vos émissions par catégorie. | [Écritures comptables durabilité](https://businesscentral.dynamics.com/?page=6220) | **Catégorie de compte**, **Nom du compte**, **Émission NH4**, **Émission de CO2** et **Émission de N2O**.|
| [Émissions moyennes par catégorie](#example-average-emissions-by-category) | Analysez vos émissions moyennes par catégorie. | [Écritures comptables durabilité](https://businesscentral.dynamics.com/?page=6220) | **Catégorie de compte**, **Nom du compte**, **Émission NH4**, **Émission de CO2** et **Émission de N2O**.|
| [Émissions de scope](#example-emissions-by-scope) | Analysez vos émissions par scope. | [Écritures comptables durabilité](https://businesscentral.dynamics.com/?page=6220) | **Scope émission**, **Catégorie de compte**, **Émission NH4**, **Émission de CO2** et **Émission de N2O**.|

## Exemple : Aperçu des émissions (somme par catégorie)

Pour analyser émissions par catégorie, procédez comme suit :

1. Ouvrez le [Écritures comptables durabilité](https://businesscentral.dynamics.com/?page=6220) liste page et activez le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Allumer **Pivot** mode (situé directement au-dessus du **Recherche** champ).
1. Faites glisser les champs **Catégorie de compte** et **Nom du compte** vers les **Groupes de lignes** zone. Faites glisser les champs dans cet ordre.
1. Faites glisser les champs **Émission NH4**, **Émission CO2**, et **Émission N2O** vers les **Valeurs** zone.
1. Renommez votre onglet d’analyse en **Aperçu des émissions (somme)** ou quelque chose qui décrit cette analyse pour vous.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-sustainability-entries.png" alt-text="Exemple 1 de comment effectuer une analyse des données sur la page des écritures comptables durabilité" lightbox="media/data-analysis-sustainability-entries.png":::

## Exemple : Émissions moyennes par catégorie

Pour analyser émissions moyennes par catégorie, procédez comme suit :

1. Ouvrez le [Écritures comptables durabilité](https://businesscentral.dynamics.com/?page=6220) liste page et activez le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Allumer **Pivot** mode (situé directement au-dessus du **Recherche** champ).
1. Faites glisser les champs **Catégorie de compte** et **Nom du compte** vers les **Groupes de lignes** zone. Faites glisser les champs dans cet ordre.
1. Faites glisser les champs **Émission NH4**, **Émission CO2**, et **Émission N2O** vers les **Valeurs** zone.
1. Pour chaque champ de la zone **Valeurs**, sélectionnez-les et modifiez la fonction d’agrégation en `Average`.
1. Renommez votre onglet d’analyse en **Aperçu des émissions (moy)** ou quelque chose qui décrit cette analyse pour vous.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-sustainability-entries-avg.png" alt-text="Exemple 2 de comment effectuer une analyse des données sur la page des écritures comptables durabilité" lightbox="media/data-analysis-sustainability-entries-avg.png":::

## Exemple : Émissions de scope

Pour analyser émissions par scope, procédez comme suit :

1. Ouvrez le [Écritures comptables durabilité](https://businesscentral.dynamics.com/?page=6220) liste page et activez le mode d’analyse.
1. Allez au **Colonnes** menu et supprimez toutes les colonnes (cochez la case à côté du **Recherche** champ).
1. Allumer **Pivot** mode (situé directement au-dessus du **Recherche** champ).
1. Faites glisser les champs **Scope émission** et **Catégorie du compte** vers les **Groupes de lignes** zone. Faites glisser les champs dans cet ordre.
1. Faites glisser les champs **Émission NH4**, **Émission CO2**, et **Émission N2O** vers les **Valeurs** zone.
1. Renommez votre onglet d’analyse en **Aperçu des émissions par scope** ou quelque chose qui décrit cette analyse pour vous.

L’image suivante montre le résultat de ces étapes.

:::image type="content" source="media/data-analysis-sustainability-entries-scope.png" alt-text="Exemple 3 de comment effectuer une analyse des données sur la page des écritures comptables durabilité" lightbox="media/data-analysis-sustainability-entries-scope.png":::

## Base de données pour une analyse ad hoc des durabilité

Les informations que vous saisissez dans une feuille durabilité sont temporaires et peuvent être modifiées tant qu’elles sont dans la feuille. Lorsque vous validez la feuille durabilité, les informations sont transférées vers des écritures de comptes de durabilité ou comptes de durabilité individuels, où elles ne peuvent pas être modifiées. Vous pouvez toutefois comptabiliser des écritures d’extourne ou de correction. La page de liste des [Entrées du grand livre de développement durable](https://businesscentral.dynamics.com/?page=6220) est la principale source de données pour l’analyse ad hoc des données de développement durable.

Pour en savoir plus sur la publication d’entrées de développement durable, accédez à [Enregistrer les entrées de développement durable](finance-sustainability-journal.md).

## Voir aussi

[Enregistrer les entrées de durabilité](finance-sustainability-journal.md)  
[Rapports de durabilité intégrés](sustainability-reports.md)   
[Vue d’ensemble Analyses, business intelligence et reporting](reports-bi-reporting.md)  
[Vue d’ensemble de la gestion de la durabilité](finance-manage-sustainability.md)   
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
