---
title: Valider des documents achat
description: Découvrez les différentes manières de valider les documents achat et de mettre à jour les documents validés.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.search.form: ''
ms.date: 08/08/2022
ms.author: edupont
ms.openlocfilehash: 1bae22c83f1e7138fbfe16bb39aea3ad9d65d788
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 09/19/2022
ms.locfileid: "9531013"
---
# <a name="posting-purchases"></a>Validation des achats

Sur un document achat, vous pouvez faire votre choix parmi les actions de validation suivantes :

* **Valider**
* **Aperçu compta.**
* **Valider et Imprimer**
* **Impression test**
* **Valider par lot**

Lorsqu’un document achat est validé, le compte du fournisseur, les écritures comptables, les écritures comptables article et les écritures comptables ressource sont mis à jour.

Pour chaque document achat, une écriture achat est créée dans la table **Ecriture comptable**. Une écriture est également créée dans le compte fournisseur de la table **Ecriture fournisseur** et une autre dans le compte fournisseur approprié. De plus, la validation de l’achat peut entraîner la création d’une écriture TVA et d’une écriture comptable pour le montant de la remise. La validation d’une écriture pour la remise dépend de la valeur du champ **Comptabilisation remises** de la table **Paramètres achats**.

Pour chaque ligne achat, les écritures suivantes sont créées :

* la table **Écriture comptable article** si la ligne achat est de type **Article**.
* la table **Écriture comptable** si la ligne achat est de type **Compte général**.
* la table **Écriture comptable ressource** si la ligne achat est de type **Ressource**.

En outre, les documents achat sont toujours enregistrés dans les tables **En-tête réception achat** et **En-tête facture achat**.

Avant de commencer à valider, vous pouvez effectuer une impression test qui contient toutes les informations de la commande achat et indique les erreurs afférentes. Pour imprimer l’état, sélectionnez **Validation**, puis **Impression test**.

> [!IMPORTANT]  
> Lorsque vous validez une commande achat pour des articles, vous pouvez créer une réception et une facture. Celles-ci peuvent être faites simultanément ou séparément. Vous pouvez également créer une réception partielle et une facture partielle en renseignant les champs **Qté à recevoir** et **Qté à facturer** sur chaque ligne commande achat avant la validation. Notez que vous ne pouvez pas créer de facture d’achat à partir d’une commande pour des produits ou des services qui n’ont pas été reçus. C'est-à-dire que, avant de pouvoir facturer, vous devez avoir validé une réception, ou vous devez choisir de réceptionner et de facturer en même temps.
>
> Pour valider une facture d’achat sans enregistrer de réception d’achat dans [!INCLUDE[prod_short](includes/prod_short.md)], créez le document sur la page **Factures d’achat**. En savoir plus, [Enregistrer les achats avec les factures achat](purchasing-how-record-purchases.md).

Vous pouvez soit valider, soit valider et imprimer. Si vous choisissez de valider et d’imprimer, un rapport est imprimé lorsque la commande est validée. Vous pouvez aussi choisir l’action **Valider par lot**, qui vous permet de valider plusieurs commandes en même temps. En savoir plus, [Valider plusieurs documents en même temps](ui-batch-posting.md).

## <a name="viewing-ledger-entries"></a>Affichage des écritures comptables

Lorsque la validation est terminée, les lignes achat validées sont supprimées de la commande. Un message vous indique lorsque la validation est terminée. Vous pouvez ensuite afficher les écritures validées dans les diverses pages qui contiennent les écritures validées, comme les pages **Écritures comptables fournisseur**, **Écritures comptables**, **Écritures comptables article**, **Écritures comptables ressource**, **Réceptions achat** et **Factures achat enregistrées**.

Dans la plupart des cas, vous pouvez ouvrir des écritures comptables à partir de la fiche ou du document concerné. Par exemple, sur la page **Fiche fournisseur**, sélectionnez l’action **Écritures**.

## <a name="editing-ledger-entries"></a>Modification des écritures comptables

Vous pouvez modifier certains champs dans les documents d’achat validés, tels que le champ **Référence de paiement**. En savoir plus sur [Modifier les documents validés](across-edit-posted-document.md). Pour les champs plus critiques qui concernent la piste d’audit, vous devez inverser ou annuler la validation. En savoir plus, [Inverser des validations feuille et annuler les réceptions/envois](finance-how-reverse-journal-posting.md).

## <a name="see-related-microsoft-training"></a>Voir la [formation Microsoft](/training/modules/receive-invoice-dynamics-d365-business-central/index) associée.

## <a name="see-also"></a>Voir aussi

[Valider les documents validés](across-edit-posted-document.md)  
[Valider plusieurs documents en même temps](ui-batch-posting.md)  
[Achats](purchasing-manage-purchasing.md)  
[Validation des documents et des feuilles](ui-post-documents-journals.md)  
[Corriger ou annuler des factures achat impayées](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[Recherche de pages et d’informations avec Tell Me](ui-search.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
