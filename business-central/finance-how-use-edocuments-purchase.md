---
title: Utilisation des documents électroniques dans le processus achat
description: Découvrez comment utiliser la fonctionnalité de document électronique liée aux factures d’achat et les commandes.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'electronic document, electronic invoice, e-document, e-invoice, receive, purchase, matching, mapping, Copilot'
ms.search.form: '50, 51, 138, 6103, 6133, 6121, 6167, 9307, 9308'
ms.date: 05/02/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
---

# Utilisation des documents électroniques dans le processus achats

Vous pouvez utiliser des documents électroniques configurés (documents électroniques) avec les documents achat.

Vous pouvez utiliser les document achat suivants avec la fonctionnalité des documents électroniques :  

- Factures achat
- Commandes achat (version 24.0)
- Avoirs achat
- Feuilles comptabilité

> [!NOTE]
> Depuis la [!INCLUDE[prod_short](includes/prod_short.md)] version 24.0, il est possible de connecter **Commandes achat** aux **e-documents** reçus.  

## Documents électroniques achat

La réception des documents électroniques achat dans Dynamics 365 Business Central peut être effectuée par lots ou manuellement.  

### Comment configurer les fournisseurs pour qu’ils travaillent avec différents documents achat  

Suivez ces étapes pour configurer les fournisseurs afin qu’ils fonctionnent correctement avec les factures électroniques entrantes : 

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Fournisseurs**, puis sélectionnez le lien associé. 
2. Choisissez le fournisseur que vous souhaitez configurer.   
3. Dans l’onglet rapide **Réception**, recherchez le champ **Recevoir le document électronique à** pour spécifier le document d’achat par défaut à générer à partir du document électronique reçu. 

   > [!NOTE]
   > Dans le champ **Recevoir le document électronique à**, les utilisateurs peuvent sélectionner une **facture d’achat** ou **Commande achat** en fonction de ce qu’ils aimeraient créer à partir de la facture électronique reçue. Cette sélection n’affecte pas la création de documents correctifs ; dans les deux scénarios, le système générera une **Avoir**.  

   > [!NOTE]
   > Si l’utilisateur choisit l’option **Commande achat** dans le champ **Recevoir le document électronique à**, le système essaiera de mettre à jour l’un des Commande achat existants, mais si le Commande achat d’un fournisseur dans le **document électronique** reçu n’existe pas, le [!INCLUDE[prod_short](includes/prod_short.md)] créera un **Commande achat**, en utilisant la même approche que la création des nouvelles **factures achat** expliquées plus loin sur cette page.  

4. Choisissez l’une des options que vous souhaitez utiliser pour le fournisseur sélectionné. 
5. Fermez la page.   

### Pour utiliser des factures achat  

#### Exécuter le traitement par lots  

> [!NOTE]
> Ce traitement par lots est destiné à la collecte automatisée de vos factures entrantes. Cela ne peut fonctionner que dans un pays ou une région où la fonctionnalité existe.  

Chaque fois qu’une **file d’attente de tâches** est exécutée, si le service externe reçoit des factures envoyées par votre fournisseur, le système collecte et importe ces factures. Pour terminer le processus, procédez comme suit : 

1. Une fois le traitement par lots terminé, les factures récemment importées sont répertoriées dans la liste sur la page **Documents électroniques**, ainsi que leurs informations détaillées de base. 
2. Pour afficher plus de détails, ouvrez un document électronique spécifique.   
3. S’il n’y a eu aucune erreur ou problème dans le document électronique, le champ **Enregistrement** mappe le numéro de document de la facture achat créée s'il est configuré sur la page **carte fournisseur** (automatiquement par le système). Sélectionnez le lien pour ouvrir le document.
 
   > [!NOTE]
   > Ce document créé par le système n’est pas le document validé. 

4. Pour accéder directement au document achat, sélectionnez le champ **Enregistrement**. Après avoir ouvert la page **Facture achat**, vérifiez le document. Si tout est correct, validez le document.  
5. Lorsque vous validez le document d’achat, le champ **Enregistrement** du **document électronique** est mis à jour de **Facture** à **Facture achat** et le numéro du document achat validé est disponible. Vous pouvez sélectionner le numéro pour ouvrir la facture achat validée. 

