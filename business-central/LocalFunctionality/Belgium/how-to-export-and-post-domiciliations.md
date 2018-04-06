---
title: Comment exporter et valider des domiciliations
description: "Vous pouvez soumettre des domiciliations à votre banque en exportant les données dans un fichier. Lorsque vous effectuez un export vers un fichier, vous pouvez choisir de valider automatiquement les écritures comptables."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 940496c083e342f1ee88aecbfe0ad449ff830d65
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="export-and-post-domiciliations"></a>Exporter et valider les domiciliations
> [!Note]
> [!INCLUDE[onprem_only](../../includes/onprem_only_md.md)]

Vous pouvez envoyer des domiciliations à votre banque en exportant les données vers un fichier. Lorsque vous exportez les données dans un fichier, vous pouvez choisir de valider automatiquement les lignes en comptabilité.  

Selon la configuration du champ **Format exp. domiciliation européenne SEPA** dans la fenêtre **Fiche compte bancaire**, l'action **Fichier domiciliations** ouvre l'une des pages de requête suivantes :  

- Fenêtre **Créer lignes FS** : pour le format Domiciliation européenne SEPA.  
- Fenêtre **Fichier domiciliation** : pour les formats nationaux.  

## <a name="to-export-and-post-domiciliations-in-sepa-format"></a>Pour exporter et valider des domiciliations au format SEPA  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles saisie domiciliation**, puis sélectionnez le lien correspondant.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Fichier domiciliations**.  
3.  Dans la fenêtre **Créer lignes FS**, sélectionnez le raccourci **Options**, puis remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations seront validées.|  
    |**Feuille**|Sélectionnez le nom feuille comptabilité à partir duquel les lignes feuille seront transférées.|  
    |**Valider lignes FS**|Sélectionnez pour valider en comptabilité.|  

4.  Cliquez sur le bouton **OK** pour exporter le fichier.  
5.  Sélectionnez un emplacement adéquat depuis lequel vous téléchargez le fichier pour l'envoyer à votre banque, puis sélectionnez **Sauvegarder**.  
6.  Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.  

    Si vous n'avez pas activé la case à cocher **Valider lignes FS**, vous devrez valider les domiciliations manuellement en comptabilité.  

    > [!NOTE]  
    >  Après avoir validé les domiciliations en comptabilité, supprimez les domiciliations validées dans la fenêtre **Feuille de domiciliation**. Pour ce faire, sélectionnez toutes les lignes dont le statut est **Validé**, puis cliquez sur le bouton **Supprimer**.  

## <a name="to-export-and-post-domiciliations-in-isabel-format"></a>Pour exporter et valider des domiciliations au format Isabel  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles saisie domiciliation**, puis sélectionnez le lien correspondant.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Fichier domiciliations**.  
3.  Dans la fenêtre **Fichier domiciliations**, sélectionnez le raccourci **Options**, puis remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations seront validées.|  
    |**Feuille**|Sélectionnez le nom feuille comptabilité à partir duquel les lignes feuille seront transférées.|  
    |**Valider lignes FS**|Sélectionnez pour valider en comptabilité.|  
    |**Date pivot**|Entrez une date pivot si vous souhaitez que la date soit différente de la date de validation sur les lignes domiciliation. La date entrée écrasera la date de validation sur les lignes feuille sélectionnées.|  
    |**N° d'immatriculation**|Entrez le numéro d'inscription figurant sur la déclaration intracommunautaire (disquette). Le numéro est inclus dans le fichier et la note d'accompagnement.|  
    |**Nom du fichier**|Entrez le nom du fichier d'exportation que vous créez.|  

4.  Cliquez sur le bouton **Imprimer** pour exporter les domiciliations, puis imprimez la note d'accompagnement, ou cliquez sur le bouton **Aperçu** pour la consulter à l'écran. Si vous ne souhaitez pas exporter le fichier pour l'instant, cliquez sur le bouton **Annuler**.  
5.  Cliquez sur le bouton **OK** pour envoyer l'état à l'imprimante.  
6.  Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.  

    Si vous n'avez pas activé la case à cocher **Valider lignes FS**, vous devrez valider les domiciliations manuellement en comptabilité.  

    > [!NOTE]  
    >  Après avoir validé les domiciliations en comptabilité, supprimez les domiciliations validées dans la fenêtre **Feuille de domiciliation**. Pour cela, sélectionnez toutes les lignes ayant le statut **Validée**, puis choisissez le bouton **Supprimer**.  

## <a name="see-also"></a>Voir aussi  
 [Prélèvements bancaires avec domiciliation](direct-debit-using-domiciliation.md)   
 [Paramétrer les domiciliations](how-to-set-up-domiciliations.md)   
 [Générer les propositions de domiciliation](how-to-generate-domiciliation-suggestions.md)   
 [Tester les domiciliations](how-to-test-domiciliations.md)   
 [Modifier et supprimer des lignes de domiciliation](how-to-edit-and-delete-domiciliation-lines.md)

