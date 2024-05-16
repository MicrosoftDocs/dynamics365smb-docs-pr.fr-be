---
title: Aperçu des tâches permettant de gérer vos ventes
description: "Découvrez comment utiliser les services de Business\_Central pour gérer les activités de vente avec vos clients avec des factures de vente, des commandes, des devis et plus encore."
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: overview
ms.search.keywords: 'trade, sell'
ms.search.form: '253,'
ms.date: 01/25/2024
ms.custom: bap-template
ms.service: dynamics-365-business-central
---

# Vente

Vous créez une facture vente ou une commande vente pour enregistrer votre accord avec un client pour vendre certains produits selon certaines conditions de livraison et de paiement.

Vous devez utiliser des commandes vente si votre processus de vente requiert que vous expédiiez des parties d’une quantité de commande, par exemple, si la quantité totale est pas disponible d’un coup. Si vous commercialisez des articles en les livrant directement du fournisseur au client, vous devez également utiliser les commandes vente. Pour tous les autres aspects, les commandes vente fonctionnent de la même manière que les factures vente. Avec les commandes vente, vous pouvez également utiliser la fonctionnalité de promesse de commande pour indiquer les dates de livraison certaines à vos clients.  

Vous pouvez négocier avec le client en créant d’abord un devis, que vous pouvez convertir en facture vente ou en commande vente lorsque vous êtes d’accord sur la vente. Une fois que le client confirme l’accord, vous pouvez envoyer une confirmation de commande pour enregistrer votre obligation de fournir les produits comme convenu.

Vous pouvez facilement corriger ou annuler une facture vente validée avant le paiement client. Par exemple, si vous souhaitez corriger une erreur de saisie, ou si le client demande une modification tôt dans le processus de commande. Si la facture vente validée est payée, vous devez créer un avoir vente ou un retour vente pour contrepasser la vente.

Les pratiques recommandées en matière de vente et de marketing reposent toutes sur la prise de décisions appropriées au bon moment. La fonctionnalité Marketing de [!INCLUDE[prod_short](includes/prod_short.md)] fournit une vue d’ensemble précise et opportune de vos informations de contact afin d’offrir des services à vos prospects de manière plus efficace et d’accroître la satisfaction de la clientèle. En savoir plus sur [Gestion des relations](marketing-relationship-management.md).

Si vous utilisez Microsoft Dynamics 365 Sales pour for Customer Engagement, vous pouvez utiliser [!INCLUDE [prod_short](includes/prod_short.md)] pour le traitement intégration transparente dans le processus allant du prospect à l'encaissement pour activités backend. Par exemple, pour traiter les commandes, gérer les stocks et gérer vos finances. En savoir plus, [Utiliser Dynamics 365 Sales depuis Business Central](marketing-integrate-dynamicscrm.md).

Dans les environnements d’entreprise où le client doit payer avant la livraison des produits vendus (par exemple la vente au détail), vous devez attendre la réception du paiement avant de fournir les produits. Dans la plupart des cas, vous traitez les paiements entrants plusieurs semaines après la livraison en lettrant les paiements à leurs factures vente validées et impayées associées. En savoir plus [Rapprocher les paiements à l’aide du lettrage automatique](receivables-how-reconcile-payments-auto-application.md).

Les documents vente peuvent être envoyés sous forme de fichiers PDF joints à l’e-mail. Le corps du message contient un extrait du document vente, comme les produits, le montant total et un lien vers le site Paypal. En savoir plus sur [Envoyer des documents par e-mail](ui-how-send-documents-email.md).

Pour tous les processus de vente, vous pouvez intégrer un flux de travail approbation. Par exemple, un flux de travail approbation peut exiger qu’un responsable approuve les ventes importantes à certains clients. En savoir plus sur [Utiliser des flux de travail](across-use-workflows.md).

Le section suivant décrit une série de tâches et inclut des liens vers les articles qui les décrivent.

## Démarrer avec les capacités ventes

Avant de vendre, précisez comment vous souhaitez gérer les processus de vente de votre entreprise.

|Pour...| Voir |
|---|---|
| Créer une fiche client pour chaque client auquel vous vendez des éléments.|[Enregistrement de nouveaux clients](sales-how-register-new-customers.md) |
| Définissez la manière dont vous effectuez les ventes, comme les prix et les remises, les groupes de prix clients et de remises, les vendeurs, les méthodes d’expédition et les agents. | [Configuration des ventes](sales-setup-sales.md) |

## Analyse vente

Cette section décrit les outils analytiques que vous pouvez utiliser pour obtenir des informations sur vos données de vente.

| Pour... | Voir |
| --- | --- |
| Découvrez les fonctionnalités d’analyse des données de vente. | [Vue d’ensemble de l’analyse vente](sales-analytics-overview.md) |
| Effectuez une analyse ad hoc des données de vente directement sur les pages de liste et les requêtes. | [Créer des rapports d’analyse vente](bi-how-create-analysis-views-reports.md) |
| Explorer états intégrés pour la vente. | [États vente intégrés](sales-reports.md) |

