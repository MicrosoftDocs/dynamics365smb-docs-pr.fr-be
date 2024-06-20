---
title: 'Modèles et lots de feuilles paiement [BE]'
description: 'Dans la version belge, les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à celle des autres types de feuille.'
author: brentholtorf
ms.topic: conceptual
ms.search.form: '256, 11300, 2000000, 2000001, 2000003, 2000020, 2000021, 2000022'
ms.date: 06/25/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Création de modèles et de lots de feuilles paiement dans la version belge

Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], les suggestions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est similaire à celle des autres types de feuille. Toutefois, la feuille paiement contient des champs qui sont propres au traitement des paiements. Avant de commencer à générer des suggestions de paiement, vous devez paramétrer un modèle feuille paiement et une feuille paiement.  

Vous pouvez affecter une page spécifique et un état de test à chaque modèle feuille. De cette façon, vous pouvez gérer vos paiements nationaux et internationaux à partir de cette page ajustée. Le *code source* spécifié est copié dans toutes les lignes feuille créées sur la base du modèle feuille. Le code est également copié dans les écritures lors de leur validation. De cette façon, vous pouvez toujours connaître l'endroit où une écriture a été validée.

Si vous affectez un compte bancaire au modèle feuille paiement, le compte bancaire est inséré sur toutes les feuilles paiement et lignes feuille paiement qui sont créées à l'aide de ce modèle. En spécifiant un compte bancaire pour le modèle feuille, vous pouvez réduire le temps nécessaire pour vérifier les suggestions de paiement.  

## Pour créer un modèle feuille paiement  

1. Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , entrez **Modèles feuille paiement**, puis choisissez le lien associé.  
2. Choisissez l'action **Nouveau**.  
3. Sur la page **Modèles feuille paiement**, renseignez les champs.  

    [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

    > [!IMPORTANT]
    > Si les champs **ID page** et **ID impression test** ne sont pas affichés, vous devez les ajouter via la personnalisation. Vous devez compléter les champs pour pouvoir continuer. Pour plus d'informations, voir [Personnaliser votre espace de travail](../../ui-personalization-user.md).
4. Répétez l'étape 2 pour chaque modèle supplémentaire.

5. Cliquez sur le bouton **OK**.  

Vous pouvez créer plusieurs lors de feuilles dans chaque modèle feuille. Plusieurs feuilles, chacune ayant son propre nom, peuvent afficher la même page. Par exemple, ceci peut être utile si chaque utilisateur doit avoir une feuille dédiée.

## Pour ajouter des feuilles paiement au modèle feuille  

1. Dans la page **Modèles feuille paiement**, choisissez l'action **Feuilles**.  
2. Sur la page **Nom FS paiements**, renseignez les champs.  

    [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

    > [!NOTE]
    > Pour que le nom feuille soit mis à jour numériquement, ajoutez un nombre au nom feuille. Par exemple, le nom FEUILLE1 augmente d'un numéro à chaque validation, vous aurez donc FEUILLE2, FEUILLE3, etc.  

    Vous pouvez ensuite tester la configuration. Pour plus d'informations, voir [Tester les paiements électroniques](how-to-test-electronic-payments.md).  

## Voir aussi

[Paiements électroniques belges](belgian-electronic-payments.md)  
[Paramétrer des opérations bancaires électroniques](how-to-set-up-electronic-banking.md)  
[Paramétrer les codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)  
[Rendre les modèles feuille obligatoires](specify-journal-template-mandatory.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]