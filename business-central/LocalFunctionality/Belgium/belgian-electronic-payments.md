---
title: Paiements électroniques, Belgique
description: Dans le module bancaire électronique de la version belge de Business Central, vous pouvez effectuer des paiements électroniques nationaux, internationaux, SEPA et SEPA hors euro.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 061b62e50a327edc31f93672837c167927770236
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773300"
---
# <a name="belgian-electronic-payments"></a>Paiements électroniques, Belgique
Dans le module bancaire électronique de [!INCLUDE[prod_short](../../includes/prod_short.md)], vous pouvez effectuer des paiements électroniques nationaux, internationaux, SEPA et SEPA hors euro.  

|Paiement électronique|Désignation|  
|------------------------|---------------------------------------|  
|National|Ces paiements sont en devise société (DS) et sont traités par une institution financière locale pour les bénéficiaires qui ont des comptes auprès d'une institution financière locale. La validité des numéros de compte bancaire est vérifiée par [!INCLUDE[prod_short](../../includes/prod_short.md)].|  
|International|Ces paiements sont en devises étrangères ou en devise société (DS) et sont traités par une institution financière locale pour les bénéficiaires qui ont des comptes auprès d'institutions financières étrangères. La validité des numéros de compte bancaire n'est pas vérifiée par [!INCLUDE[prod_short](../../includes/prod_short.md)].|  
|SEPA|Ces paiements sont en euros et sont traités dans les pays/régions qui acceptent les paiements SEPA. La validité des numéros de compte bancaire est vérifiée par [!INCLUDE[prod_short](../../includes/prod_short.md)].|  
|SEPA hors euro|Ces paiements sont dans une devise autre que l'euro et sont traités dans les pays/régions en dehors de l'Association économique européenne (AEE). La validité des numéros de compte bancaire est vérifiée par [!INCLUDE[prod_short](../../includes/prod_short.md)].|  

 Dans le système bancaire électronique, étant donné que la norme pour les paiements électroniques diffère selon les pays/régions, les paiements électroniques créés dans [!INCLUDE[prod_short](../../includes/prod_short.md)] ne peuvent être traités que par des institutions financières en Belgique. Pour les paiements internationaux, les institutions financières locales devront ensuite traiter le paiement auprès des institutions étrangères.  

> [!NOTE]  
>  Les avoirs ne peuvent pas être traités séparément, car les paiements ne doivent pas avoir un solde négatif. Pour traiter un avoir, celui-ci doit être ajouté à une ou plusieurs factures en totalisant les paiements.  

Avant de pouvoir effectuer des paiements électroniques, vous devez paramétrer le système bancaire électronique dans [!INCLUDE[prod_short](../../includes/prod_short.md)].  

## <a name="correcting-payment-lines"></a>Correction des lignes de paiement  
Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes de paiement électronique. Vous pouvez corriger les lignes de paiement comme suit :  

|Correction|Désignation|  
|----------------|---------------------------------------|  
|Ajouter une ligne feuille paiement|Si la feuille paiement contient déjà plusieurs lignes et que vous souhaitez ajouter une ligne supplémentaire, vous pouvez entrer la ligne feuille manuellement. Par exemple, si vous souhaitez rembourser un avoir à un client. Ces types de paiements client ne sont pas proposés automatiquement par le traitement par lots **Proposer paiements fournisseur**.|  
|Modifier une ligne feuille paiement|Si vous n'avez pas affecté un compte bancaire à la feuille paiement ou si vous n'avez pas spécifié de compte bancaire préféré sur la fiche fournisseur, vous devrez entrer manuellement ces informations sur chaque ligne feuille avant de valider la feuille. Si vous spécifiez un compte bancaire pour un fournisseur, le compte bancaire est copié sur toutes les lignes feuille paiement de ce fournisseur. Pour plus d'informations, voir [Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md).|  
|Supprimer une ligne feuille paiement|Le traitement par lots **Proposer paiements fournisseur** crée des propositions de paiement pour tous les fournisseurs répondant aux critères spécifiés. Si vous souhaitez empêcher le paiement pour une écriture comptable fournisseur ou un fournisseur spécifique, vous pouvez supprimer les lignes feuille correspondantes.|  

Pour plus d'informations, voir [Gérer les lignes de paiement électronique](how-to-manage-electronic-payment-lines.md).  

## <a name="see-also"></a>Voir aussi

[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)  
[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)  
[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)  
[Proposer paiements fournisseur](../../payables-how-suggest-vendor-payments.md)  
[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md)  
[Tester les paiements électroniques](how-to-test-electronic-payments.md)  
[Imprimer les fichiers de paiement](how-to-print-payment-files.md)  