Les détails des journaux sont les mêmes que ceux du processus de vente des documents électroniques.  

Étant donné que les erreurs dans le processus de vente sont principalement liées à la disponibilité du service, le document entrant peut contenir plusieurs raisons. La raison la plus courante d’une erreur est que le système ne peut pas reconnaître les lignes du document électronique que vous avez reçu de votre fournisseur. Il ne peut donc pas saisir de lignes dans votre facture achat. 

Il existe deux erreurs courantes :  

- Si vous souhaitez utiliser cette ligne spécifique de votre facture fournisseur qui a été directement imputée au compte du grand livre (G/L), vous devez avoir correctement configuré la valeur du **Texte de mappage**. Pour contourner cette erreur si vous souhaitez utiliser des comptes généraux, sélectionnez **Mapper le texte au compte** pour créer un mappage spécifique de la valeur **Texte de mappage** avec la valeur **N° cpte débit** que vous souhaitez utiliser. 
- Si vous souhaitez suivre l’inventaire et utiliser les lignes de votre facture fournisseur pour renseigner les articles sur vos lignes de document, vous devez avoir correctement configuré le **N° référence article** . Pour contourner cette erreur, mappez l’élément externe avec vos numéros d’article à l’aide de la liste de référence d’article. Pour plus d’informations, voir [Utiliser les références article](inventory-how-use-item-cross-refs.md). 

Après avoir corrigé les erreurs et les avertissements, vous pouvez spécifier manuellement quand le système doit créer une facture achat en fonction de votre configuration en sélectionnant **Créer un document**.   

#### Importer manuellement les factures  

Pour importer manuellement des documents électroniques externes, procédez comme suit :

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Service de document électronique**, puis sélectionnez le lien associé. 
2. Sur la page **Service de document électronique** , sélectionnez le service actif.   
3. Sélectionnez **Recevoir** et téléchargez le fichier de document électronique que vous avez reçu du fournisseur. 
4. Si un message d’erreur apparaît, ouvrez le document électronique pour résoudre les problèmes. 
5. Lorsque vous avez fini de résoudre les problèmes, dans le groupe **Importer manuellement**, sélectionnez **Créer un document**.  
6. Une fois le document créé dans [!INCLUDE[prod_short](includes/prod_short.md)], l’utilisation d’un travail par lots ne modifie pas la façon dont vous l’affichez. 

### Documents électroniques avec commandes achats  

#### Pour lier les commandes achat à la commande achat au document électronique reçu

Si votre **fournisseur** a configuré le champ **Recevoir le document électronique à** pour qu’il fonctionne avec **Commande achat**, une fois un document électronique créé dans [!INCLUDE[prod_short](includes/prod_short.md)] (manuellement ou à partir d’un point de terminaison externe), [!INCLUDE[prod_short](includes/prod_short.md)] effectueront les opérations suivantes :  

1. Si la **Commande achat** pour ce fournisseur particulier existe et qu’il existe un numéro de Commande achat dans le fichier **e-document** de réception, [!INCLUDE[prod_short](includes/prod_short.md)] associera automatiquement ce **document électronique** au **Commande achat** mentionné, et le **Statut du document** de ce **Document électronique** sera **En cours**, et le **Statut du document électronique** dans la sous-page **Statut du service** sera **Commande liée**. Ce lien sera visible dans le champ **Document** de ce **document électronique** spécifique. Si vous devez modifier automatiquement le **Commande achat** lié, vous pouvez le faire à l’aide de l’action **Mettre à jour le lien du Commande achat** et choisissez manuellement l’un des Commande achat existants pour ce fournisseur. Vous ne pouvez le faire qu’avant de faire correspondre les lignes entre le **document électronique** et **Commande achat**.  

