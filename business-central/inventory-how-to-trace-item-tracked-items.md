---
title: Tracer les articles suivis
description: 'Vous pouvez voir où un article suivi a été utilisé, y compris comment et quand il a été reçu, produit ou retourné grâce aux fonctionnalités de suivi des articles et de recherche d’entrées.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.forms: '6520,'
ms.date: 05/16/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="trace-item-tracked-items"></a>Tracer les éléments suivis

Vous pouvez voir où un article suivi a été utilisé, y compris le mode et le moment de réception ou de production, de transfert, de vente, de consommation ou de retour. Vous pouvez également rechercher toutes les instances d'informations d'un numéro de série ou de lot particulier dans la base de données. Vous procédez à l’aide des fonctionnalités Traçabilité et [Rechercher des écritures](ui-find-entries.md).  

Ces fonctionnalités peuvent être utiles dans le contrôle qualité lorsque vous devez savoir quels clients ont reçu des produits avec un numéro de lot particulier ou lorsque vous devez savoir de quel lot provient un composant défectueux.  

 Sur la page **Traçabilité**, vous pouvez effectuer une traçabilité en aval et en amont dans une série de mouvements de stock validés pour le numéro de lot ou de série.  

 Sur la page  **Rechercher des entrées**, vous ne pouvez pas voir la séquence des transactions, mais vous pouvez voir tous les enregistrements du numéro de série ou de lot, à la fois les entrées publiées et les enregistrements ouverts.  

 Les deux fonctions peuvent être utilisées en association en transférant un numéro de série ou de lot suivi sur la page **Rechercher des écritures** pour terminer un scénario complet de suivi. <!-- For more information, see [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).   -->

## <a name="to-trace-item-tracked-items"></a>Pour tracer des articles suivis

1.  Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Traçabilité**, puis choisissez le lien associé.  
2.  Dans les champs de filtre dans le haut de la page, entrez les numéros d'article spécifiques ou un filtre pour les numéros d'article que vous voulez suivre.  
3.  Dans le champ **Afficher composants**, sélectionnez si vous voulez aussi voir d’où provenaient les composants des articles. Le tableau suivant décrit les options.  

    |Champ|Description|  
    |----------------------------------|---------------------------------------|  
    |**Non**|Ne pas afficher les composants.|  
    |**Avec traçabilité uniquement**|Afficher uniquement les composants qui ont des numéros de lot ou de série.|  
    |**Tous**|Afficher tous les composants.|  

4.  Dans le champ **Méthode de suivi**, sélectionnez la méthode à utiliser pour suivre l’article. Le tableau suivant décrit les options.  

    |Champ|Description|  
    |----------------------------------|---------------------------------------|  
    |**Utilisation->origine**|Suivez l’article à l’endroit où il a été utilisé jusqu’à l’endroit d’où il vient. Par exemple, si un article fabriqué a été vendu à un client, la page **Traçabilité** présente ce dernier en montrant d'abord la ligne expédition vente, que vous pouvez développer pour voir l'ordre de fabrication dont il provenait.|  
    |**Origine->utilisation**|Suivez l’article à l’endroit où il a été stocké jusqu’à l’endroit où il a été utilisé. Par exemple, si un article fabriqué a été vendu à un client, la page **Traçabilité** présente ce dernier en montrant d’abord l’ordre de fabrication terminé, que vous pouvez développer pour voir les lignes expédition vente où l’article a été utilisé.|  

5.  Sélectionnez l'action **Suivi** pour exécuter le suivi.  

> [!NOTE]  
>  Seules les transactions lettrées sont indiquées. Si vous avez reçu le même lot sur plusieurs transactions, la page **Traçabilité** peut ne pas afficher toutes les transactions.   

> [!NOTE]  
>  Si l'historique d'une transaction supplémentaire dans une ligne traçabilité a déjà été suivi par une autre ligne au-dessus de celle-ci, la case à cocher **Déjà tracé** est activée. Pour une vue plus simple, ces lignes sous-jacentes ne s'affichent pas.  
>   
>  Pour trouver les lignes traçabilité où l'historique des transactions a déjà été suivi, cliquez sur le bouton **Aller sur déjà tracé**. La ligne traçabilité en question est sélectionnée et toutes les lignes sous-jacentes sont développées.  

## <a name="to-find-item-tracked-items-with-find-entries"></a>Pour rechercher des articles suivis avec Rechercher des écritures

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Rechercher des écritures**, puis sélectionnez le lien associé.  
2. Choisissez **Rechercher des références d’articles**.
3. Dans les champs **N° de série** et **N° lot**, entrez les numéros traçabilité que vous voulez suivre.  
4. Sélectionnez l'action **Rechercher** pour rechercher toutes les instances du numéro de série ou de lot dans la base de données.  

## <a name="see-also"></a>Voir aussi

[Stock](inventory-manage-inventory.md)  
[Utiliser les numéros lot, de série et paquet](inventory-how-work-item-tracking.md)  
[Détails de conception : traçabilité](design-details-item-tracking.md)  
[Détails de conception : traçabilité et réservations](design-details-item-tracking-and-reservations.md)  
[Réservation des articles](inventory-how-to-reserve-items.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
<!-- [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md)   -->
[Rechercher des écritures](ui-find-entries.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
