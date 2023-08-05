---
title: 'Domiciliation européenne belge [BE]'
description: 'Une domiciliation est un accord financier entre vous et vos clients, qui vous permet de collecter automatiquement les paiements pour les factures du client.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: '11300, 2000000, 2000001, 2000003, 2000020, 2000021, 2000022'
ms.date: 06/17/2021
ms.author: edupont
---
# Domiciliation européenne

Une domiciliation est un accord financier entre vous et vos clients, qui vous permet de collecter automatiquement les paiements pour les factures du client via un compte bancaire préféré. Les domiciliations peuvent uniquement être traitées pour les clients nationaux qui ont des comptes bancaires nationaux. Les domiciliations dans des devises étrangères ou concernant des banques étrangères ne sont pas prises en charge.  

La domiciliation est utile pour les sociétés qui comptent de nombreux clients ou abonnés, comme les sociétés de services publics ou d'édition.  

Avant de pouvoir commencer à utiliser la banque électronique pour les domiciliations, vous devez entrer certaines informations de base.  

- Numéro de domiciliation : il s'agit d'un code unique obtenu de la banque et qui identifie l'accord de domiciliation entre vous, votre client et la banque. Le contrat contient des informations sur la fréquence de paiement, les numéros de comptes bancaires et les montants. Lorsque vous envoyez vos paiements à la banque, celle-ci utilisera le numéro de domiciliation pour identifier toutes les parties concernées.  

- Compte bancaire préféré : le compte bancaire préféré sera proposé comme compte bancaire par défaut sur toutes les propositions de domiciliation pour ce client. Si nécessaire, vous pouvez modifier le compte bancaire avant de valider les propositions de domiciliation. Pour plus d'informations, voir [Générer les propositions de domiciliation](/dynamics365/business-central/LocalFunctionality/Belgium/direct-debit-using-domiciliation).  

## Paramétrer les domiciliations

Avant de pouvoir utiliser la banque électronique pour les domiciliations, vous devez entrer le compte bancaire préféré et le numéro de domiciliation du client.  

> [!NOTE]  
> Vous devez utiliser un seul compte bancaire par client pour toutes les domiciliations.  

### Pour configurer une domiciliation  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Clients**, puis choisissez le lien associé.  
2. Sélectionnez le client, puis choisissez l'action **Modifier**.  
3. Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |-----|-----------|  
    |**Domiciliation**|Entrez le numéro de domiciliation du client. Ce numéro sera utilisé lorsque vous créerez des domiciliations pour ce client.|  
    |**Compte bancaire préféré**|Entrez le compte bancaire préféré pour les transactions avec ce client. Ce compte sera utilisé lorsque vous créerez une proposition de paiement pour ce client.|  

## Générer des suggestions de domiciliation

Après avoir paramétré les domiciliations, vous pouvez commencer à générer des suggestions de domiciliation. Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], vous pouvez uniquement créer des suggestions de domiciliation pour les clients nationaux.  

### Pour générer des suggestions de domiciliation  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuille domiciliation**, puis choisissez le lien associé.  
2. Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Suggérer des domiciliations**.  
3. Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date d'échéance**|Entrez la date d'échéance à inclure dans le traitement par lots. Seules les écritures dont la date d'échéance est antérieure ou identique à cette date sont incluses.|  
    |**Accepter les escomptes**|Sélectionnez ce champ si vous souhaitez inclure dans le traitement par lots les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.|  
    |**Date d'escompte**|Entrez la date qui est utilisée pour calculer l'escompte.|  
    |**Sélectionner les remboursements possibles**|Sélectionnez ce champ si vous souhaitez inclure dans le traitement par lots les remboursements.|  
    |**Date de validation**|Entrez la date qui s'affiche comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.|  

4. Entrez les éventuels critères de filtre supplémentaires.  
5. Cliquez sur le bouton **OK**.  

Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes correspondant aux filtres.  

> [!NOTE]  
> Les suggestions de domiciliation n'incluent que les clients pour lesquels un numéro de domiciliation est configuré. Pour plus d'informations, voir la section [Paramétrer les domiciliations](#set-up-domiciliations).  

## Modifier et supprimer des lignes de domiciliation

Après avoir généré des propositions de domiciliation, vous souhaiterez peut-être modifier les lignes domiciliation. Par exemple, vous souhaiterez peut-être réaffecter un compte bancaire ou empêcher le paiement pour un client ou une écriture comptable client spécifique.  

Après avoir modifié les lignes feuille, imprimez l'état **FS domicil. - Impression test** pour tester toutes les lignes feuilles.  

Le traitement par lots **Proposer domiciliations** crée des propositions de domiciliation pour tous les clients qui correspondent aux critères spécifiés.  

### Pour modifier une ligne feuille  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles domiciliation**, puis choisissez le lien associé.  
2. Dans le champ **Nom feuille**, sélectionnez la feuille concernée.  
3. Sélectionnez la ligne feuille, puis modifiez les champs.  

### Pour supprimer une ligne feuille  

1  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles domiciliation**, puis choisissez le lien associé.  
2. Dans le champ **Nom feuille**, sélectionnez la feuille concernée.  
3. Sélectionnez la ligne feuille, puis choisissez l'action **Supprimer**.  
4. Cliquez sur le bouton **Oui**.  

## Tester les domiciliations

Pour tester les lignes feuille domiciliation, vous pouvez utiliser l'état **Feuille domiciliation - Test**. Cet état imprime un aperçu de toutes les lignes feuille, ainsi que toutes les erreurs, telles que des champs manquants ou des comptes bancaires incorrects. Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.  

### Pour imprimer un état de test de domiciliation  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuille domiciliation**, puis choisissez le lien associé.  
2. Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.  
3. Sélectionnez l'option **Impression test**.  
4. Sélectionnez le bouton **Imprimer** pour imprimer l'état, ou le bouton **Aperçu** pour l'afficher à l'écran.  

## Exporter et valider les domiciliations

Vous pouvez soumettre des domiciliations à votre banque en exportant les données dans un fichier. Lorsque vous exportez les données dans un fichier, vous pouvez choisir de valider automatiquement les lignes dans la comptabilité.  

Selon le paramétrage du champ **Format exp. prélèvement SEPA** dans la page **Fiche compte bancaire**, l'action **Domiciliations de fichier** ouvre l'une des pages de demande suivantes :  

- Page**Créer des lignes feuille comptabilité** – pour le format de prélèvement SEPA.  
- Page**Domiciliations de fichier** – pour les formats nationaux.  

### Pour exporter et valider les domiciliations

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles domiciliation**, puis choisissez le lien associé.  
2. Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Domiciliations de fichier**.  
3. Sur la page **Créer lignes FS**, renseignez les champs selon vos besoins. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

    Si votre société est paramétrée de façon à utiliser le format ISABEL, la page **Domiciliations de fichier** s'affiche à la place.
4. Cliquez sur le bouton **OK** pour exporter le fichier.  
5. Choisissez un emplacement approprié à partir duquel vous téléchargez le fichier vers votre banque, puis choisissez **Enregistrer**.  
6. Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.  

    Si vous n'activez pas la case à cocher **Valider les lignes feuille comptabilité**, vous devrez valider les domiciliations manuellement dans la feuille comptabilité.  

    > [!NOTE]  
    >  Après avoir validé les domiciliations dans la feuille comptabilité, supprimez les domiciliations validées dans la page **Feuille domiciliation**. Pour ce faire, sélectionnez toutes les lignes avec le statut **Validé**, puis choisissez l'action **Supprimer**.  

## Voir aussi

[Paiements électroniques belges](belgian-electronic-payments.md)  
[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]