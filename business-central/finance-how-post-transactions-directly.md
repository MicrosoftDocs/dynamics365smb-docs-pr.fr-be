---
title: Enregistrer les frais ou des revenus directement dans la comptabilité| Microsoft Docs
description: Pour les activités économiques qui ne sont pas représentés par un document, comme de plus petits frais ou règlements, vous pouvez créer les transactions associées en validant des lignes de feuille sur la page Feuille comptabilité.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct posting, general ledger
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: e0beff15352fb8e57f57c9d0ffdcd76bc28afbb9
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5782393"
---
# <a name="post-transactions-directly-to-the-general-ledger"></a>Valider les transactions directement vers la comptabilité

Les feuilles comptabilité vous permettent de valider des transactions financières directement dans les comptes généraux et dans d’autres comptes tels que les comptes bancaires, client, fournisseur et salarié.  

Une utilisation classique de la feuille comptabilité est de valider les dépenses des salariés avec leurs fonds propres au cours des activités commerciales, pour un remboursement ultérieur. Pour plus d’informations, voir [Enregistrer et rembourser les frais des employés](finance-how-record-reimburse-employee-expenses.md).

Les feuilles comptabilité valident les transactions financières dans les comptes généraux et d’autres comptes tels que les comptes bancaires, clients, fournisseurs et employés. La validation avec une feuille comptabilité crée toujours des écritures dans les comptes généraux. C’est le cas même lorsque, par exemple, vous validez une ligne feuille dans un compte client, parce qu’une écriture est validée dans un compte client de la comptabilité via un groupe comptabilisation. Vous pouvez personnaliser votre version d’une feuille comptabilité en configurant un nom de feuille ou un modèle feuille. Pour plus d’informations, voir [Utilisation des feuilles comptabilité](ui-work-general-journals.md).

Contrairement aux écritures qui sont validées avec des documents qui nécessitent un processus d’avoir, vous pouvez correctement contrepasser les écritures validées avec la feuille comptabilité. Pour plus d’informations, voir [Inversion d’une validation feuille et annuler les réceptions/envois](finance-how-reverse-journal-posting.md).

## <a name="to-post-a-transaction-directly-to-a-general-ledger-account"></a>Pour valider une transaction directement vers la comptabilité

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles comptabilité**, puis sélectionnez le lien associé.
2. Ouvrez la feuille comptabilité appropriée. Pour plus d’informations, voir [Utilisation des feuilles comptabilité](ui-work-general-journals.md).
3. Sur une nouvelle ligne feuille, renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. Répétez l’étape 3 pour toutes les transactions distinctes que vous souhaitez valider.

    > [!TIP]  
    > Si vous souhaitez saisir les lignes de transaction au-dessus d’une ligne compte contrepartie, par exemple, pour un compte bancaire, activez la case à cocher **Suggérer le montant contrepartie** de la ligne pour votre lot sur la page **Noms feuilles comptabilité**. Puis le champ **Montant** de la ligne compte contrepartie est automatiquement prérempli avec la valeur requise pour équilibrer les transactions.
5. Choisissez l’action **Valider** pour enregistrer les transactions sur les comptes généraux spécifiés.

## <a name="see-also"></a>Voir aussi

[Utilisation de feuilles comptabilité](ui-work-general-journals.md)  
[Enregistrer et rembourser les frais des employés](finance-how-record-reimburse-employee-expenses.md)  
[Inversion d’une validation feuille et annuler les réceptions/envois](finance-how-reverse-journal-posting.md)  
[Finances](finance.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]