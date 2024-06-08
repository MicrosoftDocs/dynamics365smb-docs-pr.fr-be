---
title: Réévaluation des soldes comptables
description: Apprenez à réévaluer les soldes des comptes du grand livre avant de produire vos états financiers.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: conceptual
ms.date: 03/14/2024
ms.custom: bap-template
ms.search.form: null
ms.service: dynamics-365-business-central
---

# Réévaluation des soldes comptables

Si vous utilisez des comptes généraux pour enregistrer des postes de bilan en devises étrangères, vous devez réévaluer les soldes des comptes avant de produire des états financiers. Les taux de change changent souvent et la réévaluation contribue à rendre vos états financiers plus précis.

## Configurer réévaluation

Vous configurez chaque compte que vous souhaitez inclure dans les réévaluations sur la page **Fiche de compte général** . Vous pouvez choisir de comptabiliser les ajustements de réévaluation dans les comptes de gains/pertes réalisés ou latents. La comptabilisation des gains et des pertes lors d’un ajustement du taux de change suit la routine de comptabilisation normale. Par exemple, vous le faites pour chaque configuration sur la page **Devises** . Pour en savoir plus sur les ajustements des taux de change, accédez à [Mettre à jour les taux de change](finance-how-update-currencies.md).

Pour minimiser les erreurs, dans le champ **Validation en devise source** , vous pouvez configurer une validation pour les devises dont vous souhaitez autoriser la comptabilisation sur des comptes généraux individuels :

* Toutes les devises (vide)
* Plusieurs devises
* Même devise
* Devise locale

## Exécuter Réévaluation

Pour réévaluer les montants en devise étrangère dans la devise locale pour les soldes des comptes généraux, sur la page **Plan comptable** , utilisez l’option **Devise du grand livre Action de réévaluation** pour démarrer un travail par lots. Le travail par lots crée des écritures d’ajustement dans le journal que vous sélectionnez. Lorsque vous validez les écritures, vous ajustez le solde en devise locale (LCY) du compte. Les soldes des comptes généraux qui s’affichent toujours en LCY reflètent désormais les modifications apportées aux devises dans lesquelles les écritures ont été comptabilisées. Cette réévaluation vous permet de produire un état financier plus précis avec moins d’effort.

Si vous utilisez une devise de reporting supplémentaire (ACY), les écritures de réévaluation du grand livre ont un montant ACY. Le montant correspondant uniquement au montant LCY sur ces écritures, et non au solde ACY sur le compte général. Si vous ajustez les taux ACY après avoir validé les ajustements, exécutez une nouvelle fois l’ajustement du taux de change pour ajuster toutes les écritures du grand livre.

> [!IMPORTANT]
> La réévaluation du compte général peut ne pas répondre à toutes les exigences en matière d’enregistrement des transactions et des actifs nécessitant une réévaluation. Par exemple, pour les instruments financiers, les titres, les actifs loués, ou si vous les utilisez pour des volumes spécifiques ou importants de transactions ou d’actifs. Nous vous recommandons de discuter avec votre auditeur si vous pouvez utiliser cette fonctionnalité et, si oui, comment vous devez l’utiliser. Par exemple, si vous autorisez le mélange des devises pour un compte, ou si vous devez conserver un compte séparé pour chaque actif que vous souhaitez suivre.

> [!NOTE]
> La réévaluation ne permet pas d’appliquer ou d’annuler des écritures, comme c’est le cas avec les écritures comptables des clients et des fournisseurs. Les ajustements se produisent sur une base de solde par devise.

## Réévaluer les comptes par rapport aux ajustements de taux de change des clients et des fournisseurs

La réévaluation simplifie la tâche d’ajustement des soldes des comptes généraux. La fonctionnalité réévalue le solde par devise et par compte général, tout comme vous le faites pour les ajustements des comptes généraux liés aux comptes bancaires. Si vous utilisez un compte général pour suivre plusieurs actifs, envisagez plutôt d’utiliser un compte fournisseur ou client.

> [!NOTE]
> La réévaluation du compte général peut ne pas répondre à toutes les exigences en matière d’enregistrement des transactions et des actifs nécessitant une réévaluation. Par exemple, pour les instruments financiers, les titres, les actifs loués, ou si vous les utilisez pour des volumes spécifiques ou importants de transactions ou d’actifs. Nous vous recommandons de discuter avec votre auditeur si vous pouvez utiliser cette fonctionnalité et, si oui, comment vous devez l’utiliser. Par exemple, si vous autorisez le mélange des devises pour un compte, ou si vous devez conserver un compte séparé pour chaque actif que vous souhaitez suivre.

Les exemples suivants illustrent la différence entre l’utilisation d’un compte général et l’utilisation d’un compte fournisseur pour suivre le solde de deux actifs monétaires qui utilisent une devise étrangère.

**Utilisez un compte général** Si vous utilisez un compte général pour suivre soit plusieurs actifs (par exemple, des prêts ou des immobilisations) dans la même devise, soit des transactions partielles individuelles pour le même actif. mais toujours dans la même devise, la réévaluation du GL fait une écriture par réévaluation pour la devise. Cela signifie que vous ne pouvez pas suivre les ajustements liés aux actifs individuels ou aux transactions individuelles pour le même actif.

**Utilisez un compte fournisseur** Si vous configurez plusieurs actifs en tant que fournisseurs et que vous y imputez des transactions, dans la même devise ou dans des devises différentes, vous obtiendrez un ajustement par devise et par fournisseur. Ou, si vous allumez le **Publication par entrée** activer le **Ajuster le taux de change** entrée de la file d’attente des travaux, vous obtiendrez une écriture d’ajustement pour chaque écriture comptable du fournisseur distincte.

Cette différence est importante lorsque vous évaluez si la réévaluation du grand livre est la fonctionnalité adaptée à vos besoins de reporting.

> [!TIP]
> Nous vous recommandons de demander à votre comptable ou auditeur quel type de compte convient le mieux à votre entreprise. Il pourrait également y avoir une application pour [!INCLUDE [prod_short](includes/prod_short.md)] sur [AppSource](https://appsource.microsoft.com/en-us/marketplace/apps?page=1&product=dynamics-365-business-central) c’est parfait pour vos scénarios commerciaux.

## Voir aussi

[Examiner les montants dans la comptabilité](finance-review-accounts.md)  
[Comprendre la comptabilité et le plan comptable](finance-general-ledger.md)  
