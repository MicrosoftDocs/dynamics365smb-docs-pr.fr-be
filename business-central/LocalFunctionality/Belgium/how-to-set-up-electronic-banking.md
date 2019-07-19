---
title: Paramétrage des opérations bancaires électroniques
description: Avec les opérations bancaires électroniques, vous pouvez effectuer des paiements électroniques à des fournisseurs et clients nationaux, internationaux, SEPA et SEPA non euro.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: d49d3cac2ecd2a32d4d30ef89e3571fefdfd5acc
ms.sourcegitcommit: 5b6dd8d881c0eb65ece6936a94dfda3185574335
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 06/28/2019
ms.locfileid: "1711012"
---
# <a name="set-up-electronic-banking"></a>Paramétrer des opérations bancaires électroniques
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

Avec les opérations bancaires électroniques, vous pouvez effectuer des paiements électroniques à des fournisseurs et clients nationaux, internationaux, SEPA et SEPA non euro.  

Votre société s'abonne à un contrat eBanking avec la banque pour gérer un compte bancaire spécifique ou plusieurs comptes bancaires. La société s'abonne également à Isabel (Interbanks Standards Association Belgium) pour envoyer des fichiers de paiement et recevoir des fichiers de relevé bancaire de la banque par voie électronique. Par conséquent, la société reçoit des cartes à puce liées au contrat eBanking. Les cartes à puce sont sécurisées par des codes PIN.  

Vous recevrez une de ces cartes à puce pour vous connecter à IBS afin d'être connecté au contrat eBanking de la société.

Lors du chargement ou du téléchargement des fichiers vers ou depuis la plateforme IBS, vous insérerez la carte à puce dans le lecteur de cartes et utiliserez un code PIN pour établir la connexion avec IBS. Une fois la session IBS établie, le contrat eBanking et l'utilisateur eBanking sont connus par le système. De plus, le contrat eBanking et les numéros de compte bancaire associés de l'utilisateur sont connus.  

<In last sentence, paragraph above, change "user linked bank account numbers" to "the user's linked bank account numbers"   -->

Avant de pouvoir les opérations bancaires électroniques, vous devez définir les informations suivantes :  

- Paramétrage des opérations bancaires électroniques.  
- Codes IBLC/BLWI - Pour plus d'informations, voir [Paramétrer les codes de transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md).  

## <a name="to-set-up-electronic-banking"></a>Pour paramétrer les opérations bancaires électroniques  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramétrage des opérations bancaires électroniques**, puis sélectionnez le lien connexe.  
2.  Dans la page **Paramétrage des opérations bancaires électroniques**, renseignez les champs comme indiqué dans le tableau suivant.   

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Totaliser lignes feuille compta.**|Sélectionnez pour indiquer si vous souhaitez regrouper les lignes feuille paiement pour chaque fournisseur.|  
    |**Limiter les textes du message de paiement**|Sélectionnez pour indiquer si vous souhaitez tronquer les longs messages de paiement. Les messages seront tronqués si supérieurs à 106 caractères pour les paiements nationaux et inférieurs à 140 caractères pour les paiements internationaux.|  
    |**Version du Kit de développement logiciel (IBS)**|Spécifiez la version d'Isabel actuellement utilisée pour les opérations bancaires électroniques dans votre organisation.|  
    |**Adresse e-mail de notification**|Spécifiez l'adresse e-mail de notification à utiliser pour les messages de solde et d'opérations bancaires électroniques. Il s'agit de l'adresse par défaut utilisée pour contacter le serveur Isabel.|  
    |**Langue**|Spécifiez la langue à utiliser pour les messages de solde et d'opérations bancaires électroniques.|  
    |**Version du service IBS**|Spécifiez la version du service utilisée pour communiquer avec le serveur Isabel.|  

3.  Renseignez les champs comme indiqué dans le tableau suivant.   

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Télécharger le mode d'intégration**|Spécifiez le mode que vous souhaitez utiliser pour télécharger le contenu vers le serveur Isabel. Les options du mode d'intégration incluent **Assisté** et **Manuel**. Si le mode d'intégration est défini sur **Assisté**, vous devez définir le champ **Version d'IBS** sur **6**. Les écritures de la table **Feuille IBS** seront créées lorsque des fichiers de règlement seront générés. Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement et aucune écriture journal n'est créée.|  
    |**Chemin de téléchargement**|Spécifiez le chemin d'accès au dossier où les dossiers seront enregistrés lors du processus de téléchargement.|  

4.  Renseignez les champs comme indiqué dans le tableau suivant.   

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Télécharger le mode d'intégration**|Spécifiez le mode que vous souhaitez utiliser pour télécharger le contenu vers le serveur Isabel. Les options incluent **Assisté** et **Manuel**. Si le mode d'intégration est défini sur **Assisté**, vous devez définir le champ **Version d'IBS** sur **6**. Les écritures de la table **Feuille IBS** seront créées lorsque le téléchargement est exécuté. Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement et aucune écriture journal n'est créée.|  
    |**Chemin de téléchargement**|Spécifiez le chemin d'accès au dossier où les dossiers seront enregistrés lors du processus de téléchargement.|  

5.  Renseignez les champs comme indiqué dans le tableau suivant.   

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**N°. de téléchargement journal IBS**|Spécifiez la souche de numéros utilisée pour les écritures journal Isabel créées pendant le processus de téléchargement de fichier.|  
    |**N°. de téléchargement journal IBS**|Spécifiez la souche de numéros utilisée pour les écritures journal Isabel créées pendant le processus de téléchargement de fichier.|  
    |**ID demande IBS**|Spécifiez une souche de numéros utilisée pour la numérotation automatique et unique des demandes.|  

6.  Choisissez le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Site Web Isabel](https://go.microsoft.com/fwlink/?LinkId=210323)   
 [Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)   
 [Paiements électroniques, Belgique](belgian-electronic-payments.md)   
 [Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Générer des suggestions de règlement](how-to-generate-payment-suggestions.md)   
 [Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Gérer les lignes de paiement électronique](how-to-manage-electronic-payment-lines.md)   
 [Imprimer les fichiers de paiement](how-to-print-payment-files.md) [Résumé des lignes règlement et des lignes feuille comptabilité](summarizing-payment-lines-and-general-journal-lines.md)
