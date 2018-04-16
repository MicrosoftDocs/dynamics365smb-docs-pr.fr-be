---
title: "Comment tester les paiements électroniques"
description: "Après avoir configuré la banque électronique et généré des propositions de paiement, vous pouvez tester les lignes feuille paiement pour repérer les éventuelles erreurs avant de valider les lignes."
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
ms.openlocfilehash: 6d3db364851f9129ed38190132a9f7ff33a7e738
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="test-electronic-payments"></a>Tester les paiements électroniques
> [!Note]
> [!INCLUDE [onprem_only](../../includes/onprem_only_md.md)]

Après avoir créé des transactions bancaires électroniques et des propositions de paiement générées, vous pouvez tester les lignes feuille paiement pour les erreurs avant de les valider.  

Les informations validées incluent notamment :  

- Les numéros de comptes bancaires sont valides.  
- Il y a des lignes paiement positives.  
- Si les paiements nationaux et internationaux sont effectués depuis un seul compte bancaire.  
- Si un seul compte bancaire peut être utilisé pour Isabel.  
- Si les lignes paiement sont en Euro pour SEPA.  
- Si une souche de numéros a été définie pour SEPA.  

Vous pouvez consulter les éventuelles erreurs dans la fenêtre **Exporter les journaux d'erreur de chèque**.  

> [!IMPORTANT]  
>  Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.  

## <a name="to-test-payment-journal-lines"></a>Pour tester les lignes feuille paiement  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles paiement**, puis sélectionnez le lien correspondant.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille concernée.  
3.  Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.  
4.  Entrez les informations ligne feuille paiement, puis choisissez l'action **Vérifier les lignes de paiement** pour valider les lignes feuille paiement. La validation effectuée sur les lignes feuille dépend du type de contrôle indiqué dans la fenêtre **Protocoles d'exportation**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des propositions de paiement](how-to-generate-payment-suggestions.md)   
 [Imprimer des fichiers de paiement](how-to-print-payment-files.md)

