---
title: Utiliser les états Power BI dans Business Central | Microsoft Docs
description: "Obtenir des informations, des informations décisionnelles et des indicateurs de performance clés à partir de vos données Business\_Central avec Power BI."
author: jswymer
ms.topic: get-started
ms.devlang: al
ms.search.keywords: 'account schedule, analysis, reporting, financial report, business intelligence, KPI'
ms.date: 04/24/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---
# <a name="work-with-power-bi-reports-in-"></a>Utiliser les états Power BI dans [!INCLUDE [prod_short](includes/prod_short.md)]

Dans cet article, vous découvrirez quelques notions de base sur l’utilisation des états. Cela inclut l’affichage Power BI des rapports à l’intérieur [!INCLUDE [prod_short](includes/prod_short.md)] (y compris les tableaux de bord et les tableaux de bord) et la modification Power BI des rapports qui sont utilisés [!INCLUDE [prod_short](includes/prod_short.md)] comme source de données. L’article traite de certains aspects qui vous aideront à démarrer en tant qu’utilisateur [!INCLUDE[prod_short](includes/prod_short.md)]. Pour obtenir des instructions générales et des instructions sur l’utilisation Power BI, voir [Documentation Power BI pour les consommateurs](/power-bi/consumer).

## <a name="overview"></a>Vue d’ensemble

Les états Power BI vous donnent un aperçu de votre [!INCLUDE[prod_short](includes/prod_short.md)]. Diverses pages dans [!INCLUDE [prod_short](includes/prod_short.md)] incluent une partie d’états Power BI qui peut afficher des états Power BI. Le tableau de bord est une page type où vous verrez une partie d’éléments Power BI. Certaines pages de liste, comme **Articles**, comprennent également une partie Power BI.

[!INCLUDE [prod_short](includes/prod_short.md)] utilise le service Power BI. Les états à afficher dans [!INCLUDE [prod_short](includes/prod_short.md)] sont stockés dans un service Power BI. Dans [!INCLUDE [prod_short](includes/prod_short.md)], vous pouvez changer l’état affiché dans la partie Power BI vers tout état Power BI disponible dans votre service Power BI. La première fois que vous vous connectez à [!INCLUDE [prod_short](includes/prod_short.md)], et jusqu’à ce que vous vous connectiez à un service Power BI, les pièces restent vides, comme indiqué ici :

![Partie Power BI dans Business Central.](./media/power-bi-part.png)

## <a name="get-started"></a>Démarrer

> [!NOTE]
> [!INCLUDE [prod_short](includes/prod_short.md)] en ligne est déjà configuré pour s’intégrer à Power BI.

### <a name="sign-up-power-bi"></a>S′inscrire à Power BI

