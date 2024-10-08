---
title: Règles d’application automatique des paiements
description: Découvrez comment configurer des règles pour l’application automatique des paiements sur la page Règles de lettrage des paiements.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'payment process, direct payment posting, reconcile payment, expenses, cash receipts'
ms.search.form: '1290, 1294, 1287'
ms.date: 06/03/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="set-up-rules-for-automatic-application-of-payments"></a>Configurer des règles pour l’application automatique des paiements

Sur la page **Règles de lettrage de paiement**, vous définissez des règles pour définir comment le texte de paiement (sur une transaction bancaire) doive être automatiquement mis en correspondance avec le texte sur les factures (impayées), les avoirs ou d’autres entrées associées lorsque vous utilisez la fonction **Lettrer automatiquement** sur la page **Feuille rapprochement bancaire**. Pour plus d’informations, consultez [Rapprocher les paiements à l’aide de l’application automatique](receivables-how-reconcile-payments-auto-application.md).

Pour définir de nouvelles règles de lettrage de paiement, choisissez quels types de données sur une ligne feuille rapprochement bancaire doivent correspondre aux données sur une ou plusieurs écritures ouvertes avant que le paiement associé ne soit automatiquement lettré avec les écritures ouvertes. La qualité de chaque lettrage automatique est indiquée par une valeur de **Faible** à **Élevée** dans le champ **Fiabilité correspondance** sur la page **Feuille rapprochement bancaire** selon la règle de lettrage de paiement qui a été utilisée.

Chaque ligne de la page **Règles de lettrage de paiement** représente une règle de lettrage de paiement. Les règles sont appliquées dans l’ordre spécifié par le champ **Ordre de tri**. Si plusieurs règles sont utilisées simultanément, c’est la fiabilité correspondance de la règle dont l’ordre de tri est le plus élevé qui est utilisée.

La fonction de lettrage automatique est basée sur des critères de correspondance classés par priorité. La fonction essaie d’abord, par ordre de priorité, de faire correspondre le texte dans les cinq champs **Partie associée** d’une ligne feuille avec le texte du compte bancaire, du nom ou de l’adresse des clients ou des fournisseurs dont les documents impayés représentent des écritures ouvertes. La fonction essaie ensuite de faire correspondre le texte des champs **Texte transaction** et **Info transaction supplémentaire** sur une ligne feuille avec le texte des champs **N° du document externe** et **N° document** sur les écritures ouvertes. Enfin, la fonction essaie de faire correspondre le montant du champ **Montant relevé** d’une ligne feuille avec le montant sur les écritures ouvertes.

> [!NOTE]
> La correspondance de texte n’est possible que pour les textes contenant plus de quatre caractères.

Outre les critères de correspondance, les remarques suivantes s’appliquent concernant le signe du montant règlement :

- Pour les montants négatifs, une correspondance est d’abord établie par rapport aux écritures ouvertes représentant les factures client, et ensuite par rapport aux avoirs fournisseur.
- Pour les montants positifs, une correspondance d’abord établie par rapport aux écritures ouvertes représentant les factures fournisseur, et ensuite par rapport aux avoirs client.

## <a name="to-set-up-a-payment-application-rule"></a>Pour définir une règle de lettrage de paiement
1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Règles de lettrage des paiements**, puis choisissez le lien associé.
2. Définissez une règle de lettrage de paiement, nouvelle ou modifiée, en renseignant les champs sur une ligne tel que décrit dans le tableau suivant.

