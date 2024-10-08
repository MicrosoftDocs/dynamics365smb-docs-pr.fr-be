---
title: Utiliser des documents électroniques vente
description: Découvrez comment utiliser la fonctionnalité de documents électroniques liée aux factures de vente.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'electronic document, electronic invoice, e-document, e-invoice, sales, deliver'
ms.search.form: '42, 43, 132, 6103, 6133, 6121, 9301, 9305'
ms.date: 04/10/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="use-e-documents-in-the-sales-process"></a>Utilisation des documents électroniques dans le processus vente

Vous pouvez utiliser des documents électroniques configurés (documents électroniques) avec les documents de vente.

Vous pouvez utiliser les documents vente suivants avec la fonctionnalité des documents électroniques :  

- Factures vente
- Commandes vente
- Avoirs vente
- Factures service
- Avoirs service
- Factures d’intérêts
- Relances

## <a name="e-documents-in-sales"></a>Documents électroniques vente

Pour créer et envoyer une facture électronique à un client, vous devez créer et valider la facture vente. Pour en savoir plus sur le processus standard, voir [Facture des ventes](sales-how-invoice-sales.md).

Après avoir validé le document vente, ouvrez la page **Factures vente validée** pour accéder à la page **Document électronique** associée.

### <a name="view-e-documents"></a>Afficher les documents électroniques

Pour afficher les documents électroniques existants, procédez comme suit.

1. Sur la page **Factures vente validée**, sélectionnez **Document électronique** et **Ouvrir document électronique**.
2. Sur la page **Documents électronique**, dans l’en-tête, vous pouvez afficher les informations de base sur la facture validée.
3. Le champ **Enregistrement** affiche le numéro de document de la facture vente validée. Sélectionnez le lien pour ouvrir le document.
4. Dans le champ **Statut du document électronique**, vous pouvez afficher le statut en temps réel du document et son emplacement dans le pipeline de processus. Si le document est validé, le statut est défini sur **Traité**.

### <a name="e-document-statuses-and-logs"></a>Journaux et statuts des documents électroniques

Pour plus de détails sur le niveau d’état de service de votre document électronique, consultez le récapitulatif **Statut du service du document électronique**. Sur les lignes, le système affiche un ou plusieurs services utilisés par le document. Dans le scénario le plus courant, chaque document utilise un seul service. Cependant, un document peut utiliser plusieurs services.

- Cochez la case **Code service document électronique** pour déterminer quel service a été utilisé.
- Cochez la case **Statut du document électronique** pour déterminer le statut de service actuel de ce document.
- Si vous souhaitez plus de détails, sélectionnez le champ **Journaux** pour le service sur la page **Journaux de documents électroniques**. Un aperçu chronologique des différents statuts du document est affiché.
- Vérifiez les champs **Numéro d’entrée** et **Création le** et d’autres informations sur la page **Journaux de documents électroniques**. Dans le champ **Statut du document électronique**, le premier statut est défini sur **Exporté**, ce qui indique que le fichier de document électronique a été créé. Le statut suivant est **Envoyé**, qui indique que le document a été envoyé au fournisseur de services, s’il est configuré.

Pour plus d’informations, sélectionnez l’entrée qui possède le statut **Exporté**, puis exécutez l’une des actions suivantes :

- **Ouvrir les journaux de mappage** : obtenez un aperçu de tous les champs exportés à partir des tables sourcées dans le champ **Valeur d’origine**. Si vous avez utilisé des règles de transformation lors du processus d’exportation, vous pouvez également obtenir la valeur finale dans le champ **Nouvelle valeur**.
- **Exporter le fichier** : exportez le fichier XML pour une révision manuelle.

Pour visualiser la communication entre vous et le service auquel vous envoyez votre document, utilisez le champ **Journaux de communications**. Ouvrez la page **Journaux de communication de documents électroniques** pour afficher les détails de la demande et le message de motifs avec ce service.

S’il y a un problème avec le fournisseur de services et que le document ne peut pas être envoyé, recherchez les indicateurs suivants sur la page **Documents électronique** :

- Le champ **Statut du document électronique** sur l’en-tête montre le statut **Erreur**.
- Le champ **Statut du document électronique** sur le récapitulatif **Statut du service de document électronique** affiche le statut **Erreur d’envoi**.
- Le récapitulatif **Erreur et avertissements** contient un ou plusieurs messages indiquant la cause du problème.

Une fois le problème résolu, exécutez manuellement les actions **Envoyer le document**. Si vous avez besoin de différentes actions, telles que **Document recréé**, **Annuler le document**, ou **Obtenir l’approbation**, vous pouvez les exécuter.

## <a name="overview-of-e-document-statuses"></a>Vue d’ensemble des statuts des documents électroniques

Pour obtenir un meilleur aperçu de tous les documents électroniques de l’entreprise, vous pouvez sélectionner le centre de rôles **Comptable** où existent les statuts des documents électroniques. Vous y trouverez des activités de documents électroniques qui ont les statuts suivants :

- **Documents électroniques sortants**

    - Traité
    - En cours
    - Erreur


## <a name="see-also"></a>Voir aussi

[Procédure : configurer les documents électroniques dans [!INCLUDE[prod_short](includes/prod_short.md)]](finance-how-setup-edocuments.md)    
[Utilisation des documents électroniques achat](finance-how-use-edocuments-purchase.md)  
[Comment étendre des documents électroniques dans [!INCLUDE[prod_short](includes/prod_short.md)]](/dynamics365/business-central/dev-itpro/developer/devenv-extend-edocuments)    
[Gestion financière](finance.md)    
[Facturer des ventes](sales-how-invoice-sales.md)    
[Enregistrer les achats avec les factures achat et les commandes](purchasing-how-record-purchases.md)    
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
