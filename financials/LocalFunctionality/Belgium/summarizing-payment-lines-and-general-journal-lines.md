---
title: "Récapitulatif des lignes paiements et des lignes feuille comptabilité"
description: "Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)] gère plusieurs types de transactions de la même manière."
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
ms.openlocfilehash: 9d481dd75aa9ea24f89be99949d3d0a188b2fdf6
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="summarizing-payment-lines-and-general-journal-lines"></a>Résumer les lignes de paiement et feuille comptabilité
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] traite les différents types de transactions de la même manière :  

- Paiements intérieurs  
- Paiements étrangers  
- Paiements SEPA  
- Paiements SEPA non libellés en Euro  

## <a name="how-payment-journal-lines-are-transferred-to-the-general-journal"></a>Comment les lignes feuille paiement sont transférées dans la feuille comptabilité  
Lorsque vous exportez les lignes feuille paiement dans un fichier, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] transfère les lignes feuille paiement dans la feuille comptabilité spécifiée. Par défaut, une ligne feuille comptabilité est créée pour chaque ligne feuille paiement.  

Les deux champs suivants dans la fenêtre **Configuration de la banque électronique** affectent la manière dont sont résumées les lignes paiement.  

- **Résumer lignes FS**  
- **Couper comm. de paiement**  

Si vous avez sélectionné la case à cocher **Résumer lignes FS** dans la fenêtre **Configuration de la banque électronique**, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] résume toutes les lignes feuille paiement pour un fournisseur spécifique sur une ligne feuille comptabilité. La description générale « Paiement %1 », où %1 est le numéro du fournisseur, est utilisée pour la description de la ligne feuille résumée. Une ligne paiement et une ligne feuille comptabilité distinctes sont créées pour traiter :  

- Les lignes feuille paiement qui contiennent des paiements partiels, avec les champs **Paiement partiel** et **Ligne individuelle** sélectionnés.  

- Les lignes feuille paiement qui contiennent une communication structurée (a réussi le test MOD97), qui définit **Communication structurée** sur True dans la feuille bancaire électronique.  

## <a name="example-1"></a>Exemple 1  
Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée. [!INCLUDE[d365fin](../../includes/d365fin_md.md)] crée :  

- Une ligne paiement combinée dans un fichier XML qui contient une communication concaténée. Un espace blanc est le délimiteur.  
- Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.  

## <a name="example-2"></a>Exemple 2  
Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée. La case à cocher **Couper comm. de paiement** est désélectionnée, et les lignes paiement SEPA et SEPA non libellées en Euro combinées dépassent 140 caractères dans la communication. [!INCLUDE[d365fin](../../includes/d365fin_md.md)] crée :  

- Deux lignes paiement combinées dans un fichier XML. La première ligne paiement contient les premières communications concaténées. La deuxième ligne paiement contient la communication de la troisième ligne.  

- Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.  

## <a name="example-3"></a>Exemple 3  
Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée. La case à cocher **Couper comm. de paiement** est également sélectionnée, et les lignes paiement SEPA et SEPA non libellées en Euro combinées dépassent 140 caractères dans la communication. [!INCLUDE[d365fin](../../includes/d365fin_md.md)] crée :  

- Une ligne paiement combinée dans un fichier XML qui contient deux communications concaténées. Des points de suspension (...) sont utilisés pour indiquer que le message est tronqué.  

- Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.  

Basés sur la structure XML, les paiements sont résumés par numéro de compte, numéro compte bancaire bénéficiaire et numéro compte bancaire. Le filtre compte bancaire peut être vide.  

Le code EndToEndId dans le message SEPA est prélevé de la communication et peut être tronqué à la longueur maximale de 45 caractères.  

## <a name="see-also"></a>Voir aussi  
 [Configurer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
 [Paramétrage de Finance](../../finance-setup-finance.md)  
 [Enregistrer des achats](../../purchasing-how-record-purchases.md) 

