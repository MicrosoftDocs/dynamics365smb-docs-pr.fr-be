---
title: 'Paiements électroniques, Belgique'
description: 'Dans le module bancaire électronique de la version belge de Business Central, vous pouvez effectuer des paiements électroniques nationaux, internationaux, SEPA et SEPA hors euro.'
author: brentholtorf
ms.topic: conceptual
ms.search.keywords: null
ms.search.form: 2000006
ms.date: 11/27/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---

# <a name="belgian-electronic-payments"></a>Paiements électroniques, Belgique

Dans la version belge de [!INCLUDE[prod_short](../../includes/prod_short.md)], vous pouvez effectuer les types de paiements électroniques suivants :  

|Paiement électronique|Description|  
|------------------------|---------------------------------------|  
|National|Une institution financière locale traite ces paiements dans la devise société (DS) pour les bénéficiaires qui ont des comptes auprès d'une institution financière locale. [!INCLUDE[prod_short](../../includes/prod_short.md)] vérifie la validité des numéros de compte bancaire.|  
|International|Une institution financière locale traite ces paiements qui sont en devises étrangères ou en devise société (DS) pour les bénéficiaires qui ont des comptes auprès d'institutions financières étrangères. [!INCLUDE[prod_short](../../includes/prod_short.md)] vérifie la validité des numéros de compte bancaire.|  
|SEPA|Ces paiements sont en euros et sont traités dans les pays/régions qui acceptent les paiements SEPA. [!INCLUDE[prod_short](../../includes/prod_short.md)] vérifie la validité des numéros de compte bancaire.|  
|SEPA hors euro|Ces paiements sont dans une devise autre que l'euro et sont traités dans les pays/régions en dehors de l'Association économique européenne (AEE). [!INCLUDE[prod_short](../../includes/prod_short.md)] vérifie la validité des numéros de compte bancaire.|  

Étant donné que la norme pour les paiements électroniques diffère selon les pays/régions, seules les institutions financières en Belgique peuvent traiter les paiements électroniques créés dans la version belge de [!INCLUDE[prod_short](../../includes/prod_short.md)]. Les institutions financières locales traitent le paiement auprès des institutions étrangères pour les paiements internationaux.  

> [!NOTE]  
> Les avoirs ne peuvent pas être traités séparément, car les paiements ne doivent pas avoir un solde négatif. Pour traiter un avoir, celui-ci doit être ajouté à une ou plusieurs factures en totalisant les paiements.  

Avant de pouvoir effectuer des paiements électroniques, vous devez paramétrer le système bancaire électronique. Pour plus d'informations, reportez-vous à [Configuration](belgian-electronic-banking.md#setup). Vous devez également spécifier les protocoles d'exportation appropriés. Pour plus d'informations, voir [Paramétrer les protocoles d'exportation](how-to-set-up-export-protocols.md).  

## <a name="activate-sepa-payments-in-the-belgian-version"></a>Activer des paiements SEPA dans la version belge

[!INCLUDE [activate-sepa-payments](../includes/BENL/activate-sepa-payments.md)]

Vous pouvez à présent effectuer des paiements SEPA. Pour plus d'informations, reportez-vous à [Exportation de paiements vers un fichier bancaire](../../finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file). Si vous n'utilisez pas la fonctionnalité AC Banking 365, vous pouvez exporter des lignes feuille paiement vers un fichier. Pour plus d'informations, reportez-vous à [Exporter des fichiers de paiement](how-to-print-payment-files.md).  

## <a name="file-non-euro-sepa-payments"></a>Classer les paiements SEPA non libellés en Euro

Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], vous pouvez effectuer des paiements SEPA hors euro auprès de la banque. Cela est utile lorsque vous effectuez des paiements vers d'autres pays/régions qui n'utilisent pas SEPA et pour les devises autres que l'euro.  

Avant de pouvoir effectuer un paiement SEPA hors euro, vous devez effectuer les tâches d'administration suivantes :  

- Paramétrez un nouveau protocole d'exportation pour un paiement SEPA hors euro.  
- Dans la table **Pays/région**, désactivez le champ **SEPA autorisé** pour chaque pays appartenant à la zone AEE.  
- Sur la page **Paramètres comptabilité**, vérifiez que le champ **Devise euro** est vide et que le champ **Exportation non-euro SEPA** est sélectionné.  
- Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient l'IBAN et le code SWIFT.  

## <a name="to-file-a-non-euro-sepa-payment"></a>Pour effectuer un paiement SEPA hors euro

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Effectuer des paiements SEPA hors euro**, puis choisissez le lien associé.  
2. Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA hors euro.|  
    |**Feuille**|Spécifiez la feuille comptabilité pour l'état de paiement SEPA hors euro.|  
    |**Valider les lignes feuille comptabilité**|Spécifiez si vous souhaitez transférer les lignes paiement vers la comptabilité.|  
    |**Inclure axes**|Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA hors euro. L'option n'est disponible que si le champ **Totaliser lignes feuille compta.** dans la page **Paramétrage des opérations bancaires électroniques** est sélectionné.|  
    |**Date d'exécution**|Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date comptabilisation sur les lignes paiement.|  
    |**Emplacement**|Entrez le nom du fichier, y compris le lecteur et le dossier, dans lequel vous souhaitez imprimer l'état.|  

## <a name="correct-payment-lines"></a>Corriger des lignes de paiement

Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes de paiement électronique. Vous pouvez corriger les lignes de paiement comme suit :  

|Correction|Désignation|  
|----------------|---------------------------------------|  
|Ajouter une ligne feuille paiement|Si la feuille paiement contient déjà plusieurs lignes et que vous souhaitez ajouter une ligne supplémentaire, vous pouvez entrer la ligne feuille manuellement. Par exemple, si vous souhaitez rembourser un avoir à un client. Ces types de paiements client ne sont pas proposés automatiquement par le traitement par lots **Proposer paiements fournisseur**.|  
|Modifier une ligne feuille paiement|Si vous n'affectez pas un compte bancaire à la feuille paiement ou si vous ne spécifiez pas de compte bancaire préféré sur la fiche fournisseur, vous devez entrer manuellement ces informations sur chaque ligne feuille avant de valider la feuille. Si vous spécifiez un compte bancaire pour un fournisseur, le compte bancaire est copié sur toutes les lignes feuille paiement de ce fournisseur. Pour plus d'informations, reportez-vous à [Configuration](belgian-electronic-banking.md#setup).|  
|Supprimer une ligne feuille paiement|Le traitement par lots **Proposer paiements fournisseur** crée des propositions de paiement pour tous les fournisseurs répondant aux critères spécifiés. Si vous souhaitez empêcher le paiement pour une écriture comptable fournisseur ou un fournisseur spécifique, vous pouvez supprimer les lignes feuille correspondantes.|  


## <a name="see-also"></a>Voir aussi

[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)  
[Opérations bancaires électroniques, Belgique](belgian-electronic-banking.md)  
[Paramétrer les fournisseurs pour des suggestions de règlement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)  
[Proposer paiements fournisseur](../../payables-how-suggest-vendor-payments.md)  
[Créer des modèles et des lots de feuilles paiement](how-to-create-payment-journal-templates-and-batches.md)  
[Tester les paiements électroniques](how-to-test-electronic-payments.md)  
[Imprimer les fichiers de paiement](how-to-print-payment-files.md)  
