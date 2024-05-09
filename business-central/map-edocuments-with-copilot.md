---
title: Mappage de documents électroniques avec les lignes commandes achat avec Copilot
description: Découvrez comment utiliser Copilot pour mapper des documents électroniques aux lignes de bon de commande.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: altotovi
ms.topic: how-to
ms.collection:
  - get-started
  - bap-ai-copilot
ms.date: 04/10/2024
ms.custom: bap-template
---

# <a name="map-e-documents-to-purchase-order-lines-with-copilot-preview"></a>Mappage de documents électroniques avec les lignes commandes achat avec Copilot (version préliminaire)

À mesure que les processus d’approvisionnement deviennent de plus en plus numériques, la fonctionnalité de documents électroniques de Business Central joue un rôle clé dans l’automatisation de la réception et du traitement des factures des fournisseurs. Copilot peut vous aider dans ce processus en améliorant le mappage et la mise en correspondance des factures des fournisseurs avec les bons de commande. Cela réduit les tâches fastidieuses qui comprendraient normalement des recherches approfondies et la saisie de données. L’avantage est aggravé par le fait que les factures des fournisseurs ne correspondent souvent pas exactement aux bons de commande, auquel cas Copilot est mieux placé pour identifier les bons de commande correspondants. Les capacités de rapprochement améliorées profitent particulièrement aux petites et moyennes entreprises qui ont besoin d’un suivi efficace des documents pour les lignes de commande d’achat. Copilot est l’assistant de travail basé sur l’IA qui stimule la créativité et améliore la productivité des utilisateurs de Business Central.