2. Si la **Commande achat** pour ce fournisseur particulier, il existe mais il n’y a pas de numéro de bon de commande dans le reçu **Document électronique** déposer, [!INCLUDE[prod_short](includes/prod_short.md)] offrira la possibilité de choisir l’un des bons de commande existants quand et si vous avez téléchargé ce document manuellement. Cela ouvre le **Commande achat** liste avec les commandes uniquement pour le fournisseur dont vous avez reçu le **Document électronique**. Sélectionnez **commande achat** que vous souhaitez facturer, puis **OK**. Si vous n’avez pas réussi à sélectionner le bon **Commande achat** ou si vous avez obtenu le **document électronique** automatiquement à partir d’un point de terminaison externe à l’aide la **file d’attente des travaux**, un nouveau **document électronique** ne sera lié à aucun document d’achat. Le **Statut du document** affichera **Erreur** et **Document électronique** dans le sous-page **Statut du service** affiche aussi **erreur traitement document importé**. Pour terminer l’association avec le **Commande achat**, choisissez l’action **Mettre à jour le lien du Commande achat** et choisissez l’un des achats existants commandes pour ce fournisseur. 

3. Si le **Commande achat** pour ce fournisseur particulier n’existe pas au moment de la création du nouveau **document électronique**, [!INCLUDE[prod_short](includes/prod_short.md)] créera un nouveau **Commande achat**, en utilisant le même modèle de création qui existe déjà pour les nouvelles **factures achat**. Le **Statut du document** de cela **Document électronique** sera **Traité**, et le **Statut du document électronique** dans le **Statut du service** la sous-page sera **Document importé créé**. Ce lien sera visible dans le champ **Document** de ce **document électronique** spécifique.   

#### Lignes correspondantes du document électronique reçu avec le Commande achat  

Vous pouvez faire correspondre vos documents électroniques reçus avec les lignes de Commande achat provenant de deux endroits différents : depuis le **Document électronique** page ou à partir de la **Commande achat** page. Le moyen le plus simple de localiser le déjà lié **Commande achat** est d’utiliser le **Commande achat liés** vignette faisant partie de **Activités liées aux documents électroniques**. Tous les documents non liés peuvent être trouvés à l’aide de la vignette **En attente des factures électroniques d’achat** où vous avez une liste de **Documents électroniques** que vous devez revoir.  

> [!NOTE]
> Le **Activités liées aux documents électroniques** avec ces deux tuiles se trouve dans ce qui suit **Tableaux de bord** : Évaluation du chef d’entreprise, chef d’entreprise, comptable, gestionnaire des stocks et expédition et réception.  

> [!NOTE]
> Si le pourcentage de TVA diffère entre le document entrant et le pourcentage de TVA de l’entreprise, les documents correspondants ne peuvent pas être utilisés dans un environnement multi-pays.  

##### Correspondance des lignes de commande achat  

Vous pouvez faire correspondre les lignes du **Commande achat** liste ou à partir de l’une des listes ouvertes **Commande achat**. Pour commencer, procédez comme suit :  

1. Sélectionnez le **Commande achat liés** tuile sur votre Tableau de bord s’il y a un numéro. 
2. Choisir une des deux options de correspondance : 

   - Si vous souhaitez faire correspondre les lignes du **Commande achat** liste, sélectionnez le **Commande achat** ligne que vous souhaitez faire correspondre et choisissez la **Mapper les lignes de documents électroniques** action.  
   - Si vous souhaitez d’abord ouvrir le **Commande achat**, ouvrez le document, puis choisissez l’option **Mapper les lignes de documents électroniques** action. 

