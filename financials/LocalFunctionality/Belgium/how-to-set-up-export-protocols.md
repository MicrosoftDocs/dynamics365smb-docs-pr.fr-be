---
title: Comment configurer des protocoles d'exportation
description: "Avant de pouvoir utiliser la banque électronique, vous devez configurer des protocoles d'exportation. Les protocoles d'exportation définissent le format de fichier généré lorsque vous exportez l'historique des paiements à traiter par la banque. Chaque ligne contient un protocole d'exportation identifié par un code et une description. Vous pouvez configurer autant de protocoles d'exportation que vous le souhaitez. Vous devez configurer un protocole d'exportation pour les paiements nationaux, les paiements internationaux, les paiements SEPA et les paiements SEPA autres que Euro."
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
ms.openlocfilehash: c18c89e76a3fe4737dda477bff3adb58ffe63278
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-export-protocols"></a>Configurer les protocoles d'exportation
Avant de pouvoir utiliser des transactions bancaires électroniques, vous devez configurer des protocoles d'exportation. Les protocoles d'exportation définissent le format de fichier généré lorsque vous exportez l'historique des paiements à traiter par la banque. Chaque ligne contient un protocole d'exportation identifié par un code et une description. Vous pouvez configurer autant de protocoles d'exportation que vous le souhaitez. Vous devez configurer un protocole d'exportation pour les paiements nationaux, internationaux, SEPA et SEPA non libellés en Euro.  

 Les protocoles d'exportation vous permettent d'attribuer le codeunit qui définit le contrôle à effectuer avant l'exportation des lignes de paiement dans un fichier et l'état qui définit le format de paiement. Par exemple, vous pouvez avoir un protocole d'exportation nommé **DOM1**. Celui-ci contient le codeunit de contrôle **Vérifier les paiements intérieurs** et l'état **Classer les paiements intérieurs**. Chaque protocole d'exportation est associé à un codeunit de contrôle et à un état correspondant, comme indiqué dans le tableau suivant.  

|**Vérifier ID objet**|**Exporter ID objet**|  
|-------------------------|--------------------------|  
|2000002 Vérifier les paiements intérieurs|État 2000001 Classer les paiements intérieurs|  
|2000003 Vérifier les paiements étrangers|État 2000002 Classer les paiements étrangers|  
|2000004 Vérifier les paiements SEPA|État 2000005 Classer les paiements SEPA|  
|2000005 Vérifier les paiements SEPA non libellés en Euro|État 2000006 Classer les paiements SEPA non libellés en Euro|  
|Si cette option ne vous intéresse pas, définissez-la sur zéro ou sélectionnez-en une autre.|XMLport 1000 (SEPA pain.001.001.03 Payments)|  

 Après avoir configuré des protocoles d'exportation, vous pouvez les utiliser dans vos feuilles paiement de banque électronique.  

## <a name="to-set-up-an-export-protocol"></a>Pour configurer un protocole d'exportation  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Protocoles d'exportation**, puis sélectionnez le lien correspondant.  
2.  Choisissez l'action **Nouveau**.  
3.  Dans la fenêtre **Protocoles d'exportation**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Spécifiez un code unique qui identifie le protocole d'exportation.|  
    |**Description**|Spécifiez une description pour l'écriture protocole d'exportation. Vous pouvez entrer au maximum 50 caractères, des chiffres ou des lettres.|  
    |**Code frais**|Spécifiez le code qui décrit le type de dépenses associées à l'écriture protocole d'exportation. Les codes frais possibles incluent **vide**, **SHA**, **BEN** et **OUR**. Pour les paiements internationaux, **SHA** est la valeur par défaut.|  
    |**Vérifier ID objet**|Spécifiez le numéro d'identification du codeunit que vous souhaitez utiliser pour effectuer un contrôle de l'objet avant l'exportation du fichier de paiement.|  
    |**Vérifier nom objet**|Spécifiez le nom d'un processus de vérification utilisé pour effectuer un contrôle de l'objet avant l'exportation du fichier de paiement. Une fois l'option **Vérifier ID objet** sélectionnée, ce champ contiendra l'option **Vérifier nom objet**.|  
    |**Exporter type objet**|Spécifiez le type de l'objet qui définit le format de l'exportation du fichier de paiement. Une fois l'option **Exporter ID objet** sélectionnée, ce champ contiendra l'option **Exporter type objet**.<br /><br /> **NOTE :** pour configurer le protocole d'exportation pour SEPA pain.001.001.03, sélectionnez **XMLPort**.|  
    |**Exporter ID objet**|Spécifiez le numéro d'identification de l'objet qui définit le format de l'exportation du fichier de paiement. Par exemple, si vous sélectionnez **2000002**, le format d'exportation pour le fichier paiement sera **Classer les paiements étrangers**.<br /><br /> **NOTE :** pour configurer le protocole d'exportation pour SEPA pain.001.001.03, sélectionnez XMLport **1000**.|  
    |**Souche de n° d'exportation**|Spécifiez la souche de numéros qui est utilisée pour affecter des numéros d'identification à l'exportation du fichier de paiement.|  

4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)

