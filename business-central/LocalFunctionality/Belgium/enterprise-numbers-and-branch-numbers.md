---
title: Numéros d'entreprise et numéros d'établissement [BE]
description: Les sociétés reçoivent un numéro d'entreprise unique et un ou plusieurs numéros d'établissement de la Banque-Carrefour des Entreprises belge.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/25/2021
ms.author: edupont
ms.openlocfilehash: 4bac2b114bd0a2f5bce5d4905220f217ab9c6a57
ms.sourcegitcommit: 41876b559872fe7adbfa5b59a6e1a71dc907fb15
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 12/14/2021
ms.locfileid: "7921104"
---
# <a name="enterprise-numbers-and-branch-numbers-in-the-belgian-version"></a>Numéros d'entreprise et numéros d'établissement dans la version belge

Les sociétés reçoivent un numéro d'entreprise unique et un ou plusieurs numéros d'établissement de la [Banque-Carrefour des Entreprises](https://crossroadsbankenterprises.com/) belge. Ces numéros sont utilisés dans tous les échanges afin de simplifier la communication avec l'administration et les autorités juridiques belges.  

## <a name="enterprise-numbers"></a>Numéros d'entreprise

Le numéro d'entreprise remplace l'actuel numéro de TVA. Pour les sociétés existantes qui ont un numéro d'identification intracommunautaire, le numéro d'entreprise est défini comme le numéro d'identification intracommunautaire précédé d'un zéro. Les nouvelles sociétés recevront un nouveau numéro d'entreprise.  

Le numéro d'entreprise figure sur les documents suivants :  

- Documents vente et achat sortants  
- États financiers  
- Relances client et factures d'intérêts  
- Formulaires et fichiers intracommunautaires  

Le numéro d'entreprise est configuré aux emplacements suivants :  

- Table informations société  
- Fiche contact  
- Table client  
- Table fournisseur  

## <a name="branch-numbers"></a>Numéros d'établissement

Un numéro d'établissement est délivré à une société pour identifier une adresse où au moins une des activités de la société est exercée, par exemple, un atelier, un bureau, un entrepôt, une agence ou une filiale. Contrairement au numéro d'entreprise, le numéro d'établissement ne doit pas obligatoirement être imprimé.  

Tous les établissements d'une société recevront un numéro unique, différent du numéro d'entreprise. Le numéro d'établissement peut être transféré à une autre société, notamment après une fusion ou un rachat.  

Le numéro d'établissement est configuré aux emplacements suivants :  

- Table informations société  
- Table magasin  

## <a name="see-also"></a>Voir aussi

[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)
[Banque-Carrefour des Entreprises](https://kruispuntdatabank.be/)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]