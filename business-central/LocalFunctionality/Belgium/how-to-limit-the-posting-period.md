---
title: Limitation de la période de validation
description: 'Vous pouvez limiter la période de validation autorisée selon trois niveaux différents : par société, par utilisateur et par modèle.'
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9d7a3bbd18e9dfc2419a6bd0edce7b8db5643fd7
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779231"
---
# <a name="limit-the-posting-period"></a>Limiter la période de validation
Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], vous pouvez limiter la période de validation autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**.  

Limiter les périodes de validation peut être utile lorsqu'une société clôture sa feuille vente à la fin de chaque mois. Cela empêche les vendeurs d'enregistrer les documents vente du mois précédent. Par ailleurs, la feuille achat peut rester ouverte pour enregistrer les factures achat entrantes du mois précédent.  

Lorsque vous validez des écritures dans la page **Modèles feuille comptabilité**, le contenu du champ **Début période validation** et du champ **Fin période validation** est activé pour un intervalle de dates. L'intervalle de dates indique quand vous pouvez valider des écritures dans un modèle feuille. Si le champ est vide, la page **Paramètres utilisateur** est activée pour un intervalle de dates pour l'utilisateur actuel. Si la page **Paramètres utilisateur** ne contient pas d'intervalle, le champ **Début période validation** et le champ **Fin période validation** dans la page **Paramètres comptabilité** sont activés pour un intervalle de dates au niveau de la société.  

## <a name="to-limit-the-posting-periods-by-company"></a>Pour limiter les périodes de validation par société  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Paramètres comptabilité**, puis sélectionnez le lien associé.  
2.  Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle la validation dans la société est activée.  
3.  Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle la validation dans la société est activée.  

## <a name="to-limit-the-posting-periods-by-user"></a>Pour limiter les périodes de validation par utilisateur  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Paramètres utilisateur**, puis sélectionnez le lien associé.  
2.  Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle l'utilisateur peut valider dans la société.  
3.  Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle l'utilisateur peut valider dans la société.  

## <a name="to-limit-the-posting-periods-by-template"></a>Pour limiter les périodes de validation par modèle  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Modèles feuille comptabilité**, puis sélectionnez le lien associé.  
2.  Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle l'utilisateur peut valider dans la société.  
3.  Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle l'utilisateur peut valider dans la société.  

## <a name="see-also"></a>Voir aussi  
 [Fonctionnalité locale, Belgique](belgium-local-functionality.md)   
 [Définir des périodes de validation](../../finance-how-specify-posting-periods.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]