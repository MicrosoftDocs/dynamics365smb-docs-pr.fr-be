---
title: Prélèvement des articles pour l’expédition entrepôt
description: Découvrez comment utiliser les documents de prélèvement entrepôt pour créer et traiter les informations de prélèvement avant de valider une expédition entrepôt.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.service: dynamics-365-business-central
ms.topic: how-to
ms.date: 04/23/2024
ms.custom: bap-template
ms.search.forms: '7335, 7339, 7345,'
---
# <a name="pick-items-for-warehouse-shipment"></a>Prélèvement des articles pour l’expédition entrepôt

Dans [!INCLUDE[prod_short](includes/prod_short.md)], vous prélevez et expédiez des articles en utilisant l’une des quatre méthodes décrites dans le tableau suivant.

|Méthode|Processus sortant|Prélèvement requis|Expédition requise|Niveau de complexité (pour plus d’informations, consultez [Vue d’ensemble de la gestion des entrepôts](design-details-warehouse-management.md))|  
|------|----------------|-----|---------|-------------------------------------------------------------------------------------|  
|A|Validation du prélèvement et de l’expédition à partir de la ligne commande|||Aucune activité entrepôt dédiée.|  
|B|Validation du prélèvement et de l’expédition à partir d’un document prélèvement stock|Activé||De base : commande par commande.|  
|A|Validation du prélèvement et de l’expédition à partir d’un document expédition entrepôt||Activé|De base : envoi/réception regroupés pour plusieurs commandes.|  
|J|Validation du prélèvement à partir d’un document prélèvement entrepôt, et validation de l’expédition à partir d’un document expédition entrepôt|Activé|Activé|Avancé|  

Learn more at [Flux de désenlogement](design-details-outbound-warehouse-flow.md).

Cet article fait référence à la méthode D dans le tableau. Pour en savoir plus sur l’expédition d’articles, consultez [Expédier des articles](warehouse-how-ship-items.md).

Lorsqu’un magasin est configuré pour appeler un traitement de prélèvement entrepôt et un traitement d’expédition entrepôt, vous pouvez utiliser les documents prélèvement entrepôt pour créer et traiter les informations de prélèvement avant de valider l’expédition entrepôt.  

Vous ne pouvez pas créer un document de prélèvement en entrepôt à partir de rien. Les prélèvements font partie d’un flux de travail où la personne qui traite une commande les crée de manière « push », ou le magasinier les crée de manière « pull » :

- En mode « push », où vous utilisez l’action **Créer prélèvement** sur la page **Expédition entrepôt**. Sélectionnez les lignes à prélever et préparez les prélèvements en spécifiant, par exemple, à partir de quels emplacements les prendre, à quels emplacements les placer, et le nombre d’unités à traiter. Les emplacements peuvent être prédéfinis pour l’entrepôt ou la ressource.
- En mode « pull », où vous utilisez l’action **Lancer** dans la page **Expédition entrepôt** pour rendre les articles disponibles pour le prélèvement. Ensuite, sur la page **Feuille prélèvement**, les employés de l’entrepôt peuvent utiliser l’action **Extraire documents entrepôt** pour retirer les prélèvements qui leur sont assignés.

