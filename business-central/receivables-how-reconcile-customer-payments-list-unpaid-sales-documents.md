---
title: Lettrer des paiements avec des documents vente échus
description: 'Vous lettrez les montants payés par les clients avec des documents vente associés et validez le paiement pour mettre à jour le client, la comptabilité, et les écritures comptables bancaires.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'payment process, cash receipts, customer payment'
ms.search.form: '1290, 1294, 1287'
ms.date: 07/08/2024
ms.service: dynamics-365-business-central
---

# Rapprochement des paiements client à partir de la liste des documents vente échus

Une fois que les clients ont effectué des paiements électroniques sur votre compte bancaire, vous devez effectuer les actions suivantes :

* Appliquer chaque paiement au document vente validé lié.
* Validez le paiement pour mettre à jour les écritures de paiement dans les comptes général, bancaire, et client.

Selon les besoins de votre entreprise, vous pouvez enregistrer ces paiements manuellement, automatiquement, et via des services de paiement.  

> [!NOTE]  
> Vous pouvez effectuer les mêmes tâches, y compris les paiements des fournisseurs, sur la page **Journal de rapprochement des paiements**. Par exemple, vous pouvez importer des relevés bancaires, utiliser l’application automatique et rapprocher les comptes bancaires. Pour plus d'informations, voir [Rapprocher les paiements à l'aide du lettrage automatique](receivables-how-reconcile-payments-auto-application.md).

Utilisez la page **Enregistrer les paiements client** pour réaliser les tâches de contrepartie des comptes internes en utilisant les chiffres de trésorerie réels pour s’assurer que les paiements sont collectés. Vous pouvez rapidement vérifier et valider les paiements individuels ou forfaitaires, traiter des paiements escomptés et trouver les documents impayés.

Validez les paiements pour des clients différents qui ont des dates d’échéance différentes en tant que paiements individuels. Les paiements pour le même client qui ont la même date d'échéance peuvent être validés comme paiement forfaitaire. Les paiements forfaitaires sont utiles, par exemple, lorsqu’un client a effectué un paiement unique qui couvre plusieurs factures vente.

## Pour configurer la feuille enregistrement de paiement

Étant donné que vous pouvez valider différents types de règlement dans différents comptes de contrepartie, vous devez sélectionner un compte de contrepartie sur la page **Paramétrage de l'enregistrement de paiement** avant de commencer le traitement des paiements client. Si vous validez toujours sur le même compte contrepartie, vous pouvez définir ce compte par défaut et éviter cette étape chaque fois que vous ouvrez la page **Enregistrer les paiements client**.  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Paramétrage de l’enregistrement de paiement**, puis choisissez le lien associé. Vous pouvez également choisir l’action **Configurer** sur la page **Enregistrer les paiements client**.
2. Renseignez les champs de la page **Paramétrage de l'enregistrement de paiement**. [!INCLUDE [tooltip-inline-tip_md](../archive/SetupAndAdministration/includes/tooltip-inline-tip_md.md)].  

> [!TIP]
> Pour faciliter l’identification ultérieure des écritures qui ont été validées via le journal, vous pouvez affecter une série de numéros spécifique au feuille paiement. La souches de numéros est utile si vous utilisez des journaux de rapprochement bancaire pour enregistrer et imputer les paiements.

## Pour enregistrer les paiements client individuellement

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Enregistrer les paiements client**, puis choisissez le lien associé.  

    La page **Enregistrer les paiements client** affiche tous les documents validés pour lesquels un paiement peut être enregistré. Vous pouvez peut également ouverte la page à partir des pages **Clients** et **Fiche client** filtrée pour le client spécifié.  
2. Cochez la case **Paiement effectué** de la ligne représentant le document validé pour lequel un paiement effectué.
3. Dans le champ **Date de réception**, entrez la date de réception du paiement. Cette date peut être différent de la date de travail.  

   Si la case **Renseigner automatiquement la date de réception** est cochée sur la page **Paramétrage de l’enregistrement de paiement**, le champ **Date de réception** contient la date travail.  
4. Dans le champ **Montant reçu**, saisissez le montant payé.

    Pour les paiements intégraux, le montant est le même que celui du champ **Montant ouvert** de la ligne. Pour les paiements partiels, le montant est inférieur à celui du champ **Montant ouvert** de la ligne.
