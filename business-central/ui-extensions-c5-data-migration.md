---
title: Utilisation de l'extension C5 Data Migration | Microsoft Docs
description: "Utilisez cette extension pour migrer des clients, des fournisseurs, des articles et des comptes généraux de Microsoft Dynamics C5 2012 vers Business Central."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 04/09/208
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: fa6779ee8fb2bbb453014e32cb7f3cf8dcfa18da
ms.openlocfilehash: 698bde6949c6053501881d07135586810fc81bdd
ms.contentlocale: fr-be
ms.lasthandoff: 04/11/2018

---

# <a name="the-c5-data-migration-extension-for-business-central"></a><span data-ttu-id="416fd-103">Extension C5 Data Migration pour Business Central</span><span class="sxs-lookup"><span data-stu-id="416fd-103">The C5 Data Migration Extension for Business Central</span></span>
<span data-ttu-id="416fd-104">Cette extension facilite la migration de clients, de fournisseurs, d'articles et de vos comptes généraux de Microsoft Dynamics C5 2012 vers [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="416fd-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="416fd-105">Vous pouvez également migrer des écritures historiques pour des comptes généraux.</span><span class="sxs-lookup"><span data-stu-id="416fd-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="416fd-106">La société dans [!INCLUDE[d365fin](includes/d365fin_md.md)] ne doit pas contenir de données.</span><span class="sxs-lookup"><span data-stu-id="416fd-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="416fd-107">En outre, après avoir commencé une migration, ne créez pas de clients, de fournisseurs, d'articles, ou de comptes jusqu'à la fin de la migration.</span><span class="sxs-lookup"><span data-stu-id="416fd-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="what-data-is-migrated"></a><span data-ttu-id="416fd-108">Quelles données sont migrées ?</span><span class="sxs-lookup"><span data-stu-id="416fd-108">What Data is Migrated?</span></span>
<span data-ttu-id="416fd-109">Les données suivantes sont migrées pour chaque entité :</span><span class="sxs-lookup"><span data-stu-id="416fd-109">The following data is migrated for each entity:</span></span>

<span data-ttu-id="416fd-110">**Clients**</span><span class="sxs-lookup"><span data-stu-id="416fd-110">**Customers**</span></span>
* <span data-ttu-id="416fd-111">Emplacement</span><span class="sxs-lookup"><span data-stu-id="416fd-111">Location</span></span>
* <span data-ttu-id="416fd-112">Pays</span><span class="sxs-lookup"><span data-stu-id="416fd-112">Country</span></span>
* <span data-ttu-id="416fd-113">Axes client (service, centre, objectif)</span><span class="sxs-lookup"><span data-stu-id="416fd-113">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="416fd-114">Conditions de livraison</span><span class="sxs-lookup"><span data-stu-id="416fd-114">Shipment method</span></span>
* <span data-ttu-id="416fd-115">Vendeur</span><span class="sxs-lookup"><span data-stu-id="416fd-115">Sales Person</span></span>
* <span data-ttu-id="416fd-116">Conditions de paiement</span><span class="sxs-lookup"><span data-stu-id="416fd-116">Payment terms</span></span>
* <span data-ttu-id="416fd-117">Mode de règlement</span><span class="sxs-lookup"><span data-stu-id="416fd-117">Payment method</span></span>
* <span data-ttu-id="416fd-118">Groupe prix client</span><span class="sxs-lookup"><span data-stu-id="416fd-118">Customer price group</span></span>
* <span data-ttu-id="416fd-119">Remise facture client</span><span class="sxs-lookup"><span data-stu-id="416fd-119">Customer invoice discount</span></span>

<span data-ttu-id="416fd-120">Si vous migrez des comptes, les données suivantes sont également migrées :</span><span class="sxs-lookup"><span data-stu-id="416fd-120">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="416fd-121">Configuration de la validation client</span><span class="sxs-lookup"><span data-stu-id="416fd-121">Customer posting setup</span></span>
* <span data-ttu-id="416fd-122">Nom feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="416fd-122">General journal batch</span></span>
* <span data-ttu-id="416fd-123">Transactions ouvertes (écritures comptables client)</span><span class="sxs-lookup"><span data-stu-id="416fd-123">Open transactions (customer ledger entries)</span></span>

