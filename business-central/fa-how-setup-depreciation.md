---
title: Paramétrer des lois d’amortissement
description: Vous spécifiez dans une loi d’amortissement comment vous souhaitez amortir ou déprécier les immobilisations.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: write down
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: eb7e0d0d082d8a86ce61b6dffab46ce6248a29d9
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5782292"
---
# <a name="set-up-fixed-asset-depreciation"></a>Configurer un amortissement immobilisation

Vous pouvez utiliser plusieurs méthodes d’amortissement pour préparer les états financiers et les déclarations de revenus. De nombreuses sociétés de grande taille utilisent la méthode de l’amortissement linéaire dans leurs états financiers car elle permet généralement la déclaration des bénéfices supérieurs. Aux fins de l’impôt sur le revenu, cependant, de nombreuses entreprises utilisent une méthode d’amortissement accélérée, comme l’amortissement dégressif. Vous définissez la méthode d’amortissement d’un actif avec le champ **Méthode d’amortissement** sur la page **Fiche immobilisation**. Pour plus d’informations sur les fonctions des différentes méthodes, consultez [Méthodes d’amortissement](fa-depreciation-methods.md).

Vous paramétrez des lois d’amortissement lorsque vous définissez les différentes manières dont l’amortissement doit être calculé pour vos différents types d’immobilisation. Chaque loi d’amortissement spécifie des conditions d’amortissement individuelles. Par exemple, vous pouvez spécifier qu’une immobilisation doit être amortie sur une période de trois ans dans une loi et sur une période de cinq ans dans une autre loi.

Lorsque vous avez créé les lois d’amortissement nécessaires, vous devez en attribuer au moins une à chaque immobilisation. La loi d’amortissement attribuée à une immobilisation est désignée comme loi d’amortissement immobilisation. Vous pouvez créer un nombre illimité de lois d’amortissement pour une immobilisation.  

## <a name="to-create-a-depreciation-book"></a>Pour créer une loi d’amortissement

Dans une loi d’amortissement immobilisation, vous spécifiez comment les immobilisations sont amorties. Pour prendre en charge plusieurs méthodes d’amortissement, vous pouvez paramétrer plusieurs lois d’amortissement.  

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Lois d’amortissement**, puis choisissez le lien associé.
2. Sur la page **Liste des lois d’amortissement**, sélectionnez l’action **Nouveau**.
3. Sur la page **Fiche loi d’amortissement**, renseignez les champs comme nécessaire. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > Vous pouvez enregistrer les transactions immobilisation sur la page **Feuille compta. immo.** ou sur la page **Feuille immo.**, selon que les transactions sont destinées pour des rapports financiers ou pour la gestion interne. Procédez comme suit pour définir quel type de feuille est utilisé pour les différentes activités immobilisation par défaut.
4. Sur le raccourci **Intégration**, cochez la case pour chaque activité immobilisation dont vous souhaitez valider les transactions via la page **Feuille compta. immo.**.
5. Répétez les étapes 2 à 4 pour chaque méthode d’amortissement ou méthode de validation que vous souhaitez attribuer à des immobilisations en tant que loi d’amortissement.

> [!IMPORTANT]
> Choisissez le champ **Utiliser arrondi dans amort.** pour arrondir les montants d’amortissement périodique calculés à des nombres entiers. Par exemple, si votre entreprise utilise également l’arrondi facture à des nombres entiers dans la page **Paramètres comptabilité**, arrondir également les montants d’amortissement à des nombres entiers peut aider à assurer la transparence.

