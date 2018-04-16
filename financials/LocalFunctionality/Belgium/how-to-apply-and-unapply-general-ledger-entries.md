---
title: "Comment lettrer et délettrer des écritures comptables"
description: "Le lettrage d'écritures comptables permet aux sociétés de travailler avec des comptes temporaires et de transfert dans la comptabilité. Les comptes temporaires et de transfert sont utilisés pour répertorier les écritures comptables en attente de traitement dans la comptabilité."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: ccd55fda375ee7df5fa4ed6e5b0353cde0211df2
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="apply-and-unapply-general-ledger-entries"></a>Lettrer et délettrer des écritures comptables
Le lettrage d'écritures comptables permet aux sociétés de travailler avec des comptes temporaires et de transfert dans la comptabilité. Les comptes temporaires et de transfert sont utilisés pour répertorier les écritures comptables en attente de traitement dans la comptabilité.  

 Vous pouvez utiliser les comptes temporaires pour :  

- Les transferts d'argent d'un compte bancaire à l'autre.  
- Les transferts de transactions financières d'un système à l'autre, dans lesquels une partie des informations est temporairement hébergée dans le système d'origine.  
- Les transactions pour lesquelles vous avez émis une facture vente à un client, mais n'avez pas encore reçu la facture achat correspondante du fournisseur.  

  Lorsque les écritures comptables ont été traitées, vous pouvez utiliser la fonction de lettrage des écritures pour mettre à jour les écritures comptables validées et le type de compte de validation.  

  Vous pouvez délettrer les écritures comptables lettrées, puis ouvrir les écritures clôturées pour effectuer les modifications.  

## <a name="to-apply-general-ledger-entries"></a>Pour lettrer des écritures comptables  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Historiques des transactions comptabilité**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.  
3.  Dans la fenêtre **Écritures comptables**, choisissez l'action **Lettrer écritures**.  

    Toutes les écritures comptables ouvertes pour le compte général s'affichent dans la fenêtre **Lettrer écritures comptables**.  

    > [!NOTE]  
    >  Par défaut, le champ **Inclure écritures** est défini sur **Ouvertes**. Vous pouvez modifier la valeur du champ **Inclure écritures** et la définir sur **Toutes** ou **Clôturées**. Vous pouvez uniquement lettrer les écritures comptables qui sont **Ouvertes**.  

4.  Sélectionnez l'écriture comptable concernée, puis, dans l'onglet **Naviguer**, dans le groupe **Lettrage**, sélectionnez **Définir ID lettrage**.  

    Le champ **Définir ID lettrage** est mis à jour avec le code utilisateur. Le montant restant s'affiche dans le champ **Solde** dans la fenêtre **Lettrer écritures comptables**.  

5.  Choisissez **Valider le lettrage**.  

    Vous pouvez valider le lettrage même si le solde est nul. Après la validation, le champ **Montant restant** est affecté comme suit :  

    - Si le **Solde** est nul, le champ **Montant restant** de toutes les écritures comptables est défini sur 0.  

    - Si le **Solde** n'est pas nul, le montant figurant dans le champ **Solde** est transféré au champ **Montant restant** pour l'écriture comptable qui était sélectionnée lorsque vous avez validé le lettrage.  

    - Pour toutes les autres écritures comptables, le champ **Montant restant** est nul, et les champs **Ouvertes**, **N° séquence lettrage final**, **Montant lettrage final** et **Date de clôture** sont mis à jour.  

    > [!NOTE]  
    >  Lors de la validation, les écritures comptables qui mettent à jour le champ **ID lettrage** sont supprimées.  

6.  Cliquez sur le bouton **OK**.  

## <a name="to-view-the-applied-general-ledger-entries"></a>Pour afficher les écritures comptables lettrées  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Historiques des transactions comptabilité**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.  
3.  Sélectionnez l'écriture comptabilité pertinente, puis choisissez l'action **Écritures lettrées**.  

    Vous pouvez afficher toutes les écritures comptables lettrées.  

4.  Cliquez sur le bouton **OK**.  

## <a name="to-unapply-general-ledger-entries"></a>Pour délettrer des écritures comptables  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Historiques des transactions comptabilité**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.  
3.  Sélectionnez l'écriture comptable que vous souhaitez délettrer, puis choisissez l'action **Annuler le lettrage**.  

    Les écritures comptables lettrées sont délettrées.  

    > [!NOTE]  
    >  Si une écriture est lettrée à une ou plusieurs écritures de lettrage, vous devez délettrer la dernière écriture de lettrage en premier. Par défaut, la dernière écriture s'affiche.  

4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)

