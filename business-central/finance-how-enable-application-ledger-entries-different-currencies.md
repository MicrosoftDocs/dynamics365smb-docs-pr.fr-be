---
title: Lettrer des écritures dans des devises différentes
description: Vous pouvez lettrer des écritures comptables dans différentes devises si vous effectuez une vente à un client dans une devise et recevez le règlement dans une autre devise.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'multiple currencies, payment, reconcile'
ms.search.form: '148, 460, 25'
ms.date: 04/01/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a>Activer le lettrage d'écritures comptables client en devises différentes

Si vous achetez des produits auprès d'un fournisseur dans une devise et que vous payez ces produits dans une autre devise, vous pouvez lettrer le paiement avec l'achat.

De même, si vous effectuez une vente à un client dans une devise et recevez le règlement dans une autre devise, vous pouvez lettrer le règlement avec la facture vente.

La procédure suivante indique comment configurer cela pour les écritures comptables fournisseur sur la page **Paramètres achats**. La configuration est semblable à celle des écritures comptables client sur la page **Paramètres ventes**.

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a>Pour activer le lettrage d'écritures comptables fournisseur en devises différentes

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Paramètres achats**, puis choisissez le lien associé.
2. Dans le champ **Lettrage entre devises**, sélectionnez l'une des options suivantes.

| Option | Description |
| --- | --- |
| Aucun |Le lettrage entre devises n'est pas autorisé. |
| Devises U.M.E. |Le lettrage entre devises UME est autorisé. |
| Tous |Lettrage autorisé entre toutes les devises. |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a>Pour configurer des comptes généraux afin d'autoriser les différences d'arrondi des devises

Si vous lettrez des écritures dans différentes devises, vous devez configurer les comptes généraux sur lesquels valider les différences d'arrondi.  

> [!NOTE]  
> Vous devez configurer les comptes généraux avant de terminer la tâche. Pour plus d'informations, voir [Description des écritures comptables et du plan comptable](finance-general-ledger.md).

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Groupes compta. client**, puis choisissez le lien associé.  
2. Dans les champs **Cpte arr. lettr. dev. débit** et **Cpte arr. lettr. dev. crédit**, saisissez les comptes généraux correspondants pour valider les différences d'arrondi.  
3. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Groupes compta. fournisseur**, puis choisissez le lien associé.  
4. Dans les champs **Cpte arr. lettr. dev. débit** et **Cpte arr. lettr. dev. crédit**, saisissez les comptes généraux correspondants pour valider les différences d'arrondi.  

## <a name="see-also"></a>Voir aussi

[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Gestion des comptes client](receivables-manage-receivables.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
