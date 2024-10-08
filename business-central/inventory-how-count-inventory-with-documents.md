---
title: Compter et Ajuster inventaire
description: Décrit comment compter l’inventaire et utiliser les documents d’inventaire pour ajuster le stock disponible.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.search.keywords: 'adjustment, status, negative, positive, increase, decrease, inventory'
ms.search.forms: '5895, 6561, 6562, 6563, 6564, 6565, 6566, 5892, 5891, 5879, 5880, 5893, 5897, 5882, 5881, 5899, 5875, 5878, 5877, 5876, 5896, 6567, 6568, 6569, 6570, 6571, 6572, 5883, 5886, 884, 5898, 5885, 5890, 5888, 5889, 5887, 5894, 6774, 6775, 6776, 6780, 6781, 6782, 6783'
ms.date: 04/19/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="count-and-adjust-inventory-using-documents"></a>Faire l’inventaire et l’ajuster à l’aide de documents

Vous pouvez effectuer l'inventaire d'un stock physique de vos articles à l'aide des documents Commande de stock physique et Enregistrement de stock physique. La page **Commande de stock physique** est utilisée pour organiser le projet d'inventaire complet, par exemple un par magasin. Utilisez la capture page **Enregistrement de stock phys.** pour communiquer et capturer le nombre réel d’articles. Vous pouvez créer plusieurs enregistrements pour une commande, par exemple, pour répartir les groupes d’articles vers différents employés.

Imprimez l’état **Enregistrement de stock phys.** depuis chaque enregistrement et contient des champs de quantité vides pour saisir l’inventaire. Quand vous avez terminé l’inventaire et quand les quantités sont saisies sur la page **Enregistrement de stock phys.**, sélectionnez l’action **Terminer**. Cette action transfère les quantités vers les lignes concernées sur la page **Enregistrement de stock physique**. [!INCLUDE [prod_short](includes/prod_short.md)] garantit que vous ne pouvez pas enregistrer deux fois un nombre d’éléments.  

> [!NOTE]
> L’utilisation de documents pour effectuer un décompte inventaire offre un plus grand contrôle et prend en charge la répartition de l’inventaire vers plusieurs employés. Vous pouvez également utiliser les feuilles effectuer la tâche, les pages **Feuilles inventaire** et **Feuilles inventaire entrepôt**. Pour en savoir plus, [Comptabiliser, ajuster et reclasser le stock avec les feuilles](inventory-how-count-adjust-reclassify.md). Cet article décrit comment utiliser des documents pour effectuer un inventaire physique.
>
> Si vous utilisez des zones dans votre Entrepôt, vous ne pouvez pas utiliser de commandes d’inventaire. À la place, utilisez la page **Feuille inventaire entrepôt** pour faire l’inventaire de vos écritures d’entrepôt avant de les synchroniser avec les écritures comptables d’article.

Réaliser l’inventaire à l’aide de documents se produit comme suit :

1. Créez une commande de stock physique avec les quantités d'articles prévus pré-remplies.
2. Générez un ou plusieurs enregistrements de stock physique depuis la commande.
3. Saisissez les quantités d'articles répertoriés sur les enregistrements, comme saisis sur les bordereaux, par exemple, puis sélectionnez le statut **Terminé**.
4. Exécutez et validez la commande de stock physique.

## <a name="to-create-a-physical-inventory-order"></a>Pour créer une commande de stock physique

Une commande de stock physique est un document complet composé d’une en-tête de commande de stock physique et de lignes de commande. Les informations relatives à une en-tête de stock physique décrivent comment effectuer l'inventaire. Les lignes de commande contiennent les informations relatives aux articles et à leurs magasins.