> [!IMPORTANT]
> - Il s’agit d’une fonctionnalité en version préliminaire prêt pour la production pour les environnements de production et sandbox dans n’importe quel pays, à l’exception du Canada.
> - Les fonctionnalités en version préliminaire prêtes pour la production sont soumises à des conditions d’utilisation supplémentaires. En savoir plus : [Conditions d’utilisation supplémentaires pour la version préliminaire de Dynamics 365](https://go.microsoft.com/fwlink/?linkid=2105274)
> - Le contenu généré par l’IA est peut-être incorrect.

Dans la version initiale du **document électronique** application, nous avons introduit des scénarios fondamentaux pour les documents électroniques pour l’ensemble du processus de vente. Cependant, il est nécessaire d’améliorer et d’automatiser le traitement des documents reçus, notamment dans le contexte des processus d’achat. Copilot affine la façon dont vous gérez les documents électroniques dans le processus d’achat, notamment en ce qui concerne les bons de commande. Le cadre de documents électroniques vous permet de spécifier le type de document d’achat à créer pour chaque fournisseur lorsque vous recevez des factures électroniques de sa part. Auparavant, la seule option consistait à créer une facture d’achat, soit sous forme de document, soit sous forme de journal du grand livre.

Vous pouvez désormais mettre à jour un bon de commande existant dans Business Central avec les informations reçues dans la facture électronique.

<!--
> [!NOTE]
> - This feature is available as a production-ready preview for production and sandbox environments in any country localization, with the exception of Canada. Production-ready previews are subject to supplemental terms of use. For more information, see [Supplemental terms of use for Dynamics 365 preview](https://go.microsoft.com/fwlink/?linkid=2105274).
> - AI-generated content may be incorrect.-->

## <a name="to-activate-copilot"></a>Pour activer le copilote

Si vous n’avez pas activé le copilote **Assistance de correspondance de documents électroniques**, vous devez le faire manuellement. Pour activer le copilote **Assistance de correspondance de documents électroniques**, suivez ces étapes : 

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Copilote et capacités IA**, puis sélectionnez le lien associé. 
2. Dans la liste des fonctionnalités, choisissez **Assistance de mise en correspondance de documents électroniques** et modifiez le statut en **Actif**.  

Vous pouvez commencer à utiliser Copilot dès qu’il est activé. 

## <a name="identify-purchase-orders"></a>Identifier commandes achat

Tout d’abord, vous pouvez identifier les bons de commande que vous pouvez automatiquement rapprocher. Si votre **fournisseur** a configuré le champ **Recevoir le document électronique à** pour qu’il fonctionne avec **Commande achat**, une fois le document électronique créé dans [!INCLUDE[prod_short](includes/prod_short.md)] (manuellement ou à partir d’un point de terminaison externe), [!INCLUDE[prod_short](includes/prod_short.md)] effectueront les opérations suivantes :

1. Si le **bon de commande** pour ce fournisseur particulier *existe et qu’il y a un numéro de bon de commande* dans le reçu **Fichier de document électronique** , [!INCLUDE[prod_short](includes/prod_short.md)] liera automatiquement ce **document électronique** au **spécifié**bon de commande. Le **Statut du document** de cela **Document électronique** sera **En cours**, et le **Statut du document électronique** dans le **Statut du service** la sous-page sera **Commande liée**.  
Ce lien sera visible dans le champ **Document** de ce **document électronique** spécifique. Si vous devez modifier automatiquement le **Commande achat** lié, vous pouvez le faire à l’aide de l’action **Mettre à jour le lien du Commande achat** et choisissez manuellement l’un des Commande achat existants pour ce fournisseur. Vous ne pouvez le faire qu’avant de faire correspondre les lignes entre le **document électronique** et **Commande achat**.  
2. Si le **Commande achat** pour ce fournisseur particulier *existe mais qu’il n’y a pas de numéro de Commande achat* dans **le document électronique** de réception fichier, [!INCLUDE[prod_short](includes/prod_short.md)] offrira la possibilité de choisir l’un des Commande achat existants quand et si vous avez téléchargé ce document manuellement, en ouvrant la liste des **Commande achat** avec les commandes uniquement. pour le fournisseur que vous avez obtenu **Document électronique**, dans lequel vous devez sélectionner **Commande achat** vous souhaitez et sélectionner **D’accord**. Si vous n’avez pas sélectionné le **Commande achat** approprié ou si vous avez obtenu le **document électronique** automatiquement d’un destinataire externe point utilisant la **file d’attente des travaux**, le nouveau **document électronique** ne sera lié à aucun document d’achat et le **Le statut du document** sera **Erreur** et le **Statut du document électronique** dans la sous-page **État du service** est **Erreur de traitement du document importé**. Pour terminer l’association avec le **Commande achat**, choisissez l’action **Mettre à jour le lien du Commande achat** et choisissez l’un des achats existants commandes pour ce fournisseur.  

## <a name="map-lines"></a>Mapper les lignes

Copilot vous aide à faire correspondre automatiquement les lignes de facture électronique avec les lignes de bon de commande et offre des informations de correspondance supplémentaires pour améliorer les correspondances.

Une fois qu’ils ont été rapprochés et mappés, [!INCLUDE [prod_short](includes/prod_short.md)] met à jour le bon de commande rapproché avec les informations de réception pertinentes pour garantir que les bonnes quantités sont reçues sur les lignes de commande.

Vous pouvez faire correspondre vos documents électroniques reçus avec les lignes de Commande achat provenant de deux endroits différents, depuis le **Documents électroniques** page ou à partir de la **Commande achat** page. Le moyen le plus simple de localiser le déjà lié **Commande achat** est d’utiliser le **Commande achat liés** vignette faisant partie de **Activités liées aux documents électroniques**. Tous les documents non liés se trouvés à l’aide de la vignette **En attente des factures électroniques d’achat** où vous avez une liste de **Documents électroniques** que vous devez revoir.  

> [!NOTE]
> Le **Activités liées aux documents électroniques** avec ces deux tuiles se trouve dans ce qui suit Tableaux de bord : **Évaluation du chef d’entreprise**, **chef d’entreprise**, **comptable**, **gestionnaire des stocks** et **expédition et réception**.

Lorsque vous souhaitez exécuter un rapprochement à partir du bon de commande, choisissez l’action **Mapper les lignes de document électronique** , qui existe à la fois sur les pages de bon de commande et de liste de bons de commande. Toutefois, si vous souhaitez exécuter le rapprochement à partir de la page **E-Documents** , choisissez l’action **Rapprocher le bon de commande** de cette page. Pour terminer la correspondance, procédez comme suit :

1. Choisir la **Mapper les lignes de documents électroniques** ou **Faire correspondre le Commande achat** action, pour les documents déjà liés.  
2. Vous pouvez remarquer que **Lignes de commande de correspondance de documents électroniques avec Copilot** l’invite fonctionne et vous avez le **Rapprochement des Commande achat** page en arrière-plan. Cela signifie que le même processus se produit mais avec le support automatique du **Copilote**, qui gère le processus de mise en correspondance à votre place. 
3. Après quelques secondes, le **Lignes de commande de correspondance de documents électroniques avec copilote** suggérera des lignes à faire correspondre avec détails supplémentaires : 

    1. Dans l’en-tête de l’invite, vous pouvez trouver les informations suivantes : 

    |Nom du champ |Désignation |
    |--------|-----------------|
    |Correspondance automatique | Spécifie le nombre de correspondances proposées automatiquement. Ceci est basé sur une comparaison de chaînes et s’il y a 80 % ou plus de descriptions qui se chevauchent, le système fera automatiquement correspondre ces descriptions sans utiliser les fonctionnalités GPT. |
    |Mis en correspondance par Copilot | Spécifie le nombre de correspondances proposées par Copilot en utilisant à la fois une comparaison de chaînes et sémantique. |
    |N° document électronique | Spécifie le numéro du document électronique lié. |
    |Montant total de la facture, hors TVA | Spécifie le montant total de la facture, hors TVA. |
    |Montant total mis en correspondance, TVA comprise | Spécifie le montant mis en correspondance, hors TVA. |
    
    2. Si toutes les lignes correspondent, vous verrez le texte vert dans le coin supérieur droit : **Toutes les lignes (100 %) correspondent. Examiner les propositions de match**.  
    3. Dans les lignes **Proposition correspondance**, vous trouver les informations suivantes :  

    |Nom du champ |Désignation |
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

4. Si vous n’êtes pas satisfait de la plupart des suggestions, ou si vous ne souhaitez pas utiliser la fonctionnalité **Lignes de commande de correspondance de documents électroniques avec copilote**, sélectionnez **L'ignorer** et vous pourrez continuer [la correspondance manuelle](finance-how-use-edocuments-purchase.md) comme expliqué précédemment.  
5. Si vous souhaitez conserver les suggestions, choisissez le bouton **Conserver** et le système enregistre toutes les suggestions faites par **Copilote**.  
6. [!INCLUDE[prod_short](includes/prod_short.md)] ferme l’invite du copilote et les lignes de la page **Rapprochement des Commande achat** seront marquées en vert, car elles sont déjà rapprochées.  
7. À partir de ce moment, vous pouvez continuer à travailler pendant que vous effectuez une correspondance manuelle, ce qui signifie que vous pouvez supprimer des correspondances, des correspondances manuelles, réinitialiser la correspondance ou si vous ne souhaitez apporter aucune modification, choisissez simplement le **Action Appliquer au Commande achat** et continuez à travailler avec le **Commande achat**. 

> [!NOTE]
> Vous pouvez choisir l’action **Mettre en correspondance avec le copilote** dans la **Rapprochement des Commande achat** à nouveau, mais dans cette Dans ce cas, il vous est demandé si vous souhaitez écraser les correspondances existantes, car toutes les lignes sont déjà mises en correspondance.  

> [!NOTE]
> L’analyse prix/coût et le contrôle de la quantité disponible font partie de l’activité de prétraitement. 

## <a name="see-also"></a>Voir aussi

[Vue d’ensemble des documents électroniques](finance-edocuments-overview.md)    
[Utiliser des documents électroniques vente](finance-how-use-edocuments.md)    
[Utiliser les documents électroniques achat](finance-how-use-edocuments-purchase.md)   
[Résoudre les problèmes des fonctionnalités de Copilot et d’IA](ai-copilot-troubleshooting.md)    
[FAQ sur l’IA responsable pour l’assistance au rapprochement bancaire](faqs-bank-reconciliation.md)    