3. Comme les deux options ont le même processus, vous ouvrirez le **Correspondance des Commande achat** page avec le contenu suivant : 

    1. Dans l’en-tête, vous trouverez les informations suivantes, qui peuvent vous aider à cartographier plus facilement les lignes : 

       |Nom du champ |Description |
       |--------|-----------------|
       |Nom du fournisseur |Spécifie le nom fournisseur du document électronique. |
       |N° document électronique |Spécifie le numéro de document électronique lié. |
       |Date du document électronique |Spécifie la date du document électronique lié.  |
       |Montant document électronique |Spécifie le montant total du document électronique lié TVA comprise. |

    2. Dans les lignes, vous pourrez retrouver les lignes importées du **Document électronique** fichier sur le côté gauche et les lignes de l’existant **Commande achat** à droite.  
    3. Toutes les lignes des deux côtés comportent des numéros d’article et des descriptions, ainsi que le **Coût unitaire direct** et **% de remise sur la ligne**.  
    4. Du côté des **Lignes importées** , vous pouvez également localiser le champ **Quantité** en tant que quantité totale de la facture électronique et le champ **Quantité correspondante** spécifiant la quantité qui correspond déjà aux lignes de Commande achat. 
    5. Du côté des **Lignes de Commande achat**, vous pouvez également trouver la **Quantité disponible** qui correspond à la quantité qui peut être rapprochée de cette ligne (quantité reçue, mais non facturée) et **Qté. à la facture**, en précisant la quantité déjà rapprochée de cette ligne. 
    6. Pour faire correspondre les lignes, sélectionnez les lignes des deux côtés que vous souhaitez faire correspondre et choisissez l’action **Correspondre manuellement** . Les lignes correspondantes seront marquées en vert. 
    7. Il est possible de faire correspondre un à un, mais il est également possible d’en faire correspondre plusieurs à un ou un à plusieurs, en sélectionnant plus de lignes d’un côté ou de l’autre avant de choisir l’action **Correspondre manuellement**. 
    8. Vous pouvez également choisir l’action **Correspondre automatiquement** pour faire correspondre automatiquement toutes les lignes ayant le même **Type**, **Numéro**, **Prix unitaire**, **Remise** et **Unité de mesure**. 
    9. Si vous faites une erreur, vous pouvez choisir l’action **Supprimer la correspondance** pour supprimer les lignes correspondantes du côté du Commande achat ou choisir l’action **Réinitialiser la correspondance** action pour réinitialiser tout ce qui correspond. 
    10. Si votre **document électronique** comporte de nombreuses lignes, vous pouvez choisir l’action **Afficher les lignes en attente** pendant le processus de mise en correspondance, pour supprimez toutes les lignes du document électronique si elles correspondent déjà complètement. Si vous avez besoin de voir toutes les lignes, vous pouvez toujours choisir l’action **Afficher toutes les lignes** . 

4. Une fois la correspondance terminée, vous devez choisir l’action **Appliquer Commande achat** .   
5. Une fois que vous avez appliqué la correspondance au **Commande achat**, [!INCLUDE[prod_short](includes/prod_short.md)] mettra à jour les champs suivants :

    1. **Numéro de facture fournisseur** et **Date du document** sur l’en-tête du document seront mis à jour avec les valeurs du document électronique que vous avez reçu et lié. 
    2. **Qté. sur la facture** dans les lignes sera mis à jour avec les valeurs de la **Qté. dans la colonne Facture** de la page **Rapprochement des Commande achat** en fonction du correspondance que vous avez effectué. 
    3. Vous pouvez désormais valider un document en choisissant l’action **Valider**.  
    4. Une fois le document publié, le champ **Document** de la page **E-Document** modifiera la valeur et il sera se rapportent à la **facture d’achat reportée**. 
    5. Fermez la page.  

> [!IMPORTANT]
> Par défaut, vous pouvez rapprocher uniquement les lignes ayant le même montant total dans les deux documents. Cela signifie que le **Coût unitaire direct** ainsi que la ligne appliquée **% de remise** doivent être les mêmes, comme dans un document que vous peut avoir un montant sans remise et un autre avec remise.  

Si vous souhaitez ajouter une certaine tolérance et autoriser la différence entre les lignes de la **facture électronique** et du **Commande achat**, suivez ces marches :   

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Paramètres achat**, puis sélectionnez le lien associé.  
2. Vous souhaitez autoriser la tolérance dans le champ **Différence de correspondance entre les documents électroniques %** , en spécifiant le pourcentage maximum autorisé de différence de coût lors de la correspondance avec les **documents électroniques entrants** ligne avec la ligne **Commande achat**. 
3. Cette configuration s’appliquera à toutes les lignes correspondantes, mais encore une fois en tenant compte de la tolérance sur le montant total, comme pour le **Coût unitaire direct** avec la **remise de ligne appliquée %**.  
4. Fermez la page.   

##### Correspondance les lignes d’un document électronique  

