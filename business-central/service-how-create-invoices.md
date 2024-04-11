---
title: "Procédure\_: créer des factures ou des avoirs service"
description: Découvrez comment créer des factures et des avoir pour votre service.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: how-to
ms.date: 02/27/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# Création des factures service ou des avoirs

La simplicité de facturation des commandes service est une fonctionnalité clé de [!INCLUDE[prod_short](includes/prod_short.md)]. Vous pouvez aussi configurer votre [!INCLUDE[prod_short](includes/prod_short.md)] afin qu’un technicien de service sur le terrain puisse créer une facture pour un service qui n’est pas connecté à un contrat ou une commande. Sinon, configurez [!INCLUDE[prod_short](includes/prod_short.md)] afin de facturer régulièrement les contrats de service. La période de facturation de chaque contrat définit la fréquence de facturation.

## Pour facturer plusieurs contrats de service

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Créer des factures de contrat de service**, puis sélectionnez le lien associé.  
2. Définissez les filtres que vous souhaitez appliquer.  
3. Dans le champ **Date comptabilisation**, entrez la date à utiliser comme date comptabilisation pour les factures service.  
4. Dans le champ **Date facturation**, saisissez la date limite de facturation des contrats. Le traitement par lots inclut les contrats dont la prochaine date de facturation est antérieure à cette date.  
5. Dans le champ **Action**, sélectionnez **Créer factures**.  
6. Sélectionnez **OK** pour créer les factures service.  
  
Vous pouvez également facturer un contrat de service directement à partir de la page **Contrat de service** si la date de la prochaine facture sur le contrat est antérieure à la date du jour.

## Pour facturer un contrat de service à partir de la page Contrat de service   

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Contrats de service**, puis sélectionnez le lien associé.  
2. Sélectionnez le contrat de service à facturer, puis ouvrez la fiche de contrat.  
3. Choisissez l’action **Créer facture service**. 
4. Choisissez **Oui** pour créer les factures service.  
  
  > [!NOTE]  
  > Vous ne pouvez pas créer de factures service pour le contrat de service lorsque la valeur du champ **Changer statut** est paramétrée sur **Ouvert**.  

## Pour valider une consommation à partir d’une commande service  

La procédure suivante décrit comment définir la partie du service que vous allez facturer au client.  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Commandes service**, puis choisissez le lien associé.  
2. Sélectionnez la commande service à facturer, puis ouvrez la fiche de commande.  
3. Choisissez l’action **Lignes service**.  
4. Recherchez les écritures requises, puis spécifiez les quantités pour lesquelles vous allez facturer le client dans le champ **Qté à facturer**.  
  
   > [!NOTE]  
   > Vous pouvez facturer le client pour le service enregistré soit entièrement, soit partiellement. Si vous décidez de facturer entièrement le client, la valeur renseignée dans le champ **Qté à facturer** doit être égale à celle renseignée dans le champ **Quantité**. Vous pouvez valider une facture entière avec une expédition entière et que vous pouvez valider une facture entière pour une expédition entière déjà validée qui n’est pas facturée ni consommée.  
   >  
   > Lorsque vous validez une facture partielle, vous pouvez spécifier la quantité à facturer de deux façons. Si vous comptez valider le service avec l’option **Livrer et facturer**, la valeur renseignée dans le champ **Qté à facturer** doit être égale à la valeur renseignée dans le champ **Qté à expédier**. Si vous voulez facturer une expédition déjà validée, la quantité à facturer ne doit pas être supérieure à la valeur renseignée dans le champ **Qté expédiée**.  
  
5. Sélectionnez **Valider**, puis **Facturer** ou **Livrer et facturer**. Pour en savoir plus, accédez à [Valider dans la gestion des services](service-service-posting.md).  
  
 La ligne service que vous sélectionnez est validée. Vous pouvez valider plusieurs lignes service en même temps en les sélectionnant et en choisissant **Valider**. Si vous procédez de la sorte, assurez-vous d'entré toutes les informations nécessaires dans les lignes.  
  
 Lorsque vous validez la commande avec l’option **Facturer**, une facture service validée est générée ainsi que les écritures comptables correspondantes et les champs appropriés sont mis à jour dans les lignes service de la commande. En outre, les documents expédition validés précédemment sont mis à jour avec les quantités facturées. Si vous sélectionnez l’option de validation **Livrer et facturer**, une expédition validée est également générée.

## Pour créer une facture service manuellement  

