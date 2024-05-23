---
title: Archiver les documents vente et les documents achat
description: 'Vous pouvez archiver les commandes vente et les commandes achat, les devis, les retours et les commandes cadres.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 02/26/2024
ms.custom: bap-template
ms.search.form: '42, 49, 50, 459, 460, 5159, 5162, 5164, 5167, 6627, 6630, 6644, 9305, 9306, 9346, 9347, 9348, 9349'
ms.service: dynamics-365-business-central
---
# <a name="archive-documents"></a>Archivage de documents

Vous pouvez archiver les commandes vente et les commandes achat, les devis, les retours et les commandes cadres. Si vous utilisez les fonctionnalités de gestion de projet, vous pouvez également archiver vos projets. Vous pouvez archiver des documents et projets plusieurs fois, ce qui enregistrant une version archivée différente chaque fois.

Pour les documents de vente si l’original existe et n’est pas validé, vous pouvez utiliser l’action **Restaurer** pour le remplacer par une version archivée. 

> [!NOTE]
> Vous pouvez uniquement restaurer les documents et projets de vente. L’action n’est pas disponible pour les documents d’achat archivés.

Pour les documents archivés où l’original est désactivé, vous pouvez réutiliser le contenu en copiant les données, par exemple en utilisant l’action **Copier à partir du document**.  

## <a name="to-set-up-automatic-document-archiving"></a>Pour configurer l’archivage automatique des documents

Automatiser l’archivage automatique pour créer une version du document archivé lorsque quelqu’un effectue les actions suivantes :

* Modifie ou supprime un document ou projet.
* Imprime, télécharge ou envoie un document par e-mail.
* Convertit un devis en commande ou en facture.
* Publie une commande.

Les étapes suivantes décrivent comment configurer l’archivage automatique des documents de vente à partir du **Paramètres ventes** page. Les étapes sont similaires pour tous les documents achat et projet. Pour les documents d’achat, utilisez le **Achats** page. Pour les projets, utilisez le **Configuration du projet** page.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Paramètres ventes**, puis choisissez le lien associé.
2. Sur le raccourci **Archivage**, spécifiez s’il faut activer l’archivage automatique pour les différents types de documents de vente. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

Le tableau suivant décrit les options disponibles pour le champ **Archiver devis**.

|Option|Désignation|
|------|-----------|
|**Jamais**| N’archivez pas les devis lorsqu’ils sont supprimés.|
|**Question**|Invitez l’utilisateur à archiver ou non les devis lorsqu’ils sont supprimés.|
|**Toujours**|Archivez automatiquement les devis lorsqu’ils sont supprimés.|

## <a name="to-manually-archive-a-sales-order"></a>Pour archiver manuellement une commande vente

La procédure suivante décrit comment archiver manuellement une commande vente. La procédure est identique pour tous les documents et projets similaires archivés.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Commandes vente**, puis sélectionnez le lien associé.  
2. Ouvrez une commande vente que vous souhaitez archiver.  
3. Sélectionnez l’action **Archiver document**.

La commande vente est archivée. Vous pouvez l’afficher sur la page **Commandes vente archivées**.

## <a name="to-restore-a-non-posted-sales-document-or-a-project-from-the-archive"></a>Pour restaurer un document ou projet vente non validée depuis les archives

La procédure suivante décrit comment restaurer une commande vente archivée dans la commande vente d’origine. Il est possible de restaurer un document seulement lorsque le document d’origine n’a pas été validé. La procédure est identique pour les commandes, les commandes ouvertes, les retours et les devis et pour les projets.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Archives commandes vente**, puis sélectionnez le lien associé.
2. Sélectionnez la commande vente archivée, ou une version de celle-ci, que vous voulez restaurer, puis sélectionnez l’action **Restaurer**.  

Le contenu de la commande vente ou projets d’origine est remplacé par celui de la version archivée.

## <a name="to-delete-archived-versions"></a>Pour supprimer les versions archivées

Utilisez une stratégie de rétention pour nettoyer les versions archivés dont vous n’avez plus besoin. Les stratégies de rétention permettent aux administrateurs de définir la durée de stockage des données. Par exemple, ils peuvent configurer une stratégie qui supprime les données après une date d’expiration. Pour en savoir plus, accédez à [Définir des stratégies de rétention](admin-data-retention-policies.md).

Il y a quelques points à noter concernant la création de stratégies de rétention pour les documents archivés et projets :

* Si le document d’origine n’a pas été supprimé, [!INCLUDE [prod_short](includes/prod_short.md)] ne supprime pas les versions archivées. Les versions archivées n’expirent pas tant que l’original existe.
* Lorsque vous configurez la stratégie de rétention, vous pouvez spécifier que vous souhaitez que la stratégie supprime toutes les versions archivées, à l’exception de la plus récente. Par exemple, vous pouvez avoir 10 versions et vouloir conserver une copie de la dernière. 
* [!INCLUDE [prod_short](includes/prod_short.md)] calcule la date d’expiration des documents en fonction de la date de la version archivée la plus récente.

## <a name="see-also"></a>Voir aussi

[Suivi des lignes document](across-how-to-track-document-lines.md)  
[Ventes](sales-manage-sales.md)  
[Fonctionnalités marché](ui-across-business-areas.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
