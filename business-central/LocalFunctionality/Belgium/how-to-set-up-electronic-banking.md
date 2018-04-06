---
title: "Comment configurer la banque électronique"
description: "Avec la banque électronique, vous pouvez effectuer des paiements électroniques aux fournisseurs et clients nationaux, internationaux, SEPA et SEPA non-euro."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 406110a824fb3f53330e799ad01b05292f001997
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-electronic-banking"></a>Configurer des opérations bancaires électroniques
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

Avec la banque électronique, vous pouvez effectuer des paiements électroniques aux fournisseurs et clients nationaux, internationaux, SEPA et SEPA non-euro.  

Votre société souscrit un contrat eBanking avec la banque pour maintenir un certain compte bancaire ou plusieurs comptes bancaires. La société s'inscrit également auprès d'Isabel pour envoyer des fichiers paiement à la banque et recevoir des fichiers relevé bancaire de la banque par voie électronique. La société reçoit ainsi des cartes à puce liées au contrat eBanking. Les cartes à puce sont sécurisées par code PIN.  

Vous recevrez l'une de ces cartes à puce pour vous connecter à IBS et être lié au contrat eBanking de la société.  

Lors du téléchargement de fichiers vers ou depuis la plateforme IBS, vous insérerez la carte à puce dans le lecteur de carte et utiliserez un code PIN pour établir la connexion à IBS. Lorsque la connexion à IBS est établie, le contrat eBanking et l'utilisateur eBanking sont reconnus par le système. Les numéros de compte liés du contrat eBanking et de l'utilisateur sont également reconnus.  

Avant de pouvoir utiliser la banque électronique, vous devez configurer les informations suivantes :  

- Configuration de la banque électronique.  
- Les codes IBLC/BLWI - Pour plus d'informations, voir [Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md).  

## <a name="to-set-up-electronic-banking"></a>Pour configurer des opérations bancaires électroniques  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramétrage bancaire électronique**, puis sélectionnez le lien connexe.  
2.  Dans la fenêtre **Configuration de la banque électronique**, dans le raccourci **Général**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Résumer lignes FS**|Sélectionnez pour indiquer si vous souhaitez regrouper les lignes feuilles paiement pour chaque fournisseur.|  
    |**Couper comm. de paiement**|Sélectionnez pour indiquer si vous souhaitez tronquer les longues communications de paiement. Les communications seront tronquées si elles contiennent plus de 106 caractères pour les paiements nationaux et plus de 140 caractères pour les paiements internationaux.|  
    |**Version IBS**|Spécifiez la version d'Isabel actuellement utilisée pour la fonction de banque électronique dans votre organisation.|  
    |**Adresse électronique de notification**|Spécifiez l'adresse électronique de notification que vous souhaitez utiliser pour les messages concernant les transactions et le solde de la banque électronique. Il s'agit de l'adresse par défaut utilisée pour contacter le serveur Isabel.|  
    |**Langue**|Spécifiez la langue que vous souhaitez utiliser pour les messages concernant les transactions et le solde de la banque électronique.|  
    |**Version de service IBS**|Spécifiez la version du service utilisée pour communiquer avec le serveur Isabel.|  

3.  Dans le raccourci **Télécharger**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Mode d'intégration du téléchargement (amont)**|Spécifiez le mode que vous souhaitez utiliser pour télécharger du contenu sur le serveur Isabel. Les options du mode d'intégration incluent **Interactif** et **Manuel**. Si le mode d'intégration est défini sur **Interactif**, vous devez définir le champ **Version IBS** sur **6**. Les écritures de la table **Journal IBS** seront créées lorsque les fichiers paiement seront générés. Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement, et aucune écriture ne sera créée.|  
    |**Chemin du téléchargement (amont)**|Spécifiez le chemin d'accès au dossier où les fichiers sont enregistrés au cours du téléchargement sur le serveur.|  

4.  Dans le raccourci **Télécharger**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Mode d'intégration du téléchargement (aval)**|Spécifiez le mode que vous souhaitez utiliser pour télécharger du contenu sur le serveur Isabel. Les options incluent **Interactif** et **Manuel**. Si le mode d'intégration est défini sur **Interactif**, vous devez définir le champ **Version IBS** sur **6**. Les écritures de la table **Journal IBS** seront créées à l'issue du téléchargement. Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement, et aucune écriture ne sera créée.|  
    |**Chemin du téléchargement (aval)**|Spécifiez le chemin d'accès au dossier où les fichiers sont enregistrés au cours du téléchargement depuis le serveur.|  

5.  Dans le raccourci **Numérotation**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nos de téléchargement (amont) du journal IBS**|Spécifiez la souche de numéros utilisée pour les écritures journal Isabel qui sont créées au cours du téléchargement sur le serveur.|  
    |**Nos de téléchargement (aval) du journal IBS**|Spécifiez la souche de numéros utilisée pour les écritures journal Isabel qui sont créées au cours du téléchargement des fichiers du serveur.|  
    |**ID demande IBS**|Spécifiez une souche de numéros utilisée pour la numérotation automatique et unique des demandes.|  

6.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323)   
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Configurer des fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des propositions de paiement](how-to-generate-payment-suggestions.md)   
 [Créer des modèles et des lots de feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md)   
 [Imprimer les fichiers paiement](how-to-print-payment-files.md) [Résumer les lignes de paiement et feuille comptabilité](summarizing-payment-lines-and-general-journal-lines.md)
 
