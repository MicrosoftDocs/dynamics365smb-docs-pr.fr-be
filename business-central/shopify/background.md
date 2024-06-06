---
title: Exécuter des tâches en arrière-plan et de manière récurrente
description: Configurer la synchronisation des données entre Business Central et Shopify en arrière-plan.
ms.date: 03/26/2024
ms.topic: article
ms.service: dynamics-365-business-central
ms.reviewer: solsen
author: brentholtorf
ms.author: bholtorf
---

# Exécution des tâches en arrière-plan

Il est efficace d’exécuter certaines tâches simultanément et de manière automatisée. Vous pouvez effectuer ces tâches en arrière-plan et également définir un calendrier pour les exécuter automatiquement. Pour exécuter des tâches en arrière-plan, deux modes sont pris en charge :

- Les tâches déclenchées manuellement sont planifiées immédiatement via **Écritures file d’attente des travaux**.
- Les tâches récurrentes sont planifiées dans **Écritures file d’attente des travaux**.

## Exécuter des tâches en arrière-plan pour un magasin spécifique

1. Sélectionnez ![l’icône Ampoule qui ouvre la fenêtre de recherche.](../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Magasin Shopify**, puis sélectionnez le lien associé.
2. Sélectionnez le magasin pour lequel vous voulez exécuter la synchronisation à l’arrière-plan pour ouvrir la page **Fiche magasin Shopify**.
3. Activez **Autoriser les synchronisations en arrière-plan**.

Désormais, lorsque l’action de synchronisation démarre, au lieu d’exécuter une tâche au premier plan, vous serez invité à attendre. Une fois la synchronisation terminée, vous pouvez passer à l’action suivante. La tâche est créée comme **Écriture file d’attente des travaux** et démarre immédiatement.

## Pour programmer des tâches récurrentes

Vous pouvez programmer les activités récurrentes suivantes pour qu’elles soient exécutées de manière automatisée. Pour plus d’informations sur la planification des tâches, voir [File d’attente](../admin-job-queues-schedule-tasks.md).

|Tâche|Objet|
|------|------------|
|**Synchroniser les commandes à partir de Shopify**|État 30104 Synchroniser les commandes à partir de Shopify|
|**Traiter les commandes Shopify**|État 30103 Créer des commandes vente Shopify|
|**Synchroniser livraisons avec Shopify**|État 30109 Synchroniser livraison avec Shopify|
|**Synchroniser les produits et/ou les prix**|État 30108 Synchroniser les produits Shopify|
|**Synchroniser le stock**|État 30102 Synchroniser le stock avec Shopify|
|**Synchroniser les images**|État 30107 Synchroniser les images Shopify|
|**Synchroniser les clients**|État 30100 Synchroniser les clients Shopify|
|**Sociétés de synchronisation**|État 30114 Synchroniser les sociétés (B2B) Shopify|
|**Synchroniser les paiements**|État 30105 Synchroniser les paiements Shopify|
|**Sync. catalogues**|État 30115 Synchroniser les catalogues (B2B) Shopify|
|**Sync. prix catalogue**|État 30116 Shopify Sync. prix catalogue (B2B)|

> [!NOTE]
> Certains éléments peuvent être mis à jour par plusieurs tâches. Par exemple lorsque vous importez des commandes, selon le paramétrage dans la **fiche magasin Shopify**, le système peut également importer et mettre à jour des données client et/ou produit. N’oubliez pas d’utiliser la même catégorie de file d’attente pour éviter les conflits.

Autres tâches pouvant être utiles pour automatiser le traitement ultérieur des documents de vente :

- État 297 TPL validation factures vente
- État 296 TPL validation commandes vente

Vous pouvez utiliser le champ **N° de commande Shopify** pour identifier les documents commerciaux importés depuis Shopify.

Pour en savoir plus sur la validation de commandes client par lot, accédez à [Pour créer une entrée de file d’attente de tâches pour la validation par lots de commandes client](../ui-batch-posting.md#to-create-a-job-queue-entry-for-batch-posting-of-sales-orders).

## Pour examiner le statut de la synchronisation

Sur le **Chef d’entreprise** Centre de rôle, le **Shopify Activités** La pièce propose plusieurs indices qui peuvent vous aider à identifier rapidement s’il y a des problèmes avec Shopify Connecteur.

- **Clients non mappés** : Shopify le client est importé, mais n’est pas lié à une entrée client correspondante dans [!INCLUDE [prod_short](../includes/prod_short.md)].
- **Produits non mappés** – Shopify le produit est importé, mais n’est pas lié à une entrée article correspondante dans [!INCLUDE [prod_short](../includes/prod_short.md)].
- **Commandes non traitées** : Shopify les commandes sont importées, mais les documents de vente [!INCLUDE [prod_short](../includes/prod_short.md)] n’ont pas été créés, souvent à cause de produits ou de clients non cartographiés.
- **Envois non traités** : Les expéditions de vente publiées provenaient de Shopify les commandes ne sont pas synchronisées avec Shopify.
- **Erreurs d’expédition** : Shopify Le connecteur n’a pas pu synchroniser les expéditions de ventes publiées avec Shopify.
- **Erreurs de synchronisation** : Il y a des entrées de file d’attente de travaux ayant échoué liées à la synchronisation avec Shopify.

## Voir aussi

[Mise en route avec le connecteur Shopify](get-started.md)  
