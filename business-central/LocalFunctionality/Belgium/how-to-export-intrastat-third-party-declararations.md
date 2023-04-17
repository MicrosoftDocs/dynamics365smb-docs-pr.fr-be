---
title: 'Exporter les déclarations de tiers intracomm. [BE]'
description: 'En Belgique, un déclarant tiers doit renseigner la déclaration D.E.B (Intrastat). Le déclarant tiers doit être une personne ou une société externe.'
author: sorenfriisalexandersen
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 06/17/2021
ms.author: soalex
---
# Exporter des déclarations tierces intracommunautaires dans la version belge

[!INCLUDE[intrastat-2022w2](../../includes/intrastat-2022w2.md)]

En Belgique, un déclarant tiers doit renseigner la déclaration D.E.B (Intrastat). Le déclarant tiers doit être une personne ou une société externe.  

## Pour exporter la déclaration tierce

Avant d'exporter le fichier, il est conseillé d'afficher un aperçu de l'état. Pour plus d'informations, voir [Imprimer l'état du formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md).  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Feuilles intracommunautaires**, puis choisissez le lien associé.  
2. Choisissez l'action **Créer fichier**.  
3. Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Déclaration Nihil**|Sélectionnez ce champ si vous n'avez aucune transaction commerciale avec des pays/régions de l'Union européenne (UE) et que vous souhaitez envoyer une déclaration vide.|  
    |**Informations de contrepartie**|Activez ce champ pour inclure des informations de contrepartie dans le fichier de déclaration d'échanges de biens intracommunautaires (nouvelle exigence à partir de 2019). La déclaration de contrepartie ajoutée au fichier est issue des champs **Code pays/région origine** et **ID partenaire** de la Feuille intracomm.|  
    |**N° entreprise/N° id. intracomm.**|Entrez le numéro d'entreprise ou d'enregistrement de TVA.|  

4. Cliquez sur le bouton **OK**.  

Ensuite, envoyez la déclaration au portail OneGate.  

## Voir aussi

[États intracommunautaires belges](belgian-intrastat-reporting.md)  
[Paramétrer des types de déclarations](how-to-set-up-declaration-types.md)  
[Paramétrer les nomenclatures produits belges](how-to-set-up-belgian-tariff-numbers.md)  
[Paramétrer les numéros d'établissement intracommunautaires](how-to-set-up-intrastat-establishment-numbers.md)  
[Imprimer l'état Formulaire de D.E.B.](how-to-print-the-intrastat-form-report.md)  
[Paramétrer les états intracommunautaires](../../finance-how-setup-report-intrastat.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
