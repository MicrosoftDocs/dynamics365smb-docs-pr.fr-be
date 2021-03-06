---
title: États et analyses de stock et d’entrepôt
description: Découvrez les états et analyses de stock et d’entrepôt disponibles dans la version standard de Business Central afin que vous puissiez suivre votre activité.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: 8a4418699f28acd3ede80616ba69c56f50781e43
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216453"
---
# <a name="inventory-and-warehouse-reports-and-analytics-in-business-central"></a>États et analyses de stock et d’entrepôt dans Business Central

Les états de stock et d’entrepôt dans [!INCLUDE [prod_short](includes/prod_short.md)] permettent aux professionnels des stocks et des affaires d’obtenir des informations et des statistiques sur les activités de stock et d’entrepôt actuelles et passées.  

## <a name="reports"></a>États

Le tableau suivant décrit certains des principaux états dans les états de stock et d’entrepôt.

|État |ID d’objet|Description  |
|---------|---------|---------|
|**Échéancier des dispo. de stock**|707|Si vous souhaitez avoir un aperçu d’articles/de points de stock spécifiques et de leur disponibilité. Cet état affiche des valeurs cumulées telles que les besoins bruts, les réceptions planifiées et prévues, le stock, etc. |
|**Évaluation du stock**|1 001|Affiche l’évaluation du stock des articles sélectionnés dans votre stock. L’état indique également des informations sur la valeur des augmentations et des diminutions de stock au fil du temps.|
|**Date expiration article : Quantité**|5809|Propose une vue d’ensemble des quantités des articles sélectionnés dans le stock dont les dates d’expiration sont incluses dans une période donnée. La liste indique le nombre d’unités de l’article sélectionné qui expirent à une date donnée. Pour chaque article spécifié lors du paramétrage de l’état, le document imprimé indique le nombre d’unités qui expirent au cours de trois périodes de même durée et la quantité d’inventaire totale de l’article sélectionné.<br>Vous pouvez définir ce que l’état doit inclure en configurant des filtres. Si vous ne définissez aucun filtre, l’état inclut tous les enregistrements. Les quantités indiquées dans l’état reflètent seulement les quantités des articles pour lesquels des dates d’expiration ont été définies.|
|**Ancienneté stock : Quantité** ou **Ancienneté stock : Valeur**|5807 ou 5808|Affiche un aperçu de l’ancienneté des articles sélectionnés dans votre stock. La liste indique la valeur ou le nombre d’unités de l’article sélectionné qui ont été ajoutées au stock ou supprimées du stock, ainsi que la date d’ajout ou de retrait. Les articles peuvent être ajoutés au stock ou supprimés de ce même stock après des achats, des ventes, et des ajustements positifs ou négatifs.|
|**Liste prix et coûts stocks**|716|Affiche la liste d’informations sur les prix des articles sélectionnés ou des points de stock : coût unitaire direct, dernier coût direct, prix unitaire, pourcentage de marge et marge. |
|**Liste emplacements entrep.**|7319|Affiche une vue d’ensemble des emplacements d’entrepôt, leur configuration et la quantité d’articles dans les emplacements. Cet état peut être utilisé pour tous les emplacements, qui ont « emplacement » comme champ obligatoire. |
|**Statut expédition entrepôt**|7313|Affiche un aperçu des documents origine ouverts avec les articles expédiés ou devant être expédiés, par magasin. Cet état peut être utilisé pour tous les magasins, pour lesquels **Envois requis** est activé. **Statut expédition entrepôt** affiche les magasins, les codes d’emplacement, le statut du document, les quantités.|
|**Liste des prélèvements stock**|813|Affiche la liste des commandes vente dans lesquelles un article est inclus. Les informations suivantes sont données pour chaque article : ligne commande vente avec le nom du client, code variante, code magasin, code emplacement, date d’expédition, quantité à expédier et unité. La quantité à livrer est totalisée pour chaque article. L’état peut être utilisé lorsque des articles vont être retirés du stock.<br>REMARQUE : cette fonctionnalité n’est pas disponible pour les fonctionnalités d’entrepôt avancées.|
|**Emplacement ajustement entrepôt**|7320|Cet état spécial est destiné uniquement à un entrepôt avancé et affiche les quantités restantes qui sont encore stockées dans l’emplacement ajustement lui-même. Normalement, cet emplacement spécifique doit être vide. La seule raison pour laquelle cet emplacement sera rempli est suite au processus de comptage physique ou si des quantités d’articles ont été retirées ou ajoutées à l’entrepôt|


## <a name="tasks"></a>Tâches

Les articles suivants décrivent certaines des tâches clés pour analyser l’état de votre entreprise :

* [Créer des rapports d’analyse](bi-how-create-analysis-views-reports.md)  
* [Voir la disponibilité des articles](inventory-how-availability-overview.md)


## <a name="see-also"></a>Voir aussi

[Configuration de stock](inventory-setup-inventory.md)  
[Stock](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)  
[Gestion d’entrepôt](warehouse-manage-warehouse.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
