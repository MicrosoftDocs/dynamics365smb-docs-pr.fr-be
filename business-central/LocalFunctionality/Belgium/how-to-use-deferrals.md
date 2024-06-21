---
title: Échelonnements dans les rapports Journal des ventes et Journal des achats
description: Apprenez à configurer et à utiliser les échelonnements dans les rapports Journal des ventes et Journal des achats dans la version belge de Business Central.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'deferral, sales ledger, purchase ledger'
ms.search.form: '279, 1700, 1701'
ms.date: 03/13/2023
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# Échelonnements dans les rapports Journal des ventes et Journal des achats

Lorsque vous utilisez les échelonnements, les rapports Journal des ventes et Journal des achats dans la version belge de Dynamics 365 Business Central ne doivent montrer que les écritures d’origine des factures et des avoirs, et non celles créées à l’aide des échelonnements.

## Configurer des échelonnements

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Paramètres codes journaux**, puis sélectionnez le lien associé.  
2. Sous le raccourci **Général**, entrez les informations dans les champs obligatoires et les champs décrits dans le tableau ci-dessous.  

    |      Champ   |         Description        |
    |--------------|----------------------------|
    | **Report général** | **Code journal** utilisé par le système pour les échelonnements créés à partir de la validation des feuilles comptabilité. |
    | **Échelonnement ventes** | **Code journal** utilisé par le système pour les échelonnements créés à partir de la validation dans les documents vente. |
    | **Report d’achat** | **Code journal** utilisé par le système pour les échelonnements créés à partir de la validation dans les documents achat. |
    
3. Sélectionner **OK**.

> [!NOTE]
> Vous pouvez configurer des codes journaux spécifiques pour les validations d’échelonnements ou utiliser le même code journal pour la feuille comptabilité, les feuilles ventes et la feuille achat.  

## Rapports belges Journal des ventes et Journal des achats

Une fois les écritures échelonnement dotées d’un code journal spécifique, vous pouvez manipuler les vues de rapport en sélectionnant **Exclure écritures échelonnement** dans les rapports Journal des ventes et Journal des achats. 

Lorsque vous **désactivez** l’option, le rapport imprime toutes les écritures liées à une période spécifiée. Lorsque vous l’**activez**, le rapport exclut les écritures échelonnement.  

> [!NOTE]
> La période suivante, d’un mois, n’inclut pas les écritures échelonnement lorsque vous les avez **activées**.

## Voir aussi

[Fonctionnalités locales pour la Belgique](belgium-local-functionality.md)
[Rendre les modèles feuille obligatoires](specify-journal-template-mandatory.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
