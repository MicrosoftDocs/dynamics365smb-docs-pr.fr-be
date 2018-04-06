---
title: "Comment imprimer des déclarations de TVA périodiques"
description: "La fonction de déclaration de TVA vous permet d'imprimer des détails sur les transactions TVA. Vous devez envoyer les déclarations de TVA suivantes aux autorités fiscales belges."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: c8bf10a154525eacabb126dd277aed8c137db7e8
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="print-periodic-vat-reports"></a>Imprimer des états TVA périodiques
Le report de TVA vous permet d'imprimer les détails de transaction TVA. Vous devez envoyer les déclarations TVA suivantes aux autorités fiscales belges :  

- Déclaration mensuelle/trimestrielle  
- Listing TVA annuel (sur papier/disquette)  
- Listing TVA-VIES (sur papier/disquette)  

## <a name="to-print-the-monthlyquarterly-declaration"></a>Pour imprimer la déclaration mensuelle/trimestrielle  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Décl. TVA - Formulaire/Intervat**, puis sélectionnez le lien correspondant.  
2.  Dans la fenêtre **TVA - Formulaire**, renseignez les champs.  

    |Champ|Description|  
    |------------------------------------|---------------------------------------|  
    |**N° de société incorrect**|Spécifie si vous souhaitez imprimer l'état qui contient des numéros d'entreprise erronés.|  
    |**Listing TVA annuel**|Spécifie si vous souhaitez imprimer l'état **Listing TVA annuel**.|  
    |**Année**|Entrez l'année de la période pour laquelle vous souhaitez imprimer l'état. Vous devez entrer l'année sous la forme d'un code à 4 chiffres. Par exemple, pour imprimer une déclaration pour 2013, entrez « 2013 » (et non « 13 »).|  
    |**Montant minimum**|Entrez le solde annuel minimal du client à inclure dans l'état. Si le solde annuel du client est inférieur au montant minimum, le client ne sera pas inclus dans la déclaration.|  
    |**Inclure clients de**|Sélectionnez cette option pour inclure dans l'état les clients de tous les pays/toutes les régions ou d'un pays/d'une région spécifique.|  
    |**Pays/région**|Sélectionnez le pays/la région à inclure dans l'état.|  

3.  Cliquez sur le bouton **Imprimer** pour imprimer l'état ou cliquez sur le bouton **Aperçu** pour le consulter à l'écran. Cliquez sur le bouton **Annuler** pour enregistrer les informations sans imprimer l'état.  

## <a name="to-print-the-vat-annual-listing-on-disk"></a>Pour imprimer le listing TVA annuel sur disquette  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Listing annuel - Disquette**, puis sélectionnez le lien correspondant.  
2.  Dans la fenêtre **Listing TVA annuel - Disquette**, remplissez les champs comme décrit dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Année**|Entrez l'année de la déclaration TVA. Vous devez entrer l'année sous la forme d'un code à quatre chiffres. Par exemple, pour imprimer une déclaration pour 2013, entrez « 2013 » (et non « 13 »).|  
    |**Minimale**|Entrez le solde annuel minimal du client à inclure dans l'état.<br /><br /> Si le solde annuel du client est inférieur au montant minimum, le client ne sera pas inclus dans la déclaration.|  
    |**Déclaration test**|Spécifie si vous souhaitez créer une déclaration test.<br /><br /> Si vous sélectionnez cette option, un attribut test utilisant la valeur 1 est écrit dans le fichier pour indiquer qu'il s'agit d'un fichier test. Si vous souhaitez tester le fichier XML avant de l'envoyer, vous pouvez télécharger ce fichier sur le site Intervat. Le fichier est alors validé sans être enregistré sur le serveur et vous recevez une notification si le fichier est valide. Par ailleurs, le numéro de séquence unique dans le fichier XML n'est pas incrémenté lorsqu'une déclaration test est créée, ce qui signifie que vous pouvez créer autant de déclarations test internes que vous le souhaitez.|  
    |**Ajouter représentant**|Spécifie si vous souhaitez inclure le représentant de la déclaration de TVA.<br /><br /> Un représentant est une personne ou une agence qui est habilitée à faire une déclaration de TVA pour votre société.|  
    |**ID**|Entrez l'ID du représentant qui est responsable de la rédaction de la déclaration de TVA.|  
    |**Nom du fichier**|Entrez le chemin et le nom du fichier dans lequel vous souhaitez créer la déclaration.|  

3.  Cliquez sur le bouton **Imprimer** pour imprimer l'état ou cliquez sur le bouton **Aperçu** pour le consulter à l'écran. Cliquez sur le bouton **Annuler** pour enregistrer les informations sans imprimer l'état.  

## <a name="to-print-the-vat-vies-declaration-report-to-disk"></a>Pour imprimer la déclaration TVA-VIES sur disquette  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **TVA - VIES : Déclaration (disquette)**, puis sélectionnez le lien correspondant.  
2.  Entrez les informations requises, puis cliquez sur le bouton **OK** pour lancer le traitement par lots qui créera un fichier XML. Pour plus d'informations, voir TVA - VIES : Déclaration (disquette).  
3.  Si vous devez apporter une correction, choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Correction TVA-VIES**, puis sélectionnez le lien correspondant.  
4.  Choisissez l'action **Modifier la liste**, puis entrez les informations qui doivent être modifiées. Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [TVA belge](belgian-vat.md)   
 [Configurer la TVA non déductible](how-to-set-up-non-deductible-vat.md)