Vous pouvez faire correspondre les lignes sur la page **E-Document** . Pour commencer, procédez comme suit :  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Documents électronique**, puis sélectionnez le lien associé. 
2. Sélectionnez **documents électroniques** que vous souhaitez correspondre.   
3. Choisissez l’action **Rapprocher le Commande achat** pour ouvrir la page **Rapprocher le Commande achat**.  
4. Répétez les mêmes étapes que celles utilisées lorsque vous avez commencé à rapprocher les Commande achat.

### Copilote aide à la mise en correspondance de documents électroniques  

> [!NOTE]
> Actuellement, le copilote **Assistance à la correspondance de documents électroniques** est en version préliminaire prête pour la production et est disponible dans le monde entier, sauf au Canada. Cela ne fonctionne qu’en anglais. 

> [!NOTE]
> Copilot est l’Assistant optimisé par l’IA qui aide les gens de votre organisation à libérer leur créativité et à automatiser les tâches fastidieuses. Le copilote **Assistance de rapprochement de documents électroniques** aide les utilisateurs à faire facilement correspondre les factures électroniques reçues avec les lignes de bon de commande existantes, en utilisant le modèle LLM pour faire correspondre les lignes entre deux documents différents. 

#### Pour activer le copilote  

Si vous n’avez pas activé le copilote **Assistance de correspondance de documents électroniques**, vous devez le faire manuellement. Pour activer le copilote **Assistance de correspondance de documents électroniques**, suivez ces étapes : 

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Copilote et capacités IA**, puis sélectionnez le lien associé. 
2. Dans la liste des fonctionnalités, choisissez **Assistance de mise en correspondance de documents électroniques** et modifiez le statut en **Actif**.  

Une fois le copilote activé, vous pouvez commencer à l’utiliser.

#### Utiliser le copilote aide à la mise en correspondance de documents électroniques 

Si le copilote est activé, les actions existantes **Mapper les lignes de documents électroniques** sur les commandes achetées et **Faire correspondre le Commande achat** sur le **Document électronique** La page obtiendra différentes icônes, symbolisant la capacité de l’IA. Vous pouvez exécuter ces actions (les mêmes que dans les exemples précédents à partir de la liste des Commande achat), depuis l’un des **Acheter en ligne**, ou de **Document électronique**. Toutes les étapes d’exécution sont les mêmes, mais lorsque vous exécutez cette action, le résultat sera différent et vous devez suivre ces étapes :  

1. Choisir la **Mapper les lignes de documents électroniques** ou **Faire correspondre le Commande achat** action, pour les documents déjà liés.  
2. Remarquer que **Lignes de commande de correspondance de documents électroniques avec Copilot** l’invite fonctionne et vous avez le **Rapprochement des Commande achat** page en arrière-plan. Cela signifie que le même processus se produit mais avec le support automatique du **Copilot**, qui gère le processus de mise en correspondance à votre place. 
3. Après quelques secondes, le **Lignes de commande de correspondance de documents électroniques avec copilote** suggérera des lignes à faire correspondre avec quelques détails supplémentaires : 

    1. Dans l’en-tête de l’invite, vous pouvez trouver les informations suivantes : 

       |Nom du champ |Description |
       |--------|-----------------|
       |Correspondance automatique | Spécifie le nombre de correspondances proposées automatiquement. Ceci est basé sur une comparaison de chaînes et s’il y a 80 % ou plus de descriptions qui se chevauchent, le système fera automatiquement correspondre ces descriptions sans utiliser les fonctionnalités GPT. |
       |Mis en correspondance par Copilot | Spécifie le nombre de correspondances proposées par le copilote en utilisant à la fois une comparaison de chaînes et sémantique. |
       |N° document électronique | Spécifie le numéro du document électronique lié. |
       |Montant total de la facture, hors TVA | Spécifie le montant total de la facture, hors TVA. |
       |Montant total mis en correspondance, TVA comprise | Spécifie le montant mis en correspondance, avec TVA. |
    
    2. Si toutes les lignes correspondent, vous verrez le texte vert dans le coin supérieur droit : **Toutes les lignes (100 %) correspondent. Examiner les propositions de match**.  
    3. Dans les lignes **Proposition correspondance**, vous pouvez trouver les informations suivantes :  

       |Nom du champ |Description |
       |--------|-----------------|
       |N° ligne document électronique | Spécifie le numéro de ligne du document électronique (provenant du fichier de document électronique d’origine). |
       |Description de la ligne document électronique | Spécifie la description de ligne du document électronique (provenant du fichier de document électronique d’origine). |
       |Quantité mise en correspondance | Spécifie la quantité qui sera appliquée à la ligne de commande achat. |
       |Proposition | Spécifie l’action proposée par AI, et ces actions suggérées sont liées à la mise en correspondance des lignes de Commande achat. |

    4. Toutes les lignes entièrement suggérées et assorties sont marquées de couleur verte. S’il y a un problème, c’est-à-dire un prix différent, mais dans la fourchette de prix autorisée, cette ligne sera marquée en jaune, et s’il y a une similitude entre les champs de description mais que la différence de prix est supérieure à celle autorisée, cette ligne sera marquée en rouge. 
    5. Si vous n’êtes pas satisfait de certaines suggestions, vous pouvez les supprimer en utilisant le **Supprimer la ligne** action.  
    6. Si vous souhaitez voir les correspondances de propositions, vous pouvez sélectionner le lien dans le **Proposition** colonne pour ouvrir la **Détails de la correspondance des documents électroniques** page. 
    7. Sur le **Détails de la correspondance des documents électroniques** page, vous pouvez comparer les détails de la **Document électronique** et **Commande achat**, pour être sûr de la correspondance proposée avant de la confirmer. 
    8. Après avoir examiné, fermez la page.   