<span data-ttu-id="416fd-124">**Fournisseurs**</span><span class="sxs-lookup"><span data-stu-id="416fd-124">**Vendors**</span></span>
* <span data-ttu-id="416fd-125">Emplacement</span><span class="sxs-lookup"><span data-stu-id="416fd-125">Location</span></span>
* <span data-ttu-id="416fd-126">Pays</span><span class="sxs-lookup"><span data-stu-id="416fd-126">Country</span></span>
* <span data-ttu-id="416fd-127">Axes fournisseur (service, centre, objectif)</span><span class="sxs-lookup"><span data-stu-id="416fd-127">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="416fd-128">Remise facture</span><span class="sxs-lookup"><span data-stu-id="416fd-128">Invoice discount</span></span>
* <span data-ttu-id="416fd-129">Conditions de livraison</span><span class="sxs-lookup"><span data-stu-id="416fd-129">Shipment method</span></span>
* <span data-ttu-id="416fd-130">Acheteur</span><span class="sxs-lookup"><span data-stu-id="416fd-130">Purchaser</span></span>
* <span data-ttu-id="416fd-131">Conditions de paiement</span><span class="sxs-lookup"><span data-stu-id="416fd-131">Payment terms</span></span>
* <span data-ttu-id="416fd-132">Mode de règlement</span><span class="sxs-lookup"><span data-stu-id="416fd-132">Payment method</span></span>
* <span data-ttu-id="416fd-133">Remises facture fournisseur</span><span class="sxs-lookup"><span data-stu-id="416fd-133">Vendor invoice discount</span></span>

<span data-ttu-id="416fd-134">Si vous migrez des comptes, les données suivantes sont également migrées :</span><span class="sxs-lookup"><span data-stu-id="416fd-134">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="416fd-135">Configuration de la validation fournisseur</span><span class="sxs-lookup"><span data-stu-id="416fd-135">Vendor posting setup</span></span>
* <span data-ttu-id="416fd-136">Nom feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="416fd-136">General journal batch</span></span>
* <span data-ttu-id="416fd-137">Transactions ouvertes (écritures comptables fournisseur)</span><span class="sxs-lookup"><span data-stu-id="416fd-137">Open transactions (vendor ledger entries)</span></span>

<span data-ttu-id="416fd-138">**Articles**</span><span class="sxs-lookup"><span data-stu-id="416fd-138">**Items**</span></span>
* <span data-ttu-id="416fd-139">Emplacement</span><span class="sxs-lookup"><span data-stu-id="416fd-139">Location</span></span>
* <span data-ttu-id="416fd-140">Pays</span><span class="sxs-lookup"><span data-stu-id="416fd-140">Country</span></span>
* <span data-ttu-id="416fd-141">Axes article (service, centre, objectif)</span><span class="sxs-lookup"><span data-stu-id="416fd-141">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="416fd-142">Remises ligne vente</span><span class="sxs-lookup"><span data-stu-id="416fd-142">Sales line discounts</span></span>
* <span data-ttu-id="416fd-143">Groupe remises client</span><span class="sxs-lookup"><span data-stu-id="416fd-143">Customer discount groups</span></span>
* <span data-ttu-id="416fd-144">Groupes remises article</span><span class="sxs-lookup"><span data-stu-id="416fd-144">Item discount groups</span></span>
* <span data-ttu-id="416fd-145">Prix vente</span><span class="sxs-lookup"><span data-stu-id="416fd-145">Sales price</span></span>
* <span data-ttu-id="416fd-146">Nomenclature produits</span><span class="sxs-lookup"><span data-stu-id="416fd-146">Tariff number</span></span>
* <span data-ttu-id="416fd-147">Unités de mesure</span><span class="sxs-lookup"><span data-stu-id="416fd-147">Units of measure</span></span>
* <span data-ttu-id="416fd-148">Code traçabilité</span><span class="sxs-lookup"><span data-stu-id="416fd-148">Item tracking code</span></span>
* <span data-ttu-id="416fd-149">Groupe prix client</span><span class="sxs-lookup"><span data-stu-id="416fd-149">Customer price group</span></span>

<span data-ttu-id="416fd-150">Si vous migrez des comptes, les données suivantes sont également migrées :</span><span class="sxs-lookup"><span data-stu-id="416fd-150">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="416fd-151">Configuration de la validation de stock</span><span class="sxs-lookup"><span data-stu-id="416fd-151">Inventory posting setup</span></span>
* <span data-ttu-id="416fd-152">Paramètres comptabilisation</span><span class="sxs-lookup"><span data-stu-id="416fd-152">General posting setup</span></span>
* <span data-ttu-id="416fd-153">Nom feuille article</span><span class="sxs-lookup"><span data-stu-id="416fd-153">Item journal batch</span></span>
* <span data-ttu-id="416fd-154">Transactions ouvertes (écritures comptables article)</span><span class="sxs-lookup"><span data-stu-id="416fd-154">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="416fd-155">S'il existe des transactions ouvertes qui utilisent des devises étrangères, les taux de change pour les devises sont également migrés.</span><span class="sxs-lookup"><span data-stu-id="416fd-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="416fd-156">Les autres taux de change ne sont pas migrés.</span><span class="sxs-lookup"><span data-stu-id="416fd-156">Other exchange rates are not migrated.</span></span>

