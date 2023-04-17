---
title: 'Tester les paiements électroniques [BE]'
description: 'Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d''eventuelles erreurs avant de les valider.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 2000001
ms.date: 06/17/2021
ms.author: edupont
---
# Tester les paiements électroniques dans la version belge

Après avoir paramétré les opérations bancaires électroniques et généré des suggestions de paiement, vous pouvez tester les lignes feuille paiement pour rechercher d'éventuelles erreurs avant de les valider.  

Certaines des informations validées sont les suivantes :  

- Si les numéros des comptes bancaires sont valides.  
- Si les lignes paiement positives sont présentes.  
- Si les paiements nationaux et internationaux sont effectués à partir d'un seul compte bancaire.  
- Si un seul compte bancaire peut être utilisé pour Isabel (Interbanks Standards Association Belgium).  
- Si des lignes de paiement sont en euros pour SEPA (Espace unique de paiement en euros).  
- Si une souche de numéros a été définie pour SEPA.  

Vous pouvez afficher les erreurs sur la page **Exporter/Vérifier les journaux des erreurs**.  

> [!IMPORTANT]  
> Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.  

## Pour tester les lignes feuille paiement  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles paiement**, puis choisissez le lien permettant d'ouvrir la page **Feuilles paiement EB**.  
2. Dans le champ **Nom de la feuille**, sélectionnez le nom de feuille comptabilité requis.  
3. Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.  
4. Entrez les informations sur les lignes feuille paiement, puis choisissez l'action **Vérifier lignes paiement** pour valider les lignes feuille paiement. La validation réalisée sur les lignes feuille dépend du type de vérification spécifié dans la page **Protocoles d'exportation**.  

## Voir aussi  

[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md)  
[Paiements électroniques belges](belgian-electronic-payments.md)  
[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)  
[Proposer paiements fournisseur](../../payables-how-suggest-vendor-payments.md)  
[Imprimer les fichiers de paiement](how-to-print-payment-files.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
