---
title: Procédure pas à pas sur les commandes de service pour les articles de service
description: Cet article vous guide à travers plusieurs processus principaux qui impliquent des commandes et des articles de service.
author: andreipa
ms.author: andreipa
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 05/31/2023
ms.custom: bap-template
ms.service: dynamics-365-business-central
---

# <a name="walkthrough-of-service-orders-for-service-items"></a>Procédure pas à pas sur les commandes de service pour les articles de service

Cette procédure détaillée illustre plusieurs processus principaux :

- Créer une commande service ad hoc et enregistrer la réparation de l’article
- Fournir un article de prêt au client pour une période de réparation
- Valider et facturer la commande service
    
## <a name="creating-a-service-order"></a>Création d’une commande service

### <a name="scenario"></a>Scénario

Charles, le responsable de service, crée une commande service pour un scénario de réparation et fournit un article de prêt au client pour la période de réparation.

### <a name="steps"></a>Étapes

1. Créez manuellement la commande service pour l’article qui doit être réparé.
   1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Commandes service**
   2. Sélectionnez l’action **Nouveau**.
   3. Entrez **10000** dans N° client. champ
   4. Sélectionnez **RÉPARER** pour le champ **Type commande service**.
   5. Dans les lignes, sélectionnez **S-100** comme **N° article**.
2. Facultatif
   1. Choisissez l’action de ligne **Résolution des problèmes** pour vérifier les solutions possibles.
   2. Choisissez l’action de ligne **Relations codes panne/solution**
   3. Sélectionnez *BRUIT* comme **Code symptôme**
   4. Sélectionnez *5-2 Bruit sonore pendant l’infusion* comme **Code panne** et fermez la page. Le code panne et les codes solution sont mis à jour dans les lignes.
3. Prêter un article de remplacement pendant la réparation de l’article
   1. Dans les lignes, sélectionnez **ARTPRÊT1** comme N° article. Confirmez l’émission de l’article de prêt en sélectionnant **Oui** pour fournir l’article de prêt. 
   2. Choisissez l’action Fonctions **Extraire codes prestation std**, sélectionnez le code standard associé au groupe de services et sélectionner **OK**.
   
### <a name="results"></a>Résultats

- Une commande service est créée pour l’article
- Le journal de documents service de la commande service affiche les activités de l’article de prêt.
- L’article de prêt a une écriture comptable pour refléter le prêt.
   

## <a name="register-performed-work-mark-loaner-as-returned"></a>Enregistrez le travail effectué, marquez l’article de prêt comme retourné.

### <a name="scenario-1"></a>Scénario

Le technicien de service marque l’article de prêt comme retourné et enregistre le travail effectué.

### <a name="steps-1"></a>Étapes

1. Localiser la tâche de service et enregistrer le temps 
   1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Tâches service**, puis choisissez le lien associé.
   2. Localisez la commande service pour laquelle vous souhaitez saisir le temps.
   3. Choisissez l’action **Feuille activité article**.
   4. Entrez les informations suivantes

    |Type|N°|Quantité|
    |----|---|--------|  
    |Article|SER102|2|

   4. Sélectionnez *TERMINÉ* dans le champ **Code état réparation**
    
2. Marquer l’article de prêt comme retourné
   1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Articles de prêt**, puis choisissez le lien associé.
   2. Localisez l’article de prêt à marquer comme retourné.
   3. Choisissez l’action **Recevoir** 
   4. Confirmez le retour de l’article de prêt en sélectionnant **Oui** pour retourner l’article de prêt.
      
### <a name="results-1"></a>Résultats

- Le **journal de documents service** de la commande service affiche les activités de l’article de prêt.
- L’article de prêt a une écriture comptable pour refléter la réception.


### <a name="scenario-2"></a>Scénario

Charles, le responsable des services, valide la commande service terminée.

1. Localiser la commande service 
   1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Commandes service**, puis choisissez le lien associé.
   2. Localisez la commande service que vous souhaitez valider.

2. Dans la commande service, validez la facture
   1. Choisissez l’action **Valider** pour terminer la commande service, sélectionnez l’action **Expédier et facturer**, puis choisissez le bouton **OK**.
   2. Confirmez l’ouverture de la facture validée en sélectionnant **Oui**. 
### <a name="results-2"></a>Résultats

- La **facture service validée** est créée.
- Les **Écritures comptables service** associées à l’article et à la ressource sont créées

## <a name="see-also"></a>Voir aussi
[Procédure pas à pas sur les contrats de service pour les articles de service](service-contract-flow.md)  
[Service](../../service-service.md)
