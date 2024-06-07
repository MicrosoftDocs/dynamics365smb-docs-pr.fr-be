---
title: Définitions de colonne dans Financial Reporting
description: Décrit les définitions de colonne dans les états financiers.
author: kennieNP
ms.author: kepontop
ms.reviewer: bnielse
ms.topic: how-to
ms.date: 03/27/2024
ms.custom: bap-template
ms.search.keywords: 'bi, power BI, analysis, KPI, account schedule, financial report'
ms.search.form: '103, 104, 108, 195, 196, 197, 198, 489, 490, 764, 765, 766'
ms.service: dynamics-365-business-central
---

# Définitions de colonne dans Financial Reporting

Utilisez les définitions de colonne pour spécifier les colonnes à inclure dans un état. Par exemple, vous pouvez créer une disposition de rapport de manière à comparer le solde période et le solde pour une même période de l'exercice actuel et du précédent. Vous pouvez avoir jusqu’à 15 colonnes dans une définition de colonne. Par exemple, plusieurs colonnes sont utiles pour afficher les budgets sur 12 mois avec une colonne indiquant le total.

## Créer ou modifier une définition de colonne

Pour créer ou modifier une définition de colonne, procédez comme suit.

> [!NOTE]
> Une versions imprimée, aperçu, enregistrée d’un état financier affiche un maximum de cinq colonnes. Par opposition, si un état financier est uniquement destiné pour l’analyse sur la page **État financier**, vous pouvez créer autant de colonnes que vous le souhaitez.

1. Sur la page **États financiers**, sélectionnez l’état financier voulu et sélectionnez l’action **Modifier la définition de colonne**.
1. Sur la page **Définition de colonne**, créez une ligne pour chaque colonne de données financières affichées dans l’état financier. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
1. Cliquez sur **OK**.
1. Ouvrez la page **État financier** de temps en temps pour vérifier que la nouvelle définition de colonne fonctionne comme prévu.

## Définitions de colonne intégrées

[!INCLUDE[prod_short](includes/prod_short.md)] fournit des exemples de définitions de colonnes qui peuvent vous aider à démarrer rapidement la configuration de rapports financiers adaptés à vos besoins.

<!-- update this when we release the new templates in 24.1
| Column definition code | Description | How to use this column definition | 
| ------------------- | ----------- | ------------------------------ | 
| TBA 1 | TBA 1 | TBA 1 |
| TBA 2 | TBA 2 | TBA 2 |
| TBA 3 | TBA 3 | TBA 3 |
| TBA 4 | TBA 4 | TBA 4 |
-->

## Exemple : Créer une définition de colonne pour calcule des pourcentages

Si vous vouliez inclure une colonne dans un état financier pour calculer des pourcentages d’un total. Par exemple, si vous avez des lignes qui ventilent des ventes par dimension, vous pouvez juger utile de disposer d’une colonne indiquant le pourcentage des ventes totales que représente chaque ligne.

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 2.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.
1. Sur la page **États financiers**, sélectionnez un état financier.  
1. Choisissez l’action **Modifier l’état financier** pour configurer une ligne d’état financier et calculer le total sur lequel le pourcentage est basé.  
1. Ajouter une ligne juste au-dessus de la première ligne pour laquelle vous voulez afficher un pourcentage.  
1. Renseignez les champs de la ligne qui suivent : 
    1. Dans le champ **Type totalisation**, entrez **Base de pourcentage**. 
    1. Dans le champ **Totalisation**, saisissez une formule pour le total sur lequel le pourcentage est basé. Par exemple, si la ligne 11 contient le total des ventes, saisissez **11**.  
1. Choisissez l’action **Modifier la définition de colonne** pour configurer une colonne.  
1. Renseignez les champs de la ligne qui suivent. 
    1. Dans le champ **Type colonne**, sélectionnez **Formule**. 
    1. Dans le champ **Formule**, saisissez une formule correspondant au montant pour lequel vous voulez calculer un pourcentage, suivie du symbole de pourcentage %. Ainsi, si le numéro de colonne N contient le solde période, saisissez **N%**.  
1. Répétez les étapes 4 à 7 pour chaque groupe de lignes que vous voulez ventiler par pourcentage.

## Comparaison de périodes comptables à l’aide de formules de période

Votre état financier peut comparer les résultats de différentes périodes comptables, par exemple le mois dernier et le même mois l’année précédente. Pour ce faire, ouvrez la page **Définition de colonne** et personnalisez-la en ajoutant le champ **Formule période comparaison** sous forme de colonne. Pour plus d’informations, consultez [Personnaliser votre espace de travail](ui-personalization-user.md). Vous pouvez ensuite définir ce champ sur une formule de période.  

