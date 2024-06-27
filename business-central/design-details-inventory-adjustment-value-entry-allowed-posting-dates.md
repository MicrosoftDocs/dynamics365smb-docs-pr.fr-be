---
title: "Message d’erreur\_: «\_La date comptabilisation n’est pas incluse dans la plage de dates comptabilisation autorisées\_»"
description: "Résolvez l’erreur sou-jacente au message «\_La date comptabilisation n’est pas incluse dans la plage de dates comptabilisation autorisées\_» lorsque vous exécutez le traitement par lots Ajuster coûts\_: Écr. article."
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: null
ms.date: 05/24/2024
ms.service: dynamics-365-business-central
---

# Message d’erreur : « La date comptabilisation n’est pas incluse dans la plage de dates comptabilisation autorisées... »

Lors de l’utilisation du traitement par lots **Ajuster coûts : Écr. article**, vous pouvez rencontrer le message d’erreur suivant :

**La date de comptabilisation n’est pas dans votre plage de dates de comptabilisation autorisées**

Ce message indique que vous n’êtes pas autorisé à publier des entrées pour la date que vous avez saisie. Vous pouvez contourner ce problème en modifiant votre configuration utilisateur.

## Modifier les paramètres utilisateur  

|Identifiant d’utilisateur  |Début période validation  | Fin période validation  |
|---------|---------|--------|
|EUROPE  |  2020/09/11      |2020/09/30      |

Dans ce cas, vous êtes autorisé à publier entre le 11 septembre et le 30 septembre. Cependant, vous n’êtes pas autorisé à valider l’entrée de valeur d’ajustement avec une date de comptabilisation le 10 septembre.  

### Aperçu de la configuration de la date comptabilisation

#### Périodes inventaire

|Date de fin  |Nom  |Terminé  |
|---------|---------|---------|
|2020/01/31     |2020 janvier      |  Oui    |
|2020/02/28     |Février 2020     |  Oui    |
|2020/03/31     |Mars 2020        |  Oui    |
|2020/04/30     |Avril 2020        |  Oui    |
|2020/05/31     |Mai 2020        |  Oui    |
|2020/06/30     |Juin 2020       |  Oui    |
|2020/07/31     |Juillet 2020        |   Oui   |
|2020/08/31     |Août 2020     |   Oui   |
|2020/09/30     |Septembre 2020  |         |
|2020/10/31     |Octobre 2020    |         |
|2020/11/30     |Novembre 2020   |         |
|2020/12/31     |Décembre 2020   |         |  

#### Paramètres comptabilité

|Champ|Valeur|
|---------|---------|
|Début période validation :  |  2020/09/10      |
|Fin période validation :    |  2020/09/30      |
|Registre temps :       |         |
|Format adresse local :|   Code postal      |  

#### Paramètres utilisateur

|ID utilisateur  |Début période validation  | Fin période validation  |
|---------|---------|--------|
|USERNAME |  2020/09/10      |2020/09/30      |

En attribuant à l’utilisateur une plage de dates comptabilisation autorisée plus large que dans la **période inventaire** ou les **paramètres comptabilité**, il devient possible d’éviter le conflit à l’origine du message d’erreur. Par exemple, la plage plus large vous permet de valider l’entrée de valeur d’ajustement avec une date de comptabilisation le 10 septembre.
  
## Voir aussi  

[Détails de conception : date comptabilisation de l’écriture valeur d’ajustement](design-details-inventory-adjustment-value-entry-posting-date.md)  
[Détails de conception : Évaluation stock](design-details-inventory-costing.md)  
[Détails de conception : lettrage article](design-details-item-application.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
