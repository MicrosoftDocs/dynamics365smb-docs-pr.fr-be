---
ms.service: dynamics-365-business-central
---
> [!NOTE]
> Vous pouvez obtenir les données de diverses entreprises dans un seul rapport avec les services Web OData. Cependant, à commencer par la 2e vague de lancement 2021 [!INCLUDE [prod_short](prod_short.md)], seul ODataV4 est pris en charge. ODataV4 n’exporte pas les données de plusieurs entreprises. La fonction **$expand** dans Power BI que vous pourriez considérer comme un autre moyen de créer un rapport multi-sociétés, ne peut pas non plus être utilisée. Elle crée une colonne avec le nom de l’entreprise, mais ne la remplit pas avec les données de l’entreprise après une actualisation.