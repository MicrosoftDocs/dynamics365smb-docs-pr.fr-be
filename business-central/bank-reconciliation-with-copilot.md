---
title: Rapprocher les comptes bancaires avec Copilot (version préliminaire)
description: Découvrez comment utiliser Copilot pour rapprocher les comptes bancaires dans Business Central.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.collection:
  - get-started
  - bap-ai-copilot
ms.date: 06/13/2024
ms.custom: bap-template
---

# <a name="reconcile-bank-accounts-with-copilot-preview"></a>Rapprocher les comptes bancaires avec Copilot (version préliminaire)

[!INCLUDE [preview-banner](~/../shared-content/shared/preview-includes/preview-banner.md)]

Cet article explique comment l’assistance au rapprochement des comptes bancaires pour vous aider à rapprocher les transactions bancaires avec les écritures comptables dans Microsoft Dynamics 365 Business Central.

[!INCLUDE [preview-note](~/../shared-content/shared/preview-includes/production-ready-preview-dynamics365.md)]

## <a name="about-bank-account-reconciliation-assist"></a>À propos de l’assistant de rapprochement bancaire

L’assistant de rapprochement bancaire est un ensemble de fonctionnalités basées sur l’IA qui vous aident à rapprocher les comptes bancaires. Il propose deux tâches distinctes via Copilot :

