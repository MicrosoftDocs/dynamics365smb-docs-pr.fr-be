---
title: Comment enregistrer les entrées de durabilité
description: Apprenez à enregistrer les émissions de GES (gaz à effet de serre).
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, journal'
ms.search.form: '6216, 6219, 6220'
ms.date: 04/02/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
---

# Comment enregistrer les entrées de durabilité  

À l’heure actuelle, la seule façon d’enregistrer les émissions de GES dans le **Compta. de durabilité** est d’utiliser les **Journaux de durabilité**.   

## Feuille durabilité  

**Les journaux de durabilité** sont conçus pour suivre et enregistrer les activités liées au développement durable en utilisant la même expérience utilisateur que les autres journaux de Business Central. Dans le journal, les utilisateurs ont la possibilité de saisir manuellement les émissions s’ils possèdent les informations nécessaires. Alternativement, s’ils ne disposent pas de ces données, ils peuvent utiliser des formules intégrées pour calculer avec précision les émissions sur la base de paramètres connus spécifiques correspondant à différents types de sources et de comptes. 

Les informations que vous saisissez dans une feuille sont temporaires et peuvent être modifiées tant qu’elles sont dans la feuille. Lorsque vous validez la feuille, les informations sont transférées vers des **écritures de comptes de durabilité** ou **Comptes de durabilité** individuels, où elles ne peuvent pas être modifiées. Vous pouvez toutefois comptabiliser des écritures d’extourne ou de correction.  

### Utiliser des modèles feuille et des feuilles 

Il existe deux **modèles de journaux de durabilité** par défaut : le modèle standard et le modèle récurrent. Pour chaque modèle feuille, vous pouvez configurer votre propre feuille personnelle sous forme de nom de feuille. Pour ce faire, vous devez choisir l’action **Lots** sur la page **Modèles de journaux de développement durable** et créer le nouveau **Feuille durabilité** sur la nouvelle page. Par exemple, vous pouvez définir votre propre lot de journaux pour chaque périmètre d’émission, à l’aide de l’option **Portée d’émission** qui vous permet de choisir entre trois périmètres existants. Vous pouvez également ajouter ou modifier le **Code source** et **Code motif** pour chacun des lots. 

>[!TIP]
>Vous pouvez avoir un lot de journal pour chacun des types d’émissions, si vous avez plusieurs lignes, car cela peut réduire le risque d’erreurs, mais vous pouvez également utiliser le lot commun pour tous les types d’émissions.   

### Validation de feuilles durabilité 

Vous pouvez activer une vérification des antécédents sur **Configuration durabilité** qui aidera à éviter les retards lors de la validation. Le contrôle vous informe lorsqu’une erreur en utilisant **la feuille durabilité** et vous empêche de valider le journal.  

Lorsque vous activez la validation, le Récapitulatif **Vérification de feuille** affiche les problèmes de la ligne actuelle et du lot entier. La validation se produit lorsque vous chargez une Feuille et lorsque vous choisissez une autre ligne feuille. La vignette **Nombre total d’erreurs** du Récapitulatif montre le nombre total de problèmes que [!INCLUDE [prod_short](includes/prod_short.md)] a trouvées, et vous pouvez le choisir pour ouvrir un aperçu des problèmes. 

### Utiliser des feuilles durabilité 

Pour commencer à travailler avec les **feuilles durabilité**, suivez les étapes :   

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche 3.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Feuille durabilité**, puis sélectionnez le lien associé. 
2. Sur la page **Feuille durabilité** , vous pouvez saisir autant de lignes que vous prévoyez de publier avec le même lot.  
3. En tant que **Type de document**, vous pouvez conserver une option vide ou choisir d’utiliser **Facture** ou **Avoir**.  
4. Dans le champ **N° de compte** , vous pouvez choisir uniquement **Comptes de durabilité** avec **sélectionné Champ de publication directe** , **Publication** en tant que **Type de comptabilité** et compte non bloqué. En outre, les comptes doivent être configurés avec une catégorie et une sous-catégorie.  

>[!NOTE]
>Si vous utilisez le lot dans lequel le périmètre d’émission est configuré, le **portée d’émission** dans le **compte de durabilité** doit être égal au **Scope émission** dans le lot utilisé.  