Par exemple, si vous disposez d’une immobilisation dont les lois d’amortissement ne spécifient pas d’arrondi, mais que les paramètres comptabilité de votre entreprise nécessitent un arrondi, alors, lorsque vous cédez l’immobilisation, vous verrez un message d’erreur indiquant qu’un montant doit être arrondi sur une écriture comptable.  

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a>Pour attribuer une loi d’amortissement à une immobilisation
1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Immobilisations**, puis sélectionnez le lien associé.
2. Sélectionnez l’immobilisation pour laquelle vous souhaitez configurer une loi d’amortissement.
3. Sur le raccourci **Loi d’amortissement**, renseignez les champs, le cas échéant.
4. Si vous devez assigner plus d’une loi d’amortissement à l’immobilisation, sélectionnez l’action **Ajouter davantage de lois d’amortissement**.
5. Sinon, sélectionnez l’action **Lois d’amortissement** pour spécifier une, voire plusieurs lois d’amortissement immobilisation.

    > [!NOTE]  
    >   Lorsque vous utilisez la méthode manuelle d’amortissement, vous devez saisir l’amortissement manuellement dans la feuille comptabilisation immobilisation. La fonction **Calculer amortissement** ignore les immobilisations qui utilisent la méthode d’amortissement manuelle. Vous pouvez recourir à cette méthode pour les immobilisations qui ne font pas l’objet d’un amortissement, par exemple les terrains.

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a>Pour attribuer une loi d’amortissement à plusieurs immobilisations avec un traitement par lots
Si vous voulez associer une loi d’amortissement à plusieurs immobilisations, vous pouvez utiliser le traitement par lots **Créer plans amortissement** pour créer des lois d’amortissement d’immobilisation.  

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Immobilisations**, puis sélectionnez le lien associé.
2. Sélectionnez l’immobilisation à laquelle vous souhaitez attribuer une loi d’amortissement, puis sélectionnez l’action **Modifier**.
3. Sur la page **Fiche livre d’amortissement**, sélectionnez l’action **Créer plans amortissement**.
4. Sur la page **Créer plans amortissement immo.**, renseignez le champ **Loi d’amortissement**.
5. Choisissez le champ **Copier immo. n°**, puis sélectionnez le numéro de l’immobilisation à utiliser comme base pour créer de nouvelles lois d’amortissement d’immobilisation.

    Si vous renseignez ce champ, les champs d’amortissement des nouvelles lois d’amortissement d’immobilisation contiennent les mêmes informations que ceux de la loi d’amortissement d’immobilisation que vous copiez. N’entrez rien dans ce champ si vous souhaitez créer de nouvelles lois d’amortissement d’immobilisation avec des champs d’amortissement vides.  
6. Sur le raccourci **Immo.**, vous pouvez positionner un filtre afin de sélectionner les immobilisations pour lesquelles vous souhaitez créer des lois d’amortissement immobilisation.
7. Cliquez sur le bouton **OK**.

## <a name="to-set-up-depreciation-posting-types"></a>Pour configurer les types de validation amortissement
Pour chaque loi d’amortissement, vous devez définir la manière dont vous souhaitez que [!INCLUDE[prod_short](includes/prod_short.md)] gère les différents types de validation. Par exemple, vous devez indiquer s’il s’agit d’un débit ou d’un crédit et si le type de validation doit être inclus dans la base d’amortissement.  

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Lois d’amortissement**, puis choisissez le lien associé.  
2. Sélectionnez la loi d’amortissement que vous souhaitez configurer, puis sélectionnez l’action **Type paramètre compta. immo.**.
3. Sur la page **Type paramètre compta. immo.**, renseignez les champs, le cas échéant.

    > [!NOTE]  
    >   Vous ne pouvez pas insérer ni supprimer de lignes sur la page **Type paramètre compta. immo**. Vous ne pouvez modifier que les lignes existantes.

Il est recommandé de ne pas modifier les paramètres des lois d’amortissement pour lesquelles des écritures ont déjà été validées. Les modifications apportées n’ont pas d’incidence sur les écritures déjà validées, ce qui rendrait les statistiques des lois d’amortissement inexactes.

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a>Pour configurer les modèles par défaut et les lots pour l’amortissement immobilisation
Pour chaque loi d’amortissement, vous définissez une configuration par défaut de modèles et de feuilles. Vous devez utiliser ces valeurs par défaut pour dupliquer les lignes d’une feuille vers une autre, créer des lignes feuille à l’aide du traitement par lots **Calculer amortissement** ou **Actualiser immobilisations**, dupliquer des coûts d’acquisition dans la feuille assurance.  

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Lois d’amortissement**, puis choisissez le lien associé.  
2. Sélectionnez la loi d’amortissement pour laquelle vous souhaitez définir les feuilles par défaut, puis sélectionnez l’action **Configuration feuille immo.**.  
3. Pour avoir une configuration par défaut pour chaque utilisateur, choisissez le champ **Code utilisateur** à sélectionner à partir de la page **Utilisateurs**.  
4. Dans les autres champs, sélectionnez le modèle feuille ou la feuille qui doit être utilisé(e) par défaut.  

## <a name="see-also"></a>Voir aussi
[Paramétrage d’immobilisations](fa-setup.md)  
[COMPTES D’IMMOBILISATIONS](fa-manage.md)  
[Finances](finance.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]