Typiquement, après avoir validé une facture service avec l’option **Facturer** ou **Livrer et facturer**, une facture service validée est crée automatiquement. Toutefois, il se peut que vous deviez émettre une facture qui est non liée à un contrat de service ou à une facture. Cette procédure explique comment émettre une facture au moment où le client reçoit le service.  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Factures service**, puis sélectionnez le lien associé.  
2. Créez une facture service.  
3. Renseignez le champ **N°** .  
  
    > [!NOTE]  
    >  Si vous avez configuré une souche de numéros pour les factures service sur la page **Paramètres Gestion des services**, vous pouvez sélectionner **Entrée** pour sélectionner le numéro de facture service suivant disponible.  
  
4. Dans le champ **N° client**, entrez le numéro d’un client. Sélectionnez le client approprié dans la liste.  
  
    Les champs de client sont automatiquement renseignés avec les informations de la fiche **Client**.  
  
5. Entrez une date dans le champ **Date comptabilisation**. Cette date est affichée sur les écritures validées. Ce champ affiche votre date de travail actuelle, mais vous pouvez modifier la date.  
6. Dans le champ **Date document** entrez une date apparaît sur la facture imprimée et est utilisée pour calculer la date d'échéance.  
7. Renseignez les lignes service de la facture. Renseignez les champs **Type**, **N°**, et **Quantité** pour enregistrer des articles, des ressources et/ou des coûts utilisés pour la maintenance.

## Pour créer une facture qui combine les lignes expédition enregistrées d’une ou de plusieurs commandes service 

Il se peut que vous deviez créer une facture service pour le service qui a déjà été expédié, à partir d’une ou plusieurs commandes service, mais pas encore facturé ni consommé. Vous pouvez renseigner les lignes facture automatiquement avec les lignes expédition validées sélectionnées pour un client spécifique.  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Factures service**, puis sélectionnez le lien associé.  
2. Renseignez les champs de la ligne selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] 
3. Créez des lignes facture pour les services expédiés mais non facturés. Vous pouvez également utiliser l’action **Extraire lignes expédition** pour ajouter des lignes expédition validées à la facture.  
4. Validez la facture service.  
  
 La facture service validée et les écritures comptables correspondantes sont créées. Les documents expédition validés précédemment sont mis à jour avec les quantités facturées et les quantités des lignes service des ordres origine.  

## Pour créer un avoir service  

Vous utilisez généralement un document de note de crédit de service lorsqu’un client retourne un article. Cependant, vous pouvez également les utiliser pour rembourser un client ou pour corriger une facture erronée.  

1. Sélectionnez l’![icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Avoirs service**, puis sélectionnez le lien associé.  
2. Renseignez les champs de la ligne selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Les champs **Date comptabilisation** et **Date document** affichent la date de travail. Si nécessaire, vous pouvez la modifier.    
4. Sur les lignes avoir, entrez les informations relatives aux articles retournés ou retirés, ou à la compensation qui sera donnée au client.  

## Corriger les erreurs dans les factures de services

Vous pouvez supprimer les factures de service auxquelles sont associées des écritures comptables de service. Cela signifie que vous pouvez corriger les erreurs ou apporter des modifications aux factures de service sans rester bloqué ni perdre de données. Par exemple, si vous oubliez d’affecter un groupe de validation de produit à un compte général, vous pouvez l’ajouter ultérieurement et recréer la facture de service.

Utilisez le :::image type="content" source="media/copilot-delete-trash-can.png" alt-text="Icône d’action Supprimer"::: action pour supprimer une facture de service. 

Lorsque vous supprimez une facture de service, les événements suivants se produisent :

* Valider une écriture comptable de service correctif
* Restaurez la date et la période de facturation dans le contrat, ce qui vous permet de recréer la facture.

> [!NOTE]
> Vous pouvez annuler plusieurs factures, mais vous devez le faire de manière séquentielle, en commençant par la dernière facture.
>
> Vous ne pouvez pas supprimer une facture de service si ses détails, tels que la période de facturation ou le **Prépayé** Les boutons à bascule ont été modifiés dans le contrat de service correspondant. Assurez-vous de supprimer les factures avant de modifier les paramètres du contrat de service.

## Voir aussi

[Valider des factures service](service-how-to-post-service-orders.md)  
[Paramétrage de la gestion des services](service-setup-service.md)  
[Validation de service](service-service-posting.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]