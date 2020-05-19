---
title: Afficher les informations sur les tables
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/20/2020
ms.author: jswymer
ms.openlocfilehash: de93063a60e6b64405b1491a67489c8bfa4657ad
ms.sourcegitcommit: 99915b493a7e49d12c530f2f9fda1fcedb518b6e
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/21/2020
ms.locfileid: "3275331"
---
# <a name="viewing-table-information"></a>Affichage d'informations sur les tables

La page **Informations sur les tables 8700** fournit des informations sur toutes les tables système et métier d'une solution Business Central. En particulier, la page affiche des informations sur la quantité de données contenues dans les tables.

Ces informations sont utiles pour résoudre les problèmes de performances, car nous allons voir la répartition de la taille des données entre les tables.

## <a name="viewing-table-information"></a>Affichage d'informations sur les tables

Pour ouvrir cette page, sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Informations sur les tables**, puis sélectionnez le lien connexe.

Le tableau suivant décrit les informations fournies pour chaque table :

|Colonne|Description|
|------|-----------|
|Nom de la société|Nom de la société, si existant, à laquelle appartient la table.|
|Nom de la table|Nom de la table.|
|Numéro table|ID unique de la table|
|Non. d'enregistrements|Nombre total d'enregistrements stockés dans la table.|
|Taille enregistrement|La taille d'enregistrement moyenne en Ko/enregistrement. La valeur est calculée à l'aide de la formule suivante : 1024 (Taille)/Nbre d'enregistrements). |

## <a name="see-also"></a>Voir aussi

[Inspection des pages](across-inspect-page.md)  
[Articles sur les performances pour les développeurs](/dynamics365/business-central/dev-itpro/performance/performance-developer)  