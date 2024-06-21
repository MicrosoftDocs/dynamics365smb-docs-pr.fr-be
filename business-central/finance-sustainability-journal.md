---
title: Enregistrer les entrées de durabilité
description: Apprenez à enregistrer les émissions de GES (gaz à effet de serre).
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, journal'
ms.search.form: '6216, 6219, 6220'
ms.date: 05/07/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="record-sustainability-entries"></a>Enregistrer les entrées de durabilité

À l’heure actuelle, la seule façon d’enregistrer les émissions de GES dans la compta. de durabilité est d’utiliser les feuille durabilité.

## <a name="sustainability-journals"></a>Feuilles durabilité

Les feuilles durabilité sont conçus pour suivre et enregistrer les activités liées au développement durable en utilisant la même expérience utilisateur que les autres journaux de Business Central. Les utilisateurs disposant des informations nécessaires peuvent saisir manuellement les émissions dans une feuille. Alternativement, s’ils ne disposent pas de ces informations, ils peuvent utiliser des formules intégrées pour calculer avec précision les émissions sur la base de paramètres connus spécifiques correspondant à différents types de sources et de comptes.

Les informations que vous saisissez dans une feuille sont temporaires et peuvent être modifiées tant qu’elles sont dans la feuille. Lorsque vous validez la feuille, les informations sont transférées vers des écritures de comptes de durabilité ou comptes de durabilité individuels, où elles ne peuvent pas être modifiées. Vous pouvez toutefois comptabiliser des écritures d’extourne ou de correction.

### <a name="use-journal-templates-and-batches"></a>Utiliser des modèles feuille et des feuilles

Par défaut, il existe deux modèles de feuilles durabilité par défaut : le modèle standard et le modèle récurrent.

Pour chaque modèle feuille, vous pouvez configurer votre propre feuille personnelle sous forme de nom de feuille. Pour ce faire, sélectionnez l’action **Lots** sur la page **Modèles de feuilles durabilité** et créez la **Feuille durabilité** sur la nouvelle page. Par exemple, vous pouvez définir votre propre lot de journaux pour chaque périmètre d’émission, à l’aide de l’option **Portée d’émission** qui vous permet de sélectionner entre trois champs existants. Pour chaque lot, vous pouvez également ajouter ou modifier les valeurs **Code source** et **Code motif**.

> [!TIP]
> Si vous disposez de plusieurs lignes, vous pouvez contribuer à réduire le risque d’erreurs en créant une feuille pour chaque type d’émission. Vous pouvez également utiliser le lot commun pour tous les types d’émissions.

### <a name="validate-sustainability-journals"></a>Valider les feuilles durabilité

Sur la page **Configuration durabilité**, vous pouvez activer une vérification des antécédents pour aider à éviter les retards lors de la validation. Si une erreur survient lorsque vous travaillez dans la feuille durabilité, la validation vous informe et vous empêche de valider la feuille.

Lorsque vous activez la validation, le Récapitulatif **Vérification de feuille** affiche les problèmes de la ligne actuelle et du lot entier. La validation se produit lorsque vous chargez une Feuille et lorsque vous choisissez une autre ligne feuille. La vignette **Problèmes totaux** du récapitulatif indique le nombre total de problèmes [!INCLUDE [prod_short](includes/prod_short.md)] trouvés. Vous pouvez sélectionner la vignette pour ouvrir une vue d’ensemble des problèmes.

### <a name="work-with-sustainability-journals"></a>Utiliser des feuilles durabilité

Pour commencer à travailler avec les feuilles durabilité, suivez ces étapes :

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche 3.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Feuille durabilité**, puis sélectionnez le lien associé.
2. Sur la page **Feuille durabilité** , saisissez autant de lignes que vous prévoyez de publier avec le même lot.
3. Vous pouvez laisser le champ **Type de document** vide ou sélectionner **Facture** ou **Avoir**.
4. Dans le champ **N° de compte**, vous pouvez sélectionner uniquement les comptes de durabilité non bloqués où le champ **Publication directe** est sélectionné et le champ **Type de comptabilité** est défini sur **Validation**. Les comptes doivent être également configurés avec une catégorie et une sous-catégorie.

    > [!NOTE]
    > Si vous utilisez le lot dans lequel le périmètre d’émission est configuré, la valeur **Champ d’émission** dans le compte de durabilité doit être égal à la valeur **Champ de l’émission** dans le lot.

