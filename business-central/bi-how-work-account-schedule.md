---
title: Créer des états financiers avec des données financières et des catégories de compte
description: Décrit comment utiliser des états financiers pour créer différentes vues et différents états pour l’analyse des données de performances financières.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 03/27/2024
ms.custom: bap-template
ms.search.keywords: 'bi, power BI, analysis, KPI, account schedule, financial report'
ms.search.form: 'Report_25, 103, 104, 108, 195, 196, 197, 198, 488, 489, 490, 764, 765, 766'
ms.service: dynamics-365-business-central
---
# <a name="prepare-financial-reporting-with-financial-data-and-account-categories"></a>Préparer Financial Reporting avec des données financières et des catégories de compte

La fonctionnalité **états financiers** vous donne un aperçu des données financières enregistrées dans votre plan comptable (COA). Configurez les états financiers pour analysent les chiffres de la comptabilité et comparent les écritures comptables et les écritures comptables budget. Les résultats s’affichent dans les graphiques et les états de votre tableau de bord, comme le graphique Trésorerie et les états Comptes de gestion et Bilan. Vous accédez à ces deux états, par exemple, avec l’action **Relevés financiers** dans les tableaux de bord Gestionnaire d’activité et Comptable.  

[!INCLUDE[prod_short](includes/prod_short.md)] fournit des exemples d’états financiers que vous pouvez utiliser immédiatement comme modèles. Vous pouvez également configurer vos propres états pour spécifier les chiffres à comparer. Par exemple, vous pouvez créer des états financiers pour calculer les marges bénéficiaires dans des axes tels que les départements ou les groupes client. Le nombre de rapports financiers que vous pouvez créer est illimité et ne nécessite aucune intervention d’un développeur.  

## <a name="prerequisites-for-financial-reporting"></a>Conditions préalables au Financial Reporting

La configuration des états financiers exige une compréhension de la structure du plan comptable. Il y a trois concepts clés auxquels vous devrez probablement prêter attention avant de concevoir vos rapports financiers :

- Mappez les comptes de validation Comptabilité aux catégories de comptes du G/L.
- Concevez la façon dont vous utilisez les dimensions.
- Configurer les budgets Comptabilité

