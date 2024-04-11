---
title: Configurer des informations générales pour les immobilisations
description: 'Avant d’utiliser des immobilisations, vous devez paramétrer des comptes généraux par défaut, des groupes de validation, des clés de ventilation, des feuilles et des modèles feuille, ainsi que les codes classe.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: how-to
ms.search.form: '5623, 5615, 5661, 5662, 5627, 5616, 5620, 5629, 5633, 5609, 5631, 5630, 5617, 5612, 5613, 5608, 5609, 5635, 9277'
ms.date: 03/25/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Configuration des informations générales sur les immobilisations

Avant de gérer des immobilisations, vous devez paramétrer des comptes généraux par défaut, des clés de ventilation, des feuilles et des modèles feuille pour valider et Reclasser Immobilisations. Définissez également une hiérarchie de classification (classes et sous-classes) pour structurer vos actifs et, si nécessaire, définissez les emplacements où vous stockez les actifs.

## Pour configurer un comportement général pour la fonctionnalité immobilisations

Définissez le comportement général de la fonctionnalité d'immobilisation et des souches de numéros document sur la page **Paramètres immobilisations**.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Paramètres immobilisations**, puis choisissez le lien associé.  
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## Pour configurer des groupes de validation immobilisation

Utiliser les groupes comptabilisation pour définir des groupes d'immobilisations. Les écritures de ces groupes comptabilisation validées dans les mêmes comptes généraux.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Groupes compta. immo.**, puis choisissez le lien associé.  
2. Sélectionnez l’action **Nouveau**.
3. Sur la page **Fiche groupe compta. immo.**, renseignez les champs, le cas échéant.

    > [!NOTE]  
    >   Pour veiller à ce que les comptes de contrepartie pour différentes validations d’immobilisation soient automatiquement insérés lorsque vous sélectionnez l’action **Insérer contrepartie immo.** sur les lignes feuille, procédez comme suit, selon la validation de réévaluation.
4. Sur le raccourci **Compte contrepartie**, dans le champ **Contrep. réévaluation**, sélectionnez le compte général dans lequel vous souhaitez valider les écritures contrepartie pour la réévaluation.

Pour en savoir plus sur l’utilisation de l’action **Insérer contrepartie immo.** sur les lignes feuille compta. immo., voir [Réévaluer les immobilisations](fa-how-revalue.md).

## Pour configurer les modèles feuille immobilisation

Un modèle est une présentation de feuille prédéfinie. Le modèle affiche des informations sur les codes suivi, les états et les souches de numéros. Pour en savoir plus, voir [Utiliser des feuilles comptabilité](ui-work-general-journals.md).

[!INCLUDE[prod_short](includes/prod_short.md)] crée automatiquement un modèle feuille immobilisation la première fois que vous ouvrez la page **Feuille immobilisation**. Vous pouvez cependant définir d’autres modèles feuille.  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Modèles feuille immo.**, puis sélectionnez le lien associé.  
2. Renseignez les champs selon vos besoins.

## Pour configurer la classe des immobilisations et les codes sous-classe

Dans les immobilisations, vous pouvez définir une hiérarchie de classification qui peut être utilisée pour regrouper les immobilisations. La hiérarchie comporte deux niveaux : les classes et les sous-classes.

### Codes classe immobilisation

Les classes d’immobilisations constituent les entrées de niveau supérieur dans la hiérarchie de classification dans laquelle vous regroupez les immobilisations. Par exemple, utilisez des classes pour diviser les actifs en actifs corporels ou incorporels. Vous devez créer au moins une classe d’immobilisations dans votre configuration.