5. Vous avez deux options : soit valider manuellement les montants, soit utiliser des formules.

    - Si vous disposez d’informations précises sur l’émission et que vous souhaitez les publier (c’est-à-dire que vous les avez sur la facture reçue), vous devez sélectionner le champ **Saisie manuelle** pour spécifier que les montants seront saisis manuellement. Dans ce cas, vous ne pouvez pas renseigner vos données dans les champs **Carburant/Électricité**, **Distance**, **Montant personnalisé**, **Multiplicateur d’installation** et **Facteur de temps** , car ils ne seront pas modifiables pour ce choix. Mais les champs **émissions de CO2**, **émissions de CH4** et **émissions de N2O** seront modifiables et vous pourrez y remplir vos données directement.
    - Si vous n’avez pas une connaissance précise de l’émission et devez la calculer, ne sélectionnez pas le champ **Saisie manuelle**. Dans ce cas, les champs **émissions de CO2**, **émissions de CH4** et **émissions de N2O** ne sont plus modifiables. Cependant, vous pouvez saisir les détails de votre calcul en fonction de la formule que vous utilisez. Vous pouvez en savoir plus sur les formules utilisées et définies dans la **Catégorie de comptes de durabilité** ici dans le [Graphique des comptes de durabilité et de comptabilité](finance-sustainability-accounts-ledger.md#account-categories).

6. Pour valider la feuille, sélectionnez l’action **Valider**. Lors de la publication dans une feuille de durabilité, les entrées sont générées dans la compta. durabilité.

Si votre formule est basée sur l’option **Calculer à partir de Comptabilité** dans la catégorie de compte de durabilité, vous devez utiliser l’action **Recueillir le montant des écritures comptables** avant de publier la feuille pour calculer les émissions en fonction de cette source de données. De plus, si vous avez apporté des modifications aux facteurs d’émission après avoir renseigné les lignes feuille, vous devez choisir l’action **Recalculer** pour obtenir le montant approprié dans la feuille.

### <a name="recurring-journals"></a>Feuilles abonnement

Une feuille abonnement est une feuille durabilité contenant des champs spécifiques pour la gestion des transactions que vous validez fréquemment avec peu ou pas de modifications. Par exemple, les transactions durables telles que l’électricité, le chauffage ou d’autres transactions similaires. Vous pouvez utiliser les feuilles abonnement pour comptabiliser des montants fixes et variables.

Avec une feuille abonnement, vous ne créez les écritures qui sont régulièrement validées qu’une fois. Des informations telles que les comptes, axes et sections analytiques, que vous saisissez restent dans la feuille après validation. Chaque fois que vous validez, vous pouvez apporter toutes les modifications requises.

Le champ **Mode abonnement** est important. Il détermine la manière dont le montant de la ligne feuille est traité après validation. Par exemple, si vous utilisez le même montant à chaque fois que vous validez la ligne, vous pouvez sélectionner l’option **F Fixe** pour laisser le montant rester au-delà de la validation. Si vous utilisez les mêmes comptes et le même texte pour la ligne, mais que le montant varie chaque fois que vous validez, vous pouvez choisir de supprimer le montant après validation, dans ce cas, l’option **Variable V**.

Le champ **Fréquence Abonnement** est également important et doit être renseigné. Ce champ de formule de date détermine la fréquence de validation de l’écriture sur la ligne feuille. En savoir plus dans [Utiliser des formules de date](ui-enter-date-ranges.md#use-date-formulas).

Ce champ **Date expiration** détermine la date à laquelle la ligne est validée pour la dernière fois. La ligne n’est plus validée après cette date. L’avantage d’utiliser le champ **Date d’expiration** est que la ligne n’est pas supprimée immédiatement de la feuille. Vous pouvez entrer une date ultérieure afin de pouvoir utiliser la ligne à l’avenir. Si le champ est blanc, la ligne est validée à chaque validation, jusqu’à ce qu’elle soit supprimée de la feuille.

## <a name="see-also"></a>Voir aussi

[Finances](finance.md)  
[Vue d’ensemble de la gestion de la durabilité](finance-manage-sustainability.md)  
[Configuration de durabilité](finance-sustainability-setup.md)  
[Graphique des comptes de durabilité et de comptabilité](finance-sustainability-accounts-ledger.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