5. Vous avez deux options : soit valider manuellement les montants, soit utiliser des formules.   

    1. Si vous disposez d’informations précises sur l’émission et que vous souhaitez les publier (c’est-à-dire que vous les avez sur la facture reçue), vous devez sélectionner le champ **Saisie manuelle** pour spécifier que les montants seront saisis manuellement. Dans ce cas, vous ne pouvez pas renseigner vos données dans les champs **Carburant/Électricité**, **Distance**, **Montant personnalisé**, **Multiplicateur d’installation** et **Facteur de temps** , car ils ne seront pas modifiables pour ce choix. Mais les **émissions de CO2**, **émissions de CH4** et **émissions de N2O** les champs seront modifiables et vous pourrez y remplir vos données directement. 
    2. Si vous ne connaissez pas votre émission avec précision, vous devez la calculer, et vous ne devez pas avoir sélectionné le champ **Saisie manuelle** , et dans ce cas le **Émission CO2**, **Émission CH4** et **Émission N2O** champs ne sera pas modifiable, mais vous pouvez saisir les détails de votre calcul en fonction de la formule que vous utilisez. Vous pouvez en savoir plus sur les formules utilisées et définies dans la **Catégorie de comptes de durabilité** ici dans le [Graphique des comptes de durabilité et de comptabilité](finance-sustainability-accounts-ledger.md#account-categories).
    
7. Pour valider la feuille, sélectionnez l’action **Valider**. Lors de la publication dans un **feuille Graphique des comptes de durabilité et de comptabilité**, les entrées sont générées dans le **Compta. durabilité**. 

Dans le cas où votre formule est basée sur le **Calculer à partir de Comptabilité** possibilité dans le **Catégorie de compte de durabilité**, vous devez utiliser le **Recueillir le montant des écritures comptables** action avant de publier le journal pour calculer les émissions en fonction de cette source de données. De plus, si vous avez apporté des modifications aux facteurs d’émission après avoir renseigné les lignes de journal, vous devez choisir le **Recalculer** action pour obtenir le montant approprié dans le journal.  

### Feuilles abonnement 

Une feuille abonnement est une **feuille durabilité** contenant des champs spécifiques pour la gestion des transactions que vous validez fréquemment avec peu ou pas de modifications. Par exemple, les transactions durables telles que l’électricité, le chauffage ou d’autres transactions similaires. L’utilisation de journaux récurrents vous permet de comptabiliser des montants fixes et variables. Avec une feuille abonnement, vous ne créez les écritures qui sont régulièrement validées qu’une fois. Par exemple, les comptes, axes, sections analytiques, etc. que vous saisissez restent dans la feuille après validation. Si des modifications sont nécessaires, vous pouvez les apporter à chaque validation. 

Le champ **Mode abonnement** est important. Il détermine la manière dont le montant de la ligne feuille est traité après validation. Par exemple, si vous utilisez le même montant à chaque fois que vous validez la ligne, vous pouvez laisser le montant rester, et dans ce cas, vous devez utiliser le **F Fixe** Comme une option. Si vous utilisez les mêmes comptes et le même texte pour la ligne, mais que le montant varie chaque fois que vous validez, vous pouvez choisir de supprimer le montant après validation, dans ce cas, l'option **Variable V**. 

Vous devez également configurer le **Fréquence Abonnement** car ce champ de formule de date détermine la fréquence de validation de l’écriture sur la ligne journal et il doit être rempli. En savoir plus sur [Utiliser des formules de date](ui-enter-date-ranges.md#use-date-formulas).  

Ce champ **Date expiration** détermine la date à laquelle la ligne est validée pour la dernière fois. La ligne n’est plus validée après cette date. L’avantage d’utiliser le champ **Date d’expiration** est que la ligne n’est pas supprimée immédiatement de la feuille. Vous pouvez entrer une date ultérieure afin de pouvoir utiliser la ligne à l’avenir. Si le champ est blanc, la ligne est validée à chaque validation, jusqu’à ce qu’elle soit supprimée de la feuille.  

## Voir aussi  
[Finance](finance.md)    
[Vue d’ensemble de la gestion de la durabilité](finance-manage-sustainability.md)   
[Configuration de durabilité](finance-sustainability-setup.md)   
[Graphique des comptes de durabilité et de comptabilité](finance-sustainability-accounts-ledger.md)   
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)   

[!INCLUDE[footer-include](includes/footer-banner.md)]