Les catégories de comptes généraux simplifient les définitions de vos rapports financiers et les rendent plus résistantes aux changements dans la structure du plan comptable. Pour en savoir plus, [utiliser les catégories de compte général pour modifier la présentation de vos états financiers](bi-row-definitions.md#use-gl-account-categories-to-change-the-layout-of-your-financial-statements).

La configuration de dimensions vous permet de découper vos données financières de manière logique pour votre organisation. Pour plus d’informations, consultez [Utiliser les dimensions](finance-dimensions.md). 

Si vous voulez afficher les écritures comptables en tant que pourcentages des écritures budget, vous devez créer des budgets Comptabilité. Pour plus d’informations, consultez [Créer des budgets](finance-how-create-budgets.md).

## <a name="financial-reports"></a>États financiers

Les états financiers organisent les comptes à partir de votre plan comptable de manière à faciliter la présentation des données. Vous pouvez configurer différentes présentations pour définir les informations que vous souhaitez extraire du plan comptable. Les états financiers fournissent aussi un emplacement pour les calculs qui ne peuvent pas être effectués directement dans le plan comptable. Par exemple, vous pouvez créer des sous-totaux pour des groupes de comptes, puis inclure ce total dans d’autres totaux. Un autre exemple consiste à calculer les marges bénéficiaires dans des axes tels que les départements ou les groupes client. De plus, vous pouvez filtrer les écritures comptables et les écritures comptables budget, par exemple, par solde période ou par montant débit.

> [!NOTE] 
> D’un point de vue mathématique, on peut considérer qu’un rapport financier est défini par deux éléments :
>
> - Un vecteur de définitions de lignes qui définissent ce qui doit être calculé.
> - Un vecteur de définitions de colonnes qui définit les données pour le calcul.
>
> Le rapport financier est alors le produit extérieur de ces deux vecteurs, où chaque valeur de cellule est calculée selon la formule de la ligne appliquée à la définition des données de la colonne.

:::image type="content" source="media/financial-report-definition.svg" alt-text="Montre comment un rapport financier est construit à partir d’une définition de ligne et d’une définition de colonne." lightbox="media/financial-report-definition.svg":::

Le **Rapports financiers** page montre comment tous les rapports financiers suivent un modèle composé des attributs suivants :

- Nom (code)
- Description
- Définition de ligne
- Définition de colonne

:::image type="content" source="media/financial-reports.png" alt-text="Montre comment tous les rapports financier sont construit à partir d’une définition de ligne et d’une définition de colonne." lightbox="media/financial-reports.png":::

> [!NOTE]
> Les exemples de rapports financiers présentés dans [!INCLUDE[prod_short](includes/prod_short.md)] ne sont pas prêt à être utilisés directement. En fonction de la façon dont vous configurez vos comptes généraux, vos dimensions, vos catégories de comptes généraux et vos budgets, vous devez ajuster les exemples de définitions de lignes et de colonnes ainsi que les rapports financiers dans lesquels ils sont utilisés pour correspondre à votre configuration.

Vous pouvez également utiliser des formules comparer deux ou plusieurs états financiers et définitions de colonne. Les comparaisons permettent de faire les choses suivantes :

- créer des états financiers personnalisé ;
- créer autant d’états financiers que nécessaire, chacun étant doté d’un nom unique ;
- configurer différentes présentations d'états et imprimer les états avec les chiffre actuels.

## <a name="learning-path-create-financial-reports-in-microsoft-dynamics-365-business-central"></a>Parcours d’apprentissage : Créer des rapports financiers dans Microsoft Dynamics 365 Business Central

Vous souhaitez apprendre à créer des budgets, puis à utiliser des rapports financiers, des dimensions et des définitions de lignes et de colonnes pour générer les rapports financiers généralement nécessaires ?

Commencez par le parcours d’apprentissage [Créer des rapports financiers dans Microsoft Dynamics 365 Business Central](/training/paths/create-financial-reports-dynamics-365-business-central) suivant.

## <a name="create-a-new-financial-report"></a>Créer un état financier

Vous utilisez les états financiers pour analyser les comptes généraux ou pour comparer les écritures comptables et les écritures comptables budget. Par exemple, vous pouvez afficher les écritures comptables en tant que pourcentages des écritures budget.

Les états financiers dans la version standard de [!INCLUDE[prod_short](includes/prod_short.md)] peuvent ne pas convenir aux besoins de votre entreprise. Pour créer rapidement vos propres états financiers, commencez par en copier un existant, tel que décrit à l’étape 3 ci-dessous.

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 1.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.  
1. Sur la page **États financiers**, choisissez l’action **Nouveau** pour créer un nom d’état financier. Sinon, réutiliser les paramètres d’un état financier existant, choisissez l’action **Copier l’état financier**.
1. Remplissez le nom court du rapport (le nom ne peut pas être modifié) et la description.
1. Choisissez une définition de ligne et une définition de colonne.
1. Vous pouvez éventuellement choisir des vues d’analyse pour les définitions de ligne et de colonne.
1. Choisissez l’action **Modifier l’état financier** pour accéder à plus de propriétés sur l’état financier.
1. Dans l’onglet rapide **Options**, vous pouvez modifier la description du rapport, modifier les définitions de ligne et de colonne et définir comment afficher les dates. Vous pouvez afficher les dates par jour, semaine, mois, trimestre, année ou périodes comptables. Pour en savoir plus, accédez à [Comparaison de périodes comptables à l’aide de formules de période](bi-column-definitions.md#comparing-accounting-periods-using-period-formulas).
1. Dans l’onglet rapide **Dimensions** , vous pouvez définir des filtres de dimension pour le rapport.
1. Vous pouvez prévisualiser le rapport dans la zone située sous l’onglet rapide **Dimensions** .

> [!TIP]
> Après avoir créé un état financier, vous pouvez utiliser la page **État financier** pour prévisualiser et le valider. Pour ouvrir la page, sélectionnez l’action **Afficher l’état financier**.  

> [!NOTE]
> Lorsque vous ouvrez un état financier en mode Afficher ou Modifier, le volet Filtre est disponible. N’utilisez pas le Volet Filtre pour définir des filtres pour les données de votre état. Ces filtres peuvent provoquer des erreurs ou ne pas réellement filtrer les données. Utilisez plutôt les champs des **Options** et **Dimensions** FastTabs pour configurer des filtres pour le rapport.

### <a name="create-or-edit-a-row-definition"></a>Créer ou modifier une définition de ligne

Les définitions de lignes dans les états financiers fournissent un emplacement pour les calculs qui ne peuvent pas être effectués directement dans le plan comptable. Par exemple, vous pouvez créer des sous-totaux pour des groupes de comptes, puis inclure ce total dans d’autres totaux. Vous pouvez également calculer des étapes intermédiaires qui ne sont pas affichées dans le rapport final.

Pour plus d'informations, voir [Définitions de ligne dans les états financiers](bi-row-definitions.md).

### <a name="create-or-edit-a-column-definition"></a>Créer ou modifier une définition de colonne

Utilisez les définitions de colonne pour spécifier les colonnes à inclure dans l’état. Par exemple, vous pouvez créer une disposition de rapport de manière à comparer le solde période et le solde pour une même période de l'exercice actuel et du précédent. Vous pouvez avoir jusqu’à 15 colonnes dans une définition de colonne. Par exemple, plusieurs colonnes sont utiles pour afficher les budgets sur 12 mois avec une colonne indiquant le total.

Pour plus d'informations, voir [Définitions de colonnes dans les états financiers](bi-column-definitions.md).

## <a name="using-dimensions-in-financial-reports"></a>Utilisation de dimensions dans les rapports financiers

En analyse financière, un axe correspond à des données que vous ajoutez à une écriture comme une sorte de marqueur. Ces données permettent de regrouper des écritures dotées de caractéristiques similaires, telles que les clients, les régions, les produits et les commerciaux, et de récupérer facilement ces groupes à des fins d'analyse. Vous pouvez utiliser les axes sur des écritures de feuilles, de documents et de budgets.

Chaque axe décrit l’objet de l’analyse. Une analyse à deux axes, par exemple, est une analyse des ventes par zone. En utilisant plus de deux dimensions lors de la création d’une entrée, vous pouvez effectuer une analyse plus complexe. Un exemple d’analyse complexe consiste à explorer les ventes par campagne de vente, par groupe de clients et par zone. Cela vous permet d’obtenir un meilleur aperçu de votre activité commerciale, comme la mesure du bon fonctionnement de votre société, les domaines dans lesquels elle prospère ou non, et ceux dans lesquels il est nécessaire d’affecter davantage de ressources. Ces informations vous aident à prendre des décisions commerciales plus éclairées. Pour en savoir plus, consultez [Utiliser les axes analytiques](finance-dimensions.md).

## <a name="set-up-financial-reports-with-overviews"></a>Configurer des états financiers avec des aperçus

Vous pouvez utiliser un état financier pour créer un état comparant les chiffres de la comptabilité avec les chiffres budgétés.

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 3.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.
1. Sur la page **États financiers**, sélectionnez un état financier.  
1. Choisissez l’action **Modifier la définition de ligne**.  
1. Sur la page **Définition de ligne**, sélectionnez le nom de l’état financier par défaut dans le champ **Nom**.
1. Choisissez l’action **Insérer des comptes généraux**.  
1. Sélectionnez les comptes à inclure dans votre relevé, puis cliquez sur **OK**.

    Ces comptes sont insérés dans l’état financier. Si vous le souhaitez, vous pouvez aussi modifier la définition de colonne.  
1. Choisissez l’action **Modifier l’état financier**.  
1. Sur la page **État financier**, sur le raccourci **Dimensions**, définissez le filtre budget sur le nom du filtre souhaité.  
1. Cliquez sur **OK**.  

Vous pouvez maintenant copier et coller votre budget dans un classeur.  

## <a name="integrate-financial-reports-with-excel"></a>Intégrer les rapports financiers avec Excel

Vous pouvez intégrer un rapport financier avec un modèle de classeur Excel, ajuster la mise en page en fonction de vos besoins, puis mettre à jour le modèle Excel avec les données de [!INCLUDE[prod_short](includes/prod_short.md)]. Par exemple, cette intégration facilite la génération de vos états financiers mensuels et annuels dans un format qui vous convient.

### <a name="set-up-excel-integration-for-a-financial-report-create-an-excel-template"></a>Configurer l’intégration Excel pour un rapport financier (créer un modèle Excel)

Pour configurer l’intégration Excel pour un rapport financier, suivez ces étapes pour créer un modèle Excel pour un rapport.

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 4.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.
1. Sur la page **États financiers**, sélectionnez l’état financier pour activer Excel, puis sélectionnez l’action **Exporter vers Excel**.
1. Choisissez l’action **Création document**. Cette action télécharge un modèle de classeur Excel avec une seule feuille de calcul nommée d’après le nom du rapport.
1. Copiez la feuille de calcul et renommez-la en **Données**.
1. Renommez la feuille de calcul du rapport à votre guise.
1. Dans la feuille de calcul du rapport, marquez toutes les cellules qui affichent les données du rapport financier (y compris les en-têtes de colonnes et de lignes). Sur le ruban **Accueil** , recherchez le menu **Numéro** et choisissez **Général** . comme format.
1. Choisissez la cellule la plus à gauche de la zone contenant les données du rapport financier et définissez une référence à la cellule équivalente dans la feuille de calcul Données. Faites glisser la formule vers la droite pour l’étendre à toutes les cellules de la première ligne, puis faites glisser la ligne vers le bas pour couvrir toutes les lignes du rapport financier.
1. Masquez la feuille de calcul **Données**.
1. Formatez la feuille de calcul du rapport en fonction de vos besoins.
1. Enregistrez le classeur dans OneDrive ou dans un endroit similaire où le fichier est sauvegardé et versionné.
1. Fermez le classeur.

### <a name="run-a-financial-report-with-an-excel-template"></a>Exécuter un rapport financier avec un modèle Excel

Pour exécuter un rapport financier avec un modèle Excel, procédez comme suit :

1. Sélectionnez l’icône en forme ![d’ampoule qui ouvre la fonction Tell Me 4.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.
1. Sur la page **États financiers**, sélectionnez l’état financier pour activer Excel, puis sélectionnez l’action **Exporter vers Excel**.
1. Choisissez l’action **Mettre à jour la copie du document existant**.
1. Téléchargez votre modèle Excel (fermez le classeur Excel avant de le télécharger).
1. Sur la page **Recherche de nom/valeur** , choisissez la feuille de calcul Données.
1. [!INCLUDE[prod_short](includes/prod_short.md)] exécute le rapport financier et fusionne les données résultantes avec votre modèle Excel.

## <a name="print-and-save-financial-reports"></a>Imprimer et enregistrer des états financiers

Vous pouvez imprimer des états financiers à l’aide des services d’impression de votre appareil. [!INCLUDE[prod_short](includes/prod_short.md)] offre également les possibilités d’enregistrer les états sous forme de classeurs Excel, de documents Word, de fichiers PDF et XML.

1. Sélectionnez ![icône en forme d’ampoule qui ouvre la fonction Tell Me 4.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.
1. Sur la page **États financiers**, sélectionnez l’état à imprimer, puis sélectionnez l’action **Imprimer**.
1. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
1. Dans le champ **Imprimante**, sélectionnez l’appareil auquel l’état est envoyé.
    1. L’option **(Géré par le navigateur)** indique qu’il n’y a pas d’imprimante désignée pour l’état. Dans ce cas, le navigateur gérera l’impression et affiche une expérience standard, où vous pourrez choisir une imprimante locale connectée à votre appareil. **(Géré par le navigateur)** n’est pas disponible dans l’application mobile [!INCLUDE[prod_short](includes/prod_short.md)] ou application pour Teams.
1. Choisissez l’action **Imprimer**.

### <a name="schedule-a-financial-report-or-save-as-a-pdf-word-or-excel-document"></a>Planifier un état financier ou l’enregistrer au format PDF, Word ou Excel

Enregistrez un état financier sous forme de fichier formats, tels que PDF, XML, Word ou Excel. [!INCLUDE[prod_short](includes/prod_short.md)] peut aussi générer des états financiers Abonnement.

1. Sélectionnez l’icône en forme ![d’ampoule qui ouvre la fonction Tell Me 4.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.
1. Sur la page **États financiers**, sélectionnez l’action **Imprimer**.
1. Définissez l’état en conséquence, puis choisissez l’action **Envoyer à**.
1. Sélectionnez le format de fichier ou l’action **Planifier**, puis sélectionnez **OK**.
1. Pour générer un état financier planifié ou récurrent, remplissez les champs. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].<br><br>Pour les états financiers récurrents, définissez les champs **Date/heure de début au plus tôt** et **Date/heure d’expiration** avec la première et la dernière date, respectivement, pour générer l’état financier. Sélectionnez également les jours où l’état est généré en définissant le champ **Formule de la date de la prochaine exécution** en suivant le format expliqué dans la section [Utiliser des formules de date](ui-enter-date-ranges.md#use-date-formulas).


## <a name="best-practices-for-working-with-financial-report-definitions"></a>Meilleures pratiques pour utiliser les définitions de rapports financiers

Les définitions des rapports financiers ne sont pas versionnées. Lorsque vous modifiez une définition de rapport, l’ancienne version est remplacée lorsque votre modification est enregistrée dans la base de données. La liste suivante contient quelques bonnes pratiques pour utiliser les définitions d’états financiers :

- Si vous ajoutez des définitions de rapport, choisissez un bon code et remplissez le champ de description avec un texte significatif tout en sachant à quoi vous utilisez le rapport. Ces informations aident vos collègues (et votre futur moi) à travailler avec le rapport et peut-être à modifier la définition du rapport.
- Avant de modifier une définition de rapport, envisagez d’en faire une copie comme sauvegarde, au cas où votre modification ne fonctionnerait pas comme prévu. Vous pouvez soit simplement copier la définition (lui donner un bon nom), soit l’exporter. Pour en savoir plus, voir [importer ou exporter des définitions de rapports financiers](#import-or-export-financial-report-definitions).
- Si vous avez besoin d’une nouvelle copie d’une définition [!INCLUDE[prod_short](includes/prod_short.md)] fournie, un moyen simple d’en obtenir une consiste à créer une nouvelle société contenant uniquement des données de configuration. Ensuite, exportez la définition et importez-la dans l’entreprise où la définition doit être actualisée.

## <a name="import-or-export-financial-report-definitions"></a>Importer ou exporter des définition de états financiers

Vous pouvez importer et exporter des définition de rapport financiers comme des packages de configuration RapidStart. Par exemple, les packages de configuration s’avèrent utiles pour le partage d’informations avec d’autres sociétés. Le package est créé dans un fichier .rapidstart, qui compresse le contenu.

> [!NOTE]
> Lorsque vous importez des définition de rapport financiers, les enregistrements existants portant les mêmes noms que ceux que vous importez sont remplacés par les nouvelles définitions. Le package de configuration d’une définition de rapport n’écrasera aucune définition de ligne ou de colonne existante utilisée dans la définition de rapport.

Pour importer ou exporter des définitions de rapports financiers, procédez comme suit :

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 4.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **États financiers**, puis choisissez le lien associé.
1. Choisissez l’état financier, puis choisissez l’action **Importer l’état financier** ou **Exporter l’état financier**, selon ce que vous voulez faire.

Pour en savoir plus sur l’importation ou l’exportation de définitions de lignes ou de colonnes de rapports financiers, consultez les articles suivants : 

- [Importer ou exporter des définitions de lignes de Financial Reporting](bi-row-definitions.md#import-or-export-financial-reporting-row-definitions) ou
- [Importer ou exporter des définition de colonnes de Financial Reporting](bi-column-definitions.md#import-or-export-financial-report-column-definitions)

## <a name="see-also"></a>Voir aussi

[Définitions de ligne dans les états financiers](bi-row-definitions.md)  
[Définitions de colonne dans les états financiers](bi-column-definitions.md)  
[Exécution et impression des états](ui-work-report.md)  
[Business Intelligence financière](bi.md)  
[Finances](finance.md)  
[Configuration de Finance](finance-setup-finance.md)  
[Les écritures comptables et le plan comptable](finance-general-ledger.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
