---
title: États et analyses de production
description: Découvrez les états et analyses de production disponibles dans la version standard de Business Central afin que vous puissiez suivre votre activité.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: 0cacf41f0a055267af5b0ce5a8b68b34d86a1cb5
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216452"
---
# <a name="production-reports-and-analytics-in-business-central"></a>États et analyses de production dans Business Central

Les états de production dans [!INCLUDE [prod_short](includes/prod_short.md)] permettent aux professionnels de la production et des affaires d’obtenir des informations et des statistiques sur les activités de production actuelles et passées.  

## <a name="reports"></a>États

Le tableau suivant décrit certains des principaux états dans les états de production.

|État |ID d’objet|Description  |
|---------|---------|---------|
|**Nomenclature multi-niveau**|99000753|Affiche la liste des nomenclatures multi-niveaux pour l’article ou les articles que vous définissez dans les filtres. La nomenclature de production est entièrement éclatée pour tous les niveaux.|
|**Article – Capable de fabriquer (Temps)**|5871|Indique comment cinq chiffres de disponibilité principaux différents évoluent dans le temps pour un article de nomenclature. Ces chiffres sont modifiés en fonction des événements d’offre et de demande prévus et de l’approvisionnement qui est basé sur les composants disponibles qui peuvent être assemblés ou produits.<br>Vous pouvez utiliser l’état pour vérifier si vous pouvez traiter une commande vente d’un article à une date spécifique, en consultant sa disponibilité actuelle ainsi que les quantités potentielles que ses composants peuvent fournir si un ordre d’assemblage a été lancé. L’état indique la date et le nombre d’unités d’un élément d’assemblage et de production que vous pouvez fabriquer, en fonction de la disponibilité des composants et de la disponibilité actuelle de l’article. Cela est affiché en tant que quantité totale.<br>Les informations sont affichées dans un graphique dans lequel chaque chiffre de disponibilité est une ligne qui progresse dans la chronologie et se déplace vers le haut ou vers le bas en fonction des modifications des quantités. Les chiffres de quantité proviennent du même moteur qui fournit des informations dans la fenêtre **Disponibilité article par niveau de nomenclature**. |
|**Distribution coût total nomenclature**|5872|Indique graphiquement la manière dont le coût d’un article assemblé ou produit est distribué dans sa nomenclature.<br>Ces informations peuvent être utiles pour décider, par exemple, de changer de fournisseurs de composants, de remplacer une utilisation interne de capacité par un travail externalisé, ou inversement, ou lors de l’examen et de la modification de la nomenclature d’un article.<br>Le premier graphique de l’état affiche le coût unitaire total des composants et des ressources de travail de l’article parent, réparti en cinq parts de coût différentes au maximum et représenté graphiquement par des couleurs différentes.<br>Le graphique en secteurs avec la légende *Par matière/travail* affiche la répartition proportionnelle entre les coûts de matériel et de travail de l’article parent, ainsi que ses propres frais généraux de fabrication. La part du coût matière inclut les coûts matière de l’article. La part du coût de travail inclut la capacité, les frais généraux opératoires et les coûts de sous-traitance. Les parts de coûts sont affichées différemment en fonction des choix indiqués dans le champ **Afficher uniquement**.<br>Le graphique en secteurs avec la légende *Par direct/indirect* affiche la répartition proportionnelle entre les coûts directs et indirects de la nomenclature. La part des coûts directs inclut les coûts matière, de capacité et les coûts de sous-traitance de l’article. La part des coûts indirects inclut les frais généraux opératoires et les frais généraux de fabrication.<br>Le tableau en bas de l’état est inclus lorsque vous activez la case à cocher **Inclure détails**. Il affiche les valeurs sélectionnées dans la fenêtre Coûts totaux nomenclature par mono-niveau ou multi-niveau, en fonction du choix que vous avez effectué dans le champ **Afficher coût total comme**.|
|**Coût détaillé**|99000756|Affiche la liste des coûts par article en tenant compte du rebut.|
|**Cas d’emploi (multi-niveau)**|99000757|Affiche où et en quelle quantité sont utilisés les articles dans la structure produit.<br>L’état indique uniquement l’article comme cas d’emploi lorsque l’article de base est utilisé comme article de niveau supérieur. Par exemple, si l’article A est utilisé pour fabriquer l’article B, et que l’article B est utilisé pour fabriquer l’article C, l’état affiche l’article B si vous exécutez cet état pour l’article A. Si vous exécutez l’article B, l’article C est affiché comme cas d’emploi.<br>Vous pouvez également ouvrir la page **Ligne cas d’emploi** directement à partir de l’article.|
|**Liste de comparaison des nomenclatures article**|99000758|Cet état vous donne la possibilité de comparer des produits finis similaires concernant les coûts. Vous verrez une liste de tous les composants et leurs coûts, ainsi que les quantités nécessaires. La date de calcul est normalement fixée à la date de travail. |
|**Statistiques O.F.**|99000791|Spécifie les différents coûts qui se sont cumulés de l’ordre de fabrication sélectionné.<br>Le contenu de l’état est presque identique à la page **Statistiques O.F.**.<br>Pour les ordres de fabrication utilisant la méthode de fabrication *Fabrication à la commande*, la fenêtre n’affiche que le coût matière et capacité des articles au niveau de nomenclature le plus élevé.|
|**Liste des tâches par capacité**|99000780|Indique les ordres de fabrication en attente de traitement dans les centres ou les postes de charge. Les documents imprimés indiquent la capacité du centre ou du poste de charge). L’état comprend les données telles que l’heure début et fin, la date O.F. et la quantité d’entrée.|
|**Charge centre de charge** ou **Charge poste de charge**|99000783 ou 99000784|Les deux états affichent la liste de la charge d’un centre de charge ou d’un poste de charge. La charge d’un centre de charge/poste de charge représente la somme du nombre d’heures nécessaires pour exécuter toutes les commandes réelles et planifiées dans un centre de charge, sur une période précise.|
|**Liste des ruptures O.F.**|99000788|Cet état peut être utilisé pour voir tous les composants qui ne sont pas disponibles en raison d’un stock manquant. Ainsi, cet aperçu peut être utilisé pour voir si le calendrier d’un ordre de fabrication planifié ou lancé et si le temps planifié peuvent être respectés.|


## <a name="tasks"></a>Tâches

Les articles suivants décrivent certaines des tâches clés pour analyser l’état de votre entreprise :

* [Afficher la charge des centres de charge et des postes de charge](production-how-to-view-the-load-on-work-centers.md)  
* [Voir la disponibilité des articles](inventory-how-availability-overview.md)

## <a name="see-also"></a>Voir aussi

[Paramétrage de la production](production-configure-production-processes.md)  
[Production](production-manage-manufacturing.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
