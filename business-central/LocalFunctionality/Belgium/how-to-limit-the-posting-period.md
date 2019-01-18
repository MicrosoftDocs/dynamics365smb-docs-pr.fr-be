---
title: "Limitation de la période de validation"
description: "Vous pouvez limiter la période de validation autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 5306359e022a7d86f93c06971db9a14ca8f861db
ms.contentlocale: fr-be
ms.lasthandoff: 11/26/2018

---
# <a name="limit-the-posting-period"></a>Limiter la période de validation
Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez limiter la période de validation autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**.  

Limiter les périodes de validation peut être utile lorsqu'une société clôture sa feuille vente à la fin de chaque mois. Cela empêche les vendeurs d'enregistrer les documents vente du mois précédent. Par ailleurs, la feuille achat peut rester ouverte pour enregistrer les factures achat entrantes du mois précédent.  

Lorsque vous validez des écritures dans la page **Modèles feuille comptabilité**, le contenu du champ **Début période validation** et du champ **Fin période validation** est activé pour un intervalle de dates. L'intervalle de dates indique quand vous pouvez valider des écritures dans un modèle feuille. Si le champ est vide, la page **Paramètres utilisateur** est activée pour un intervalle de dates pour l'utilisateur actuel. Si la page **Paramètres utilisateur** ne contient pas d'intervalle, le champ **Début période validation** et le champ **Fin période validation** dans la page **Paramètres comptabilité** sont activés pour un intervalle de dates au niveau de la société.  

## <a name="to-limit-the-posting-periods-by-company"></a>Pour limiter les périodes de validation par société  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.  
2.  Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle la validation dans la société est activée.  
3.  Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle la validation dans la société est activée.  

## <a name="to-limit-the-posting-periods-by-user"></a>Pour limiter les périodes de validation par utilisateur  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres utilisateur**, puis choisissez le lien associé.  
2.  Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle l'utilisateur peut valider dans la société.  
3.  Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle l'utilisateur peut valider dans la société.  

## <a name="to-limit-the-posting-periods-by-template"></a>Pour limiter les périodes de validation par modèle  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille comptabilité**, puis sélectionnez le lien connexe.  
2.  Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle l'utilisateur peut valider dans la société.  
3.  Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle l'utilisateur peut valider dans la société.  

## <a name="see-also"></a>Voir aussi  
 [Fonctionnalité locale, Belgique](belgium-local-functionality.md)   
 [Définir des périodes de validation](../../finance-how-specify-posting-periods.md)

