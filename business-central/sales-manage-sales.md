---
title: Aperçu des tâches permettant de gérer la comptabilité fournisseur | Microsoft Docs
description: Décrit comment gérer les activités des ventes.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8c80cbbc4ed4feb088116577157407dd8fb98aaf
ms.sourcegitcommit: c11ad91a389ed72532f5513654fdc7909b20aed9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/22/2021
ms.locfileid: "5935024"
---
# <a name="sales"></a>Ventes
Vous créez une facture vente ou une commande vente pour enregistrer votre accord avec un client pour vendre certains produits selon certaines conditions de livraison et de paiement.

Vous devez utiliser des commandes vente si votre processus de vente requiert que vous expédiiez des parties d’une quantité de commande, par exemple, si la quantité totale est pas disponible d’un coup. Si vous commercialisez des articles en les livrant directement du fournisseur au client, vous devez également utiliser les commandes vente. Pour tous les autres aspects, les commandes vente fonctionnent de la même manière que les factures vente. Avec les commandes vente, vous pouvez également utiliser la fonctionnalité de promesse de livraison pour indiquer les dates de livraison certaines à vos clients.  

Vous pouvez négocier avec le client en créant d’abord un devis, que vous pouvez convertir en facture vente ou en commande vente lorsque vous êtes d’accord sur la vente. Une fois que le client a confirmé l’accord, vous pouvez envoyer une confirmation de commande pour enregistrer votre obligation de fournir les produits comme convenu.

Vous pouvez facilement corriger ou annuler une facture vente validée avant qu’elle ne soit payée. Cela est utile si vous souhaitez corriger une erreur de saisie, ou si le client demande une modification tôt dans le processus de commande. Si la facture vente validée est payée, vous devez créer un avoir vente ou un retour vente pour contrepasser la vente.

Les pratiques recommandées en matière de vente et de marketing reposent toutes sur la prise de décisions appropriées au bon moment. La fonctionnalité Marketing de [!INCLUDE[prod_short](includes/prod_short.md)] fournit une vue d’ensemble précise et opportune de vos informations de contact afin d’offrir des services à vos prospects de manière plus efficace et d’accroître la satisfaction de la clientèle. Pour plus d’informations, reportez-vous à [Gestion des relations](marketing-relationship-management.md).

Si vous utilisez Dynamics 365 Sales for Customer Engagement, vous pouvez bénéficier de l’intégration parfaite dans le processus allant du prospect à l’encaissement à l’aide de Business Central pour les activités principales, telles que le traitement des commandes, la gestion des stocks et de vos finances. Pour plus d’informations, voir [Utilisation de Dynamics 365 Sales depuis Business Central](marketing-integrate-dynamicscrm.md).

Dans les environnements d’entreprise où le client doit payer avant la livraison des produits vendus (par exemple la vente au détail), vous devez attendre la réception du paiement avant de fournir les produits. Dans la plupart des cas, vous traitez les paiements entrants plusieurs semaines après la livraison en lettrant les paiements à leurs factures vente validées et impayées associées. Pour plus d’informations, voir [Rapprocher les paiements à l’aide du lettrage automatique](receivables-how-reconcile-payments-auto-application.md).

Les documents vente peuvent être envoyés sous forme de fichiers PDF joints à l’e-mail. Le corps du message contient alors un extrait du document vente, comme les produits, le montant total et un lien vers le site Paypal. Pour plus d’informations, voir [Envoyer des documents par e-mail](ui-how-send-documents-email.md).

Pour tous les processus de vente, vous pouvez incorporer un flux de travail d’approbation, par exemple, pour exiger que les ventes en grande quantité à certains clients soient approuvés par le responsable de la comptabilité. Pour plus d’informations, voir [Utilisation des flux de travail](across-use-workflows.md).

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.

| À | Voir |
| --- | --- |
|Créer une fiche client pour chaque client auquel vous vendez des éléments.|[Enregistrer de nouveaux clients](sales-how-register-new-customers.md)|
| Créer un devis dans lequel vous proposer des biens selon des conditions négociables avant de convertir le devis en facture vente. |[Créer des devis](sales-how-make-offers.md) |
| Créer une facture vente pour enregistrer votre accord avec un client pour vendre des biens selon certaines conditions de livraison et de paiement. |[Facturer des ventes](sales-how-invoice-sales.md) |
| Traiter une commande vente qui implique un envoi partiel ou un envoi direct. |[Vendre des produits](sales-how-sell-products.md) |
|Comprenez ce qui se passe lorsque vous publiez des documents vente.|[Validation des ventes](ui-post-sales.md)|
|Préparer au prélèvement pour l’expédition.|[Imprimer la liste des prélèvements](sales-how-print-picking-list.md)|
|Paramétrez les lignes vente ou achat standard que vous pouvez rapidement insérer dans les documents, par exemple, pour les ordres de réapprovisionnement récurrents.|[Créer des lignes ventes et achat récurrentes](sales-how-work-standard-lines.md)|  
| Lier une commande vente à une commande achat pour vendre un article qui sera livré directement par votre fournisseur à votre client. |[Effectuer des livraisons directes](sales-how-drop-shipment.md) |
|Faites expédier par un fournisseur un article de catalogue vers votre entrepôt pour pouvoir l’expédier à votre client.|[Créer des commandes spéciales](sales-how-to-create-special-orders.md)|
| Effectuer une action sur une facture vente enregistrée impayée pour créer automatiquement un avoir et soit annuler la facture vente, soit la recréer pour que vous puissiez y apporter des corrections. |[Corriger ou annuler des factures vente impayées](sales-how-correct-cancel-sales-invoice.md) |
| Créer un avoir vente pour rembourser une facture vente validée spécifique pour indiquer les produits que retourné par le client et le montant règlement que vous remboursez. |[Traiter les retours ou annulations de ventes](sales-how-process-sales-returns-cancellations.md) |
|Gérez l’engagement de vos clients à acheter de grandes quantités livrées en plusieurs expéditions sur une certaine période.|[Utiliser des commandes ouvertes vente](sales-how-to-create-blanket-sales-orders.md)|
|Vendez les éléments d’assemblage qui ne sont pas disponibles actuellement en créant un ordre d’assemblage associé pour fournir la quantité totale ou partielle de la commande vente.|[Vente d’articles à assembler pour commande](assembly-how-to-sell-items-assembled-to-order.md)|
|Facturez un client une seule fois pour plusieurs livraisons en combinant les expéditions sur une seule facture.|[Regroupement de bons de livraison sur une seule facture](sales-how-to-combine-shipments-on-a-single-invoice.md)|
|Informez vos clients des dates de livraison en calculant, soit la date de simulation de délai, soit la date disponible à la vente.|[Calculer des dates promesse livraison](sales-how-to-calculate-order-promising-dates.md)|
|Résolvez la confusion lorsque deux enregistrements ou plus existent pour le même client.|[Fusionner l’enregistrement des doublons](sales-how-merge-duplicate-records.md)|

## <a name="see-related-training-at-microsoft-learn"></a>Voir la formation associée sur [Microsoft Learn](/learn/paths/sell-items-services-dynamics-365-business-central/)

## <a name="see-also"></a>Voir aussi
[Définition des ventes](sales-setup-sales.md)  
[Enregistrer de nouveaux clients](sales-how-register-new-customers.md)  
[Gestion des comptes client](receivables-manage-receivables.md)  
[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Gestion de projets](projects-manage-projects.md)    
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Fonctionnalités marché](ui-across-business-areas.md)

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]
