---
title: Enregistrer la consommation ou l′utilisation des articles et des ressources du projet
description: Décrit comment enregistrer la consommation ou l’utilisation des articles ou des ressources sur des projets pour faciliter la gestion de projets.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, consumption
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 65975621fff862b64333c87e70f34b75f8e2cbdb
ms.sourcegitcommit: 93c8681054b059cec38cb29b86de20be37980676
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938109"
---
# <a name="record-consumption-or-usage-for-jobs"></a>Enregistrer la consommation ou l′utilisation pour les projets

Sur la page **Lignes planning projet**, vous pouvez consulter et enregistrer l’utilisation sur les différentes parties de votre projet, qui est automatiquement mis à jour lorsque vous modifiez et transférez des informations entre les projets et les feuilles projet ou les factures projet. Cela suppose d′avoir configuré un projet pour que l′option **Appliquer le lien d′utilisation** soit activée. Pour plus d’informations, voir [Configuration de projets](projects-how-setup-jobs.md).  

Par exemple, pour les lignes planning de type **Budget**, vous pouvez saisir la quantité d’une ressource et indiquer la quantité à transférer vers la feuille projet. Si le type de la ligne planning est **Facturable**, vous pouvez saisir la quantité de la ressource et indiquer la quantité à transférer vers une facture. Pour plus d′informations sur la facturation du client, voir [Projets de facturation](projects-how-invoice-jobs.md). En comparant la quantité d′origine, la quantité restante ou la quantité validée, vous pouvez rapidement consulter les informations d′utilisation. Pour plus d’informations sur l’estimation des valeurs budgétées lors de la planification, voir [Gérer les budgets de projets](projects-how-manage-budgets.md).  

Les procédures suivantes décrivent comment enregistrer les quantités (budgétées) et les coûts réels avec la feuille projet. Sinon, vous pouvez utiliser les documents achat pour enregistrer l′achat d′un projet. Pour plus d′informations, voir [Gérer les fournitures d’un projet](projects-how-manage-project-supplies.md).

## <a name="to-record-usage-for-a-job-planning-line-of-type-budget"></a>Pour enregistrer l’utilisation d’une ligne planning projet de type Budget

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Projets**, puis sélectionnez le lien associé.  
2. Sélectionnez le projet concerné, puis cliquez sur **Lignes planning projet**.
3. Sélectionnez une ligne planning projet de type **Budget** ou **Budget et Facturable** pour laquelle vous voulez enregistrer une utilisation.  

    > [!NOTE]
    > Vous pouvez également enregistrer l’utilisation d′une ligne planning projet de type **Facturable**. En général, vous utilisez ces lignes pour créer des factures, mais vous pouvez également les transférer vers une feuille. Pour plus d’informations, voir [Facturation des projets](projects-how-invoice-jobs.md) <!--However, when you do that, a job planning line of type **Budget** is created to match the billable line. For more information, see [Manage Job Budgets](projects-how-manage-budgets.md).-->

4. Dans le champ **Qté à transférer sur la feuille**, entrez le nombre que vous souhaitez transférer vers la facture. La quantité par défaut est la même valeur que celle du champ **Quantité**.

    Le champ **Quantité restante** indique la quantité qui reste pour terminer le projet et à transférer à la feuille.  
5. Choisissez l’action **Créer des lignes feuille projet**.

    > [!TIP]
    > Si vous allez ajouter d’autres lignes planning projet pour ce projet, attendez avec cette étape jusqu’à ce que vous ayez ajouté toutes les lignes planning projet.
6. Sur la page **Projet Transférer la ligne planning projet**, renseignez les champs selon vos besoins, puis cliquez sur le bouton **OK**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. Cliquez sur **Ouvrir la feuille projet**.  
8. Sur la page **Feuille projet**, sélectionnez la ligne appropriée, puis cliquez sur **Valider**.
9. Sur la page **Lignes planning projet**, examinez l’utilisation enregistrée en observant les champs **Quantité**, **Quantité restante** et **Qté à transférer sur la feuille**.  
10. Répétez les étapes 3 à 8 pour enregistrer l’utilisation supplémentaire.  

## <a name="to-create-job-journal-lines-manually"></a>Pour créer des lignes feuille projet manuellement

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Feuilles projet**, puis sélectionnez le lien associé.  
2. Dans le champ **Nom de la feuille**, choisissez un nom de feuille projet approprié.  
3. Dans une nouvelle ligne, entrez le numéro de document, le numéro de projet, le numéro tâche projet, le type et la quantité du type consommé.  
4. Lorsque les lignes feuilles projets sont renseignées, cliquez sur **Valider**.  

## <a name="to-view-job-usage-estimates-and-post-updates"></a>Pour visualiser les estimations projet et valider les mises à jour

Vous pouvez visualiser l′utilisation projet jusqu’à son achèvement en une étape. Pour ce faire, utilisez le traitement par lots **Projet Calc. utilisation restante** pour toutes les tâches jusqu’à la fin du projet.  

Cela vous permet de suivre vos estimations initiales, de les comparer aux résultats réels, ainsi que d’apporter des modifications et d’ajouter de nouvelles écritures, selon les besoins. Par exemple, alors que vous aviez estimé qu’un projet nécessitait 10 heures de travail, vous en avez effectué 15. Vous pouvez ajouter les cinq heures supplémentaires à la ligne feuille existante ou créer une ligne feuille pour les déclarer en tant qu’heures supplémentaires, ce qui constitue un autre type de tâche. Le coût et le prix appropriés sont calculés. Vous pouvez les valider dans la feuille.  

> [!NOTE]  
>   Les écritures article créent des écritures comptables article et diminuent les articles en stock. Le traitement par lots **Valider coûts ajustés** permet de transférer le coût du stock à la comptabilité. Les écritures ressource créent des écritures comptables ressource.  

1. Choisissez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles projet**, puis sélectionnez le lien associé.  
2. Sélectionnez une feuille projet appropriée, puis cliquez sur l’action **Calc. utilisation restante**.  
3. Sur la page **Projet Calc. utilisation restante**, entrez le numéro et la date de comptabilisation du document devant être insérés dans la feuille, puis sélectionnez le bouton **OK**.  
4. Mettez à jour la feuille avec toutes les modifications qui peuvent être nécessaires.  
5. Sélectionnez l’action **Valider**.



## <a name="to-review-planning-lines-for-a-job-ledger-entry"></a>Pour consulter les lignes planning pour une écriture comptable projet

Après avoir validé les lignes feuilles projets, vous pouvez voir les lignes planning associées à des écritures de la feuille projet qui ont été validées.

> [!NOTE]  
> Cela nécessite que la case **Appliquer le lien d′utilisation** soit cochée pour le projet. Pour plus d’informations, voir [Configuration de projets](projects-how-setup-jobs.md).  

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Feuilles projet**, puis sélectionnez le lien associé.  
2. Sélectionnez une feuille projet appropriée, puis cliquez sur **Écritures comptables**.  
3. Sur la page **Écritures comptables projet**, cliquez sur **Afficher les lignes planning projet liées**.

## <a name="see-also"></a>Voir aussi
[Gestion de projets](projects-manage-projects.md)  
[Finances](finance.md)  
[Achats](purchasing-manage-purchasing.md)         
[Ventes](sales-manage-sales.md)      
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
