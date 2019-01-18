---
title: "Limitation de la période de validation"
description: "Vous pouvez limiter la période de validation autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 5306359e022a7d86f93c06971db9a14ca8f861db
ms.contentlocale: fr-be
ms.lasthandoff: 11/26/2018

---
# <a name="limit-the-posting-period"></a><span data-ttu-id="6e13d-103">Limiter la période de validation</span><span class="sxs-lookup"><span data-stu-id="6e13d-103">Limit the Posting Period</span></span>
<span data-ttu-id="6e13d-104">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez limiter la période de validation autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**.</span><span class="sxs-lookup"><span data-stu-id="6e13d-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can limit the period by which posting is permitted on three different levels: **by company**, **by user**, and **by template**.</span></span>  

<span data-ttu-id="6e13d-105">Limiter les périodes de validation peut être utile lorsqu'une société clôture sa feuille vente à la fin de chaque mois.</span><span class="sxs-lookup"><span data-stu-id="6e13d-105">Limiting posting periods can be useful when a company closes its sales journal at the end of each month.</span></span> <span data-ttu-id="6e13d-106">Cela empêche les vendeurs d'enregistrer les documents vente du mois précédent.</span><span class="sxs-lookup"><span data-stu-id="6e13d-106">This keeps salespeople from registering sales documents from the previous month.</span></span> <span data-ttu-id="6e13d-107">Par ailleurs, la feuille achat peut rester ouverte pour enregistrer les factures achat entrantes du mois précédent.</span><span class="sxs-lookup"><span data-stu-id="6e13d-107">At the same time, the purchase journal may stay open to register incoming purchase invoices from the previous month.</span></span>  

<span data-ttu-id="6e13d-108">Lorsque vous validez des écritures dans la page **Modèles feuille comptabilité**, le contenu du champ **Début période validation** et du champ **Fin période validation** est activé pour un intervalle de dates.</span><span class="sxs-lookup"><span data-stu-id="6e13d-108">When you post on the **General Journal Templates** page, the contents of the **Allow Posting From** field and **Allow Posting To** field are checked for a date interval.</span></span> <span data-ttu-id="6e13d-109">L'intervalle de dates indique quand vous pouvez valider des écritures dans un modèle feuille.</span><span class="sxs-lookup"><span data-stu-id="6e13d-109">The date interval indicates when you can post to a journal template.</span></span> <span data-ttu-id="6e13d-110">Si le champ est vide, la page **Paramètres utilisateur** est activée pour un intervalle de dates pour l'utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="6e13d-110">If the field is blank, the **User Setup** page is checked for a date interval for the current user.</span></span> <span data-ttu-id="6e13d-111">Si la page **Paramètres utilisateur** ne contient pas d'intervalle, le champ **Début période validation** et le champ **Fin période validation** dans la page **Paramètres comptabilité** sont activés pour un intervalle de dates au niveau de la société.</span><span class="sxs-lookup"><span data-stu-id="6e13d-111">If the **User Setup** page does not contain an interval, the **Allow Posting From** field and the **Allow Posting To** field on the **General Ledger Setup** page is checked for a date interval at the company level.</span></span>  

## <a name="to-limit-the-posting-periods-by-company"></a><span data-ttu-id="6e13d-112">Pour limiter les périodes de validation par société</span><span class="sxs-lookup"><span data-stu-id="6e13d-112">To limit the posting periods by company</span></span>  

1.  <span data-ttu-id="6e13d-113">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="6e13d-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6e13d-114">Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle la validation dans la société est activée.</span><span class="sxs-lookup"><span data-stu-id="6e13d-114">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which posting to the company is enabled.</span></span>  
3.  <span data-ttu-id="6e13d-115">Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle la validation dans la société est activée.</span><span class="sxs-lookup"><span data-stu-id="6e13d-115">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date on which posting to the company is enabled.</span></span>  

## <a name="to-limit-the-posting-periods-by-user"></a><span data-ttu-id="6e13d-116">Pour limiter les périodes de validation par utilisateur</span><span class="sxs-lookup"><span data-stu-id="6e13d-116">To limit the posting periods by user</span></span>  

1.  <span data-ttu-id="6e13d-117">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres utilisateur**, puis choisissez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="6e13d-117">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6e13d-118">Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle l'utilisateur peut valider dans la société.</span><span class="sxs-lookup"><span data-stu-id="6e13d-118">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which the user can post to the company.</span></span>  
3.  <span data-ttu-id="6e13d-119">Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle l'utilisateur peut valider dans la société.</span><span class="sxs-lookup"><span data-stu-id="6e13d-119">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date the user will be able to post to the company.</span></span>  

## <a name="to-limit-the-posting-periods-by-template"></a><span data-ttu-id="6e13d-120">Pour limiter les périodes de validation par modèle</span><span class="sxs-lookup"><span data-stu-id="6e13d-120">To limit the posting periods by template</span></span>  

1.  <span data-ttu-id="6e13d-121">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="6e13d-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6e13d-122">Pour spécifier le début de la période, sélectionnez le champ **Début période validation**, puis entrez la date la plus proche à laquelle l'utilisateur peut valider dans la société.</span><span class="sxs-lookup"><span data-stu-id="6e13d-122">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which the user can post to the company.</span></span>  
3.  <span data-ttu-id="6e13d-123">Pour spécifier la fin de la période, sélectionnez le champ **Fin période validation**, puis entrez la date limite à laquelle l'utilisateur peut valider dans la société.</span><span class="sxs-lookup"><span data-stu-id="6e13d-123">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date the user will be able to post to the company.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6e13d-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6e13d-124">See Also</span></span>  
 <span data-ttu-id="6e13d-125">[Fonctionnalité locale, Belgique](belgium-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="6e13d-125">[Belgium Local Functionality](belgium-local-functionality.md) </span></span>  
 [<span data-ttu-id="6e13d-126">Définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="6e13d-126">Specify Posting Periods</span></span>](../../finance-how-specify-posting-periods.md)

