---
title: Clôturer des périodes comptables pour un exercice comptable
description: Cet article décrit comment clôturer les périodes comptables de l’exercice comptable pour la clôture de l’exercice.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'year closing, close accounting period, close fiscal year, bank account detailed trial balance'
ms.search.form: '100,'
ms.date: 05/07/2024
ms.service: dynamics-365-business-central
---
# <a name="close-accounting-periods"></a>Clôture des périodes comptables

Lorsqu'un exercice comptable est terminé, vous devez clôturer les périodes qui le composent.

## <a name="to-close-accounting-periods"></a>Pour clôturer des périodes comptables

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Périodes comptables**, puis sélectionnez le lien associé.
2. Sur la page **Périodes comptables**, sélectionnez l'action **Clôturer exercice**.

    Si plusieurs exercices comptables sont ouverts, le plus ancien est automatiquement sélectionné pour être clôturé. Un message identifie l’exercice à clôturer et les résultats de sa clôture.
3. Pour clôturer l'exercice, cliquez sur **Oui**.

L'exercice comptable est désormais clôturé, et les champs **Fermé** et **Verrouillage date** sont sélectionnés pour toutes les périodes de l'exercice. Vous ne pouvez pas rouvrir l'exercice comptable ni supprimer la coche des champs **Fermé** et **Verrouillage date**.

> [!NOTE]  
> Vous ne pouvez pas clôturer un exercice comptable avant d’en créer un nouveau. Sachez que lorsqu’un exercice comptable est clôturé, vous ne pouvez pas modifier la date début de l’exercice comptable suivant.

Même si un exercice comptable est clôturé, vous pouvez toujours y valider des écritures. Dans ce cas, les écritures sont marquées comme validées dans un exercice comptable clôturé et le champ **Ecr. exercice précédent** est activé.

Une fois qu'un exercice comptable a été clôturé, vous devez clôturer les comptes de gestion et transférer les résultats de l'exercice sur un compte du bilan. Vous pouvez répéter cette opération chaque fois que vous validez dans l'exercice comptable clôturé.

## <a name="see-also"></a>Voir aussi

[Clôture plans](year-close-books.md)  
[Validation de l’écriture de clôture d’exercice](year-how-post-year-end-close-entry.md)  
[Utilisation des périodes et exercices comptables](finance-accounting-periods-and-fiscal-years.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
