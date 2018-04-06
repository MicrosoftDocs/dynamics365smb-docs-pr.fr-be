---
title: "Comment limiter la période de validation"
description: "Vous pouvez limiter la période pour laquelle la validation est autorisée à trois niveaux différents : **Société**, **Utilisateur** et **Modèle**."
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
ms.openlocfilehash: df4fa3653ca223bb69aae104743d1ea77b297c3c
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="limit-the-posting-period"></a><span data-ttu-id="b3272-103">Limiter la période de validation</span><span class="sxs-lookup"><span data-stu-id="b3272-103">Limit the Posting Period</span></span>
<span data-ttu-id="b3272-104">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous pouvez limiter la période pour laquelle la validation est autorisée à trois niveaux différents : **Société**, **Utilisateur** et **Modèle**.</span><span class="sxs-lookup"><span data-stu-id="b3272-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can limit the period by which posting is permitted on three different levels: **by company**, **by user**, and **by template**.</span></span>  

<span data-ttu-id="b3272-105">Il peut être utile de limiter les périodes de validation lorsqu'une société clôture sa feuille vente à la fin de chaque mois.</span><span class="sxs-lookup"><span data-stu-id="b3272-105">Limiting posting periods can be useful when a company closes its sales journal at the end of each month.</span></span> <span data-ttu-id="b3272-106">Cela empêche les vendeurs d'enregistrer des documents vente du mois précédent.</span><span class="sxs-lookup"><span data-stu-id="b3272-106">This keeps salespeople from registering sales documents from the previous month.</span></span> <span data-ttu-id="b3272-107">Dans le même temps, la feuille achat peut rester ouverte pour enregistrer les factures achat entrantes du mois précédent.</span><span class="sxs-lookup"><span data-stu-id="b3272-107">At the same time, the purchase journal may stay open to register incoming purchase invoices from the previous month.</span></span>  

<span data-ttu-id="b3272-108">Lorsque vous effectuez une validation dans la fenêtre **Modèles feuille comptabilité**, le contenu des champs **Début période validation** et **Fin période validation** est vérifié pour obtenir un intervalle de dates.</span><span class="sxs-lookup"><span data-stu-id="b3272-108">When you post in the **General Journal Templates** window, the contents of the **Allow Posting From** field and **Allow Posting To** field are checked for a date interval.</span></span> <span data-ttu-id="b3272-109">L'intervalle de date indique à quel moment vous pouvez valider sur un modèle feuille.</span><span class="sxs-lookup"><span data-stu-id="b3272-109">The date interval indicates when you can post to a journal template.</span></span> <span data-ttu-id="b3272-110">Si le champ est vide, la fenêtre **Paramètres utilisateur** est vérifiée pour obtenir un intervalle de dates pour l'utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="b3272-110">If the field is blank, the **User Setup** window is checked for a date interval for the current user.</span></span> <span data-ttu-id="b3272-111">Si la fenêtre **Paramètres utilisateur** ne contient pas d'intervalle, les champs **Début période validation** et **Fin période validation** dans la fenêtre **Paramètres comptabilité** sont vérifiés pour obtenir un intervalle de dates au niveau de la société.</span><span class="sxs-lookup"><span data-stu-id="b3272-111">If the **User Setup** window does not contain an interval, the **Allow Posting From** field and the **Allow Posting To** field in the **General Ledger Setup** window is checked for a date interval at the company level.</span></span>  

## <a name="to-limit-the-posting-periods-by-company"></a><span data-ttu-id="b3272-112">Pour limiter les périodes de validation par société</span><span class="sxs-lookup"><span data-stu-id="b3272-112">To limit the posting periods by company</span></span>  

1.  <span data-ttu-id="b3272-113">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Paramètres comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="b3272-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b3272-114">Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle la validation sur la société est autorisée.</span><span class="sxs-lookup"><span data-stu-id="b3272-114">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which posting to the company is enabled.</span></span>  
3.  <span data-ttu-id="b3272-115">Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle la validation sur la société est autorisée.</span><span class="sxs-lookup"><span data-stu-id="b3272-115">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date on which posting to the company is enabled.</span></span>  

## <a name="to-limit-the-posting-periods-by-user"></a><span data-ttu-id="b3272-116">Pour limiter les périodes de validation par utilisateur</span><span class="sxs-lookup"><span data-stu-id="b3272-116">To limit the posting periods by user</span></span>  

1.  <span data-ttu-id="b3272-117">Choisissiez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres utilisateur**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="b3272-117">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b3272-118">Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle l'utilisateur peut effectuer la validation sur la société.</span><span class="sxs-lookup"><span data-stu-id="b3272-118">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which the user can post to the company.</span></span>  
3.  <span data-ttu-id="b3272-119">Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle l'utilisateur peut effectuer la validation sur la société.</span><span class="sxs-lookup"><span data-stu-id="b3272-119">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date the user will be able to post to the company.</span></span>  

## <a name="to-limit-the-posting-periods-by-template"></a><span data-ttu-id="b3272-120">Pour limiter les périodes de validation par modèle</span><span class="sxs-lookup"><span data-stu-id="b3272-120">To limit the posting periods by template</span></span>  

1.  <span data-ttu-id="b3272-121">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Modèles feuille comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="b3272-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b3272-122">Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle l'utilisateur peut effectuer la validation sur la société.</span><span class="sxs-lookup"><span data-stu-id="b3272-122">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which the user can post to the company.</span></span>  
3.  <span data-ttu-id="b3272-123">Pour spécifier la fin de la période, cliquez sur le champ **Fin période validation**, puis entrez la dernière date à laquelle l'utilisateur pourra procéder à une validation dans la société.</span><span class="sxs-lookup"><span data-stu-id="b3272-123">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date the user will be able to post to the company.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b3272-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3272-124">See Also</span></span>  
 <span data-ttu-id="b3272-125">[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="b3272-125">[Belgium Local Functionality](belgium-local-functionality.md) </span></span>  
 [<span data-ttu-id="b3272-126">Définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="b3272-126">Specify Posting Periods</span></span>](../../finance-how-specify-posting-periods.md)

