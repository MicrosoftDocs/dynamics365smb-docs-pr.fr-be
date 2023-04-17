---
title: 'Paramétrage des protocoles d''exportation [BE]'
description: 'Avant d''utiliser la banque électronique, vous devez paramétrer des protocoles d''exportation qui définissent le format de fichier généré lorsque vous exportez l''historique des paiements que la banque doit traiter.'
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: 2000005
ms.date: 06/17/2021
ms.author: edupont
---
# Paramétrer les protocoles d'exportation dans la version belge
Avant de pouvoir utiliser les opérations bancaires électroniques, vous devez paramétrer les protocoles d'exportation. Les protocoles d'exportation définissent le format de fichier généré lorsque vous exportez l'historique des paiements que la banque doit traiter. Chaque ligne contient un protocole d'exportation identifié par un code et une description. Vous pouvez paramétrer autant de protocoles d'exportation que vous le souhaitez. Vous devez paramétrer un protocole d'exportation pour les paiements nationaux, internationaux, SEPA et SEPA hors euro.  

 Avec les protocoles d'exportation, vous pouvez affecter le codeunit qui définit la vérification à effectuer avant d'exporter les lignes paiement dans un fichier, et l'état qui définit le format de paiement. Par exemple, vous pouvez avoir un protocole d'exportation nommé **DOM1**. Ce protocole d'exportation contient le codeunit de vérification **Vérifier les paiements nationaux** et l'état **Effectuer des paiements nationaux**. Chaque protocole d'exportation a un codeunit de vérification et un état correspondant, comme indiqué dans le tableau suivant.  

|**Vérifier l'ID objet**|**Exporter l'ID objet**|  
|-------------------------|--------------------------|  
|2000002 Vérifier les paiements nationaux|État 2000001 Effectuer des paiements nationaux|  
|2000003 Vérifier les paiements internationaux|État 2000002 Effectuer des paiements internationaux|  
|2000004 Vérifier les paiements SEPA|État 2000005 Effectuer des paiements SEPA|  
|2000005 Vérifier les paiements SEPA hors euro|État 2000006 Effectuer des paiements SEPA hors euro|  
|Si vous ne souhaitez pas utiliser cette option, définissez-la sur zéro ; sinon, sélectionnez une autre option.|XMLport 1000 (Paiements SEPA pain.001.001.03)|  

 Après avoir paramétré les protocoles d'exportation, vous pouvez les utiliser dans vos feuilles paiement bancaire électronique.  

## Pour paramétrer un protocole d'exportation  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Protocoles d'exportation**, puis choisissez le lien associé.  
2.  Choisissez l'action **Nouveau**.  
3.  Dans la page **Protocoles d'exportation**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Spécifiez un code qui identifie de façon unique le protocole d'exportation.|  
    |**Description**|Spécifiez une description pour le protocole d'exportation. Vous pouvez entrer au maximum 50 caractères, des chiffres ou des lettres.|  
    |**Code dépenses**|Spécifiez le code qui décrit le type de dépenses associées au protocole d'exportation. Les valeurs sont : **vide**, **SHA**, **BEN** et **OUR**. Pour les paiements internationaux, **SHA** est la valeur par défaut.|  
    |**Vérifier l'ID objet**|Spécifiez le numéro d'identification du codeunit que vous souhaitez utiliser pour vérifier l'objet avant l'exportation du fichier de paiement.|  
    |**Vérifier le nom de l'objet**|Spécifiez le nom du processus de vérification utilisé pour vérifier l'objet avant l'exportation du fichier de paiement. Après avoir sélectionné **Vérifier l'ID objet**, ce champ indique **Vérifier le nom de l'objet**.|  
    |**Exporter le type d'objet**|Spécifiez le type de l'objet qui définit le format d'exportation de l'export du fichier de paiement. Après avoir sélectionné **Exporter l'ID objet**, ce champ indique **Exporter le type d'objet**.<br /><br /> **REMARQUE :** pour paramétrer le protocole d'exportation pour SEPA pain.001.001.03, sélectionnez **XMLPort**.|  
    |**Exporter l'ID objet**|Spécifiez le numéro d'identification de l'objet qui définit le format d'exportation de l'export du fichier de paiement. Par exemple, si vous sélectionnez **2000002**, le format d'exportation du fichier de paiement est **Remplir les paiements internationaux**.<br /><br /> **REMARQUE :** pour paramétrer le protocole d'exportation pour SEPA pain.001.001.03, sélectionnez XMLport **1000**.|  
    |**Souche de n° d'exportation**|Spécifiez la souche de numéros qui est utilisée pour affecter des numéros d'identification à l'export du fichier de paiement.|  
    |**Paiement groupé**|Spécifie si ce protocole d’exportation est utilisé pour les paiements groupés.|  

4.  Cliquez sur le bouton **OK**.  

## Voir aussi  
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
