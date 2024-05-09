---
title: Analyse des données par axe analytique
description: Cet article décrit comment analyser les données d’entreprise par axes analytiques pour mieux comprendre votre activité.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '545, 555, 556, 557, 558, 9372, 9370, 9371'
ms.date: 04/19/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="analyze-data-by-dimensions"></a>Analyse des données par axe analytique

En analyse financière, un axe correspond à des données que vous ajoutez à une écriture comme une sorte de marqueur pour grouper les écritures similaires. Par exemple, les dimensions regroupent souvent les entrées pour les clients, les régions, les produits et les vendeurs. Les groupes vous permettent de récupérer facilement des données les concernant pour les analyser. Vous pouvez utiliser les axes sur des écritures de feuilles, de documents et de budgets.

Chaque axe décrit l’objet de l’analyse. Une analyse à deux axes, par exemple, est une analyse des ventes par zone. En utilisant plus de deux dimensions lors de la création d’une entrée, vous pouvez effectuer une analyse plus complexe. Un exemple d’analyse complexe consiste à explorer les ventes par campagne de vente, par groupe de clients et par zone. Cela vous permet d’obtenir un meilleur aperçu de votre activité commerciale, comme la mesure du bon fonctionnement de votre société, les domaines dans lesquels elle prospère ou non, et ceux dans lesquels il est nécessaire d’affecter davantage de ressources. Ces informations vous aident à prendre des décisions commerciales plus éclairées. Pour plus d’informations, consultez [Utiliser les dimensions](finance-dimensions.md).

> [!TIP]
> Pour analyser rapidement les données transactionnelles par axe, vous pouvez filtrer les totaux du plan comptable (COA) et les entrées de toutes les pages **Écritures** par axes analytiques. Recherchez l’action **Définir le filtre axe**.

> [!NOTE]
> Si vous découvrez qu’une section analytique incorrecte a été utilisée sur les écritures comptables comptabilisées, vous pouvez la corriger et mettre à jour vos vues d’analyse. Pour en savoir plus, consultez [Dépannage et correction des axes analytiques](finance-troubleshooting-correcting-dimensions.md#changing-dimension-assignments-after-posting).

## <a name="set-up-an-analysis-view"></a>Configurer une vue d’analyse

Les vues analytiques utilisent une combinaison sélectionnée d’axes analytiques. Vous stockez, récupérez et mettez à jour cet ensemble d’axes analytiques en créant une fiche **Vue d’analyse**.

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Vues d’analyse**, puis sélectionnez le lien associé.  
2. Sur la page **Liste des vues d’analyse**, cliquez sur l’action **Nouveau**.
3. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Pour ajouter des codes axe aux quatre codes du raccourci **Axes analytiques**, cliquez sur l’action **Filtre**, renseignez les champs et cliquez sur **OK**.  
5. Pour mettre à jour la vue, choisissez l’action **Mettre à jour**.

## <a name="analyze-by-dimensions"></a>Analyse par axe analytique

Utilisez les vues d’analyse que vous avez déjà configurées avec la matrice **Vues analytiques** pour afficher les montants de votre comptabilité.

1. Sélectionnez l’icône en forme ![d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Vues d’analyse**, puis sélectionnez le lien associé.  
2. Sélectionnez la vue d’analyse appropriée et choisissez l’action **Vues analytiques**.
3. Sur la page **Analyse vente par axe analytique**, renseignez les champs pour définir les données affichées et leur présentation.
4. Choisissez l’action **Afficher matrice** pour ouvrir la page matricielle de la vue d’analyse.
5. Pour accéder au détail d’un montant dans la page matrice, choisissez le montant.  

- Les colonnes à gauche contiennent des informations basées sur l’option sélectionnée dans le champ **Afficher lignes** de l’en-tête.  
- Les colonnes à droite contiennent des informations basées sur l’option sélectionnée dans le champ **Afficher colonnes** de l’en-tête.

> [!IMPORTANT]  
> Vous ne pouvez pas sélectionner une période plus courte que celle indiquée en tant que compression date sur la fiche **Vue d’analyse**. Les actions **Jeu suivant** et **Jeu précédent** ne sont pas disponibles si vous avez sélectionné **Période** dans le champ **Afficher lignes** ou les champs **Afficher colonnes**.  

> [!NOTE]  
> Vous pouvez utiliser l'état **Axes analytiques - Détail** pour afficher un classement détaillé du mode d'utilisation des axes sur des écritures pour une période donnée. Vous pouvez utiliser l’état **Axes analytiques - Total** pour afficher uniquement les montants totaux.  

> [!TIP]  
> Vous pouvez également modifier la vue en changeant la valeur des champs **Afficher lignes** et **Afficher colonnes**. Pour contrepasser un paramètre de vue, choisissez l’action **Inverser lignes et colonnes**.

## <a name="update-an-analysis-view"></a>Mettre à jour une vue d’analyse

Les montants sur la page **Vues analytiques** offrent une image de l’état de la société au moment de la dernière mise à jour. Pour obtenir l’état actuel, exécutez l’action de mise à jour pour mettre à jour la vue d’analyse.

Suivez la procédure suivante pour mettre à jour une vue d’analyse à partir de la page **Vues analytiques**. Les étapes sont similaires à celles de la mise à jour des pages **Fiche vue d’analyse** et **Liste des vues d’analyse**.  

1. Sélectionnez ![l’icône en forme d’Ampoule qui ouvre la fenêtre de recherche.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Vues d’analyse**, puis sélectionnez le lien associé.
2. Sélectionnez la vue d’analyse appropriée et choisissez l’action **Vues analytiques**.
3. Sur la page **Vues analytiques**, sélectionnez le champ **Code vue analytique**.  
4. Sélectionnez la ligne contenant la vue d’analyse appropriée.  
5. Sur la page **Vues d’analyse**, sélectionnez la vue d’analyse, puis l’action **Mettre à jour**.  

> [!TIP]  
> Si vous activez la case à cocher **Mise à jour à la validation** sur la fiche vue d’analyse, la vue est automatiquement mise à jour lorsqu’une transaction associée est validée.

> [!NOTE]  
> Pour mettre à jour tout ou partie des vues d’analyse en même temps, utiliser le traitement par lots **Mise à jour vues d’analyse**.  

## <a name="see-also"></a>Voir aussi

[Business Intelligence financière](bi.md)  
[Finances](finance.md)  
[Configuration de Finance](finance-setup-finance.md)  
[Comptabilité et plan comptable](finance-general-ledger.md)  
[Utiliser les axes analytiques](finance-dimensions.md)  
[Utiliser [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