Pour créer les lignes de commande de stock physique, vous utilisez généralement la action **Calculer les lignes** pour ajouter le stock actuel comme lignes de la commande. Vous pouvez aussi utiliser la action **Copier du document** pour remplir les lignes avec le contenu de toute autre commande de stock physique ouverte ou validée. La procédure suivante décrit uniquement comment utiliser la Action **Calculer les lignes**.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Commandes de stock**, puis choisissez le lien associé.
2. Choisissez l'action **Nouveau**.
3. Renseignez les champs requis du raccourci **Général**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Dans l’onglet **Actions**, dans le groupe **Fonctions**, choisissez **Autre**, puis choisissez **Calculer les lignes**.
5. Sélectionnez des options, le cas échéant.
6. Définissez les filtres, par exemple, pour inclure uniquement un sous-ensemble d’articles à comptabiliser avec le premier enregistrement.

    > [!TIP]
    > Pour planifier l’exécution de l’inventaire par plusieurs employés, définir différents filtres à chaque utilisation de l’action **Calculer les lignes** pour remplir la commande avec le sous-ensemble d’articles de l’inventaire qu’un utilisateur enregistrera. Ainsi, en générant plusieurs enregistrements de stock physique par plusieurs employés, vous réduisez le risque de comptabilisation de doublons d’articles. Pour en savoir plus, rendez-vous sur [Pour créer un enregistrement d’inventaire physique](#to-create-a-physical-inventory-recording).

7. Cliquez sur le bouton **OK**.

Une ligne pour chaque article qui existe sur l’emplacement sélectionné et conformément aux filtres et options définis est ajoutée sur la commande. Pour les articles configurés pour le suivi des articles, la case à cocher **Utiliser le suivi des articles** est sélectionnée et les informations relatives à la quantité prévue des numéros de lot et de série est disponible en sélectionnant **Lignes**, puis **Lignes de suivi des articles**. Pour en savoir plus, rendez-vous sur [Gérer le suivi des articles lors du comptage des stocks](#handle-item-tracking-when-counting-inventory).

Vous pouvez désormais créant un ou plusieurs enregistrements, qui correspondent aux instructions données aux employés en charge du décompte.  

> [!NOTE]
> Si vous utilisez le suivi spécifique aux colis, vous pouvez également utiliser des documents pour compter et ajuster l’inventaire avec les numéros de colis. Pour commencer à utiliser cette fonctionnalité, vous devez activer **Mise à jour des fonctionnalités : activer l’utilisation du suivi des colis dans les commandes d’inventaire physique** dans la **Gestion des fonctionnalités** page. Les commandes d’inventaire physique existantes sont mises à jour, cependant, [!INCLUDE [prod_short](includes/prod_short.md)] ne peuvent pas renseigner le **numéro de colis.** . Vous devez recréer ces lignes à l’aide de l’action **Calculer les lignes** sur la page **Commande d’inventaire physique** .
>
> Vous pouvez saisir le numéro de colis pour les articles pour lesquels le suivi du colis est nécessaire sur le **Phys. Page Lignes d’enregistrement des stocks** . Choisissez **Terminer** pour finaliser l’enregistrement.
>
> Après avoir choisi **Terminer** sur la page **Ordre d’inventaire physique** , [!INCLUDE [prod_short](includes/prod_short.md)] calcule les différences par rapport au colis et à d’autres détails de suivi de l’article, et effectue des ajustements positifs ou négatifs.

## <a name="to-create-a-physical-inventory-recording"></a>Pour créer un enregistrement de stock physique

Pour chaque commande d’inventaire physique, vous pouvez créer un ou plusieurs documents d’enregistrement d’inventaire physique sur lesquels les salariés saisissent les quantités comptées. Les employés peuvent saisir les quantités soit manuellement, soit avec un appareil de numérisation.

Par défaut, un enregistrement est créé pour toutes les lignes sur la commande de stock physique. Pour éviter que deux employés comptent les mêmes articles si vous répartissez le comptage, remplissez progressivement l’ordre d’inventaire physique en définissant des filtres sur le traitement par lots **Calculer les lignes** . Créez ensuite l’enregistrement de l’inventaire physique en cochant la case **Seules les lignes ne figurant pas dans les enregistrements** . Ce paramètre veille à ce que chaque nouvel enregistrement contienne des articles différents de ceux des autres enregistrements.

Pour un décompte manuel, vous pouvez imprimer une liste, l’état **Enregistrement de stock physique**, sur lequel figure une colonne vide où les employés de l'entrepôt peuvent écrire les quantités comptabilisées. Une fois le décompte effectué, vous saisissez les quantités enregistrées sur les lignes concernées de la page **Enregistrement de stock physique**. Enfin, transférez les quantités enregistrées dans la commande de stock physique concernée en définissant le statut sur **Terminé**.

1. Sur une page **Commande d’inventaire physique** qui contient des lignes pour les éléments à compter dans un enregistrement, vous devez choisir l’action **Créer un nouvel enregistrement** .
1. Dans l’onglet **Actions**, dans le groupe **Fonctions**, choisissez **Autre**, puis choisissez **Créer un nouvel enregistrement**.
1. Sélectionnez les options et définissez les filtres, le cas échéant.
1. Cliquez sur le bouton **OK**.
1. Pour chaque ensemble d’article à comptabiliser, importez-les sur la commande de stock physique concernée et répétez les étapes 1 à 3 en veillant à bien cocher la case **Uniquement les lignes qui ne figurent pas dans les enregistrements**.
1. Dans l’onglet  **Lié**, choisissez **Commande**, puis choisissez l’action  **Enregistrements** pour ouvrir la page  **Liste des enregistrements d’inventaire physique** .
1. Ouvrez l'enregistrement approprié.
1. Sur le raccourci **Général**, complétez les champs, comme nécessaire.
1. Pour les articles qui utilisent le suivi des articles, créez une ligne supplémentaire pour chaque numéro de lot ou code de numéro de série en sélectionnant l'action **Fonctions**, puis l'action **Copier la ligne**. Pour en savoir plus, rendez-vous sur [Gérer le suivi des articles lors du comptage des stocks](#handle-item-tracking-when-counting-inventory).  
1. Choisissez l’action **Imprimer** pour préparer le document physique que les employés utilisent pour noter les quantités comptabilisées.

## <a name="to-finish-a-physical-inventory-recording"></a>Pour finaliser un enregistrement de stock physique

Une fois que les employés ont compté les quantités, enregistrez les quantités dans [!INCLUDE [prod_short](includes/prod_short.md)].

1. Sur la page **Liste des enregistrements de stock physique**, sélectionnez l'enregistrement de stock physique que vous souhaitez terminer, puis sélectionnez l'action **Modifier**.
2. Sur le raccourci **Lignes**, renseignez la quantité comptabilisée réellement dans le champ **Quantité** pour chaque ligne.
3. Pour les articles avec des numéros de série ou de lot (la case **Utiliser le suivi des articles** est cochée), saisissez les quantités comptabilisées sur les lignes pour les numéros de lot et de série de l’article. Pour en savoir plus, rendez-vous sur [Gérer le suivi des articles lors du comptage des stocks](#handle-item-tracking-when-counting-inventory).
4. Sélectionnez la case à cocher **Enregistrée** sur chaque ligne.
5. Une fois que vous avez saisi toutes les données pour un enregistrement de stock physique, sélectionnez l'action **Terminer**. Vous observerez que toutes les lignes doivent avoir la case **Enregistrée** sélectionnée.

    > [!NOTE]
    > Lorsque vous avez terminé un enregistrement de stock physique, chaque ligne est transférée vers la ligne sur la commande de stock physique associée qui correspond exactement. Pour correspondre, les valeurs des champs **N° article**, **Code variante**, **Code magasin** et **Code emplacement** doivent être identiques sur l’enregistrement et les lignes de commande.>
    > 
    > Si une ligne de commande de stock physique correspondante n’existe pas, et si la case **Autoriser l’enregistrement sans commande** est cochée, une nouvelle ligne est ajoutée et la case **Enregistré sans commande** sur la ligne de commande de stock physique concernée est sélectionnée. Sinon, un message d’erreur s’affiche et le processus est annulé.> Si plusieurs lignes d’enregistrement de stock physique correspondent à une ligne de commande de stock physique, un message s’affiche et le processus est annulé. Si, pour une raison ou une autre, deux lignes de stock physique identiques arrivent sur la commande de stock physique, vous pouvez utiliser une action pour résoudre le problème. Pour en savoir plus, [Pour rechercher les doublons de lignes de commande de stock physique](#to-find-duplicate-physical-inventory-order-lines).

## <a name="to-complete-a-physical-inventory-order"></a>Pour finaliser une commande de stock physique

Une fois l’enregistrement d’un inventaire physique terminé, le champ  **Enregistreur de quantité (base)** de la commande d’inventaire physique associée est mis à jour avec les valeurs comptées (enregistrées) et la case à cocher  **Sur les lignes d’enregistrement** est sélectionnée. Si une quantité comptée diffère de la quantité attendue, les champs **Qté pos. (base)** et **Qté nég. (base)** affichent la différence.

Pour accéder les quantités prévues et toute différence enregistrée pour les articles avec le suivi des articles, sélectionnez l’action **Lignes**, puis choisissez **Lignes de suivi des articles** pour sélectionner différentes vues pour les numéros de lot et de série impliqués dans l’inventaire.

Vous pouvez aussi choisir l’action **Diff. commande de stock physique** pour visualiser les différences entre la quantité prévue et la quantité comptabilisé.

### <a name="to-find-duplicate-physical-inventory-order-lines"></a>Pour rechercher les doublons de lignes de commande de stock physique

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Commandes de stock**, puis choisissez le lien associé.
2. Ouvrez la commande de stock physique à afficher les doublons de lignes.
1. Dans l’onglet **Lié**, choisissez **Autre**, puis choisissez **Afficher les lignes en double**.

Tout doublon de ligne de commande de stock physique s’affiche de telle sorte que vous puissiez les supprimer et ne conserver qu’une ligne avec un ensemble de valeurs unique dans les champs **N° article**, **Code variante**, **Code magasin** et **Code emplacement**.

### <a name="to-post-a-physical-inventory-order"></a>Pour valider une commande de stock physique

Après avoir effectué une commande de stock physique et modifié son statut sur **Terminé**, vous pouvez la valider. Vous pouvez définir uniquement le statut d’une commande de stock physique sur **Terminé** sous les conditions suivantes :

- Tous les enregistrements du stock physique concerné ont un statut défini sur **Terminé**.
- Chaque ligne de commande de stock physique est comptabilisée par au moins une ligne d’enregistrement de stock.
- Les cases à cocher **Dans les lignes enregistrement** et **Qté prévue (calculée)** sont sélectionnées pour toutes les lignes de commande de stock physique.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Commandes de stock**, puis choisissez le lien associé.
2. Sélectionnez la commande de stock physique que vous souhaitez compléter, puis sélectionnez l'action **Modifier**.

    Sur la page **Commande de stock physique**, la quantité enregistrée s'affiche dans le champ **Qté enregistrée (de base)**.
3. Sélectionnez l'action **Terminer**.

    La valeur du champ **Statut** est **Terminé**. Vous ne pouvez désormais modifier l’ordre qu’en choisissant l’action **Rouvrir** .
4. Pour valider la commande, sélectionnez l'action **Valider**, puis le bouton **OK**.

    Les écritures comptables des articles sont mises à jour ainsi que les écritures de suivi des articles concernées.

    [!INCLUDE [preview-posting-inventory](includes/preview-posting-inventory.md)]

### <a name="to-view-posted-physical-inventory-orders"></a>Pour afficher les commandes de stock physique validées

Après validation, la commande de stock physique est supprimée et vous pouvez afficher et évaluer le document en tant que commande de stock physique validée. La commande validée inclut ses enregistrements de stock physique et tout commentaire effectué

1. Sélectionnez ![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Commandes de stock physique validées**, puis choisissez le lien associé.
2. Sur la page **Commandes de stock physique validées**, sélectionnez la commande de stock validée à afficher, puis sélectionnez l’action **Afficher**.
3. Dans l’onglet **Lié**, choisissez **Commande**, puis choisissez l’action **Enregistrements** pour afficher une liste des enregistrements d’inventaire physique associés.  

## <a name="handle-item-tracking-when-counting-inventory"></a>Gérer le suivi des articles lors de l’exécution de l’inventaire

Le suivi des articles concerne les numéros de lot ou de série attribués aux articles. Lorsque vous comptabilisez d’un article enregistré dans le stock, par exemple, 10 différents numéros de lot, l’employé doit être en mesure d’enregistrer quelles unités, et leur nombre, de chaque numéro de lot figurent en stock. Pour en savoir plus, voir [Utiliser les numéros de lot et de série](inventory-how-work-item-tracking.md).

La case à cocher **Utiliser le suivi des articles** sur les lignes de commande de stock physique est automatiquement sélectionnée si un code de suivi des articles est configuré pour l’article. Vous pouvez la cocher ou la décocher manuellement.

### <a name="example---prepare-a-physical-inventory-recording-for-an-item-tracked-item"></a>Exemple : Préparer un enregistrement de stock physique pour un article suivi

Imaginons un stock physique pour l'article A, enregistré en stock sous la forme de dix différents numéros de série.

1. Sur la ligne d’enregistrement pour l’article, sélectionnez la case **Utiliser le suivi des articles**.
2. Sélectionnez le champ **N° de série**, sélectionnez le premier numéro de série existant dans le stock pour l'article, puis cliquez sur le bouton **OK**.

    Copiez la ligne pour le premier article suivi pour insérer des lignes supplémentaires correspondant au nombre de numéros de série enregistrés en stock.

3. Choisissez l’action **Fonctions**, puis **Copier ligne**.
4. Sur la page **Copier la ligne enregistrement de stock physique**, saisissez **9** dans le champ **Nombre de copies**, puis sélectionnez le bouton **OK**.
5. Sur la première ligne, sélectionnez le champ **N° de série** et sélectionnez le numéro de série suivant pour l’article.
6. Répétez l’étape 5 pour les huit numéros de série restants. Assurez-vous de ne pas sélectionner deux fois le même numéro.
7. Choisissez l’action **Imprimer** pour préparer le bordereau que les employés utilisent pour écrire les numéros de lot/de série et les articles comptabilisés.

Vous observerez que l'état **Enregistrement de stock physique** contient dix lignes pour l'article A, un pour chaque numéro de série.

### <a name="example---record-and-post-counted-lot-number-differences"></a>Exemple : Enregistrer et valider les différences de numéro de lot comptabilisé

Un article suivi est enregistré en stock avec la série de numéro « LOT ».

**Stock prévu** :

|N° lot|Quantité|
|-|-|
|LOT1001|80|
|LOT1003|30|
|LOT1006|10|
|Total|120|

**Quantités enregistrées** :

|N° lot|Quantité|
|-|-|
|LOT1001|80|
|LOT0002|12|
|LOT1003|20|
|LOT1006|10|
|Total|112|

**Quantités à valider** :

|N° lot|Quantité prévue|Quantité enregistrée|Quantité à valider|
|-|-|-|-|
|LOT1001|80|80|0|
|LOT1002|0|12|+12|
|LOT1003|30|20|-10|
|LOT1006|10|0|-10|
|Total|120|112|-8|

Sur la page **Commande de stock physique**, le champ **Qté négative (de base)** contient **8**. Pour la ligne de commande, la page **Liste traçabilité stock physique** affiche les quantités positives ou négatives pour chaque n° de lot.

## <a name="inventory-documents"></a>Documents d’inventaire

Les types de documents suivants sont utiles pour gérer votre entrepôt :

* Utilisez **Réception d’inventaire** pour enregistrer les ajustements positifs des articles en fonction de la qualité, de la quantité et du coût.
* Utilisez **Expéditions d’inventaire** pour radier les marchandises manquantes ou endommagées.

Vous pouvez imprimer ces documents à tout moment, les publier, les rouvrir et leur attribuer des valeurs communes telles que des dimensions dans l’en-tête. Pour réimprimer les documents après leur publication, utilisez les pages **Réception d’inventaire validée** et **Expédition du stock validé**.

> [!NOTE]
> Avant de pouvoir utiliser ces documents, vous devez spécifier une souche de numéros pour créer leurs identificateurs. Pour en savoir plus, accédez à [Pour configurer la numérotation des documents d’inventaire](#to-set-up-numbering-for-inventory-documents).

### <a name="to-set-up-numbering-for-inventory-documents"></a>Pour paramétrer la numérotation des documents de stock

La procédure suivante indique comment définir la numérotation des documents stock.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Paramètres stock**, puis choisissez le lien associé.
2. Sur le Raccourci **Numérotation**, spécifiez dans les champs suivants la souche de numéros pour les documents :

   - **Numéros de reçus d’invt.**  
   - **Numéros de reçus d’inventaire affichés.**  
   - **Invt. Numéros d’expédition**  
   - **Numéros d’expédition d’inventaire affichés**  

### <a name="to-create-and-post-an-inventory-document"></a>Pour créer et publier un document d’inventaire

La procédure suivante montre comment créer, imprimer et valider un reçu d’inventaire. La procédure est identique pour des expéditions de stock.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Réceptions de stock**, puis choisissez le lien associé.  
2. Dans l’en-tête de la page **Reçu d’investissement**, choisissez l’emplacement dans le champ **Code d’emplacement**, puis remplissez les champs restants si nécessaire.
3. Sur le Raccourci **Lignes**, dans le champ **Article**, choisissez l’article en stock. Dans le champ **Quantité**, saisissez le nombre d’articles à ajouter.
4. Pour imprimer un rapport de **reçu d’inventaire** à partir de la page **reçu d’inventaire**, choisissez l’action **Imprimer** .

Les fonctions suivantes sont disponibles sur la page **Reçu d’investissement**  :

- Choisissez les actions **Libérer** ou **Rouvrir** pour définir le statut de la prochaine étape de traitement.  
- Choisissez l’action **Valider** pour enregistrer la réception stock, ou choisissez **Publier et imprimer** pour valider la réception et imprimer le rapport de test.  

    [!INCLUDE [preview-posting-inventory](includes/preview-posting-inventory.md)]

## <a name="printing-inventory-documents"></a>Impression des documents stock

Vous pouvez spécifier les états à imprimer à différentes étapes en choisissant l’une des options suivantes dans le champ **Utilisation** de la page **Sélection d’états – Stock** :

* Réception stock
* Expédition stock
* Réception stock validée
* Expédition stock validée

> [!NOTE]
> Les rapports disponibles peuvent varier en fonction de la localisation de votre pays/région. L’application de base n’inclut aucune présentation.

## <a name="see-also"></a>Voir aussi

[Compter, Ajuster et reclasser l’inventaire à l’aide de journaux](inventory-how-count-adjust-reclassify.md)    
[Travailler avec des numéros de série et de lot](inventory-how-work-item-tracking.md)    
[STOCKS ET EN-COURS](inventory-manage-inventory.md)    
[Vue d’ensemble de la gestion des entrepôts](design-details-warehouse-management.md)    
[Ventes](sales-manage-sales.md)    
[Achats](purchasing-manage-purchasing.md)    
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