<span data-ttu-id="416fd-157">**Plan comptable**</span><span class="sxs-lookup"><span data-stu-id="416fd-157">**Chart of Accounts**</span></span>  
* <span data-ttu-id="416fd-158">Dimensions standard : département, centre de coût, objectif</span><span class="sxs-lookup"><span data-stu-id="416fd-158">Standard dimensions: Department, Cost Center, Purpose</span></span>  
* <span data-ttu-id="416fd-159">Transactions comptables historiques</span><span class="sxs-lookup"><span data-stu-id="416fd-159">Historical G/L transactions</span></span>  

> [!Note]
> <span data-ttu-id="416fd-160">Les transactions comptables historiques sont traitées un peu différemment.</span><span class="sxs-lookup"><span data-stu-id="416fd-160">Historical G/L transactions are treated a little differently.</span></span> <span data-ttu-id="416fd-161">Lorsque vous migrez des données, vous définissez un paramètre **Période courante**.</span><span class="sxs-lookup"><span data-stu-id="416fd-161">When you migrate data you set a **Current Period** parameter.</span></span> <span data-ttu-id="416fd-162">Ce paramètre spécifie comment traiter les transactions comptables.</span><span class="sxs-lookup"><span data-stu-id="416fd-162">This parameter specifies how to process G/L transactions.</span></span> <span data-ttu-id="416fd-163">Les transactions postérieures à cette date sont migrées individuellement.</span><span class="sxs-lookup"><span data-stu-id="416fd-163">Transactions after this date are migrated individually.</span></span> <span data-ttu-id="416fd-164">Les transactions antérieures à cette date sont regroupées par compte et migrées en tant que montant unique.</span><span class="sxs-lookup"><span data-stu-id="416fd-164">Transactions before this date are aggregated per account and migrated as a single amount.</span></span> <span data-ttu-id="416fd-165">Par exemple, supposons qu'il existe des transactions en 2015, 2016, 2017, 2018 et que vous spécifiez le 01 janvier 2017 dans le champ Période courante.</span><span class="sxs-lookup"><span data-stu-id="416fd-165">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span></span> <span data-ttu-id="416fd-166">Pour chaque compte, les montants des transactions effectuées au plus tard le 31 décembre 2106 sont regroupés sur une ligne feuille comptabilité unique pour chaque compte général.</span><span class="sxs-lookup"><span data-stu-id="416fd-166">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span></span> <span data-ttu-id="416fd-167">Toutes les transactions postérieures à cette date sont migrées individuellement.</span><span class="sxs-lookup"><span data-stu-id="416fd-167">All trascations after this date will be migrated individually.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="416fd-168">Pour migrer des données</span><span class="sxs-lookup"><span data-stu-id="416fd-168">To migrate data</span></span>
<span data-ttu-id="416fd-169">Quelques étapes suffisent pour exporter des données de C5 et les importer dans [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="416fd-169">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

1. <span data-ttu-id="416fd-170">Dans C5, utilisez la fonctionnalité **Exporter la base de données** pour exporter les données.</span><span class="sxs-lookup"><span data-stu-id="416fd-170">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="416fd-171">Envoyez ensuite le fichier d'exportation vers un fichier compressé (zippé).</span><span class="sxs-lookup"><span data-stu-id="416fd-171">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="416fd-172">Dans [!INCLUDE[d365fin](includes/d365fin_md.md)], sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Icône Page ou état pour la recherche"), saisissez **Migration de données**, puis sélectionnez **Migration de données**.</span><span class="sxs-lookup"><span data-stu-id="416fd-172">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="416fd-173">Exécutez les étapes du guide de configuration assistée.</span><span class="sxs-lookup"><span data-stu-id="416fd-173">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="416fd-174">Veillez à choisir **Importer à partir de Microsoft Dynamcis C5 2012** comme source de données.</span><span class="sxs-lookup"><span data-stu-id="416fd-174">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note]
> <span data-ttu-id="416fd-175">Les sociétés ajoutent souvent des champs pour personnaliser C5 pour leur activité spécifique.</span><span class="sxs-lookup"><span data-stu-id="416fd-175">Companies often add fields to customize C5 for their specific line of business.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="416fd-176"> n'effectue pas la migration de données à partir des champs personnalisés.</span><span class="sxs-lookup"><span data-stu-id="416fd-176"> does not migrate data from custom fields.</span></span> <span data-ttu-id="416fd-177">En outre, la migration échouera si vous avez plus de 10 champs personnalisés.</span><span class="sxs-lookup"><span data-stu-id="416fd-177">Also, migration will fail if you have more than 10 custom fields.</span></span>

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="416fd-178">Affichage du statut de la migration</span><span class="sxs-lookup"><span data-stu-id="416fd-178">Viewing the Status of the Migration</span></span>
<span data-ttu-id="416fd-179">Utilisez la page **Vue d’ensemble de la migration des données** pour contrôler la réussite de la migration.</span><span class="sxs-lookup"><span data-stu-id="416fd-179">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="416fd-180">La page affiche des informations telles que le nombre d'entités incluses dans la migration, le statut de la migration, ainsi que le nombre d'articles qui ont été migrés et l'état de réussite de leur migration.</span><span class="sxs-lookup"><span data-stu-id="416fd-180">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="416fd-181">Elle affiche également le nombre d'erreurs, ce qui vous permet d'étudier ce qui ne s'est pas passé correctement et, si possible, d'accéder facilement à l'entité pour résoudre les problèmes.</span><span class="sxs-lookup"><span data-stu-id="416fd-181">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="416fd-182">Pour plus d'informations, voir la section suivante de cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="416fd-182">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="416fd-183">Pendant que vous attendez les résultats de la migration, vous devez actualiser la page pour afficher les résultats.</span><span class="sxs-lookup"><span data-stu-id="416fd-183">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="how-to-avoid-double-posting"></a><span data-ttu-id="416fd-184">Comment éviter la double validation</span><span class="sxs-lookup"><span data-stu-id="416fd-184">How to Avoid Double-Posting</span></span>
<span data-ttu-id="416fd-185">Pour éviter la double validation en comptabilité, les comptes de contrepartie suivants sont utilisés pour les transactions ouvertes :</span><span class="sxs-lookup"><span data-stu-id="416fd-185">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span></span>  
  
* <span data-ttu-id="416fd-186">Pour les fournisseurs, nous utilisons le compte Comptabilité fournisseur dans le groupe comptabilisation fournisseur.</span><span class="sxs-lookup"><span data-stu-id="416fd-186">For vendors, we use the A/P account from the vendor posting group.</span></span>  
* <span data-ttu-id="416fd-187">Pour les clients, nous utilisons le compte Comptabilité client dans le groupe comptabilisation client.</span><span class="sxs-lookup"><span data-stu-id="416fd-187">For customers, we use the A/R account from the customer posting group.</span></span>  
* <span data-ttu-id="416fd-188">Pour les articles, nous créons un paramètre comptabilisation où le compte ajustement est le compte spécifié comme compte stock dans les paramètres comptabilisation stock.</span><span class="sxs-lookup"><span data-stu-id="416fd-188">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span></span>  

## <a name="correcting-errors"></a><span data-ttu-id="416fd-189">Correction des erreur</span><span class="sxs-lookup"><span data-stu-id="416fd-189">Correcting Errors</span></span>
<span data-ttu-id="416fd-190">Si quelque chose se passe mal et qu'une erreur survient, le champ **Statut** affiche **Terminé avec des erreurs**, et le champ **Nombre d'erreurs** en indique le nombre.</span><span class="sxs-lookup"><span data-stu-id="416fd-190">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="416fd-191">Pour afficher la liste des erreurs, vous pouvez ouvrir la page **Erreurs de migration des données** en sélectionnant :</span><span class="sxs-lookup"><span data-stu-id="416fd-191">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="416fd-192">le nombre dans le champ **Nombre d'erreurs** pour l'entité.</span><span class="sxs-lookup"><span data-stu-id="416fd-192">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="416fd-193">l'entité, puis l'action **Afficher les erreurs**.</span><span class="sxs-lookup"><span data-stu-id="416fd-193">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="416fd-194">Dans la page **Erreurs de migration des données**, pour corriger une erreur vous pouvez sélectionner un message d'erreur, puis **Modifier l'enregistrement** pour ouvrir une page qui affiche les données migrées pour l'entité.</span><span class="sxs-lookup"><span data-stu-id="416fd-194">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="416fd-195">Après avoir corrigé une ou plusieurs erreurs, vous pouvez sélectionner **Migrer** pour migrer uniquement les entités que vous avez corrigées, sans entièrement redémarrer la migration.</span><span class="sxs-lookup"><span data-stu-id="416fd-195">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="416fd-196">Si vous avez corrigé plusieurs erreur, vous pouvez utiliser la fonctionnalité **Sélectionner davantage** pour sélectionner plusieurs lignes à migrer.</span><span class="sxs-lookup"><span data-stu-id="416fd-196">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="416fd-197">Sinon, s'il existe des erreurs qu'il n'est pas important de corriger, vous pouvez les sélectionner, puis cliquer sur **Ignorer les sélections**.</span><span class="sxs-lookup"><span data-stu-id="416fd-197">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="416fd-198">Si vous avez des articles inclus dans une nomenclature, vous pouvez être amené à effectuer la migration plus d'une fois si l'article d'origine n'est pas créé avant les variantes qui y font référence.</span><span class="sxs-lookup"><span data-stu-id="416fd-198">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="416fd-199">Si une variante article est créée en premier lieu, la référence à l'article d'origine peut entraîner un message d'erreur.</span><span class="sxs-lookup"><span data-stu-id="416fd-199">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="416fd-200">Vérifier les données après avoir effectué une migration</span><span class="sxs-lookup"><span data-stu-id="416fd-200">Verifying Data After Migrating</span></span>
<span data-ttu-id="416fd-201">Si vous souhaitez vérifier que vos données ont été migrées correctement, vous pouvez consulter les pages suivantes dans C5 et [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="416fd-201">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="416fd-202">Microsoft Dynamics C5 2012</span><span class="sxs-lookup"><span data-stu-id="416fd-202">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]| <span data-ttu-id="416fd-203">Traitement par lots à utiliser</span><span class="sxs-lookup"><span data-stu-id="416fd-203">Batch Job to Use</span></span> |
|-----|-----|-----|
|<span data-ttu-id="416fd-204">Écritures client</span><span class="sxs-lookup"><span data-stu-id="416fd-204">Customer Entries</span></span>| <span data-ttu-id="416fd-205">Feuilles comptabilité</span><span class="sxs-lookup"><span data-stu-id="416fd-205">General Journals</span></span>| <span data-ttu-id="416fd-206">CUSTMIGR</span><span class="sxs-lookup"><span data-stu-id="416fd-206">CUSTMIGR</span></span> |
|<span data-ttu-id="416fd-207">Écritures fournisseur</span><span class="sxs-lookup"><span data-stu-id="416fd-207">Vendor Entries</span></span>| <span data-ttu-id="416fd-208">Feuilles comptabilité</span><span class="sxs-lookup"><span data-stu-id="416fd-208">General Journals</span></span>| <span data-ttu-id="416fd-209">VENDMIGR</span><span class="sxs-lookup"><span data-stu-id="416fd-209">VENDMIGR</span></span>|
|<span data-ttu-id="416fd-210">Ecritures article</span><span class="sxs-lookup"><span data-stu-id="416fd-210">Item Entries</span></span>| <span data-ttu-id="416fd-211">Feuilles article</span><span class="sxs-lookup"><span data-stu-id="416fd-211">Item Journals</span></span>| <span data-ttu-id="416fd-212">ITEMMIGR</span><span class="sxs-lookup"><span data-stu-id="416fd-212">ITEMMIGR</span></span> |
|<span data-ttu-id="416fd-213">Écritures comptables</span><span class="sxs-lookup"><span data-stu-id="416fd-213">G/L Entries</span></span>| <span data-ttu-id="416fd-214">Feuilles comptabilité</span><span class="sxs-lookup"><span data-stu-id="416fd-214">General Journals</span></span>| <span data-ttu-id="416fd-215">GLACMIGR</span><span class="sxs-lookup"><span data-stu-id="416fd-215">GLACMIGR</span></span> |

## <a name="stopping-data-migration"></a><span data-ttu-id="416fd-216">Arrêter la migration des données</span><span class="sxs-lookup"><span data-stu-id="416fd-216">Stopping Data Migration</span></span>
<span data-ttu-id="416fd-217">Vous pouvez arrêter de migrer les données en sélectionnant **Arrêter toutes les migrations**.</span><span class="sxs-lookup"><span data-stu-id="416fd-217">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="416fd-218">Si vous le faites, toutes les migrations en attente sont également arrêtées.</span><span class="sxs-lookup"><span data-stu-id="416fd-218">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="416fd-219">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="416fd-219">See Also</span></span>
<span data-ttu-id="416fd-220">[Personnalisation de [!INCLUDE[d365fin](includes/d365fin_md.md)] à l'aide des extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="416fd-220">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="416fd-221">Mise en route</span><span class="sxs-lookup"><span data-stu-id="416fd-221">Getting Started</span></span>](product-get-started.md) 

