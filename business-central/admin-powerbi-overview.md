---
title: Vue d’ensemble Architecture et composant d’intégration Power BI pour Business Central| Microsoft Docs
description: Il est facile d’obtenir des informations exploitables, de la veille économique et des KPI de vos applications Business Central pour Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: 9514f0355932c1b1cbd30acfdb9f6dab46db8a0a
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: fr-BE
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697827"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prodshort"></a><span data-ttu-id="d8f31-103">Vue d’ensemble Architecture et composant d’intégration Power BI pour [!INCLUDE[prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="d8f31-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prodshort](includes/prodshort.md)]</span></span>

<span data-ttu-id="d8f31-104">Dans cet article, vous découvrirez les différents aspects de l’intégration de Power BI à [!INCLUDE[prodshort](includes/prodshort.md)] pour vous aider à comprendre sa mise en œuvre et son utilisation.</span><span class="sxs-lookup"><span data-stu-id="d8f31-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prodshort](includes/prodshort.md)] to help you understand its implementation and use.</span></span>

## <a name="components"></a><span data-ttu-id="d8f31-105">Composants</span><span class="sxs-lookup"><span data-stu-id="d8f31-105">Components</span></span>

<span data-ttu-id="d8f31-106">Le tableau suivant décrit les principaux composants impliqués dans l’intégration Power BI.</span><span class="sxs-lookup"><span data-stu-id="d8f31-106">The following table describes the major components involved with Power BI integration.</span></span>

|<span data-ttu-id="d8f31-107">Composant</span><span class="sxs-lookup"><span data-stu-id="d8f31-107">Component</span></span>|<span data-ttu-id="d8f31-108">Description</span><span class="sxs-lookup"><span data-stu-id="d8f31-108">Description</span></span>|
|---------|-----------|
|<span data-ttu-id="d8f31-109">Power BI</span><span class="sxs-lookup"><span data-stu-id="d8f31-109">Power BI</span></span>|<span data-ttu-id="d8f31-110">Un service d’hébergement et de gestion des états basé sur le cloud.</span><span class="sxs-lookup"><span data-stu-id="d8f31-110">A cloud-based report hosting and management service.</span></span>|
|<span data-ttu-id="d8f31-111">Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="d8f31-111">Power BI Desktop</span></span>|<span data-ttu-id="d8f31-112">Un outil de création pour créer des états et des tableaux de bord, et vous permet d’exécuter des états.</span><span class="sxs-lookup"><span data-stu-id="d8f31-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span></span> <span data-ttu-id="d8f31-113">Il est disponible en téléchargement gratuit sur Microsoft Store et est installé localement.</span><span class="sxs-lookup"><span data-stu-id="d8f31-113">It's available as a free download on Microsoft Store and is installed locally.</span></span>|
|[!INCLUDE[prodshort](includes/prodshort.md)]|<span data-ttu-id="d8f31-114">Solution en ligne ou sur site avec des connecteurs exposés à Power BI et possibilité d’intégrer une partie de Power BI.</span><span class="sxs-lookup"><span data-stu-id="d8f31-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span></span>|

## <a name="whats-available-from-the-start"></a><span data-ttu-id="d8f31-115">Ce qui est disponible dès le départ</span><span class="sxs-lookup"><span data-stu-id="d8f31-115">What's available from the start</span></span>

<span data-ttu-id="d8f31-116">Le tableau suivant décrit les fonctionnalités disponibles.</span><span class="sxs-lookup"><span data-stu-id="d8f31-116">The following table describes available features.</span></span>

|<span data-ttu-id="d8f31-117">Fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="d8f31-117">Feature</span></span>|<span data-ttu-id="d8f31-118">Support [!INCLUDE[prodshort](includes/prodshort.md)] en ligne ou sur site</span><span class="sxs-lookup"><span data-stu-id="d8f31-118">[!INCLUDE[prodshort](includes/prodshort.md)] online or on-premises support</span></span>|
|-------|---------------------|
|<span data-ttu-id="d8f31-119">Connecteurs Power BI</span><span class="sxs-lookup"><span data-stu-id="d8f31-119">Power BI connectors</span></span>|<span data-ttu-id="d8f31-120">Les deux.</span><span class="sxs-lookup"><span data-stu-id="d8f31-120">Both.</span></span> <span data-ttu-id="d8f31-121">Différents connecteurs pour la solution ligne et la solution sur site.</span><span class="sxs-lookup"><span data-stu-id="d8f31-121">Different connectors for online and on-premises.</span></span> <span data-ttu-id="d8f31-122">Connecteur identique utilisé pour le service Power BI Desktop et Power BI</span><span class="sxs-lookup"><span data-stu-id="d8f31-122">Same connector used for Power BI Desktop and Power BI Service</span></span> |
|<span data-ttu-id="d8f31-123">Expérience intégrée pour afficher un état donné dans un Récapitulatif dans [!INCLUDE[prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="d8f31-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prodshort](includes/prodshort.md)]</span></span>|<span data-ttu-id="d8f31-124">Les deux.</span><span class="sxs-lookup"><span data-stu-id="d8f31-124">Both.</span></span> <span data-ttu-id="d8f31-125">Nécessite une configuration pour afficher les états sur site.</span><span class="sxs-lookup"><span data-stu-id="d8f31-125">Requires configuration to display reports for on-premises.</span></span>|
|<span data-ttu-id="d8f31-126">Gestion des états Power BI depuis [!INCLUDE[prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="d8f31-126">Power BI report management from [!INCLUDE[prodshort](includes/prodshort.md)]</span></span>|<span data-ttu-id="d8f31-127">En ligne</span><span class="sxs-lookup"><span data-stu-id="d8f31-127">Online</span></span>|
|<span data-ttu-id="d8f31-128">États Power BI par défaut sur les tableaux de bord déployés vers Power BI</span><span class="sxs-lookup"><span data-stu-id="d8f31-128">Default Power BI reports on role centers deployed to Power BI</span></span>|<span data-ttu-id="d8f31-129">En ligne</span><span class="sxs-lookup"><span data-stu-id="d8f31-129">Online</span></span>|
|<span data-ttu-id="d8f31-130">Applications Power BI sur Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="d8f31-130">Power BI Apps on Microsoft AppSource</span></span>|<span data-ttu-id="d8f31-131">En ligne.</span><span class="sxs-lookup"><span data-stu-id="d8f31-131">Online.</span></span>|

## <a name="architecture"></a><span data-ttu-id="d8f31-132">Architecture</span><span class="sxs-lookup"><span data-stu-id="d8f31-132">Architecture</span></span>

[!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="d8f31-133">s’intègre à Power BI via un connecteur utilisant OData.</span><span class="sxs-lookup"><span data-stu-id="d8f31-133">integrates with Power BI through a connector using OData.</span></span> <span data-ttu-id="d8f31-134">La source de données pour les états Power BI est exposée comme services Web OData.</span><span class="sxs-lookup"><span data-stu-id="d8f31-134">The data source for Power BI reports is exposed as OData web services.</span></span>

![Architecture Power BI pour l’intégration avec Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a><span data-ttu-id="d8f31-136">Flux général</span><span class="sxs-lookup"><span data-stu-id="d8f31-136">General Flow</span></span>

<span data-ttu-id="d8f31-137">Le diagramme suivant illustre le flux de travail de base pour les utilisateurs lors de la connexion de [!INCLUDE[prodshort](includes/prodshort.md)] à Power BI.</span><span class="sxs-lookup"><span data-stu-id="d8f31-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prodshort](includes/prodshort.md)] to Power BI.</span></span>

![Flux de travai Power BI pour l’intégration avec Business Central](./media/power-bi-flow.png)

1. <span data-ttu-id="d8f31-139">L’utilisateur s’inscrit à un compte Power BI.</span><span class="sxs-lookup"><span data-stu-id="d8f31-139">User signs up for a Power BI account.</span></span>
2. <span data-ttu-id="d8f31-140">L’utilisateur se connecte à Power BI depuis [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="d8f31-140">User connects to Power BI from [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>
3. [!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="d8f31-141">vérifie la licence.</span><span class="sxs-lookup"><span data-stu-id="d8f31-141">verifies the license.</span></span>
4. [!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="d8f31-142">déploie les états par défaut sur le service Power BI.</span><span class="sxs-lookup"><span data-stu-id="d8f31-142">deploys default reports to the Power BI service.</span></span> <span data-ttu-id="d8f31-143">Cette étape ne se produit que pour [!INCLUDE[prodshort](includes/prodshort.md)] en ligne.</span><span class="sxs-lookup"><span data-stu-id="d8f31-143">This step only happens for [!INCLUDE[prodshort](includes/prodshort.md)] online.</span></span>
5. [!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="d8f31-144">rend les états dans Power BI disponibles pour la sélection dans [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="d8f31-144">makes reports in Power BI available for selection in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="d8f31-145">Les états par défaut sont automatiquement affichés dans des parties de Power BI.</span><span class="sxs-lookup"><span data-stu-id="d8f31-145">Default reports are automatically displayed in Power BI parts.</span></span>
6. <span data-ttu-id="d8f31-146">L’utilisateur crée un état dans Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="d8f31-146">User creates a report in Power BI Desktop.</span></span>
7. <span data-ttu-id="d8f31-147">L’utilisateur publie l’état vers le service Power BI.</span><span class="sxs-lookup"><span data-stu-id="d8f31-147">User publishes the report to the Power BI service.</span></span> <span data-ttu-id="d8f31-148">Les états sont ensuite disponibles pour la sélection dans [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="d8f31-148">The reports are then available for selection in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="d8f31-149">Voir la formation associée sur [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="d8f31-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="d8f31-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8f31-150">See Also</span></span>

[<span data-ttu-id="d8f31-151">Business Central et Power BI</span><span class="sxs-lookup"><span data-stu-id="d8f31-151">Business Central and Power BI</span></span>](admin-powerbi.md)  
[<span data-ttu-id="d8f31-152">Power BI pour les consommateurs</span><span class="sxs-lookup"><span data-stu-id="d8f31-152">Power BI for consumers</span></span>](/power-bi/consumer/end-user-consumer)  
[<span data-ttu-id="d8f31-153">Le « nouveau look » du service Power BI</span><span class="sxs-lookup"><span data-stu-id="d8f31-153">The 'new look' of the Power BI service</span></span>](/power-bi/service-new-look)  
[<span data-ttu-id="d8f31-154">Démarrage rapide : Se connecter aux données dans Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="d8f31-154">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
[<span data-ttu-id="d8f31-155">Documentation Power BI</span><span class="sxs-lookup"><span data-stu-id="d8f31-155">Power BI documentation</span></span>](/power-bi/)  
[<span data-ttu-id="d8f31-156">Veille économique</span><span class="sxs-lookup"><span data-stu-id="d8f31-156">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="d8f31-157">Mise en route</span><span class="sxs-lookup"><span data-stu-id="d8f31-157">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="d8f31-158">Importation des données métier à partir d'autres systèmes financiers</span><span class="sxs-lookup"><span data-stu-id="d8f31-158">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="d8f31-159">[Configuration de [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="d8f31-159">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
<span data-ttu-id="d8f31-160">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)] comme source de données Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="d8f31-160">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
<span data-ttu-id="d8f31-161">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)] comme source de données Power Apps](across-how-use-financials-data-source-powerapps.md)</span><span class="sxs-lookup"><span data-stu-id="d8f31-161">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span></span>  
<span data-ttu-id="d8f31-162">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)] dans Power Automate](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="d8f31-162">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  