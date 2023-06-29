---
title: 'Lignes règlement et lignes feuille comptabilité [BE]'
description: 'Business Central totalise les lignes règlement et les lignes feuille pour paiements nationaux, internationaux, SEPA et hors euro.'
author: SorenGP
ms.topic: conceptual
ms.search.form: 11308
ms.date: 06/25/2021
ms.author: edupont
---
# <a name="summarizing-payment-lines-and-general-journal-lines-in-the-belgian-version"></a><a name="summarizing-payment-lines-and-general-journal-lines-in-the-belgian-version"></a>Résumé des lignes règlement et des lignes feuille comptabilité dans la version belge

Business Central totalise les lignes règlement et les lignes feuille pour les types de paiements suivants :  

- Paiements nationaux  
- Paiements internationaux  
- Paiements SEPA  
- Paiements SEPA hors euro  

## <a name="how-payment-journal-lines-are-transferred-to-the-general-journal"></a><a name="how-payment-journal-lines-are-transferred-to-the-general-journal"></a>Transfert des lignes feuille paiement vers la feuille comptabilité

Lorsque vous exportez les lignes feuille paiement vers un fichier, [!INCLUDE[prod_short](../../includes/prod_short.md)] transfère les lignes feuille paiement vers la feuille comptabilité spécifiée. Par défaut, une ligne feuille comptabilité est créée pour chaque ligne feuille paiement.  

Les deux champs suivants de la page **Paramétrage des opérations bancaires électroniques** affectent la manière dont les lignes paiement sont totalisées :  

- **Totaliser lignes feuille compta.**  
- **Limiter les textes du message de paiement**  

Si vous avez activé la case à cocher **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques**, [!INCLUDE[prod_short](../../includes/prod_short.md)] totalise toutes les lignes feuille paiement d'un fournisseur spécifique en une ligne feuille comptabilité. La description générale « Paiement %1 », où %1 correspond au numéro de fournisseur, est utilisée pour la description de la ligne feuille totalisée. Une ligne paiement distincte et une ligne feuille comptabilité distincte sont créées pour gérer :  

- Les lignes feuille paiement contenant des paiements partiels, avec les champs **Paiement partiel** et **Ligne distincte** sélectionnés.  

- Les lignes feuille paiement contenant un message au format standard (qui a réussi le test MOD97), qui définit le champ **Message au format standard** sur Vrai dans la feuille opérations bancaires électroniques.

## <a name="example-1"></a><a name="example-1"></a>Exemple 1

Dans cet exemple, vous exportez les lignes paiement, et la case à cocher **Totaliser lignes feuille compta.** est activée. [!INCLUDE[prod_short](../../includes/prod_short.md)] crée :  

- Une ligne paiement combinée dans un fichier XML qui contient un message de paiement concaténé. L'espace blanc est le séparateur.  
- Une ligne paiement dans la feuille comptabilité avec une description générique contenant le nom du fournisseur.  

## <a name="example-2"></a><a name="example-2"></a>Exemple 2

Dans cet exemple, vous exportez les lignes paiement, et la case à cocher **Totaliser lignes feuille compta.** est activée. La case à cocher **Limiter les textes du message de paiement** est désactivée, et les lignes paiement SEPA et SEPA hors euro combinées dépassent 140 caractères dans le message de paiement. [!INCLUDE[prod_short](../../includes/prod_short.md)] crée :  

- Deux lignes paiement combinées dans un fichier XML. La première ligne paiement contient les premiers messages de paiement concaténés. La deuxième ligne paiement contient le message de paiement de la troisième ligne.  

- Une ligne paiement dans la feuille comptabilité avec une description générique contenant le nom du fournisseur.  

## <a name="example-3"></a><a name="example-3"></a>Exemple 3

Dans cet exemple, vous exportez les lignes paiement, et la case à cocher **Totaliser lignes feuille compta.** est activée. La case à cocher **Limiter les textes du message de paiement** est également activée, et les lignes paiement SEPA et SEPA hors euro combinées dépassent 140 caractères dans le message de paiement. [!INCLUDE[prod_short](../../includes/prod_short.md)] crée :  

- Une ligne paiement combinée dans un fichier XML qui contient deux messages de paiement concaténés. Les points de suspension (…) sont utilisés pour indiquer que le message est tronqué.  

- Une ligne paiement dans la feuille comptabilité avec une description générique contenant le nom du fournisseur.  

Selon la structure XML, les paiements sont totalisés par numéro de compte, numéro de compte bancaire du bénéficiaire et numéro de compte bancaire. Le filtre de compte bancaire peut être vide.  

La valeur EndToEndId dans le message SEPA est extraite du message de paiement et peut être tronquée à la longueur maximale de 45 caractères.  

## <a name="see-also"></a><a name="see-also"></a>Voir aussi

 [Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)   
 [Configuration de Finance](../../finance-setup-finance.md)  
 [Enregistrer des achats](../../purchasing-how-record-purchases.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
