---
title: Lettrage et délettrage des écritures comptables
description: Le lettrage des écritures comptables temporaires permet aux sociétés d'utiliser des comptes temporaires et de transfert dans la comptabilité. Les comptes temporaires et de transfert sont utilisés pour stocker les écritures comptables temporaires qui sont en attente d'un traitement ultérieur dans la comptabilité.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: f21b23039c57a29d06a260b0abe74d8b57d00f71
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2019
ms.locfileid: "911689"
---
# <a name="apply-and-unapply-general-ledger-entries"></a>Lettrer et délettrer les écritures comptables
Le lettrage des écritures comptables temporaires permet aux sociétés d'utiliser des comptes temporaires et de transfert dans la comptabilité. Les comptes temporaires et de transfert sont utilisés pour stocker les écritures comptables temporaires qui sont en attente d'un traitement ultérieur dans la comptabilité.  

 Vous pouvez utiliser les comptes temporaires pour :  

- Les transferts d'argent d'un compte bancaire à un autre.  
- Les transferts de transaction financière d'un système à un autre où une partie des informations réside temporairement dans le système d'origine.  
- Les transactions pour lesquelles vous avez émis une facture vente à un client mais vous n'avez pas encore reçu la facture achat correspondante du fournisseur.  

 Lorsque les écritures comptables ont été traitées, vous pouvez utiliser la fonction Lettrer écritures pour mettre à jour les écritures comptables validées et le type de compte de validation.  

 Vous pouvez délettrer les écritures comptables lettrées puis ouvrir les écritures clôturées pour apporter des modifications.  

## <a name="to-apply-general-ledger-entries"></a>Pour lettrer des écritures comptables  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Hist. trans. comptabilité**, puis sélectionnez le lien connexe.  
2.  Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.  
3.  Dans la page **Écritures comptables**, choisissez l'action **Lettrer écritures**.  

    Toutes les écritures comptables ouvertes pour le compte général sont affichées sur la page **Lettrer écritures comptables**.  

    > [!NOTE]  
    >  Par défaut, le champ **Inclure écritures** est défini sur **Ouvert**. Vous pouvez modifier la valeur du champ **Inclure écritures** sur **Tous** ou **Clôturé**. Vous pouvez lettrer uniquement les écritures comptables qui ont le statut **Ouvert**.  

4.  Sélectionnez l'écriture comptable appropriée, puis, sous l'onglet **Naviguer**, dans le groupe **Lettrage**, choisissez **Lettrer**.  

    Le champ **ID lettrage** est mis à jour avec l'ID utilisateur. Le montant restant est affiché dans le champ **Solde** de la page **Lettrer écritures comptables**.  

5.  Sélectionnez **Valider le lettrage**.  

    Vous pouvez valider le lettrage même si le solde est égal à 0. Une fois validé, le champ **Montant restant** est affecté comme suit :  

    - Si le **Solde** est égal à 0, le champ **Montant restant** de toutes les écritures comptables est défini sur 0.  

    - Si le **Solde** n'est pas égal à 0, le montant du champ **Solde** est transféré vers le champ **Montant restant** pour l'écriture comptable qui a été sélectionnée lors de la validation du lettrage.  

    - Pour toutes les autres écritures comptables, le champ **Montant restant** est défini sur 0 et les champs **Ouvert**, **N° séquence lettrage final**, **Montant lettrage final** et **Date de clôture** sont mis à jour.  

    > [!NOTE]  
    >  Une fois validées, les écritures comptables qui mettent à jour le champ **ID lettrage** sont supprimées.  

6.  Choisissez le bouton **OK**.  

## <a name="to-view-the-applied-general-ledger-entries"></a>Pour afficher les écritures comptables lettrées  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Hist. trans. comptabilité**, puis sélectionnez le lien connexe.  
2.  Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.  
3.  Sélectionnez l'écriture comptable appropriée, puis choisissez l'action **Écritures lettrées**.  

    Vous pouvez afficher toutes les écritures comptables lettrées.  

4.  Choisissez le bouton **OK**.  

## <a name="to-unapply-general-ledger-entries"></a>Pour délettrer des écritures comptables  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Hist. trans. comptabilité**, puis sélectionnez le lien connexe.  
2.  Sélectionnez un historique des transactions comptabilité, puis choisissez l'action **Comptabilité**.  
3.  Sélectionnez l'écriture comptable que vous souhaitez délettrer, puis choisissez l'action **Annuler le lettrage**.  

    Les écritures comptables lettrées sont delettrées.  

    > [!NOTE]  
    >  Si une écriture est lettrée par plusieurs écritures lettrage, vous devez commencer par délettrer la dernière écriture lettrage. Par défaut, la dernière écriture s'affiche.  

4.  Choisissez le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale, Belgique](belgium-local-functionality.md)
