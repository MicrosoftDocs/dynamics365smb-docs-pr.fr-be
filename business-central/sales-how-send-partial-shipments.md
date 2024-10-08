---
title: Traiter les livraisons partielles
description: Les expéditions des commandes client peuvent être traitées dans Business Central avec des expéditions partielles à l’aide des champs Avis d’expédition et Quantité à expédier.
author: brentholtorf
ms.service: dynamics-365-business-central
ms.topic: conceptual
ms.search.keywords: 'shipping advice, partial shipments, partial deliveries, trade, customer sales order'
ms.date: 02/14/2024
ms.author: bholtorf
ms.reviewer: bholtorf
---
# <a name="process-partial-shipments"></a>Traiter les livraisons partielles

Dans une expédition partielle, une commande n’est pas expédiée en une seule fois. Par exemple, pour une commande de 100 unités, vous en expédiez 40 immédiatement et 60 ultérieurement. Il n’y a aucune limite quant au nombre de livraisons pouvant être effectuées pour une commande.

Cependant, avant de pouvoir utiliser des livraisons partielles dans [!INCLUDE [prod_short](includes/prod_short.md)], vous devez spécifier que le client accepte les livraisons partielles en définissant le champ **Avis d’expédition** sur la page **Fiche client**. Sinon, si le client n’accepte que des expéditions complètes, mais demande ensuite ou accepte une expédition partielle pour une commande client spécifique, vous pouvez modifier le champ **Avis d’expédition** avant validation.

Par défaut, [!INCLUDE [prod_short](includes/prod_short.md)] définit le champ dans la page **Fiche client** comme **Partiel**, ce qui permet des livraisons partielles. Toutefois, si le champ est défini pour spécifier **Complet**, puis le champ **Qté à expédier** apparait bloqué dans les commandes client pour ce client.

[!INCLUDE [order-ship-invoice_md](includes/order-ship-invoice.md)]

## <a name="see-also"></a>Voir aussi

[Vente de produits avec une commande vente client](sales-how-sell-products.md)  
[Expédition des articles](warehouse-how-ship-items.md)  
[Réalisation de livraisons directes](sales-how-drop-shipment.md)  
[Ventes](sales-manage-sales.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Administration](admin-setup-and-administration.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
