---
title: Automatisation des relances dans les collectes
description: 'Gagner du temps dans les recouvrements en automatisant les processus de création, d’émission et d’envoi de rappels aux clients.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: how-to
ms.search.keywords: 'collection, remindes'
ms.search.form: null
ms.date: 03/12/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="automate-reminders-in-collections"></a>Automatisation des relances dans les collectes

Gagner en efficacité dans les recouvrements en automatisant le processus de création, d’émission et d’envoi de rappels aux clients. L’automatisation peut réduire considérablement le temps que vous consacrez aux collections, fournir une meilleure vue d’ensemble du processus et vous donner un contrôle total sur chaque étape.

Sur la page **Automatisation des rappels** , vous définissez les actions individuelles (étapes). Vous pouvez combiner les étapes de création, d’émission et d’envoi de rappels, ou vous pouvez créer une automatisation distincte pour chaque étape si cela convient mieux à vos processus de recouvrement. Les automatisations sont basées sur des conditions de rappel et des niveaux de rappel. Pour en savoir plus, accédez à [Créer des niveaux et conditions de rappel](finance-setup-reminders.md). Vous pouvez définir des filtres pour les termes de rappel pour une automatisation dans son ensemble et définir des filtres pour chaque action de l’automatisation. Vous pouvez également joindre les factures impayées aux e-mails sous forme de fichiers PDF.

L’automatisation se produit via une entrée dans la file d’attente des tâches. Lorsque vous configurez une automatisation, utilisez le champ **Cadence** pour spécifier comment et quand elle s’exécute. Si vous choisissez **Manuel**, l’automatisation s’exécute une fois lorsque vous utilisez l’action **Démarrer** . Vous pouvez également choisir **Hebdomadaire**, **Mensuel** ou choisir **Personnalisé** pour définir une cadence plus détaillée. Si vous choisissez **Personnalisé**, vous devez saisir une formule de date. Pour en savoir plus sur la saisie d’une formule de date, accédez à [Utiliser les formules de date](ui-enter-date-ranges.md#use-date-formulas). Lorsque vous choisissez une option autre que **Manuel**, l’automatisation s’exécute jusqu’à ce que vous la mettiez en pause pour la mettre en attente. Si vous souhaitez être encore plus précis sur le moment où il s’exécute, utilisez l’action **Entrées de la file d’attente des tâches** pour ouvrir les **Entrées de la file d’attente des tâches** page et ajustez la récurrence, par exemple sur un jour quotidien ou un jour de semaine spécifique.

## <a name="automate-the-reminders-flow"></a>Automatisez le flux de rappels

Les sections suivantes décrivent comment configurer des rappels pour créer, émettre et envoyer automatiquement.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Automatisation des relances**, puis sélectionnez le lien associé.
1. Sélectionnez **Nouveau**, puis renseignez les champs du raccourci **Général**.
1. Dans le champ **Filtre des termes de rappel** , choisissez le ou les termes de rappel pour lesquels utiliser cette automatisation.
1. Dans le champ **Cadence** , choisissez la fréquence d’exécution de l’automatisation.
1. Dans l’onglet rapide **Actions** , choisissez **Nouveau**, puis indiquez si l’automatisation crée, émet ou envoie des rappels. Cliquez sur **OK**.
1. En fonction du type d’action effectuée par l’automatisation, remplissez les champs nécessaires sur la page de configuration. Pour en savoir plus sur les paramètres, accédez à [Paramètres des actions de rappel](#settings-for-reminder-actions).
1. Après avoir configuré les actions pour l’automatisation, vous pouvez utiliser les actions **Monter** et **Descendre** pour ajuster l’ordre dans lequel ils s’exécutent.

## <a name="settings-for-reminder-actions"></a>Paramètres des actions de rappel

Les paramètres de configuration diffèrent pour les actions Créer, Émettre et Envoyer un rappel. Les sections suivantes décrivent comment les utiliser.

### <a name="create"></a>Créer

* Définir le niveau le plus élevé sur toutes les lignes de relance.  
* Créer des relances pour les écritures suspendues. Par exemple, ce paramètre est utile si vous êtes en conflit avec un client et que vous souhaitez qu’il ait une vue d’ensemble.
* Créez des rappels pour toutes les factures impayées, et pas seulement les factures en retard. Le rapport affiche les factures en retard et factures qui sont simplement impayées mais pas en retard dans des sections distinctes.
* Définissez des filtres pour rendre le rappel plus spécifique.

### <a name="issue"></a>Émission

Lorsque vous émettez un rappel, vous créez des écritures dans le grand livre client qui contiennent la date comptable et la date fiscale. Utilisez les paramètres sur le **Configuration des rappels de problèmes** pour spécifier s’il faut remplacer ces informations sur le rappel émis par les informations du rappel créé. Par exemple, si vous avez créé le rappel hier et que vous l’émettez aujourd’hui, la date d’échéance est décalée d’un jour.

### <a name="send"></a>Envoyer

> [!NOTE]
> L’automatisation d’envoi nécessite que vous ayez configuré la messagerie électronique dans [!INCLUDE [prod_short](includes/prod_short.md)]. Pour en savoir plus sur la configuration des e-mails, consultez [Configurer e-mail](admin-how-setup-email.md).

Le contenu des e-mails, tel que les textes des pièces jointes, les textes du corps des e-mails et la langue, proviennent de la configuration de la durée de rappel. Pour en savoir plus sur les paramètres d'e-mails, accédez à [Créer des niveaux et conditions de rappel](finance-setup-reminders.md).

Utilisez les paramètres sur le **Configuration de l’envoi de rappels** la page contrôle les éléments suivants :

* Paramètres généraux, tels que la description et le nombre de fois où vous envoyez le même rappel.
* Paramètres pour ce qu’il faut inclure dans le rappel.
* Paramètres permettant de suivre les rappels que vous envoyez en créant des interactions, si vous imprimez ou envoyez le rappel par e-mail, et si vous souhaitez joindre uniquement les factures en retard, toutes les factures ou aucune facture. 

## <a name="access-the-history-of-a-reminder"></a>Accéder à l’historique d’un rappel

[!INCLUDE [prod_short](includes/prod_short.md)] garde une trace de chaque exécution d’une automatisation. Vous pouvez accéder à l’historique en choisissant le **Entrées de journal** action. Vous pouvez également utiliser le **Rappels émis** action pour accéder à une liste des rappels que vous avez émis.

## <a name="handle-errors"></a>Gestion des erreurs

Sur le **Actions** Raccourci, pour chaque action, vous pouvez spécifier si vous souhaitez que l’automatisation s’arrête si l’action comporte une erreur. Si vous le faites, l’automatisation ne traitera pas les actions qui suivront. Pour activer ou désactiver cette fonctionnalité, utilisez le **Définir l’arrêt en cas d’erreur** ou **Effacer l’arrêt en cas d’erreur** Actions.

## <a name="change-action-settings-for-an-automation"></a>Modifier les paramètres d’action pour une automatisation

Vous pouvez modifier les paramètres d’une automatisation à tout moment. Sur le **Actions** Raccourci, choisissez **Installation**, puis effectuez vos modifications.

## <a name="see-also"></a>Voir aussi

[Configuration des conditions et niveaux](finance-setup-reminders.md)  
[Envoi des rappels de soldes impayés](receivables-send-reminders.md)  
