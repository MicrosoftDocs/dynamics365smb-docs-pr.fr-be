---
title: Configuration des conditions et niveaux
description: Configurez Business Central afin de pouvoir envoyer des rappels sur les paiements dus et ajouter des frais ou des frais en raison du retard.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'payment due, debt, overdue, fee, charge, reminder'
ms.search.form: '431, 432, 436, 478'
ms.date: 03/12/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Configuration des conditions et niveaux de relance

Vous pouvez utiliser des relances pour informer aux clients les soldes échus et demande paiement. [!INCLUDE [reminder-terms](includes/reminder-terms.md)]

> [!TIP]
> Après avoir configuré les conditions et les niveaux de rappel, vous pouvez les inclure dans les processus automatisés de création, d’émission et d’envoi de rappels. Pour en savoir plus sur le processus automatisé, accédez à [Automatiser les rappels dans les collections](finance-automate-reminders.md).

## Conditions de relance

Si des clients ont des impayés, vous devez décider quand et comment envoyer une relance. En outre, vous pouvez être amené à débiter leurs comptes d’intérêts ou de frais. Vous pouvez configurer autant de conditions relance que vous le souhaitez.  

> [!NOTE]
> Si vous souhaitez calculer les intérêts sur les paiements échus, vous pouvez le faire lorsque vous créez des relances. Cependant, si vous souhaitez calculer les intérêts et en informer vos clients sans envoyer une relances, utilisez un [factures d’intérêts](finance-setup-finance-charges.md). Pour plus d’informations, consultez [Relances](receivables-collect-outstanding-balances.md#reminders) ou [Frais financiers](receivables-collect-outstanding-balances.md#finance-charges).

### Configurer les textes des pièces jointes et du corps des e-mails pour les communications

Sur la page **Configuration des conditions de rappel** , vous pouvez configurer les textes des pièces jointes et les e-mails standard à utiliser soit pour tous les niveaux de rappel, soit créer des messages spécifiques pour chaque niveau. Par exemple, le message que vous envoyez pour le premier niveau de rappel peut avoir un ton ou un contenu différent de celui du deuxième ou du troisième. Pour créer des pièces jointes et des textes de messages électroniques pour tous les niveaux, choisissez **Communication client** en haut de la page. Pour créer des messages pour des lignes spécifiques, sur l’onglet rapide **Niveau de rappel** , choisissez une ligne, puis choisissez la **Communication client** action sur le raccourci.

Par défaut, les textes des pièces jointes et des e-mails utilisent votre paramètre de langue. Toutefois, si vous envoyez des rappels à des clients dans d’autres pays, vous souhaiterez peut-être communiquer dans différentes langues. Vous pouvez créer des textes pour chaque langue [!INCLUDE [prod_short](includes/prod_short.md)] prise en charge en utilisant l’action **Ajouter du texte pour la langue** . Si vous le faites, assurez-vous que les langues sont les mêmes pour les textes des pièces jointes et les textes des e-mails. S’ils ne correspondent pas et que le terme de rappel comporte plusieurs niveaux, l’automatisation risque de ne pas être en mesure de personnaliser le message pour un ou plusieurs niveaux. Pour vérifier que les langues correspondent, utilisez l’action **Aperçu des communications** et comparez les communications pour les textes.

Lorsque vous envoyez un e-mail, le rappel est un rapport que vous joignez à l’e-mail. Vous définissez le rapport qui génère le rappel sur la page **Rappel de sélection de rapport/frais financiers** , où vous sélectionnez également le rapport contenant le texte du corps de l’e-mail dans le **Champ Nom de la présentation du corps de l’e-mail** . Lorsque vous envoyez des e-mails à vos clients, les textes du Raccourci **Texte de l’e-mail** sont insérés dans le rapport sélectionné dans le **Nom de la présentation du corps de l’e-mail** champ. Le rapport standard comporte un champ de texte pour ce texte. Si vous le souhaitez, vous pouvez modifier ce rapport, par exemple pour ajouter ou supprimer du contenu. Modifiez la mise en page de ces rapports sur la page **Mise en page des rapports** . Pour en savoir plus sur les présentations de rapport, accédez à [Commencez à créer des présentations de rapport](ui-get-started-layouts.md).

> [!NOTE]
> Pour communiquer par e-mail directement depuis [!INCLUDE [prod_short](includes/prod_short.md)] , vous devez être configuré pour le faire. Pour en savoir plus sur la connexion des comptes e-mails avec [!INCLUDE [prod_short](includes/prod_short.md)], consultez [Configurer e-mail](admin-how-setup-email.md).

### Configurer des conditions de relance

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Conditions de relance**, puis sélectionnez le lien associé.  
2. Renseignez les champs selon vos besoins. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  
3. Pour utiliser plusieurs combinaisons de conditions de relance, créez un code pour chacun d'eux.

## Niveaux relance

Pour chaque terme de rappel, vous pouvez définir un nombre illimité de niveaux de rappel, même si la plupart des entreprises n’utilisent que deux ou trois niveaux. La première fois qu'une relance est créée pour un client, le paramétrage utilisé est celui du niveau 1. Lorsque la relance est émise, le numéro du niveau est enregistré dans les écritures relance qui sont créées et associées à l'écriture comptable client spécifique. S’il est nécessaire de relancer le client, toutes les écritures comptables relance associées aux écritures comptables client ouvertes sont vérifiées afin de localiser le numéro de niveau le plus élevé. Les conditions du niveau suivant seront alors utilisées pour la nouvelle relance.

Si vous créez plus de relances qu'il n'y a de niveaux relance, les conditions utilisées sont celles du niveau le plus élevé. Vous pouvez utiliser autant de relances que le champ **Nombre max. de relances** des conditions relance le permet.

### Pour configurer des niveaux de relance

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Conditions de relance**, puis sélectionnez le lien associé.  
2. Sur la page **Conditions de relance**, cliquez sur la ligne comportant les conditions pour lesquelles configurer des niveaux, puis cliquez sur l’action **Niveaux**.  
3. Renseignez les champs selon vos besoins. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

    > [!TIP]
    > Le cadre du champ **Calculer l’intérêt** détermine si l’intérêt apparaîtra sur la relance lorsque la relance est émise. Cependant, le champ **Comptabiliser intérêts** sur la page **Conditions de relance** détermine si les intérêts calculés doivent être imputés aux comptes généraux et clients.
    >
    > Pour indiquer que les intérêts doivent être calculés, choisissez le champ **Calculer les intérêts**.

    En option, pour chaque niveau de relance, spécifiez des frais supplémentaires en DS et en devise étrangère. Vous pouvez créer plusieurs frais supplémentaires en devise pour chaque code de la page **Niveaux relance**.  

    Les frais supplémentaires peuvent être calculés de trois manières différentes qui sont définies par la valeur du champ **Type calcul frais supplémentaires**.  

    - **Statique**

        Les frais sont calculés en fonction des valeurs des champs **Frais supplémentaires** sur la ligne pour le niveau de relance lui-même.  
    - **Dynamique unique**

        Les frais sont calculés en fonction des valeurs des champs **Configuration frais supplémentaires** sur les lignes pertinentes pour le niveau de relance lui-même.
    - **Dynamique cumulé**

        Les frais sont calculés en fonction des valeurs des champs **Configuration frais supplémentaires** sur les lignes combinées pour le niveau de relance lui-même.

4. Sélectionnez l'action **Devises**.
5. Sur la page **Devises niveau relance**, définissez un code de niveau pour chaque relance et le numéro du niveau de rappel correspondant, une devise et des frais supplémentaires.

    > [!NOTE]  
    > Lorsque vous créez une relance en devise, les conditions devise définies ici permettront de créer des relances. Si aucune condition devise n'a été définie, les conditions devise société définies sur la page **Niveaux relance** seront utilisées et converties dans la devise appropriée.

    Pour chaque niveau relance, vous pouvez indiquer le texte à imprimer avant (**Texte début**) ou après (**Texte fin**) les écritures de la relance.

6. Choisissez les actions **Texte de début** ou **Texte de fin** respectivement, puis renseignez la page **Texte relance**.
7. Pour insérer automatiquement des valeurs correspondantes dans le texte de relance, entrez les espaces réservés suivants dans le champ **Texte**.  

    |Paramètre substituable|Valeur|  
    |-----------------|-----------|  
    |%1|Contenu du champ **Date du document** de l'en-tête de relance|  
    |%2|Contenu du champ **Date d'échéance** de l'en-tête de relance|  
    |%3|Contenu du champ **Taux d'intérêt** dans les conditions d'intérêts de retard associées|  
    |%4|Contenu du champ **Montant ouvert** de l'en-tête de relance|  
    |%5|Contenu du champ **Montant intérêts** de l'en-tête de relance|  
    |%6|Contenu du champ **Frais supplémentaires** de l'en-tête de relance|  
    |%7|Montant total de la relance|  
    |%8|Contenu du champ **Niveau relance** de l'en-tête de relance|  
    |%9|Contenu du champ **Code devise** de l'en-tête de relance|  
    |%10|Contenu du champ **Date de validation** de l'en-tête de relance|  
    |%11|Nom de la société|  
    |%12|Contenu du champ **Frais supplémentaires par ligne** de l'en-tête de relance|  

    Par exemple, si vous saisissez **Vous devez %9 %7 dus au %2**, la relance contient le texte suivant : **Vous devez 1 200,50 USD dus au 02/02/2024.**.

    > [!NOTE]
    > [!INCLUDE [prod_short](includes/prod_short.md)] La date d’échéance est calculée selon la formule de date que vous saisissez. Pour plus d’informations, voir [Utiliser des formules date](ui-enter-date-ranges.md#use-date-formulas).

8. Pour spécifier la langue d’un e-mail, choisissez l’action **Ajouter du texte pour la langue** . Le champ **Code de langue** est mis à jour pour afficher votre sélection. Sur l’onglet rapide **Texte de l’e-mail** , saisissez le contenu du message dans la langue sélectionnée.

Après avoir configuré les conditions de rappel, vous pouvez les attribuer aux clients sur les pages Fiche client. Pour plus d'informations, reportez vous à [Enregistrer de nouveaux clients](sales-how-register-new-customers.md).  

## Voir aussi

[Collecte des soldes restants](receivables-collect-outstanding-balances.md)  
[Envoi des rappels de soldes impayés](receivables-send-reminders.md)  
[Configuration des conditions des frais financiers](finance-setup-finance-charges.md)  
[Configuration de Finance](finance-setup-finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
