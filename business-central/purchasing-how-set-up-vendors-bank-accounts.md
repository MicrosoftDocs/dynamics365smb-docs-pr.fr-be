---
title: Configurer des comptes bancaires fournisseur
description: Découvrez comment associer des comptes bancaires aux fiches fournisseur dans Business Central, y compris les informations de contact, les codes SWIFT et IBAN.
author: rubenseishima
ms.service: dynamics365-business-central
ms.topic: article
ms.date: 07/04/2022
ms.author: a-reishima
ms.openlocfilehash: 1839f54de2382ad5b7d8b6b936181e105a56e06b
ms.sourcegitcommit: 5560a49ca4ce85fa12e50ed9e14de6d5cba5f5c3
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 07/13/2022
ms.locfileid: "9144437"
---
# <a name="set-up-vendor-bank-accounts"></a>Configurer des comptes bancaires fournisseur

Tout comme vous pouvez utiliser des informations de compte bancaire sur [!INCLUDE [prod_short](includes/prod_short.md)] pour suivre les transactions bancaires de votre entreprise, vous pouvez également définir les coordonnées bancaires des fournisseurs. Les données de compte bancaire du fournisseur peuvent simplifier les paiements aux fournisseurs lorsqu'elles sont combinées avec l'extension [AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md) ou la fonctionnalité [Exporter des paiements vers un fichier bancaire](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md), par exemple.

## <a name="add-or-edit-a-vendor-bank-account"></a>Ajouter ou modifier un compte bancaire fournisseur

[!INCLUDE [purchase-vendor-bank-account](includes/purchase-vendor-bank-account.md)]

> [!TIP]
> Vous pouvez définir des comptes bancaires fournisseur supplémentaires sur la page **Liste comptes bancaires fourn.**.

## <a name="set-up-a-preferred-vendor-bank-account"></a>Configurer un compte bancaire fournisseur favori

Si un fournisseur possède un ou plusieurs comptes bancaires et que vous souhaitez définir une option préférée pour les lignes du journal des paiements, procédez comme suit :

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche 1.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Fournisseurs**, puis choisissez le lien associé.
2. Ouvrez la fiche pour le fournisseur.
3. Sur le raccourci **Paiements**, choisissez le compte bancaire fournisseur par défaut dans le champ **Code de compte bancaire préféré**.

## <a name="see-related-training-at-microsoft-learn"></a>Voir la formation associée sur [Microsoft Learn](/learn/modules/cash-management-dynamics-365-business-central/)

## <a name="see-also"></a>Voir aussi

[Définition des achats](purchasing-setup-purchasing.md)  
[Enregistrer un nouveau fournisseur](purchasing-how-register-new-vendors.md)  
[Configurer des comptes bancaires](bank-how-setup-bank-accounts.md)  
[Utiliser l'extension AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md)  
[Configurer le service Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]