Avant de pouvoir utiliser Power BI avec [!INCLUDE[prod_short](includes/prod_short.md)], vous devrez vous inscrire au service Power BI. Si vous ne vous êtes pas encore inscrit, accédez à [https://powerbi.microsoft.com](https://powerbi.microsoft.com). Au moment de votre inscription, utilisez votre adresse e-mail professionnelle et votre mot de passe.

Une fois que vous avez un compte Power BI, vous pouvez vous connecter à [https://powerbi.microsoft.com/](https://powerbi.microsoft.com/).

Le service Power BI héberge tous les états dont vous disposez. Pour afficher un rapport dans votre espace de travail personnel, sélectionnez **Mon espace de travail** > **Rapports**. Ensuite, sélectionnez simplement l’état que vous souhaitez afficher. Si vous avez accès à un ou plusieurs espaces de travail Power BI partagés, vous pouvez également consulter les rapports dans ces espaces de travail.

Avec [!INCLUDE[prod_short](includes/prod_short.md)] en ligne, vous aurez automatiquement un ensemble d’états par défaut sur votre espace de travail. Si vous souhaitez créer vos propres états, vous pouvez utiliser Power BI Desktop pour créer des états, puis les publier dans votre espace de travail. Pour plus d’informations, consultez [Prise en main de la création d’états dans Power BI Desktop pour afficher les données [!INCLUDE [prod_long](includes/prod_long.md)]](across-how-use-financials-data-source-powerbi.md).

[!INCLUDE[note-multicompany-reports](includes/note-multicompany-reports.md)]

## <a name="connect-to-power-bi---one-time-only"></a><a name="connect"></a>Se connecter à Power BI - une fois seulement

Lorsque vous vous connectez pour la première fois [!INCLUDE [prod_short](includes/prod_short.md)], vous verrez peut-être une partie Power BI vide (comme indiqué dans la figure précédente) sur différentes pages. La première chose à faire est de vous connecter à votre compte Power BI. Une fois connecté, vous pouvez voir les états. Vous ne devez effectuer cette étape qu’une seule fois.

1. Sélectionnez le lien **Prise en main de Power BI** dans la partie **États Power BI**.
2. La configuration assistée **Configuration des états Power BI dans Business Central** démarre. Sélectionnez **Suivant** continuer.
3. Sur la page **Vérifier votre licence Power BI**. Exécutez l’une des étapes suivantes :

    - Si vous ne vous êtes pas encore inscrit à Power BI, sélectionnez [Accéder à la page d′accueil Power BI](https://powerbi.microsoft.com). Créez un compte, puis revenez sur [!INCLUDE[prod_short](includes/prod_short.md)] et terminez la configuration.

    - Si vous possédez déjà une licence, sélectionnez **Suivant**.
4. Dans la page suivante, [!INCLUDE[prod_short](includes/prod_short.md)] va maintenant charger un rapport de démonstration sur Power BI. Cette étape prendra quelques minutes, donc c′est fait en arrière-plan. Pour terminer la configuration, sélectionnez **Suivant**, puis **Terminer**.

Le processus de connexion démarre. Pendant le processus, [!INCLUDE [prod_short](includes/prod_short.md)] communique avec le service Power BI pour déterminer si vous avez un compte et une licence Power BI valides. Une fois votre licence vérifiée, l’état Power BI par défaut s’affiche sur la page. Si aucun état n’est affiché, vous pouvez sélectionner un état dans la partie.

> [!TIP]
> Avec [!INCLUDE [prod_short](includes/prod_short.md)] en ligne, cette étape chargera automatiquement les états Power BI par défaut utilisés dans [!INCLUDE [prod_short](includes/prod_short.md)] vers votre espace de travail Power BI.

<!--#### From [!INCLUDE [prod_short](includes/prod_short.md)] on-premises

Connecting to Power BI from [!INCLUDE [prod_short](includes/prod_short.md)] is similar to online. However, you might be prompted on the **MICROSOFT ENTRA SERVICE PERMISSIONS** page to grant access to Power BI Services. To grant access, select **Authorize Azure Services**, and then **Accept**.

Once connected, you can select a report from the Power BI part on pages.-->

## <a name="work-with-power-bi-reports"></a>Utiliser les états Power BI

### <a name="get-the-latest-data"></a>Obtenir les dernières données

Chaque état Power BI est basé sur un ensemble de données qui obtient des données des sources [!INCLUDE[prod_short](includes/prod_short.md)]. Vous voulez vous assurer que les données de vos états Power BI sont à jour avec les données dans [!INCLUDE[prod_short](includes/prod_short.md)]. C’est ce qu’on appelle l’*actualisation*.  En fonction de la configuration de votre organisation Power BI, l’actualisation risque de ne pas se faire automatiquement. Il existe deux façons d’actualiser les données : manuellement ou en planifiant une actualisation. L’actualisation manuelle est effectuée à la demande, si nécessaire. Avec l’actualisation programmée, actualisez automatiquement à des intervalles de temps définis.

#### <a name="refresh-manually"></a>Actualiser manuellement

Dans Power BI Online, le volet de navigation, sous **jeux de données**, sélectionnez **Plus d’options (...)** à côté de l’ensemble de données, puis sélectionnez **Actualiser maintenant**.

#### <a name="schedule-a-refresh"></a>Programmer une actualisation

Dans Power BI online, Dans le volet de navigation, sous Ensembles de données, sélectionnez Plus d’options (...) à côté de l’ensemble de données, puis sélectionnez **Actualiser maintenant**. Renseignez les informations sous la section **Planifier l’actualisation**, et sélectionnez **Appliquer**.

Pour plus d’informations, voir [Configurer une actualisation planifiée](/power-bi/connect-data/refresh-scheduled-refresh).

### <a name="show-reports-on-list-pages"></a>Afficher les états sur les pages de liste

[!INCLUDE[prod_long](includes/prod_long.md)] comprend un Récapitulatif Power BI sur plusieurs pages de liste clé. Ce Récapitulatif fournit des informations supplémentaires sur les données de la liste. Lorsque vous vous déplacez entre les lignes de la liste, l'état est mis à jour et filtré pour l'écriture sélectionnée.

Pour savoir comment créer des états pour les pages de liste, voir [Création d′états Power BI pour l′affichage des données de liste dans [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-powerbi-reports-factbox.md).

> [!TIP]
> Si vous ne voyez pas le récapitulatif Power BI, il peut être masqué sur votre espace de travail par personnalisation. Sélectionnez l’icône ![Paramètres](media/ui-experience/settings_icon_small.png "Icône Paramètres du tableau de bord"), puis l’action **Personnaliser**. Pour plus d’informations, voir [Personnaliser votre espace de travail](ui-personalization-user.md).
>
> Ou si vous avez une ancienne version de Business Central, accédez à la barre d’action, sélectionnez **Actions** > **Afficher** > **Afficher/Masquer les rapports Power BI**.

### <a name="switch-reports"></a>Changer de rapports

Une partie Power BI sur une page peut afficher n’importe quel état Power BI à votre disposition. Pour basculer vers un autre état, choisissez l’action **Sélectionner un état** depuis la liste déroulante des commandes en haut de la partie.  

La page **Sélection des états Power BI** affiche une liste de tous les états Power BI auxquels vous avez accès. Cette liste est extraite de n’importe lequel de vos propres espaces de travail ou des espaces de travail qui ont été partagés avec vous dans le service Power BI. Sélectionnez la zone **Activer** pour chaque état que vous souhaitez afficher sur la page d’accueil, puis choisissez **OK**. Vous serez redirigé(e) vers la page et le dernier état que vous avez activé apparaîtra. A l’aide de la liste déroulante des commandes, utilisez les commandes **Précédent** et **Suivant** pour naviguer entre les états.  

### <a name="get-more-reports"></a>Obtenez plus de rapports

Si vous ne voyez aucun état sur la page **Sélectionner des états Power BI**, ou si vous ne voyez pas l’état souhaité, choisissez **Obtenir des états**. Cette action vous permet de rechercher des états à partir de deux emplacements : *Mon organisation* ou *Prestations de service*.

- Choisissez **Mon organisation** pour accéder aux services Power BI. À partir de là, vous pouvez afficher les rapports au sein de votre organisation que vous avez le droit de consulter. Vous pouvez ensuite les ajouter à votre espace de travail.
- Choisissez **Services** pour accéder à Microsoft AppSource où vous pouvez installer les applications Power BI.  

> [!TIP]
> Si vous avez Power BI Desktop, vous pouvez également créer des états Power BI. Puis, une fois ces états publiés dans votre espace de travail Power BI, ils apparaîtront sur cette page **Sélectionner des états Power BI**.  

### <a name="manage-and-modify-reports"></a>Gérer et modifier les états

Vous pouvez apporter des modifications à un état dans la partie Power BI. Les modifications que vous apportez seront ensuite publiées dans le service Power BI. Si l’état est partagé avec d’autres utilisateurs, ils verront également les modifications, sauf si vous enregistrez les modifications dans un nouvel état.

Pour modifier un état, choisissez l’action **Gérer un état** dans la liste déroulante des commandes dans la partie Power BI. Ensuite, commencez à apporter des modifications. Une fois les modifications terminées, sélectionnez **Fichier** > **Enregistrer**. S’il s’agit d’un état partagé et si vous ne souhaitez pas effectuer la modification pour tous les utilisateurs, sélectionnez **Enregistrer sous** pour éviter de faire ce changement pour tous les utilisateurs.

Lorsque vous revenez au tableau de bord, l’état mis à jour apparaîtra. Si vous avez utilisé **Enregistrer sous**, vous devrez choisir **Sélectionner un état**, puis activez le nouvel état pour l’afficher.

> [!NOTE]
> Cette fonctionnalité n’est pas disponible avec [!INCLUDE [prod_short](includes/prod_short.md)] sur site.

### <a name="upload-reports"></a><a name="upload"></a>Télécharger des états

Les états Power BI peuvent être distribués entre les utilisateurs sous forme de fichiers .pbix. Si vous avez des fichiers .pbix, vous pouvez les télécharger et les partager avec tous les utilisateurs de [!INCLUDE [prod_short](includes/prod_short.md)]. Les états sont partagés au sein de chaque société dans [!INCLUDE [prod_short](includes/prod_short.md)].  

Pour télécharger un état, sélectionnez l’action **Télécharger l’état** dans la liste déroulante des commandes sur la partie **États Power BI**. Puis localisez le fichier .pbix qui définit les états que vous souhaitez partager. Vous pouvez modifier le nom par défaut du fichier.  

Une fois l’état téléchargé sur votre espace de travail Power BI, il se télécharge automatiquement sur les espaces de travail Power BI des autres utilisateurs.

> [!NOTE]
> Le téléchargement d’un état [!INCLUDE[prod_short](includes/prod_short.md)] nécessite que vous disposiez d’autorisations de SUPER utilisateur dans [!INCLUDE[prod_short](includes/prod_short.md)]. Vous n’avez besoin d’aucune autorisation spéciale pour télécharger des rapports sur votre espace de travail via le Power BI service.

## <a name="upload-reports-from-files"></a><a name="upload"></a>Télécharger des états à partir de fichiers

Les états Power BI peuvent être distribués entre les utilisateurs sous forme de fichiers .pbix. Si vous disposez d’un fichier .pbix, vous pouvez télécharger le fichier dans un espace de travail. Pour télécharger un état, procédez comme suit :

1. Dans votre nouvel espace de travail, sélectionnez **Obtenir des données**.

2. Dans la zone Fichiers, sélectionnez **Extraire**.

3. Sélectionner **Fichier local**, accédez à l’emplacement où vous avez enregistré le fichier et sélectionnez **Ouvrir**.

Pour plus d’informations, consultez [Télécharger l’état vers le service](/power-bi/paginated-reports/paginated-reports-quickstart-aw#upload-the-report-to-the-service).

<!--
> [!NOTE]
> Uploading a report requires that you have a [Premium capacity](/power-bi/service-premium-what-is) work space. For more information, see [Managing Premium capacities](/power-bi/admin/service-premium-capacity-manage). -->

> [!TIP]
> Si vous utilisez [!INCLUDE[prod_short](includes/prod_short.md)] en ligne, vous pouvez également télécharger un état depuis [!INCLUDE[prod_short](includes/prod_short.md)]. Pour plus d’informations, consultez [Utiliser les états Power BI dans [!INCLUDE [prod_short](includes/prod_short.md)] - Télécharger des états](across-working-with-powerbi.md#upload).

## <a name="share-reports-with-others"></a><a name="share"></a>Partager des états avec d’autres

Une fois qu’un état est dans votre espace de travail, vous pouvez le partager avec d’autres personnes de votre organisation.

Pour partager un état, dans une liste d’états ou dans un état ouvert, sélectionnez **Partager**. Dans le volet **Partager l’état**, entrez les adresses e-mail complètes des individus ou des groupes de distribution avec lesquels vous souhaitez le partager. Suivez les instructions à l’écran pour terminer le partage. Pour plus d’informations, consultez [Partager un tableau de bord ou un état](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report).

> [!NOTE]
> Vous devez, ainsi que les personnes avec lesquelles vous partagez le rapport, disposer d’une [Power BI licence Pro](/power-bi/service-features-license-type). Sinon, le contenu doit se trouver dans une [Capacité Premium](/power-bi/service-premium-what-is). Pour en savoir plus, consultez [Moyens de partager votre travail dans Power BI](/power-bi/service-how-to-collaborate-distribute-dashboards-reports).

## <a name="fixing-problems"></a>Résolution des problèmes

Toutefois, si une erreur se produit, cette section fournit une solution de rechange pour les problèmes les plus courants.  

### <a name="you-dont-have-a-power-bi-account"></a>Vous n’avez pas de compte Power BI

Aucun compte Power BI n’a été créé. Pour obtenir un compte Power BI valide, vous devez avoir une licence et vous devez avoir déjà ouvert une session dans Power BI, pour créer votre espace de travail Power BI.

### <a name="message-there-are-no-enabled-reports-choose-select-report-to-see-a-list-of-reports-that-you-can-display"></a>Message : Aucun état n’est activé. Choisissez Sélectionner un état pour afficher la liste des états disponibles.

Ce message apparaît si l’état par défaut n’a pas pu être déployé sur votre espace de travail Power BI. Ou l’état a été déployé, mais n’a pas été actualisé avec succès. Accédez à l’état dans votre espace de travail Power BI, sélectionnez **Ensemble de données**, **Paramètres**, puis mettez à jour les informations d’identification manuellement. Une fois le jeu de données actualisé, revenez dans [!INCLUDE[prod_short](includes/prod_short.md)] et sélectionnez manuellement l’état dans la page **Sélectionner des états**.

#### <a name="you-cant-see-a-report-on-the-select-report-page-on-a-list-page"></a>Vous ne pouvez pas voir un rapport sur la page Sélectionner un rapport sur une page de liste

C’est probablement parce que le nom de l’état ne contient pas le nom de la page de liste. Effacez le filtre pour obtenir la liste complète des états disponibles dans Power BI.

## <a name="see-also"></a>Voir aussi

[Business Central et Power BI](admin-powerbi.md)    
[Création d’états Power BI pour afficher les données [!INCLUDE [prod_long](includes/prod_long.md)] ](across-how-use-financials-data-source-powerbi.md)    
[Power BI Vue d’ensemble Architecture et composant d’intégration pour [!INCLUDE[prod_short](includes/prod_short.md)]](admin-powerbi-overview.md)    
[Se connecter aux versions locales vers Power BI [!INCLUDE [prod_short](includes/prod_short.md)] local](across-working-with-business-central-in-powerbi.md)    
[Power BI pour les consommateurs](/power-bi/consumer/end-user-consumer)     
[Le « nouveau look » du service Power BI](/power-bi/service-new-look)    
[Démarrage rapide : Se connecter aux données dans Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)    
[Power BI La documentation de](/power-bi/)    
[Veille économique](bi.md)    
[Préparation aux activités commerciales](ui-get-ready-business.md)    
[Importation des données métier à partir d’autres systèmes financiers](across-import-data-configuration-packages.md)    
[Configuration de [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)    
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)] comme source de données Power BI](across-how-use-financials-data-source-powerapps.md)    
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)] comme source de données Power Apps](across-how-use-financials-data-source-powerapps.md)    
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)] dans Power Automate](across-how-use-financials-data-source-flow.md)  




[!INCLUDE[footer-include](includes/footer-banner.md)]
