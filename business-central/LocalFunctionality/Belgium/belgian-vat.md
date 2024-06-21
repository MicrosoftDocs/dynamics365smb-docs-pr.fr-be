---
title: TVA belge
description: Les améliorations belges de la fonction de déclaration de TVA vous permettent d'imprimer facilement des détails sur les transactions TVA.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.form: '11300, 11301,11303,11306,11307,11308'
ms.date: 03/02/2022
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="belgian-vat"></a>TVA belge

[!INCLUDE[prod_short](../../includes/prod_short.md)] comprend des extensions belges aux fonctionnalités de déclaration de TVA qui vous permettent d'imprimer les détails des transactions TVA. Vous devez envoyer les états suivants aux autorités fiscales belges :  

- Déclaration mensuelle/trimestrielle - Cet état permet de créer des déclarations de TVA mensuelles ou trimestrielles, en fonction des revenus de votre société.  

- Liste annuelle de TVA (sur papier/disque)

    Cet état permet de déclarer annuellement tous les montants facturés pour les biens et les services à toutes les sociétés belges avec un numéro de TVA enregistré.  

- Liste des ventes UE

    Cet état permet de déclarer les ventes de marchandises à d'autres pays/régions dans l'Union européenne. Pour en savoir plus, reportez-vous à la rubrique [À propos de l'état Liste des ventes UE](../../finance-how-report-vat.md#ecsaleslist).  

Vous êtes également tenu de fournir un relevé imprimé détaillant les transactions TVA aux autorités fiscales belges. Pour plus d'informations, voir Déclaration TVA.  

## <a name="non-deductible-vat"></a>TVA non déductible

En Belgique, la TVA peut être entièrement ou partiellement déductible. Des dépenses comme les frais de représentation ou les achats de voitures ne sont que partiellement déductibles et la transaction doit spécifier quel pourcentage de la TVA est non déductible. Par exemple, vous créez un compte général pour les immobilisations comme les voitures, et un autre compte pour les frais de représentation. Pour chaque compte, vous spécifiez quel pourcentage de la TVA déclarée est non déductible en définissant le champ **Pourcentage TVA non déductible**. Ensuite, lorsque vous validez une transaction, la TVA déductible sera validée sur le compte TVA correspondant, et la TVA non déductible sera ajoutée au montant de base et validée sur le même compte que les immobilisations corporelles et incorporelles.  

Pour les immobilisations, la TVA non déductible est amortie simplement comme le coût d'acquisition de base de l'immobilisation. Vous devez paramétrer des groupes comptabilisation immobilisation distincts pour chaque pourcentage de TVA non déductible, étant donné que chaque groupe comptabilisation immobilisation est validé sur un compte général où le champ **Pourcentage TVA non déductible** spécifie quel pourcentage de TVA doit être validé sur le même compte que l'immobilisation.  

Si vous sélectionnez le champ **TVA non déductible comprise** dans une ligne déclaration TVA, la TVA non déductible est incluse dans le montant TVA. L'état **Calculer et valider décl. TVA** ajoute la partie non déductible de ce montant aux champs **Montant TVA non déductible** et **Montant TVA devise origine non déductible** dans les écritures TVA résultantes.  

## <a name="see-also"></a>Voir aussi

[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)  
[Imprimer les déclarations de TVA périodiques](how-to-print-periodic-vat-reports.md)  
[Configurer la TVA non déductible](how-to-set-up-non-deductible-vat.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
