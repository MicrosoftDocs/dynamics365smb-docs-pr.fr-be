---
title: "Définition des plages de dates dans Business Central | Microsoft Docs"
description: "En savoir plus pour obtenir un état affichant les données de périodes spécifiques à l'aide de plages de dates dans Business Central."
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter
ms.date: 05/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 552578ce097f7f647ed0962fec0448059d3ca3b2
ms.contentlocale: fr-be
ms.lasthandoff: 03/22/2018

---
# <a name="entering-date-ranges"></a><span data-ttu-id="d8097-103">Saisie de plages de dates</span><span class="sxs-lookup"><span data-stu-id="d8097-103">Entering Date Ranges</span></span> 
<span data-ttu-id="d8097-104">Vous pouvez définir des filtres contenant une date de début et une date de fin pour afficher uniquement les données contenues dans cette plage de données ou cet intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="d8097-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="d8097-105">Des règles spéciales s'appliquent à la définition des plages de dates.</span><span class="sxs-lookup"><span data-stu-id="d8097-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="d8097-106">Prenons par exemple **Palmarès des clients** :</span><span class="sxs-lookup"><span data-stu-id="d8097-106">Let's take the **Customer Top 10** as an example:</span></span>

![Définition d'une plage de dates dans la page de demande de la liste du palmarès des clients](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="d8097-108">Vous pouvez limiter ici l'état à une plage de dates telles que les 2 dernières semaines, ou un total de 6 semaines, ou toute plage de votre choix.</span><span class="sxs-lookup"><span data-stu-id="d8097-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="d8097-109">Pour définir les plages de dates, vous entrez des dates puis utilisez **..**</span><span class="sxs-lookup"><span data-stu-id="d8097-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="d8097-110">ou **|** pour définir la plage.</span><span class="sxs-lookup"><span data-stu-id="d8097-110">or **|** to set the range.</span></span> <span data-ttu-id="d8097-111">Dans notre exemple, pour afficher les 10 clients principaux des deux premières semaines de mai, vous devez définir le filtre de date sur *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="d8097-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="d8097-112">Voici d'autres exemples :</span><span class="sxs-lookup"><span data-stu-id="d8097-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="d8097-113">Signification</span><span class="sxs-lookup"><span data-stu-id="d8097-113">Meaning</span></span> | <span data-ttu-id="d8097-114">Exemple :</span><span class="sxs-lookup"><span data-stu-id="d8097-114">Example</span></span> | <span data-ttu-id="d8097-115">Ecritures incluses</span><span class="sxs-lookup"><span data-stu-id="d8097-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="d8097-116">Egal à</span><span class="sxs-lookup"><span data-stu-id="d8097-116">Equal to</span></span>| <span data-ttu-id="d8097-117">15 12 16</span><span class="sxs-lookup"><span data-stu-id="d8097-117">12 15 16</span></span> |<span data-ttu-id="d8097-118">Uniquement les écritures validées le 15 décembre 2016.</span><span class="sxs-lookup"><span data-stu-id="d8097-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="d8097-119">Intervalle</span><span class="sxs-lookup"><span data-stu-id="d8097-119">Interval</span></span>| <span data-ttu-id="d8097-120">15 12 16..15 17 17</span><span class="sxs-lookup"><span data-stu-id="d8097-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="d8097-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="d8097-121">..12 15 16</span></span>|<span data-ttu-id="d8097-122">Celles validées entre le 15 décembre 2016 et le 15 janvier 2017 inclus.</span><span class="sxs-lookup"><span data-stu-id="d8097-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="d8097-123">Écritures validées le 15 décembre 2016 ou à une date antérieure.</span><span class="sxs-lookup"><span data-stu-id="d8097-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="d8097-124">Et/ou</span><span class="sxs-lookup"><span data-stu-id="d8097-124">Either/or</span></span>|<span data-ttu-id="d8097-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="d8097-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="d8097-126">Celles validées le 15 ou le 16 décembre 2016.</span><span class="sxs-lookup"><span data-stu-id="d8097-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="d8097-127">Les écritures validées aux deux dates sont également affichées.</span><span class="sxs-lookup"><span data-stu-id="d8097-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="d8097-128">Vous pouvez aussi combiner les divers types de format.</span><span class="sxs-lookup"><span data-stu-id="d8097-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="d8097-129">Exemple :</span><span class="sxs-lookup"><span data-stu-id="d8097-129">Example</span></span> | <span data-ttu-id="d8097-130">Ecritures incluses</span><span class="sxs-lookup"><span data-stu-id="d8097-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="d8097-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="d8097-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="d8097-132">Écritures validées le 15 décembre 2016 ou à des dates situées entre le 1er décembre 2016 et le 31 mai 2017 inclus.</span><span class="sxs-lookup"><span data-stu-id="d8097-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="d8097-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="d8097-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="d8097-134">Les écritures validées le 14 décembre ou avant, ou écritures validées le 30 décembre ou après, c.-à-d. toutes les écritures à l'exception de celles validées à des dates situées entre le 15 et le 29 décembre.</span><span class="sxs-lookup"><span data-stu-id="d8097-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="d8097-135">Remarquez que nous avons utilisé le format de date américaine MMJJAA.</span><span class="sxs-lookup"><span data-stu-id="d8097-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="d8097-136">A mesure que [!INCLUDE[d365fin](includes/d365fin_md.md)] deviendra disponible sur d'autres marché, vous pourrez utiliser les formats auxquels vous êtes habitué.</span><span class="sxs-lookup"><span data-stu-id="d8097-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="see-also"></a><span data-ttu-id="d8097-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8097-137">See Also</span></span>
<span data-ttu-id="d8097-138">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d8097-138">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="d8097-139">Saisir les critères pour les filtres</span><span class="sxs-lookup"><span data-stu-id="d8097-139">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="d8097-140">Fonctionnalités marché</span><span class="sxs-lookup"><span data-stu-id="d8097-140">General Business Functionality</span></span>](ui-across-business-areas.md)

