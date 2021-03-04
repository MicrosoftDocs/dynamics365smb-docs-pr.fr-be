---
title: Exportation et validation des domiciliations
description: Vous pouvez soumettre des domiciliations à votre banque en exportant les données dans un fichier. Lorsque vous exportez les données dans un fichier, vous pouvez choisir de valider automatiquement les lignes dans la comptabilité.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 935e7d2c7a244703e3aa75ac789bd3ec5ab661b6
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 10/01/2020
ms.locfileid: "3914003"
---
# <a name="export-and-post-domiciliations"></a>Exporter et valider les domiciliations
Vous pouvez soumettre des domiciliations à votre banque en exportant les données dans un fichier. Lorsque vous exportez les données dans un fichier, vous pouvez choisir de valider automatiquement les lignes dans la comptabilité.  

Selon le paramétrage du champ **Format exp. prélèvement SEPA** dans la page **Fiche compte bancaire**, l'action **Domiciliations de fichier** ouvre l'une des pages de demande suivantes :  

- Page**Créer des lignes feuille comptabilité** – pour le format de prélèvement SEPA.  
- Page**Domiciliations de fichier** – pour les formats nationaux.  

## <a name="to-export-and-post-domiciliations-in-sepa-format"></a>Pour exporter et valider les domiciliations au format SEPA  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles domiciliation**, puis sélectionnez le lien associé.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Domiciliations de fichier**.  
3.  Sur la page **Créer des lignes feuille comptabilité**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations sont validées.|  
    |**Feuille**|Sélectionnez la feuille comptabilité à partir de laquelle les lignes feuille sont transférées.|  
    |**Valider les lignes feuille comptabilité**|Sélectionnez ce champ pour valider les lignes feuille dans la comptabilité.|  

4.  Cliquez sur le bouton **OK** pour exporter le fichier.  
5.  Choisissez un emplacement approprié à partir duquel vous téléchargez le fichier vers votre banque, puis choisissez **Enregistrer**.  
6.  Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.  

    Si vous n'activez pas la case à cocher **Valider les lignes feuille comptabilité**, vous devrez valider les domiciliations manuellement dans la feuille comptabilité.  

    > [!NOTE]  
    >  Après avoir validé les domiciliations dans la feuille comptabilité, supprimez les domiciliations validées dans la page **Feuille domiciliation**. Pour ce faire, sélectionnez toutes les lignes avec le statut **Validé**, puis cliquez sur le bouton **Supprimer**.  

## <a name="to-export-and-post-domiciliations-in-isabel-format"></a>Pour exporter et valider les domiciliations au format Isabel  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuilles domiciliation**, puis sélectionnez le lien associé.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille requise, puis choisissez l'action **Domiciliations de fichier**.  
3.  Dans la page **Domiciliations de fichier**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Sélectionnez le modèle feuille comptabilité à partir duquel les domiciliations sont validées.|  
    |**Feuille**|Sélectionnez la feuille comptabilité à partir de laquelle les lignes feuille sont transférées.|  
    |**Valider les lignes feuille comptabilité**|Sélectionnez ce champ pour valider les lignes feuille dans la comptabilité.|  
    |**Date pivot**|Entrez une date pivot si vous souhaitez que la date soit différente de la date comptabilisation sur les lignes de domiciliation. La date saisie remplace la date comptabilisation sur les lignes feuille sélectionnées.|  
    |**N° inscription**|Entrez le numéro d'inscription qui figure sur le disque de déclaration intracommunautaire. Le numéro figure dans le fichier et sur la note jointe.|  
    |**Emplacement**|Entrez le nom du fichier d'exportation que vous créez.|  

4.  Cliquez sur le bouton **Imprimer** pour exporter les domiciliations et imprimer la note jointe, ou cliquez sur le bouton **Aperçu** pour l'afficher à l'écran. Si vous ne souhaitez pas exporter le fichier maintenant, cliquez sur le bouton **Annuler**.  
5.  Cliquez sur le bouton **OK** pour envoyer l'état vers l'imprimante.  
6.  Cliquez sur le bouton **Oui** pour valider automatiquement les lignes feuille domiciliation.  

    Si vous n'activez pas la case à cocher **Valider les lignes feuille comptabilité**, vous devrez valider les domiciliations manuellement dans la feuille comptabilité.  

    > [!NOTE]  
    >  Après avoir validé les domiciliations dans la feuille comptabilité, supprimez les domiciliations validées dans la page **Feuille domiciliation**. Pour ce faire, sélectionnez toutes les lignes avec le statut **Validé**, puis cliquez sur le bouton **Supprimer**.  

## <a name="see-also"></a>Voir aussi  
 [Prélévement à l'aide de la domiciliation](direct-debit-using-domiciliation.md)   
 [Paramétrer les domiciliations](how-to-set-up-domiciliations.md)   
 [Générer les propositions de domiciliation](how-to-generate-domiciliation-suggestions.md)   
 [Tester les domiciliations](how-to-test-domiciliations.md)   
 [Modifier et supprimer les lignes domiciliation](how-to-edit-and-delete-domiciliation-lines.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]