---
title: "Paiements électroniques belges"
description: "Dans le module de banque électronique, dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez effectuer des paiements électroniques nationaux, internationaux, SEPA ou SEPA non libellés en Euro."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 3da762ff74d8065e1c2af18ccfa4a8390092c316
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="belgian-electronic-payments"></a>Paiements électroniques belges
Dans le module de banque électronique, dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez effectuer des paiements électroniques nationaux, internationaux, SEPA ou SEPA non libellés en Euro.  

|Paiement électronique|Description|  
|------------------------|---------------------------------------|  
|FRANCE|Ces paiements sont dans la devise locale (DS) et sont traités par une institution financière locale pour les bénéficiaires qui ont des comptes auprès d'une institution financière locale. La validité des numéros de comptes bancaires sera vérifiée par [!INCLUDE[d365fin](../../includes/d365fin_md.md)].|  
|International|Ces paiements sont soit dans des devises locales, soit en DS, et sont traités par une institution financière locale pour les bénéficiaires qui ont des comptes auprès d'institutions financières étrangères. La validité des numéros de comptes bancaires ne sera pas vérifiée par [!INCLUDE[d365fin](../../includes/d365fin_md.md)].|  
|SEPA|Ces paiements sont en euros et sont traités dans des pays/régions qui acceptent les paiements SEPA. La validité des numéros de comptes bancaires sera vérifiée par [!INCLUDE[d365fin](../../includes/d365fin_md.md)].|  
|SEPA non libellé en Euro|Ces paiements sont dans une autre devise que l'euro et ont été effectués vers un pays/une région qui ne fait pas partie de la European Economic Association (EEA). La validité des numéros de comptes bancaires sera vérifiée par [!INCLUDE[d365fin](../../includes/d365fin_md.md)].|  

 Dans la banque électronique, comme la norme pour les paiements électroniques varie d'un pays/d'une région à l'autre, les paiements électroniques créés dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)] peuvent uniquement être traités par des institutions financières en Belgique. Pour les paiements internationaux, les institutions financières locales devront alors traiter le paiement avec les institutions étrangères.  

> [!NOTE]  
>  Les avoirs ne peuvent pas être traités séparément, car les paiements ne peuvent pas avoir un solde négatif. Pour pouvoir être traité, un avoir doit être ajouté à une ou plusieurs factures en totalisant les paiements.  

Avant de pouvoir effectuer des paiements électroniques, vous devez configurer la banque électronique dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)].  

## <a name="correcting-payment-lines"></a>Correction des lignes paiement  
Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes paiement électronique. Vous pouvez corriger les lignes paiement de l'une des manières suivantes.  

|Correction|Description|  
|----------------|---------------------------------------|  
|Ajouter une ligne feuille paiement|Si la feuille paiement contient déjà de nombreuses lignes et que vous souhaitez en ajouter une, vous pouvez l'entrer manuellement. Par exemple, si vous souhaitez rembourser un avoir à un client. Ces types de paiements client ne sont pas automatiquement proposés par le traitement par lots **Proposer paiements fournisseur**.|  
|Modifier une ligne feuille paiement|Si vous n'avez pas attribué un compte bancaire à la feuille paiement ou si vous n'avez pas spécifié de compte bancaire préféré sur la fiche Fournisseur, vous devrez entrer manuellement ces informations sur chaque ligne feuille avant de valider la feuille. Si vous spécifiez un compte bancaire pour un fournisseur, le compte bancaire sera copié dans toutes les lignes feuille paiement pour ce fournisseur. Pour plus d'informations, reportez-vous à [Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md).|  
|Supprimer une ligne feuille paiement|Le traitement par lots **Proposer paiements fournisseur** crée des propositions de paiement pour tous les fournisseurs qui correspondent aux critères spécifiés. Si vous souhaitez empêcher le paiement pour une écriture comptable fournisseur ou un fournisseur spécifique, vous pouvez supprimer les lignes journal correspondantes.|  

Pour plus d'informations, voir [Gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md).  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)  
[Banque électronique belge](belgian-electronic-banking.md)   
[Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
[Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
[Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
[Générer des propositions de paiement](how-to-generate-payment-suggestions.md)   
[Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
[Tester les paiements électroniques](how-to-test-electronic-payments.md)   
[Gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md)   
[Imprimer des fichiers de paiement](how-to-print-payment-files.md)