5. Répétez les étapes 2 à 4 pour les autres lignes pour des documents validés pour lesquels des paiements sont effectués.  
6. Sélectionnez l'action **Valider les paiements**.  

Les informations de paiement saisies sont validées pour les documents sur les lignes dont la case **Paiement effectué** est cochée. Les écritures de paiement sont validées dans les comptes général, bancaire, et client.

## Pour rapprocher des paiements forfaitaires

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Enregistrer les paiements client**, puis choisissez le lien associé.
2. Cochez la case **Paiement effectué** pour les lignes pour les documents validés pour le même client pour lequel un paiement forfaitaire a été effectué.  

    > [!NOTE]  
    > Le champ **Nom** du client doit être le même sur toutes les lignes validées à inclure dans paiement forfaitaire.  

    Si la case **Renseigner automatiquement la date de réception** est cochée sur la page **Paramétrage de l’enregistrement de paiement**, le champ **Date de réception** contient la date travail.  
3. Dans le champ **Date de réception**, entrez la date de réception du paiement. Cette date peut être différent de la date de travail.  

    > [!NOTE]  
    > Cette date doit être identique sur toutes les lignes qui seront validées comme paiement forfaitaire.  
4. Dans le champ **Montant reçu**, entrez les montants sur plusieurs lignes pour obtenir le paiement forfaitaire.  

    > [!TIP]  
    > Essayez de valider le plus de paiements intégraux possible avec le montant forfaitaire. Entrez des montants identiques au montant du champ **Montant ouvert** sur autant de lignes que possible.  
5. Répétez les étapes 2 à 4 pour les autres lignes représentant les documents validés pour le même client pour lequel un paiement forfaitaire effectué.  
6. Sélectionnez l'action **Valider comme paiement forfaitaire**.

   Les informations de paiement saisies sont validées pour les documents sur les lignes dont la case **Paiement effectué** est cochée. Les écritures de paiement sont validées dans les comptes général, bancaire, et client. Chaque paiement est lettré au document vente validé lié.  

