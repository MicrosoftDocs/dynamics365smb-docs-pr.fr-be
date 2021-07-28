---
title: Exporter des fichiers de paiement dans la version belge
description: Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier de paiement dans la version belge de Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 73c142f460f208a6350e48bba54535fd2d77c7d6
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 07/08/2021
ms.locfileid: "6435206"
---
# <a name="export-payment-files-in-the-belgian-version"></a>Exporter des fichiers de paiement dans la version belge

Après avoir effectué une impression test et corrigé toutes les erreurs, vous pouvez exporter les lignes feuille paiement dans un fichier de paiement.  

Un fichier de paiement contient les paiements nationaux, internationaux, SEPA ou SEPA hors euro. Le fichier peut être envoyé vers une banque par voie électronique. Vous ne pouvez créer qu'un seul fichier pour chaque date comptabilisation et chaque code devise. Lorsque vous exportez les paiements dans un fichier, une note associée est imprimée, qui peut également être envoyée à la banque.  

Dans la feuille paiement, le champ **Statut** sur les lignes exportées est défini sur **Validé**.  

## <a name="to-print-a-payment-file"></a>Pour imprimer un fichier de paiement  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuille paiement**, puis choisissez le lien permettant d'ouvrir la page **Modèles feuille paiement EB**.  
2. Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.  
3. Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.  

    Les protocoles d'exportation contrôlent le fichier de paiement généré dans la feuille paiement. Vous pouvez combiner plusieurs formats d'exportation dans un même traitement par lots, par exemple national, international, SEPA ou une combinaison de ceux-ci. Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un seul format d'exportation ou protocole d'exportation.  

    > [!NOTE]
    > En définissant le protocole d'exportation, vous définissez également le type de validation qui est exécuté dans la feuille paiement.
4. Entrez les informations ligne feuille paiement, puis choisissez l'action **Vérifier lignes paiement**.

    La page **Exporter/Vérifier les journaux des erreurs** affiche les erreurs éventuelles. S'il existe des erreurs, vous devez les corriger avant de continuer.

5. S'il n'existe aucune erreur, choisissez l'action **Exporter lignes paiement**.  

    L'état que vous avez spécifié dans le protocole d'exportation approprié traite les lignes paiement et génère le fichier.  

## <a name="see-also"></a>Voir aussi

[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)  
[Paiements électroniques belges](belgian-electronic-payments.md)  
[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)  
[Proposer paiements fournisseur](../../payables-how-suggest-vendor-payments.md)  
[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md)  
[Tester les paiements électroniques](how-to-test-electronic-payments.md)  