1. Sélectionnez ![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Classes immo.**, puis choisissez le lien associé.
2. Saisissez les codes et les noms des classes immobilisation que vous souhaitez créer.

### Codes sous-classe immobilisation

Les sous-classes d’immobilisations constituent les entrées de niveau secondaire dans la hiérarchie de classification dans laquelle vous regroupez les immobilisations. Chaque sous-classe pointe vers une classe de niveau supérieur. Utilisez code sous-classe immobilisation permet de regrouper des immobilisations dans des catégories plus spécifiques, comme les bâtiments, les véhicules, le mobilier et les machines. Vous devez créer au moins une sous-classe d’immobilisations dans votre configuration.

1. Sélectionnez l’icône ![en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Sous-classes immo.**, puis choisissez le lien associé.
2. Saisissez les codes et les noms des sous-classes immobilisation que vous souhaitez créer.

## Commencer à enregistrer les actifs

Si vous utilisez les immobilisations dans [!INCLUDE[prod_short](includes/prod_short.md)] pour la première fois, vous devez d’abord paramétrer le module de comptabilité avant de définir des immobilisations. La manière de procéder est différente si vous intégrez les immobilisations en comptabilité.  

La procédure suivante est utilisée si les transactions immobilisation doivent être validées en comptabilité.  

1. Effectuez les configurations de base pour les immobilisations.  
2. Remplissez une fiche immobilisation pour chaque immobilisation existante.  
3. Créez une loi d’amortissement d’une immobilisation pour chaque type d’amortissement (par exemple les états financiers). Pour chaque loi d’amortissement, définir des conditions, par exemple l’intégration en comptabilité.

    Activez l’intégration comptable en procédant comme suit. Premièrement, assurez-vous que l’intégration du grand livre n'est pas activée pour toutes les lois d’amortissement, puis validez les écritures ouvertes, et enfin activez l’intégration en comptabilité.  
4. Sélectionnez l’![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Lois d’amortissement**, puis choisissez le lien associé.  
5. Sélectionnez la fiche de loi d’amortissement pertinente, puis sélectionnez l’action **Modifier** pour ouvrir la page **Fiche Lois d’amortissement**.
6. Sur l’onglet rapide **Intégration** , désactivez toutes les options. Si vous disposez de plusieurs lois d'amortissement, répétez cette étape pour chacun d'eux.  
7. Dans la feuille immobilisation, entrez les lignes suivantes pour chaque immobilisation :
   * Ligne avec le coût d’acquisition.
   * Une ligne avec l’amortissement cumulé jusqu’à la fin de l’exercice comptable précédent.
   * Une ligne avec l’amortissement cumulé du début de l’exercice comptable en cours jusqu’à la date à laquelle [!INCLUDE[prod_short](includes/prod_short.md)] est défini pour démarrer le calcul de l’amortissement.

    Si vous disposez d’autres soldes ouverts, vous pouvez également les saisir maintenant, (dépréciation, réévaluation, par exemple).  
8. Une fois que vous saisi et validé les lignes feuille pour chaque immobilisation, activez l’intégration en comptabilité dans les lois d’amortissement.

Si les immobilisations ne sont pas intégrées en comptabilité, ignorez les étapes 6 et 8.

## Pour configurer les codes emplacement immobilisation (facultatif)

Les codes emplacement immobilisation définissent l’emplacement de l’immobilisation, tel que le service commercial, l’accueil, l’administration, la production ou un entrepôt. Vous pouvez les utiliser pour enregistrer l’emplacement d’une immobilisation. Ces informations sont utiles pour les assurances et le suivi du stock.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Emplacements immo.**, puis choisissez le lien associé.
2. Saisissez les codes et les noms des emplacements immobilisation que vous souhaitez créer.

## Pour configurer les clés de ventilation d’immobilisations (facultatif)

Utilisez clé de ventilation pour allouer transactions en départements ou en projets. Vous pouvez, par exemple, définissez une clé de ventilation pour répartir les coûts d’amortissement des véhicules entre le service administratif pour 35 % et le service commercial pour 65 %. Pour plus d’informations, reportez vous à [Répartition des coûts et du revenu](year-allocate-costs-income.md).

Les clés de ventilation s’appliquent à des classes d’immobilisations et non à des immobilisations individuelles.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Groupes compta. immo.**, puis choisissez le lien associé.  
2. Sur la page **Groupes compta. immo.**, sélectionnez l’action **Ventilations**, puis choisissez un type de validation.
3. Sur la page **Ventilations immo.**, renseignez les champs selon vos besoins.
4. Répétez les étapes 2 et 3 pour chacun des types de validation pour lesquels vous souhaitez définir des clés de ventilation.

## Pour configurer les lots feuille immobilisation (facultatif)

Vous pouvez définir plusieurs feuilles, c’est-à-dire des feuilles individuelles pour chaque modèle feuille. Par exemple, chaque employé peut avoir sa propre feuille dont le nom correspond à ses initiales. Pour en savoir plus, consultez [Utiliser des feuilles comptabilité](ui-work-general-journals.md).  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Modèles feuille immo.**, puis sélectionnez le lien associé.  
2. Sélectionnez le modèle feuille pertinent, puis l’action **Lots**.
3. Sur la page **Lots feuille immo.**, renseignez les champs selon vos besoins.

## Pour configurer des modèles feuille reclassement immobilisation (facultatif)

Utiliser les feuilles reclassement dédiées transférer, fractionner ou regrouper des immobilisations. [!INCLUDE[prod_short](includes/prod_short.md)] crée automatiquement un modèle feuille reclassement immobilisation la première fois que vous ouvrez la page **Feuille reclass. immo**. Vous pouvez paramétrer d’autres modèles feuille reclassement. Pour en savoir plus, voir [Utiliser des feuilles comptabilité](ui-work-general-journals.md).  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Modèles feuille reclass. immo.**, puis sélectionnez le lien associé.  
2. Renseignez les champs selon vos besoins.

## Pour configurer les lots feuille reclassement immobilisation (facultatif)

Vous pouvez définir plusieurs feuilles, c’est-à-dire des feuilles individuelles pour chaque modèle feuille reclassement. Par exemple, chaque employé peut avoir sa propre feuille reclassement dont le nom correspond à ses initiales. Pour en savoir plus, consultez [Utiliser des feuilles comptabilité](ui-work-general-journals.md).

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Modèles feuille reclass. immo.**, puis sélectionnez le lien associé.  
2. Sélectionnez le modèle feuille pertinent, puis l’action **Lots**.
3. Sur la page **Nom feuilles reclass. immo.**, renseignez les champs selon vos besoins.

## Voir aussi

[Paramétrage d’immobilisations](fa-setup.md)  
[Vue d’ensemble des immobilisations](fa-manage.md)  
[Finances](finance.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