- Amélioration de la correspondance des transactions avec les écritures comptables

    Il se peut que vous connaissiez déjà le bouton **Faire correspondre automatiquement** sur la page **Rapprochement bancaire** qui fait correspondre automatiquement la plupart des transactions bancaires avec les écritures comptables. Nous appelons cette opération *automatch*. Bien que la correspondance automatique fonctionne bien, les algorithmes utilisés peuvent parfois aboutir à de nombreuses transactions sans correspondance. Copilot utilise la technologie d’IA pour inspecter les transactions non correspondances et identifier davantage de correspondances, en fonction des dates, des montants et des descriptions. Par exemple, si un client a payé plusieurs factures en une seule fois, Copilot rapproche la ligne de relevé bancaire unique avec les multiples écritures comptables des factures.

    [En savoir plus sur cette tâche](#reconcile-bank-accounts-with-copilot).

- Comptes généraux suggérés

    Pour les transactions bancaires résiduelles qui n’ont pu être mises en correspondance avec aucune écriture du grand livre, Copilot utilise la technologie d’IA pour comparer la description de la transaction avec les noms des comptes généraux, en suggérant le compte général le plus probable pour effectuer la validation. Par exemple, si des transactions sans correspondance ont *Fuel Stop 24*, Copilot pourrait suggérer que vous les validez dans le compte *Transport*.

    [En savoir plus sur cette tâche](#post-unmatched-bank-transaction-amounts-to-suggested-gl-accounts).

## <a name="available-languages"></a>Langues disponibles

[!INCLUDE[bank-recon-assist-language-support](includes/bank-recon-assist-language-support.md)]

## <a name="prerequisites"></a>Conditions préalables

- L’assistance au rapprochement des comptes bancaires est activée. Cette tâche doit être effectuée par un administrateur. [En savoir plus sur la configuration des fonctionnalités Copilot et IA](enable-ai.md).
- Les comptes bancaires dans Business Central que vous souhaitez rapprocher sont liés à un compte bancaire en ligne ou configurés avec un format d’importation de relevé bancaire.
- Vous êtes familier avec le rapprochement des comptes bancaires dans Business Central, comme décrit dans [Rapprocher les comptes bancaires](bank-how-reconcile-bank-accounts-separately.md).

## <a name="reconcile-bank-accounts-with-copilot"></a>Rapprochement de compte bancaire avec Copilot

<!-- Similar to the **Match Automatically** capability on the **Bank Acc. Reconciliation** page, Bank account reconciliation assist can also automatically matches transactions in banks statements with bank entries. The difference is that **Match Automatically** uses a native rules-based algorithm, while Bank account reconciliation assist is based AI technology though Copilot. Bank account reconciliation assist is intended to supplement the **Match Automatically** capability. While **Match Automatically** is fairly successful at matching transactions, there are some instances where it can't&mdash;which is where Bank account reconciliation assist comes. By using the **Reconcile with Copilot** action on **Bank Acc. Reconciliation** page, you can find even more matches.-->

Copilot dans le rapprochement des comptes bancaires est destiné en complément de l’opération de rapprochement automatique. Ainsi, lorsque vous utilisez Copilot, l’opération de correspondance automatique s’exécute en premier pour effectuer les correspondances initiales. Ensuite, Copilot s’exécute pour tenter de faire correspondre les transactions que l’opération de correspondance automatique n’a pas gérées.

Il existe deux approches pour rapprocher les comptes bancaires avec Copilot :

- Utilisez Copilot pour démarrer un nouveau rapprochement sur un compte bancaire, directement à partir de la liste **Rapprochement des comptes bancaires**.
- Utilisez Copilot sur un rapprochement nouveau ou existant sur un **Rapprochement bancaire**.

# [À partir de la liste Rapprochement bancaire](#tab/fromlist)

Pour cette approche, vous créez un rapprochement de compte bancaire à partir de zéro. Cette approche nécessite que vous sélectionniez le compte bancaire. Si le compte bancaire n’est pas lié à un compte en ligne, vous devez aussi importer le fichier de relevés bancaires.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Rapprochements bancaires**, puis sélectionnez le lien associé.
1. Sélectionnez **Rapprocher avec Copilot** pour ouvrir la fenêtre **Rapprocher avec Copilot**.
1. Définissez champ **Effectuer un rapprochement pour ce compte bancaire** sur le compte bancaire que vous souhaitez rapprocher.

    ![Capture d’écran affiche la fenêtre de rapprochement avec Copilot pour un rapprochement à partir de zéro.](media/reconcile-bank-accounts-new-copilot.svg)

1. Si le compte bancaire sélectionné n’est pas lié à un compte bancaire en ligne, vous devez importer le fichier de relevés bancaires. Pour importer le fichier, sélectionnez la valeur dans le champ **Utiliser les données de transaction à partir de** ou sélectionnez le bouton du trombone en regard du bouton **Générer**. Ensuite, utilisez **Sélectionner le fichier à importer** pour importer le fichier de relevé bancaire en le faisant glisser depuis votre appareil ou en parcourant votre appareil.
1. Pour effectuer un rapprochement avec Copilot, sélectionnez **Générer**.

    Copilot commence à générer des correspondances proposées. Une fois l’opération terminée, la fenêtre **Rapprocher avec Copilot** affiche les résultats du processus de mise en correspondance.

1. Passez en revue les correspondances proposées comme décrit dans la section suivante.

# [À partir d’une carte de rapprochement bancaire](#tab/fromcard)

Pour cette approche, vous utilisez Copilot soit sur un nouveau rapprochement de compte bancaire que vous créez manuellement, soit en modifiant un rapprochement existant.

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Rapprochements bancaires**, puis sélectionnez le lien associé.
1. Utilisez l’une des procédures suivantes :

    - Sélectionnez **Nouveau** pour démarrer un nouveau rapprochement.
    - Sélectionnez et ouvrez un rapprochement existant dans la liste.

1. Sur la carte **Rapprochement bancaire**, sélectionnez **Rapprocher avec Copilot**.

    ![Capture d’écran Affiche le rapprochement avec le bouton Copilot sur la carte Rapprochement bancaire.](media/bank-reconciliation-copilot-card.svg)

    Copilot commence à générer des correspondances proposées. Une fois l’opération terminée, la fenêtre **Rapprocher avec Copilot** affiche les résultats du processus de mise en correspondance.

1. Passez en revue les correspondances proposées comme décrit dans la section suivante.
---

### <a name="review-save-or-discard-proposed-matches"></a>Examiner, enregistrer ou supprimer les correspondances proposées

Après avoir exécuté Copilot, la fenêtre **Rapprocher avec Copilot** affiche les résultats détaillés, y compris les correspondances proposées. À ce stade, aucune correspondance proposée par Copilot n’a été enregistrée. Par conséquent, vous avez la possibilité d’inspecter les propositions et de les enregistrer ou de les supprimer à votre guise.

![Capture d’écran affiche la fenêtre de rapprochement avec Copilot avec les correspondances proposées](media/bank-reconciliation-copilot-window.png)

La fenêtre **rapprochement avec Copilot** est divisée en deux sections. La section supérieure fournit des détails généraux sur le résultat. La section inférieure **Propositions correspondante** répertorie les correspondances suggérées par Copilot.

Le tableau suivant décrit les champs de la section supérieure.

| Champ | Désignation |
|---|---|
| Correspondance automatique | Le nombre de lignes dans le relevé bancaire mises en correspondance par l’opération de mise en correspondance automatique. Sélectionnez la valeur pour afficher la carte de rapprochement. |
| Mis en correspondance par Copilot | Le nombre de lignes de relevé bancaire pour lesquelles Copilot a proposé des correspondances. Vous pouvez afficher les détails des correspondances dans la section **Propositions de correspondance**. |
| Solde final du relevé | Le solde final indiqué sur le relevé bancaire à rapprocher avec le compte bancaire. |
| Valider si lettré intégralement | Activez cette option valider automatiquement le rapprochement du compte bancaire lorsque toutes les lignes (100 %) correspondent et que vous avez sélectionné **Conserver**. |

Dans la section **Propositions de correspondance** , examinez les correspondances proposées ligne par ligne. Prenez ensuite les mesures appropriées :

- Pour ignorer une seule correspondance proposée, sélectionnez-la dans la liste, puis sélectionnez **Supprimer la ligne**.
- Pour supprimer toutes les correspondance proposées et fermer la fenêtre **Rapprocher avec Copilot**, choisissez le bouton Supprimer (poubelle) ![bouton Supprimer](media/copilot-delete-trash-can.png) à côté du bouton **Conserver** en bas de la fenêtre.
- Pour valider automatiquement le rapprochement complet lorsque vous l’enregistrez, activez l’option **Valider si entièrement appliqué**.
- Pour enregistrer les correspondances actuellement affichées dans la fenêtre **Rapprocher avec Copilot**, sélectionnez **Conserver**.

## <a name="post-unmatched-bank-transaction-amounts-to-suggested-gl-accounts"></a>Valider montants transactions bancaires sans correspondance vers les comptes généraux suggérés

Cette section, vous apprendrez à utiliser Copilot pour valider des montants de lignes de relevé de compte bancaire non rapprochés (comme indiqué dans le camp **Différence**) vers un compte général. Cette tâche ne peut être effectuée qu’à partir d’un rapprochement existant.

1. Accédez à la liste des **Rapprochements de comptes bancaires** et ouvrez le rapprochement existant qui inclut les lignes non rapprochées.

    Cette étape vous donne une vue claire de toutes les lignes de relevé bancaire non rapprochées à transférées vers le compte général.

1. Dans le volet **Lignes de relevé bancaire**, identifiez les lignes de relevé bancaire sans correspondance et sélectionnez une ou plusieurs lignes que vous souhaitez rapprocher.

    Copilot se concentre sur les lignes sélectionnées pour enregistrer les nouveaux paiements sur le compte général.

1. Sélectionnez **Valider différence vers le compte général** pour démarrer le processus.

    ![Capture d’écran qui montre le bouton Valider la différence sur le compte général sur le carte Rapprochement bancaire.](media/bank-reconciliation-transfer-gl-copilot-card.png)

    Copilot commencer à générer des propositions pour le valider les nouveaux paiements.

1. Une fois Copilot a fini de générer des propositions, la fenêtre **Propositions Copilot pour la validation des différences dans les comptes généraux** s’affiche.

    La section **Proposition correspondante** Cette fenêtre affiche les propositions. L’expérience ressemble à l’expérience de réconciliation avec Copilot.

    ![Capture écran affiche les propositions Copilot pour la validation des différences dans la fenêtre les comptes généraux.](media/bank-reconciliation-gl-transfer-proposed-matches.png)

1. Examinez les proposition ligne par ligne pour garantir l’exactitude des paiements à valider.

    - Si vous explorez la proposition en la sélectionnant dans la liste, vous êtes redirigé vers une liste de comptes. De là, vous pouvez Sélectionner un autre compte. Faites ce te type de correction manuelle que lors de l’utilisation du flux **Valider la différence sur le compte général**, et non dans le flux de rapprochement.
    - Si vous sélectionnez **Enregistrer** à côté d’une proposition, vous pouvez ajouter le mappage au **Mappage de texte à compte** page. Ensuite, la prochaine fois que ce texte apparaîtra lors de la mise en correspondance, il sera mappé au compte proposé.

1. Supprimez ou enregistrez les propositions.

    - Pour ignorer une proposition spécifique, sélectionnez-la dans la liste, puis sélectionnez **Supprimer la ligne**. Pour rejeter toutes les propositions et fermer Copilot, sélectionnez le bouton Supprimer (poubelle) ![Bouton Supprimer.](media/copilot-delete-trash-can.png) à côté du bouton **Conserver** en bas de la fenêtre.
    - Si les propositions répondent à vos exigences et que vous souhaitez les enregistrer, sélectionnez **Conserver**.

         Cette étape confirme le transfert des propositions actuellement sélectionnées du grand livre du compte bancaire vers le compte général. Elle valide les nouveaux paiements sur les comptes généraux proposés et applique les lignes correspondantes aux écritures comptables du compte bancaire qui en résultent.

## <a name="next-steps"></a>Étapes suivantes

[Valider votre rapprochement bancaire](bank-how-reconcile-bank-accounts-separately.md#validate-your-bank-reconciliation)

## <a name="see-also"></a>Voir aussi

[Résoudre les problèmes des fonctionnalités de Copilot et d’IA](ai-copilot-troubleshooting.md)  
[FAQ sur l’IA responsable pour l’assistance au rapprochement bancaire](faqs-bank-reconciliation.md)  
[Paramétrage des opérations bancaires](bank-setup-banking.md)  
[Rapprochement des comptes bancaires](bank-how-reconcile-bank-accounts-separately.md)  
[Lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md)