|Champ|Description|
|-|-|
|**Fiabilité correspondance**|Spécifie la fiabilité de la règle de lettrage que vous définissez sur la ligne. <br /></br>Une valeur spécifiée dans ce champ est affichée dans le champ **Fiabilité correspondance** sur la page **Feuille rapprochement bancaire** en fonction de la qualité du lettrage de paiement automatique sur la ligne feuille.|
|**Priorité**|Spécifie la priorité de la règle de lettrage par rapport aux autres règles de lettrage définies en tant que lignes sur la page **Règles lettrage paiement**. 1 représente la priorité la plus élevée.|
|**Correspondance partie associée**|Spécifie la quantité d’informations sur le client ou le fournisseur (par exemple, l’adresse, le nom de la ville et le numéro de compte bancaire) sur la ligne feuille rapprochement bancaire qui doivent correspondre aux informations sur l’écriture ouverte avant que la règle de lettrage soit utilisée pour lettrer automatiquement le paiement avec l’écriture ouverte.|
|**Numéro de document/Ext. Numéro de document correspondant**|Spécifie si le texte de la ligne feuille rapprochement bancaire doit correspondre à la valeur du champ **N° document** ou du champ **N° document externe** sur l’écriture ouverte avant que la règle de lettrage soit utilisée pour lettrer automatiquement le paiement avec l’écriture ouverte.|
|**Nombre d’entrées dans la tolérance de montant trouvée**|Spécifie combien d’écritures pour un client ou un fournisseur doivent correspondre au montant (écart de règlement compris) avant que la règle de lettrage soit utilisée pour lettrer automatiquement un paiement avec l’écriture ouverte.|
|**Révision requise**|Spécifie si le lettrage de paiement automatique doit être révisé manuellement par l’utilisateur avant la validation. Choisissez le champ **Lignes à vérifier** sur la page **Feuille des applications de paiement** pour démarrer une expérience guidée dans laquelle vous pouvez facilement examiner plusieurs lettrages en série sur la page **Révision lettrage paiement**.|

Le tableau suivant décrit les règles de lettrage de paiement standard dans [!INCLUDE[prod_short](includes/prod_short.md)].

> [!Important]
> Les règles de lettrage de paiement peuvent être différentes dans votre implémentation de [!INCLUDE[prod_short](includes/prod_short.md)].

| Fiabilité correspondance | Priorité | Correspondance partie associée | N° document/N° document ext. rapprochés | Nombre d'écritures dans niveau de tolérance trouvées |
|------------------|----------|-----------------------|--------------------------------|--------------------------------|
| Haut             | 0        | Intégrale                 | Oui - Multiple                 | Une correspondance                      |
| Haut             | 2        | Intégrale                 | Oui - Multiple                 | Correspondances multiples               |
| Haut             | 3        | Intégrale                 | Oui                            | Une correspondance                      |
| Haut             | 4        | Intégrale                 | Oui                            | Correspondances multiples               |
| Haut             | 5        | Partielle             | Oui - Multiple                 | Une correspondance                      |
| Haut             | 6        | Partielle             | Oui - Multiple                 | Correspondances multiples               |
| Haut             | 7        | Partielle             | Oui                            | Une correspondance                      |
| Haut             | 8        | Intégrale                 | N°                             | Une correspondance                      |
| Haut             | 9        | N°                    | Oui - Multiple                 | Une correspondance                      |
| Haut             | 10       | N°                    | Oui - Multiple                 | Correspondances multiples               |
| Moyenne           | 0        | Intégrale                 | Oui - Multiple                 | Non applicable                 |
| Moyenne           | 2        | Intégrale                 | Oui                            | Non applicable                 |
| Moyenne           | 3        | Intégrale                 | N°                             | Correspondances multiples               |
| Moyenne           | 4        | Partielle             | Oui - Multiple                 | Non applicable                 |
| Moyenne           | 5        | Partielle             | Oui                            | Non applicable                 |
| Moyenne           | 6        | N°                    | Oui                            | Une correspondance                      |
| Moyenne           | 7        | N°                    | Oui-Multiple                   | Non applicable                 |
| Moyenne           | 8        | Partielle             | N°                             | Une correspondance                      |
| Moyenne           | 9        | N°                    | Oui                            | Non applicable                 |
| Mauvaises              | 0        | Intégrale                 | N°                             | Aucune correspondance                     |
| Mauvaises              | 2        | Partielle             | N°                             | Correspondances multiples               |
| Mauvaises              | 3        | Partielle             | N°                             | Aucune correspondance                     |
| Mauvaises              | 4        | N°                    | N°                             | Une correspondance                      |
| Mauvaises              | 5        | N°                    | N°                             | Correspondances multiples               |

## <a name="see-also"></a>Voir aussi
[Rapprocher les paiements à l'aide de l'application automatique](receivables-how-reconcile-payments-auto-application.md)  
[Gestion des comptes client](receivables-manage-receivables.md)  
[Ventes](sales-manage-sales.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