4. Si vous n’êtes pas satisfait de la plupart des suggestions, ou si vous ne souhaitez pas utiliser la fonctionnalité **Lignes de commande de correspondance de documents électroniques avec Copilot**, sélectionnez **L'ignorer** et vous pourrez continuer la correspondance manuelle comme expliqué précédemment.  
5. Si vous souhaitez conserver les suggestions, choisissez le bouton **Conserver** et le système enregistrera toutes les suggestions faites par **Copilote**.  
6. [!INCLUDE[prod_short](includes/prod_short.md)] fermera l’invite de Copilot et les lignes de la page **Rapprochement des Commande achat** seront marquées en vert, car elles sont déjà rapprochées. 
7. Vous pouvez désormais continuer à travailler pendant que vous effectuez une correspondance manuelle ; cela signifie que vous pouvez supprimer des correspondances, les faire correspondre manuellement ou réinitialiser la correspondance. Si vous ne souhaitez pas apporter de modifications, choisissez simplement l’action **Appliquer au bon de commande** et continuez à travailler avec le **Bon de commande**. 

> [!NOTE]
> Vous pouvez choisir l’action **Mettre en correspondance avec Copilot** sur la **Rapprochement des Commande achat** à nouveau, mais dans cette Dans ce cas, il vous sera demandé si vous souhaitez écraser les correspondances existantes, car toutes les lignes ont déjà été mises en correspondance.  

> [!NOTE]
> L’analyse prix/coût et le contrôle de la quantité disponible font partie de l’activité de prétraitement.   

## Vue d’ensemble des statuts des documents électroniques

Pour obtenir un meilleur aperçu de tous les documents électroniques de l’entreprise, vous pouvez sélectionner le centre de rôles **Comptable** où existent les statuts des documents électroniques. Vous y trouverez des activités de documents électroniques qui ont les statuts suivants :

- **Documents électroniques entrants :**

    - Traité
    - En cours
    - Erreur


## Voir aussi

[Configurer des documents électroniques](finance-how-setup-edocuments.md)    
[Utilisation du documents électroniques dans le processus vente](finance-how-use-edocuments.md)   
[Extension de la fonctionnalité des documents électroniques](/dynamics365/business-central/dev-itpro/developer/devenv-extend-edocuments)    
[Gestion financière](finance.md)    
[Facturation des ventes](sales-how-invoice-sales.md)    
[Enregistrer les achats avec les factures achat et les commandes](purchasing-how-record-purchases.md)    
[Utiliser Business Central](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]