Si un paiement avec la banque n’est pas représenté par une ligne sur la page **Enregistrer les paiements client**, cela peut être parce que le document connexe n’a pas été validé. Dans ce cas, vous pouvez utiliser la fonction de recherche pour trouver rapidement le document et le valider pour traiter le paiement. Pour plus d’informations, voir [Pour rechercher un document vente spécifique qui n’est pas totalement facturé](#to-find-a-specific-sales-document-that-isnt-fully-invoiced).  

Si un paiement avec la banque n’est représenté par aucun document, vous pouvez ouvrir une ligne feuille comptabilité préremplie depuis la page **Enregistrer les paiements client** pour valider le paiement directement dans le compte contrepartie sans lettrer le paiement avec un document. Sinon, vous pouvez enregistrer le paiement dans la feuille jusqu’à ce que l’origine du paiement soit résolue. Pour plus d'informations, reportez-vous à [Pour enregistrer ou valider un paiement sans document connexe](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md#to-record-or-post-a-payment-without-a-related-document).  

## Pour traiter manuellement les paiements client avec remises

Si vous convenu d’un escompte avec le client, les montants règlement peuvent être inférieurs aux montants facture si le paiement est effectué avant la date d’escompte convenue.  

Les procédures suivantes expliquent méthodes différentes permettant de valider des paiements escomptés sur la page **Enregistrement de paiement**.  

* Le montant règlement est égal au montant escompté ouvert, et la date d'échéance est antérieure à la date d'escompte. Vous validez le paiement tel quel.  
* Le montant règlement est égal au montant escompté ouvert, mais la date d'échéance est postérieure à la date d'escompte. Vous validez le paiement comme partiel. Le document reste ouvert pour collecter/payer le montant ouvert. Vous pouvez également définir la date d’escompte ultérieurement pour permettre la réalisation de la totalité du paiement.  
* Le montant règlement est inférieur au montant escompté ouvert. Vous validez le paiement comme partiel. Le document reste ouvert pour collecter/payer le montant ouvert.  
* Le montant règlement est supérieur au montant escompté ouvert. Vous validez les paiements tels quels. Seul le montant ouvert est validé. Le montant supplémentaire est crédité au client.  

### Pour traiter un montant règlement égal au montant escompté, et lorsque la date d'échéance est antérieure à la date d'escompte

1. Sélectionnez ![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Enregistrer les paiements client**, puis choisissez le lien associé.  
2. Saisissez le montant du paiement dans le champ **Montant reçu**. Le montant est égal au montant du champ **Montant ouvert remise incl.**.

    La case **Paiement effectué** est automatiquement cochée, et le champ **Date de réception** contient la date de travail.
3. Saisissez la date du paiement dans le champ **Date de réception**. La date est antérieure à la date du champ **Date d'escompte**.
4. Vérifiez que le champ **Montant ouvert** indique zéro (0).  
5. Sélectionnez l'action **Valider les paiements** pour valider l'intégralité du paiement sur les comptes général, bancaire et client.

### Pour traiter un montant règlement égal au montant escompté, mais lorsque la date d'échéance est postérieure à la date d'escompte

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Enregistrer les paiements client**, puis choisissez le lien associé.  
2. Saisissez le montant du paiement dans le champ **Montant reçu**. Le montant est égal au montant du champ **Montant ouvert remise incl.**.

    La case **Paiement effectué** est automatiquement cochée, et le champ **Date de réception** contient la date de travail.
3. Dans le champ **Date de réception**, saisissez une date d'échéance ultérieure à celle indiquée dans le champ **Date d'escompte**.

   La police des champs de date devient rouge et un message d'erreur s'affiche au bas de la page. Les deux étapes suivantes résolvent ce problème.
4. Sélectionnez l'action **Détails**.  
5. Sur la page  **Détails de l’enregistrement du paiement**, dans le champ  **Date de remise sur paiement** du raccourci  **Remise sur paiement**, saisissez une date postérieure à la date du champ  **Date de réception** de la page  **Configuration de l’enregistrement du paiement** .  

    Le message d’erreur et la police rouge disparaissent, vous pouvez traiter le paiement escompté.
6. Vérifiez que le champ **Montant ouvert** indique le montant qui reste à régler pour le montant total de la facture.  
7. Sélectionnez l'action **Valider les paiements** pour valider le paiement partiel sur les comptes général, bancaire et client.  

Le document connexe reste ouvert.

### Pour traiter un paiement inférieur au montant escompté ouvert

1. Sélectionnez l’![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Enregistrer les paiements client**, puis choisissez le lien associé.  
2. Saisissez le montant du paiement dans le champ **Montant reçu**. Le montant est inférieur au montant du champ **Montant ouvert remise incl.**.

    La case **Paiement effectué** est automatiquement cochée, et le champ **Date de réception** contient la date de travail.  
3. Saisissez la date du paiement dans le champ **Date de réception**. La date est antérieure à la date du champ **Date d'escompte**.
4. Vérifiez que le champ **Montant ouvert** indique le montant qui reste à régler pour le montant escompté.  
5. Sélectionnez l'action **Valider les paiements** pour valider le paiement partiel sur les comptes général, bancaire et client.  

Le document connexe reste ouvert.

### Pour traiter un paiement supérieur au montant escompté ouvert

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Enregistrer les paiements client**, puis choisissez le lien associé.  
2. Saisissez le montant du paiement dans le champ **Montant reçu**. Le montant est supérieur au montant du champ **Montant ouvert remise incl.**.  

    La case **Paiement effectué** est automatiquement cochée, et le champ **Date de réception** contient la date de travail.
3. Saisissez la date du paiement dans le champ **Date de réception**. La date est antérieure à la date du champ **Date d'escompte**.
4. Vérifiez que le champ **Montant ouvert** indique zéro (0).  
5. Sélectionnez l'action **Valider les paiements** pour valider l'intégralité du paiement sur les comptes général, bancaire et client.  

Le document connexe est clôturé, et le client est crédité du montant règlement excédentaire.  

## Pour rechercher un document vente spécifique qui n’est pas totalement facturé

La page **Enregistrer les paiements client** vous aide dans les tâches de contrepartie des comptes internes avec les chiffres réels de règlement pour assurer une collecte efficace auprès des clients et le paiement des sommes dues aux fournisseurs. Elle affiche les paiements entrants en attente sous la forme de lignes représentant les documents vente pour lesquels un montant doit être payé.  

Généralement, lorsqu’un paiement est effectué, enregistré en banque ou autrement, le document de vente ou d’achat est représenté sous forme de ligne sur la page **Enregistrer les paiements des clients**. Le document attend que vous comptabilisiez le paiement sur le montant impayé. Cependant, parfois un paiement qui a effectué n’est pas représenté par une ligne sur la page **Enregistrer les paiements client**, généralement parce que la facture du document n’est pas encore totalement validé.

Utiliser l’action **Recherche de documents** pour rechercher parmi les documents qui n’ont pas été entièrement facturés. Vous pouvez effectuer une recherche avec un ou plusieurs des critères suivants :  

* Numéro de document  
* Montant ou plage de montants  

La procédure suivante explique comment trouver un document spécifique à l'aide de deux critères de recherche.  

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Enregistrer les paiements client**, puis choisissez le lien associé.
2. Avec le pointeur sur n'importe quelle ligne, sélectionnez l'action **Rechercher des documents**.
3. Sur la page **Recherche de document**, entrez une valeur de recherche dans le champ **N° document**.  

    > [!NOTE]  
    > La valeur que vous entrez dans ce champ est indiquée entre caractères génériques masqués. Cela signifie que la Action recherche tous les numéros de document qui contiennent la valeur saisie.
4. Dans le champ **Montant**, saisissez le montant spécifique sur le document que vous recherchez.  
5. Dans le champ **% écart de quantité**, saisissez la valeur du pourcentage pour définir la plage des montants dans laquelle rechercher le document ouvert.  

    Si vous saisissez 10, l’action recherche les montants compris dans une plage de plus ou moins 10 pour cent de la valeur dans le champ **Montant**.
6. Sélectionnez l'action **Rechercher**.  

Si un ou plusieurs documents correspondent aux critères de recherche, la page **Résultat de la recherche de documents** s’ouvre et affiche les lignes représentant ces documents. Chaque ligne contient un numéro de document, une description et un montant.

Si un paiement avec la banque n’est représenté par aucun document, vous pouvez ouvrir une ligne feuille comptabilité préremplie depuis la page **Enregistrer les paiements client** pour valider le paiement directement dans le compte contrepartie sans lettrer le paiement avec un document. Sinon, vous pouvez enregistrer le paiement dans la feuille jusqu’à ce que l’origine du paiement soit résolue.  

## Pour enregistrer ou valider un paiement sans document connexe

Si un paiement en banque n’est pas représenté par un document, vous pouvez utiliser l’action **Journal général** pour ouvrir une ligne journal général préremplie à partir du **Enregistrer les paiements des clients** page. Utilisez le journal pour valider le paiement directement sur le compte d’équilibrage sans appliquer le paiement à un document. Sinon, vous pouvez enregistrer le paiement dans la feuille jusqu’à ce que l’origine du paiement soit résolue.  

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Enregistrer les paiements client**, puis choisissez le lien associé.
2. Sélectionnez l'action **Feuille comptabilité**.  

    La page **Feuille comptabilité** s’affiche avec une ligne préremplie où figure le compte contrepartie du nom de feuille défini sur la page **Paramétrage de l’enregistrement de paiement**.  
3. Renseignez les autres champs de chaque ligne feuille. Par exemple, fournissez le montant, le numéro de client ou les informations du relevé bancaire. Pour plus d'informations, reportez-vous à [Valider les transactions directement vers la comptabilité](finance-how-post-transactions-directly.md).  

Vous pouvez soit valider la ligne feuille mettre à jour le total sur le compte contrepartie. Sinon, vous pouvez laisser la ligne feuille non validée et ajouter par exemple une note indiquant que le paiement a besoin d’une autre analyse.  

Si vous ne validez pas la ligne journal, sa valeur est ajoutée à la valeur dans le champ **Montant ouvert remise incl.** sur la page **Enregistrement du paiement**.  

## Voir aussi

[Gestion des comptes client](receivables-manage-receivables.md)  
[Ventes](sales-manage-sales.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]