---
title: Comment restreindre et autoriser l’utilisation d’un enregistrement
description: 'Pour restreindre l’utilisation d’un enregistrement, vous pouvez incorporer deux réponses de flux de travail dans un flux de travail qui contrôle l’utilisation de l’enregistrement.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 04/26/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="restrict-and-allow-usage-of-a-record"></a>Restriction et autorisation de l’utilisation d’un enregistrement

Si vous souhaitez restreindre l’utilisation d’un enregistrement à certaines activités, par exemple, jusqu’à ce qu’il ait été approuvé, vous pouvez ajouter deux réponses de flux de travail dans un flux de travail qui contrôle l’utilisation de l’enregistrement. Une réponse de flux de travail limitera l’utilisation de l’enregistrement telle que définie par l’événement et les conditions du flux de travail. Une autre réponse de flux de travail autorise l’utilisation de l’enregistrement telle que définie par l’événement et les conditions du flux de travail. Deux réponses existent dans la version par défaut de [!INCLUDE[prod_short](includes/prod_short.md)] à cet effet : **Ajouter une limitation d’enregistrement** et **Supprimer une limitation d’enregistrement**.

> [!NOTE]  
> La version par défaut de [!INCLUDE[prod_short](includes/prod_short.md)] permet de restreindre la validation d’un enregistrement, son exportation pour paiement, et l’impression sous la forme d’un chèque. Pour prendre en charge d'autres restrictions, un partenaire Microsoft doit personnaliser le code de l'application.  

> [!NOTE]  
> La fonctionnalité de flux de travail pour restreindre et autoriser l'utilisation d'un enregistrement n'est pas liée à la fonctionnalité de blocage de la validation d'un enregistrement d'article, de client et de fournisseur.

La procédure suivante explique comment restreindre la validation de commandes d’achat tant qu’elles n’ont pas été approuvées. Le nouveau flux de travail est basé sur le modèle de *flux de travail approbation facture achat*.  

## <a name="create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a>Créer une étape de flux de travail qui limite la validation de commandes d’achat non approuvées

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Flux de travail**, puis choisissez le lien associé.  
2. Sur la page **Flux de travail**, choisissez l’action **Créer flux de travail à partir du modèle**. En savoir plus sur [Créer des flux de travail à partir de modèles de flux de travail](across-how-to-create-workflows-from-workflow-templates.md).
3. Sur la page **Modèles de flux de travail**, sélectionnez le modèle *Flux de travail approbation facture achat*.  

   Remarquez que les deux premières étapes du flux de travail concernent la restriction, puis l’autorisation de l’utilisation des factures d’achat. Modifiez la condition d’événement de la première étape du nouveau flux de travail pour indiquer qu’il s’applique aux commandes d’achat.  
4. Dans le raccourci **Étapes du flux de travail**, cliquez sur le champ **Condition** pour la première étape, puis, pour le filtre **Type document**, sélectionnez **Commande**.  
5. Modifiez, supprimez ou ajoutez d’autres étapes de flux de travail pour prendre en charge un processus entreprise qui commence par restreindre la validation des commandes achat non approuvées.  

## <a name="see-also"></a>Voir aussi

[Utilisation des flux de travail approbation](across-use-workflows.md)  
[Création des flux de travail d’approbation](across-how-to-create-workflows.md)  
[Flux de travail](across-workflow.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
