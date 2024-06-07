---
title: Exporter des fichiers de paiement dans la version belge
description: 'Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement dans la version belge de Business Central.'
author: brentholtorf
ms.topic: conceptual
ms.search.form: 2000001
ms.date: 01/10/2022
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Exporter des fichiers de paiement dans la version belge

Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez exporter les lignes feuille paiement dans un fichier de paiement.  

Un fichier de paiement contient les paiements nationaux, internationaux, SEPA ou SEPA hors euro. Le fichier peut être envoyé vers une banque par voie électronique. Vous ne pouvez créer qu'un seul fichier pour chaque date comptabilisation et chaque code devise. Lorsque vous exportez les paiements dans un fichier, une note associée est imprimée, qui peut également être envoyée à la banque.  

Dans la feuille paiement, le champ **Statut** sur les lignes exportées est défini sur **Validé**.  

## Pour imprimer un fichier de paiement  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez *Feuille paiement*, puis choisissez le lien permettant d'ouvrir la page **Modèles feuille paiement EB**.  
2. Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.  
3. Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.  

    Les protocoles d'exportation contrôlent le fichier de paiement généré dans la feuille paiement. Vous pouvez combiner plusieurs formats d'exportation dans un même traitement par lots, par exemple national, international, SEPA ou une combinaison de ceux-ci. Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un seul format d'exportation ou protocole d'exportation.  

    > [!NOTE]
    > En définissant le protocole d'exportation, vous définissez également le type de validation qui est exécuté dans la feuille paiement.
4. Entrez les informations de la ligne feuille paiement.

    1. Choisissez l'action **Proposer paiements fournisseur**.
    2. Dans la page **Proposer paiements fournisseur**, définissez les options et filtres pertinents.

        Ce traitement par lots traite les écritures comptables fournisseur ouvertes et crée une suggestion de paiement sous forme de lignes dans une feuille paiement. Les écritures comptables fournisseur ouvertes résultent de la validation des factures et des factures d'intérêts.

        Seules les écritures comptables des fournisseurs pour lesquels le champ **Proposer paiements** est sélectionné sur leur fiche **Fournisseur** sont incluses dans le traitement par lots. Les propositions sont enregistrées dans une feuille paiement. Vous devez spécifier une dernière date d'échéance qui sera utilisée dans le traitement par lots.

        En outre, seules les écritures fournisseur qui ne sont pas marquées comme **En attente** dans la page **Écritures comptables fournisseur** sont incluses dans le traitement par lots. Vous pouvez également exécuter le traitement par lots de manière à y inclure également les paiements pour lesquels vous pouvez obtenir une remise.

        Lorsque vous entrez un montant disponible, les fournisseurs seront classés par **Priorité**.

        Vous pouvez définir les éléments qui sont inclus dans l'état en définissant des filtres. Pour définir des champs supplémentaires sous l'onglet, choisissez le champ. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]
    3. Supprimez ou modifiez les lignes en fonction des besoins.
    4. Si aucun compte bancaire n'est indiqué sur le modèle feuille paiement, indiquez un compte bancaire avec lequel payer sur chaque ligne.
5. Choisissez l'action **Vérifier lignes paiement**.

    La page **Exporter/Vérifier les journaux des erreurs** affiche les erreurs éventuelles. S'il existe des erreurs, vous devez les corriger avant de continuer.

6. S'il n'existe aucune erreur, choisissez l'action **Exporter lignes paiement**.  

    L'état que vous avez spécifié dans le protocole d'exportation approprié traite les lignes paiement et génère le fichier.  

## Voir aussi

[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)  
[Paiements électroniques belges](belgian-electronic-payments.md)  
[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)  
[Proposer paiements fournisseur](../../payables-how-suggest-vendor-payments.md)  
[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md)  
[Tester les paiements électroniques](how-to-test-electronic-payments.md)  
