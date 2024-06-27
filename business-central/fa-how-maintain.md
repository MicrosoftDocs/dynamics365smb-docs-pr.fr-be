---
title: Mise à jour des immobilisations
description: Enregistrez les réparations et l’entretien d’une immobilisation pour en préserver la valeur.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'repair, service'
ms.search.form: '5642, 5625'
ms.date: 05/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# Mise à jour des immobilisations

Les frais d’entretien sont des dépenses d’exploitation liées aux choses que vous faites pour préserver l’état de vos immobilisations. Contrairement aux améliorations des immobilisations, l’entretien n’augmente pas la valeur de vos actifs.

Chaque fois une immobilisation envoyée en réparation, vous enregistrez les informations, par exemple la date de réparation, le fournisseur et le numéro de téléphone de l'intervenant. Vous saisissez les informations de maintenance sur plusieurs pages :

* Fiche immobilisation
* Commande achat
* Facture achat
* Feuille compta. immo.

L'actualisation permet d'ajuster des valeurs en fonction de modifications générales de niveau de prix. Utiliser action **Réévaluer immobilisations** recalculer les coûts de maintenance.

## Enregistrer une coût de maintenance directement sur une immobilisation

Vous pouvez enregistrer chaque tâche de maintenance d’un actif, telle qu’une visite de service, utilisez la page **Saisie de la maintenance**.  

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Immobilisations**, puis choisissez le lien associé.  
2. Sélectionnez l’immobilisation pour laquelle vous souhaitez enregistrer la maintenance, puis sélectionnez l’action **Saisie de la maintenance**.
3. Sur la page **Saisie de la maintenance**, renseignez les champs comme nécessaire. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## Valider les coûts de maintenance à partir d’une feuille comptabilisation immobilisation

1. Sélectionnez ![icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Liste de la loi d’amortissement**, puis choisissez le lien associé.  
2. Sélectionnez la loi d’amortissement qui est attribuée à une immobilisation, puis sélectionnez l’action **Modifier**.
3. Sur la page **Carte du livre d’amortissement**, assurez-vous que la case **Maintenance** n’est pas cochée afin de ne pas comptabiliser les coûts de maintenance dans le grand livre général.
4. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Feuilles comptabilisation immobilisation**, puis choisissez le lien associé.  
5. Créez une feuille comptable initiale et complétez les champs, le cas échéant.
6. Dans le champ **Type compta. immo**, sélectionnez **Maintenance**.
7. Sélectionnez l’action **Insérer contrepartie immo.**. Une seconde ligne feuille est créée pour le compte contrepartie qui est configuré pour la validation de la maintenance.

    > [!NOTE]  
    > L’étape 7 ne fonctionne que si vous avez configuré ce qui suit : sur la page **Fiche groupe compta. immo.** du groupe de validation de l’immobilisation, le champ **Compte maintenance** contient le compte débit général et le champ **Compte contrepartie maintenance** contient le compte général dans lequel vous souhaitez valider les écritures contrepartie pour réévaluation. Pour plus d’informations, reportez vous à [Pour configurer des groupes de validation immobilisation](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).
8. Sélectionnez l’action **Valider**.

## Enregistrer le coût de maintenance à partir d’une facture d’achat

Les étapes suivantes décrivent comment enregistrer les coûts de maintenance d’une immobilisation à partir d’une facture d’achat. La procédure est identique pour des commandes achat.

1. Sélectionnez ![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Facture achat**, puis sélectionnez le lien associé.
2. Sur le raccourci **Général**, complétez les champs, comme nécessaire. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Dans le champ **Type** du raccourci **Lignes**, sélectionnez **Immobilisations**.
4. Dans le champ **N°**, choisissez l’actif, puis spécifiez la quantité et le coût.
5. Dans le champ **Type compta. immo**, sélectionnez **Maintenance**.
6. Valider facture achat.

## Suivre visites d’entretien

Vous pouvez imprimer l’état **Maintenance - Service suivant** afin de lister les immobilisations programmé une visite de service. Vous pouvez également utiliser cet état à mettez à jour le champ **Date prochain service** des fiches immobilisation.  

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Maintenance - Service suivant**, puis choisissez le lien associé.  
2. Renseignez les champs **Date début** et **Date fin**.  
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## Surveillance des coûts de maintenance

Vous pouvez afficher des statistiques pour surveiller les coûts de maintenance.  

1. Sélectionnez l’![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Immobilisations**, puis choisissez le lien associé.
2. Sélectionnez l’immobilisation pour laquelle vous souhaitez afficher les coûts de maintenance, puis sélectionnez l’action **Lois d’amortissement**.
3. Sur la page **Lois d’amortissement immobilisation**, sélectionnez la loi d’amortissement immobilisation pertinente, puis sélectionnez l’action **Statistiques**.
4. Sur la page **Statistiques immobilisation**, sélectionnez le champ **Maintenance**.

Utilisez la page **Écritures comptables maintenance** affichant les écritures qui constituent le montant dans le champ **Maintenance**.

## Afficher ou imprimer les coûts de maintenance pour plusieurs immobilisations

Dans l’état **Maintenance - Analyse**, vous pouvez choisir de examiner la maintenance sur un, deux ou trois codes maintenance pour une date ou une période donnée. Le rapport peut visualiser le total de toutes les immobilisations sélectionnées, soit celui de chaque immobilisation.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Maintenance - Analyse**, puis sélectionnez le lien associé.
2. Renseignez les champs selon vos besoins.
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## Visualiser des écritures comptables maintenance

Vous pouvez également explorer les coûts de maintenance en visualisant les écritures comptables.  

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") saisissez **Immobilisations**, puis choisissez le lien associé.
2. Sélectionnez l’immobilisation pour laquelle vous souhaitez afficher les écritures comptables, puis sélectionnez l’action **Lois d’amortissement**.
3. Sur la page **Écritures comptables maintenance**, sélectionnez la loi d’amortissement immobilisation pertinente, puis l’action **Statistiques**.

## Afficher ou imprimer les écritures comptables de maintenance pour plusieurs immobilisations

Dans l’état **Maintenance - Détails**, vous pouvez afficher ou imprimer les écritures comptables de maintenance pour un ou plusieurs actifs.  

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Maintenance - Détails**, puis sélectionnez le lien associé.
2. Renseignez les champs selon vos besoins.
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## Voir aussi

[Immobilisations](fa-manage.md)  
[Paramétrage d’immobilisations](fa-setup.md)  
[Finances](finance.md)  
[Préparation aux activités commerciales](ui-get-ready-business.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
