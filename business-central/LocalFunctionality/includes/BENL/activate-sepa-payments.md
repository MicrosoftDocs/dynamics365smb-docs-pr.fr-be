---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 4830a9d3a70bc83c5f69e1746fd934803112e0ea
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 10/01/2020
ms.locfileid: "3916517"
---
Pour soumettre des paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA dans votre société.  

Les procédures suivantes décrivent comment paramétrer des paiements SEPA et comment modifier la configuration pour des fournisseurs spécifiques.  

## <a name="to-enable-countriesregions-for-sepa"></a>Pour activer des pays/régions pour SEPA  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Pays/Régions**, puis sélectionnez le lien associé.  
2. Choisissez l'action **Modifier la liste**.  
3. Activez la case à cocher **SEPA autorisé** pour chaque pays ou région que vous souhaitez activer pour SEPA.  
4. Cliquez sur le bouton **OK**.  

## <a name="to-enable-bank-accounts-for-sepa"></a>Pour activer des comptes bancaires pour SEPA  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Comptes bancaires**, puis sélectionnez le lien associé.  
2. Sélectionnez le compte bancaire que vous souhaitez activer pour SEPA, puis choisissez l'action **Modifier**.  
3. Dans le raccourci **Général**, dans le champ **Pays/Région**, sélectionnez le code adéquat.  

    > [!NOTE]  
    > Le code pays/région spécifié doit être activé pour SEPA, comme décrit dans la procédure précédente.  

4. Entrez une valeur dans le champ **Solde minimum**.  
5. Dans le raccourci **Transfert**, dans le champs **Code SWIFT**, entrez un code.  
6. Cliquez sur le bouton **OK**.  

## <a name="to-set-up-a-sepa-iso-20022-export-protocol"></a>Pour paramétrer un protocole d'exportation SEPA ISO 20022  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Protocoles d'exportation**, puis sélectionnez le lien associé.  
2. Sur la page **Protocoles d'exportation**, sélectionnez l'action **Nouveau**.  
3. Renseignez les champs. [!INCLUDE [tooltip-inline-tip_md](../../../includes/tooltip-inline-tip_md.md)]
4. Cliquez sur le bouton **OK**.  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a>Pour configurer des comptes bancaires fournisseur pour SEPA  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Fournisseurs**, puis sélectionnez le lien associé.  
2. Sélectionnez le fournisseur concerné, puis choisissez l'action **Comptes bancaires**.  
3. Sélectionnez le compte bancaire fournisseur à paramétrer pour SEPA, puis choisissez l'action **Modifier**.  
4. Dans le raccourci **Transfert**, dans les champs **IBAN** et **Code SWIFT**, entrez le code international d'identification bancaire ou la banque auprès de laquelle le fournisseur a son compte.  
5. Cliquez sur le bouton **OK**.  