> [!NOTE]  
> Le prélèvement pour une expédition entrepôt des articles assemblés pour une commande vente suit les mêmes étapes que les prélèvements entrepôt ordinaires pour les expéditions, comme décrit dans cet article. Cependant, le nombre de lignes prélèvement pour la quantité à expédier peut grandement varier, car le prélèvement entrepôt concerne les composants et non l’article assemblé.  
>
> Les lignes prélèvement entrepôt sont créées suivant la valeur du champ **Quantité restante** sur les lignes de l’ordre d’assemblage associé à la ligne commande vente en cours d’expédition. Tous les composants sont prélevés en une seule action. Learn more at [Traitement des articles à assembler pour commande dans les expéditions entrepôt](warehouse-how-ship-items.md#handling-assemble-to-order-items-in-warehouse-shipments).  
>  
> Pour plus d’informations sur le prélèvement de composants pour les ordres d’assemblage, notamment les situations où les éléments d’assemblage ne sont pas associés à une expédition vente, consultez [Prélever pour la fabrication, l’assemblage ou les tâches dans les configurations de stockage avancées](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md).  

## <a name="check-whether-items-are-available-for-picking"></a>Vérifier si les articles sont disponibles pour le prélèvement

[!INCLUDE [inventory-availability-overview](includes/inventory-availability-overview.md)]

## <a name="to-create-pick-documents-in-bulk-with-the-pick-worksheet"></a>Pour créer des documents de prélèvement en bloc avec la feuille prélèvement

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Feuille prélèvement**, puis choisissez le lien associé.  

2. Choisissez l’action **Extraire documents entrepôt**.  

    La liste comprendra toutes les expéditions qui ont été lancées pour le prélèvement, y compris celles pour lesquelles des instructions de prélèvement ont déjà été créées. Les documents dont les lignes prélèvement ont été entièrement prélevées et enregistrées n’apparaissent pas dans cette liste.  
3. Sélectionnez les expéditions pour lesquelles vous souhaitez préparer un prélèvement.

    > [!NOTE]  
    >  Si vous essayez de sélectionner un document d’expédition ou de prélèvement interne pour lequel vous avez déjà créé des instructions pour toutes ses lignes, vous recevrez un message indiquant qu’il n’y a rien à gérer. Pour combiner des instructions de prélèvement entrepôt que vous avez déjà créées en une seule instruction de prélèvement, vous devez d’abord supprimer les prélèvements entrepôt individuels.

4. Renseignez le champ **Méthode de tri** pour trier les lignes.  

    > [!NOTE]  
    >  La façon dont les lignes sont triées dans la feuille ne se répercute pas automatiquement sur l’instruction de prélèvement. Cependant, les mêmes possibilités de tri et de classement des opportunités existent. Vous pouvez facilement recréer l’ordre des lignes planifié dans la feuille lorsque vous créez ou triez les instructions de prélèvement.

5. Remplissez le champ **Qté à traiter**, soit manuellement, soit en utilisant l’action **Remplir qté à traiter**.  

    La page affiche les quantités disponibles dans les emplacements de transbordement. Cette information est utile pour planifier les affectations de travail dans les situations de transbordement. [!INCLUDE[prod_short](includes/prod_short.md)] proposera toujours en premier un prélèvement dans un bac de transbordement.
6. Si nécessaire, modifiez les lignes. Vous pouvez aussi supprimer des lignes pour rendre le prélèvement plus efficace. Par exemple, si plusieurs lignes comportent des articles situés dans des bacs de transbordement, vous pouvez créer un prélèvement pour toutes les lignes. Les articles transbordés seront expédiés avec les autres articles de l’expédition, et les emplacements de transbordement pourront à nouveau recevoir d’autres articles entrants.  

    > [!NOTE]  
    >  Si vous supprimez des lignes, elles sont supprimées de la feuille. Elles ne sont pas supprimées de la liste de sélection de prélèvement.  

7. Choisissez l’action **Créer prélèvement**. La page **Créer prélèvement** s’ouvre, où vous pouvez ajouter plus d’informations au prélèvement que vous créez. Spécifiez la façon de combiner les lignes prélèvement dans les documents prélèvement en sélectionnant l’une des options suivantes.  

    |Option|Description|
    |-|-|
    |Par entrepôt Document|Crée des documents prélèvement distincts pour les lignes feuille avec le même document d’origine entrepôt.|
    |Par client/fourn./mag.|Créez des documents prélèvement distincts pour chaque client (commandes vente), fournisseur (retours achat) et magasin (ordres de transfert).|
    |Par article|Créez des documents prélèvement distincts pour chaque article sur la feuille prélèvement.|
    |Par zone origine|Créez des documents prélèvement distincts pour chaque zone où vous prendrez les articles.|
    |Par emplacement|Créez des documents prélèvement distincts pour chaque emplacement où vous prendrez les articles.|
    |Par délai|Créez des documents prélèvement distincts pour les documents origine qui ont la même date d’échéance.|

    Indiquez la façon dont les documents prélèvement sont créés en sélectionnant l’une des options suivantes.

    |Option|Description|
    |-|-|
    |Montant Nombre de lignes prélèvement|Crée des documents prélèvement qui n’ont pas plus que le nombre de lignes spécifié dans chaque document.|
    |Montant Nombre de docs origine prélèvement|Crée des documents prélèvement qui chacun couvre pas plus que le nombre spécifié de documents origine.|
    |Code utilisateur affecté|Crée des documents prélèvement uniquement pour les lignes qui sont affectées au magasinier sélectionné.|
    |Méthode de tri|Choisissez parmi les options disponibles pour trier les lignes du document prélèvement créé.|
    |Filtrer déconditionnement|Masque les lignes prélèvement déconditionnement intermédiaires lorsqu’une plus grande unité est convertie en une unité de mesure inférieure et est prélevée dans son intégralité.|
    |Ne pas remplir qté à traiter|Laisse le champ Qté à traiter vide sur les lignes prélèvement créées.|
    |Imprimer prélèvement|Imprime les documents prélèvement lors de leur création. Vous pouvez également imprimer à partir des documents prélèvement créés.|

8. Cliquez sur **OK**. [!INCLUDE [prod_short](includes/prod_short.md)] créera le prélèvement en fonction de vos sélections.  

## <a name="to-pick-items-for-a-warehouse-shipment"></a>Pour prélever des articles pour une expédition entrepôt

1. Sélectionnez l’![icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Prélèvements entrepôt**, puis choisissez le lien associé.  

    Si vous souhaitez travailler à un prélèvement particulier, sélectionnez-le dans la liste ou filtrez cette dernière afin de trouver les prélèvements qui vous ont été spécifiquement affectés. Ouvrez la fiche prélèvement.  
2. Si le champ **ID utilisateur affecté** est vide, entrez votre ID pour vous identifier, si nécessaire.  
3. Prélevez les articles.  

    Si le magasin est configuré pour utiliser des emplacements, les emplacements par défaut des articles sont utilisés pour suggérer où prendre les articles. Les instructions contiennent au moins deux lignes distinctes pour les actions Prendre et Placer.  

    Si l’entrepôt est configuré pour utiliser le rangement et le prélèvement dirigés, la priorité emplacement est utilisée pour calculer les meilleurs emplacements pour le prélèvement. Ces emplacements sont suggérés sur les lignes prélèvement. Les instructions contiennent au moins deux lignes distinctes pour les actions Prendre et Placer.  

    * La première ligne, avec **Prendre** dans le champ **Type d’action**, indique l’endroit où se trouvent les articles dans la zone de prélèvement. Si vous expédiez un grand nombre d’articles sur une seule ligne d’expédition, vous devrez peut-être prélever les articles dans plusieurs emplacements ; il y a donc une ligne Prendre pour chaque emplacement.
    * La ligne suivante, avec **Placer** dans le champ **Type d’action**, indique l’endroit où vous devez placer les articles dans l’entrepôt. Vous ne pouvez pas modifier la zone et l’emplacement de cette ligne.

    > [!NOTE]
    > Si vous devez prélever ou placer les articles d’une ligne dans plusieurs emplacements, notamment parce que l’emplacement indiqué est plein, utilisez l’action **Eclater ligne** sur le raccourci **Lignes**. L’action crée une ligne pour la quantité restante à gérer.
        
    Vous pouvez trier les lignes prélèvement en fonction de critères divers, tels que l’article, le numéro emplacement ou la date d’échéance. Le tri peut aider à optimiser le processus de rangement, par exemple :

    * Si les lignes Prendre et Placer de chaque ligne expédition ne se suivent pas directement et que vous souhaitez qu’elles se suivent, triez-les en sélectionnant **Article** dans le champ **Méthode de tri**.  
    * Si les classements des emplacements reflètent la disposition physique de l’entrepôt, utilisez la méthode de tri **Priorité emplacement** pour organiser le travail par emplacements.

  > [!NOTE]  
  > Les lignes sont triées par ordre croissant, en fonction des critères sélectionnés. Si vous triez par document, le tri est effectué d’abord par type de document en fonction du champ **Document source d’activité d’entrepôt** . Si vous triez par de livraison, le tri est effectué d’abord par type de destination en fonction du champ **Type de destination d’entrepôt** .

4. Après avoir prélevé et placé les articles dans la zone ou l’emplacement d’expédition, choisissez l’action **Enregistrer prélèvement**.  

Vous pouvez alors apporter les articles au quai de chargement et valider l’expédition, dont le document origine lié, sur la page **Expédition entrepôt**. Learn more at [Expédier des articles](warehouse-how-ship-items.md).

## <a name="see-also"></a>Voir aussi

- [Vue d’ensemble de la gestion d’entrepôt](design-details-warehouse-management.md)
- [Gestion du stock](inventory-manage-inventory.md)  
- [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
- [Gestion nomenclature d’assemblage](assembly-assemble-items.md)    
- [Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