## Devis de commande à facture de vente

Le tableau suivant décrit comment utiliser des processus de vente simples.

|Pour...| Voir |
|---|---|
| Créer un devis dans lequel vous proposer des biens selon des conditions négociables avant de convertir le devis en facture vente. |[Réalisation des devis](sales-how-make-offers.md) |
| Traiter une commande vente (peut-être avec un Livraison partielle ou un envoi direct.) |[Vente des produits](sales-how-sell-products.md) |
| Créez une facture vente pour enregistrer votre accord avec un client de vendre certains produits selon certaines conditions de livraison et de paiement. |[Facturation des ventes](sales-how-invoice-sales.md) |
|Comprenez ce qui se passe lorsque vous publiez des documents vente.|[Validation des ventes](ui-post-sales.md)|

Si vous avez besoin de processus de vente plus complexes, le tableau suivant répertorie les articles qui expliquent ce que vous pouvez faire avec [!INCLUDE[prod_short](includes/prod_short.md)].

|Pour...| Voir |
|---|---|
| Exécutez une commande client avec plusieurs livraisons partielles. | [Traiter les livraisons partielles](sales-how-send-partial-shipments.md) |
| Paramétrez les lignes vente ou achat standard que vous pouvez rapidement insérer dans les documents, par exemple, pour les ordres de réapprovisionnement récurrents.|[Créer des lignes ventes et achat récurrentes](sales-how-work-standard-lines.md)|  
|Gérez l’engagement de vos clients à acheter de grandes quantités livrées en plusieurs expéditions sur une certaine période.|[Utilisation des commandes cadres vente](sales-how-to-create-blanket-sales-orders.md)|
|Facturez un client une seule fois pour plusieurs livraisons en combinant les expéditions sur une seule facture.|[Regroupement de bons de livraison sur une seule facture](sales-how-to-combine-shipments-on-a-single-invoice.md)|
|Vendez les éléments d’assemblage qui ne sont pas disponibles actuellement en créant un ordre d’assemblage associé. L’ordre d’assemblage peut fournir la quantité totale ou partielle figurant sur la commande client.|[Vente d’articles à assembler pour commande](assembly-how-to-sell-items-assembled-to-order.md)|

## Effectuer un prélèvement et une expédition

Le tableau suivant décrit comment prélever des articles pour une commande client et les expédier au client.

| À | Voir |
| --- | --- |
|Préparer au prélèvement pour l’expédition.|[Impression de la liste des prélèvements](sales-how-print-picking-list.md)|
| Lier une commande vente à une commande achat pour vendre un article qui sera livré directement par votre fournisseur à votre client. |[Effectuer des livraisons directes](sales-how-drop-shipment.md) |
|Faites expédier par un fournisseur un article de catalogue vers votre entrepôt pour pouvoir l’expédier à votre client.|[Création des commandes spéciales](sales-how-to-create-special-orders.md)|
|Informez vos clients des dates de livraison en calculant, soit la date de simulation de délai, soit la date disponible à la vente.|[Calcul des dates promesse livraison](sales-how-to-calculate-order-promising-dates.md)|
| Découvrez comment suivre un colis à partir d’une expédition de vente validée. | [Suivi des paquets](sales-how-track-packages.md) |

## Commandes annulées, remboursements et retours

Le tableau suivant décrit comment gérer les commandes annulées, les remboursements et les retours de marchandises.

| À | Voir |
| --- | --- |
| Effectuer une action sur une facture vente enregistrée impayée pour créer automatiquement un avoir et soit annuler la facture vente, soit la recréer pour que vous puissiez y apporter des corrections. |[Corriger ou annuler des factures vente impayées](sales-how-correct-cancel-sales-invoice.md) |
| Créer un avoir vente pour rembourser une facture vente validée spécifique pour indiquer les produits que retourné par le client et le montant remboursez. |[Traitement des retours ou annulations de ventes](sales-how-process-sales-returns-cancellations.md) |

## Autres processus de vente

Le tableau suivant décrit comment traiter autres des processus de vente.

| À | Voir |
| --- | --- |
|Résolvez la confusion lorsque deux enregistrements ou plus existent pour le même client.|[Fusion des enregistrements en double](sales-how-merge-duplicate-records.md)|

## Voir aussi

[Définition des ventes](sales-setup-sales.md)  
[Enregistrement de nouveaux clients](sales-how-register-new-customers.md)  
[Vue d’ensemble de l’analyse vente](sales-analytics-overview.md)   
[Gestion des comptes client](receivables-manage-receivables.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Fonctionnalités marché](ui-across-business-areas.md)

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