Une période comptable ne doit pas nécessairement correspondre au calendrier. Toutefois, chaque exercice doit avoir le même nombre de périodes comptables, bien que chaque période peut varier.  

[!INCLUDE[prod_short](includes/prod_short.md)] utilise la formule de période pour calculer la durée de la période de comparaison en fonction de la période représentée dans le filtre date du formulaire de sélection de l’état. La période de comparaison est basée sur la période de la date de début du filtre de date. Le tableau suivant présente les abréviations des spécifications de période.

| Abréviation | Description                                                                           |
| ------------ | ------------------------------------------------------------------------------------- |
| P            | Période.                                                                                |
| DP           | Dernière période de l’exercice, du semestre ou du trimestre.                                   |
| FP           | Fin de période de l’exercice, du semestre ou du trimestre. Utilisez FP dans les formules pour définir la période qui commence ou termine la formule. Par exemple, EC\[1..FP\] désigne la durée entre le début de l’exercice comptable en cours et la fin de la période.|
| EC           | Exercice comptable. Par exemple, EC\[1..3\] désigne le premier trimestre de l’exercice courant. |

Exemples de formule :

| Formule | Description |
|-----|-----|
| \<Blank\>       | Période courante. |
| \-1P            | Période précédente.            |
| \-1EC\[1..DP\]  | Ensemble de l’exercice comptable précédent.                  |
| \-1EC           | Période de l’exercice comptable précédent équivalente à la période en cours.       |
| \-1EC\[1..3\]   | Premier trimestre de l’exercice comptable précédent.        |
| \-1EC\[1..FP\]  | Du début de l’exercice comptable précédent à la fin de la période de l’exercice comptable précédent, les deux périodes incluses. |
| \-1EC\[FP..DP\] | De la fin de la période de l’exercice comptable précédent à la dernière période de l’exercice comptable précédent, les deux périodes incluses.   |

Pour effectuer des calculs basés par périodes, entrer une formule dans le champ **Formule date comparaison** à la place. Par exemple, si le champ est défini sur -1A, [!INCLUDE [prod_short](includes/prod_short.md)] procède à une comparaison à la même période un an avant.

> [!NOTE]
> Il n’est pas toujours évident de déterminer les périodes à comparer, car vous pouvez définir un filtre date sur un état qui couvre des dates différentes des périodes comptables dans le plan comptable. Ainsi, si vous créez un état financier dans lequel vous souhaitez comparer cette période avec la même période l’année précédente, définissez le champ **Formule date comparaison** sur **-1EC**. Ensuite, vous exécutez l’état le **28 février** et définissez le filtre date sur **Janvier et février**. Par conséquent, l’état financier compare les mois de janvier et février de cette année au mois de janvier de l’année précédente, qui est la seule période comptable terminée des deux pour l’année précédente.  

Pour plus d’informations, consultez [Utiliser des dates civiles et des heures](ui-enter-date-ranges.md).

[!INCLUDE [report-best-practices-column-defs](includes/report-best-practices-column-defs.md)]

## Importer ou exporter des définition de colonnes de état financier

À partir de la 1re vague de lancement 2024 (version 24.1), vous pouvez importer et exporter des définitions de colonnes de rapports financiers sous forme de RapidStart paquets de configuration. Par exemple, les packages de configuration s’avèrent utiles pour le partage d’informations avec d’autres sociétés. Le package est créé dans un fichier .rapidstart, qui compresse le contenu.

> [!NOTE]
> Lorsque vous importez des états financiers/définition de colonne, les enregistrements existants portant les mêmes noms que ceux que vous importez sont remplacés par les nouvelles définitions. Le package de configuration d’une définition de rapport n’écrasera aucune définition de ligne ou de colonne existante utilisée dans la définition de rapport.

Pour importer ou exporter des définitions de colonne de rapports financiers, procédez comme suit :

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 4.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Définitions de colonne**, puis sélectionnez le lien associé.
1. Choisissez la définition de ligne, et choisissez l’action **Importer définition de colonne** ou **Exporter définition de colonne**, selon ce que vous voulez faire.

## Voir aussi

[Définitions de ligne dans les états financiers](bi-row-definitions.md)  
[Préparation de l’état financier](bi-how-work-account-schedule.md)  
[Business Intelligence financière](bi.md)  
[Finances](finance.md)  
[Configuration de Finance](finance-setup-finance.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
