---
title: Enregistrer les frais ou des revenus directement dans la comptabilité
description: Vous pouvez créer des transactions sur la page Journal général pour les activités commerciales qui n’impliquent pas de document.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'direct posting, general ledger'
ms.search.form: '39, 251'
ms.date: 06/13/2024
ms.service: dynamics-365-business-central
---
# Validation directe des transactions en comptabilité.

Les feuilles comptabilité vous permettent de valider des transactions financières directement dans les comptes généraux et dans d’autres comptes tels que les comptes bancaires, client, fournisseur et salarié.  

Une utilisation classique de la feuille comptabilité est de valider les dépenses des salariés au cours des activités commerciales, pour un remboursement. Pour plus d’informations, voir [Enregistrer et rembourser les frais des employés](finance-how-record-reimburse-employee-expenses.md).

Les feuilles comptabilité valident les transactions financières dans les comptes généraux et d’autres comptes tels que les comptes bancaires, clients, fournisseurs et employés. La validation avec une feuille comptabilité crée des écritures dans les comptes généraux. Les entrées sont créées, par exemple, vous validez une ligne feuille dans un compte client, parce qu’une écriture est validée dans un compte client de la comptabilité via un groupe comptabilisation. Vous pouvez personnaliser votre version d’une feuille comptabilité en configurant un nom de feuille ou un modèle feuille. Pour en savoir plus, voir [Utiliser des feuilles comptabilité](ui-work-general-journals.md).

Les entrées que vous validez avec des documents nécessitent un processus de note de crédit. Cependant, vous pouvez contre-passer les écritures que vous validez dans le journal général. Pour plus d’informations, voir [Inversion d’une validation feuille et annuler les réceptions/envois](finance-how-reverse-journal-posting.md).

## Pour valider une transaction directement vers la comptabilité

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Feuilles comptabilité**, puis choisissez le lien associé.
2. Ouvrez la feuille générale. Pour en savoir plus, voir [Utiliser des feuilles comptabilité](ui-work-general-journals.md).
3. Sur une nouvelle ligne feuille, renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. Répétez l’étape 3 pour toutes les transactions que vous souhaitez valider.

    > [!TIP]  
    > Si vous souhaitez saisir les lignes de transaction avant une ligne compte contrepartie, par exemple, pour un compte bancaire, activez la case à cocher **Suggérer le montant contrepartie** de la ligne pour votre lot sur la page **Noms feuilles comptabilité**. Le champ **Montant** de la ligne compte contrepartie est automatiquement prérempli avec la valeur requise pour équilibrer les transactions.
5. Choisissez l’action **Valider** pour enregistrer les transactions sur les comptes généraux spécifiés.

## Voir aussi

[Utilisation des feuilles comptabilité](ui-work-general-journals.md)  
[Enregistrement et remboursement des frais des employés](finance-how-record-reimburse-employee-expenses.md)  
[Inverser des validations feuille et annuler les réceptions/envois](finance-how-reverse-journal-posting.md)  
[Finances](finance.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]