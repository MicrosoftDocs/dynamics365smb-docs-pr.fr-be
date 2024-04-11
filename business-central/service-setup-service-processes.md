---
title: Configurer les processus de gestion des services
description: Apprenez comment configurer les processus qui permettent de vérifier que les clients sont satisfaits de votre services.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: how-to
ms.search.keywords: 'service, number sequences, setup, warnings, fee, contracts, warranties'
ms.date: 02/27/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Configurer des processus de gestion des services

Voici quelques exemples des paramètres que vous pouvez appliquer aux processus de gestion des services :  
  
* Certains paramètres généraux pour différents processus, comme les avertissements, les calculs de service suivants pour les articles de service, les frais de démarrage à évaluer, le niveau de reporting panne à utiliser, etc.  
* Les types au cas où les techniciens doit saisir des informations sur les documents service. Par exemple, vous pouvez lui demander de spécifier le type de commande, les dates de début et/ou de fin du travail et le type de travail effectué.  
* Certains paramètres par défaut pour les temps de réponse et les garanties. Ceux-ci incluent un délai de réponse par défaut pour commencer le service, les taux de remise garantie pour les pièces et le travail, et le délai de validité des garanties.  
* Les paramètres pour les contrats, tels que le nombre maximum de jours que vous pouvez utiliser pour les commandes contrat de service, si vous utilisez des codes motif lorsqu’un contrat est annulé, des textes standard pour les descriptions et les valeurs contractuelles.  
* Les souches de numéros à utiliser pour les documents et les articles relatifs au service.  

## Pour saisir les paramètres généraux et obligatoires

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Paramètres Gestion des services**, puis choisissez le lien associé.
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## Configurer les politiques de publication des factures de service pour les utilisateurs

Les entreprises ont souvent des processus uniques pour les factures et les expéditions. Par exemple, les processus peuvent varier d’une personne validant tout sur un ordre service à plusieurs employés, chacun dans leurs propres pages.

Vous pouvez utiliser des stratégies de validation pour empêcher les utilisateurs de valider des factures de service ou leur demander de valider les factures avec l’expédition de service associée. Pour paramétrer une politique validation, Sur la page **Configuration de l’utilisateur**, dans les champs **Stratégie validation facture service**, choisissez l’une des options suivantes :

* **Autorisé** (Par défaut) : conservez le comportement actuel, où un utilisateur peut choisir l’option de validation, comme **Expédier**, **Facturer**, et **Expédier et facturer**.
* **Interdit** : empêchez les utilisateurs de valider des factures service. [!INCLUDE [prod_short](includes/prod_short.md)] affiche une boîte de dialogue de confirmation qui fournit uniquement le **Bateau** option.
* **Obligatoire** : Permettez aux gens de publier des factures avec les expéditions de services. [!INCLUDE [prod_short](includes/prod_short.md)] affiche une boîte de dialogue de confirmation qui fournit uniquement le **Bateau et facture** option.

Ce paramètre affecte les documents suivants :

* Commandes service
* Expéditions entrepôt
* Factures service
* Avoirs service

Le tableau suivant décrit les différentes effets sur différents documents.

|Document  |Autoriser<br>Affiche une série d’options   |Interdit<br>Boîte de dialogue de conformation  |Obligatoire<br>Boîte de dialogue de confirmation  |
|---------|---------|---------|---------|
|Commande service     | * Expédition<br>* Facturer<br>* Expédition et facturation<br>* Livrer et consommer         |* Expédition<br>* Livrer et consommer  |Souhaitez-vous valider l’expédition et la facture ?         |
|Expédition entrepôt     |* Expédition<br>* Expédition et facturation         |Souhaitez-vous valider l’expédition ?         | Souhaitez-vous valider l’expédition et la facture ?        |
|Facture service     | Souhaitez-vous valider la facture ?         | Erreur : vous ne pouvez pas publier.       |Souhaitez-vous valider la facture ?         |
|Avoir Service     | Souhaitez-vous valider l’avoir ?         | Erreur : vous ne pouvez pas publier.        |Souhaitez-vous valider l’avoir ?         |

> [!NOTE]
> Lorsque vous validez des factures service et des notes de crédit, vous ne disposez d’aucune option de validation. Les documents présentent toujours les transactions physiques et financières ensemble. Vous ne pouvez pas valider partiellement les factures et les avoirs service.

## Voir aussi  

[Configuration du signalement de défaillance](service-how-setup-fault-reporting.md)  
[Configuration de l’affectation des ressources](service-how-setup-resource-allocation.md)  
[Configurer des codes prestations standards](service-how-setup-service-coding.md)  
[Configurer des frais supplémentaires pour les services](service-how-setup-service-costs-pricing.md)  
[Configurer les processus incident](service-how-setup-troubleshooting.md)  
[Gestion des services](service-service.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
