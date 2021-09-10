---
title: Aanbiedingen van derden
description: Werk de aanbiedingsinstellingen van derden bij om te bepalen of in de handelscatalogus producten uit je bestaande Amazon Seller Central-aanbiedingen worden geïmporteerd.
redirect_from: /sales-channels/asc/ob-third-party-listings.html: 
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 519
ht-degree: 0%

---

# Aanbiedingen van derden

De instellingen voor aanbiedingen van derden maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via het [opslagdashboard](./amazon-store-dashboard.md).

Deze instellingen bepalen of uw [!DNL Commerce]-catalogus producten uit bestaande [!DNL Amazon Seller Central]-aanbiedingen importeert. Het wordt aanbevolen om aanbiedingen uit Amazon te importeren om ervoor te zorgen dat alle aanbiedingen overeenkomen met producten van [!DNL Commerce]. Wanneer je aanbiedingen deel uitmaken van je [!DNL Commerce]-catalogus, kunt je al je producten uit één catalogus beheren en gebruikmaken van Amazon-verkoopkanaalfuncties. Deze functies zijn onder andere het uitvoeren van bestellingen en het beheren van bestellingen met Amazon, intelligente prijsaanpassingen en beheer van hoeveelheden.

Wanneer Amazon zo is geconfigureerd dat je je Amazon-aanbiedingen importeert, importeert je Amazon-aanbiedingen in je [!DNL Commerce]-catalogus, zodat ze proberen ze aan te passen aan bestaande producten. Als er niet automatisch een overeenkomst wordt gevonden, kunt u de Amazon-aanbieding als een nieuw [!DNL Commerce]-product importeren of de aanbieding handmatig aan een product aanpassen.

Als je je Amazon-aanbiedingen wilt importeren, kies dan de kenmerken [!DNL Commerce] met waarden voor Amazon Seller SKU en Amazon ASIN. Als u [!DNL Commerce] [productkenmerken](./ob-creating-magento-attributes.md) niet hebt, kunt u deze maken en toewijzen. Door deze kenmerken toe te wijzen, kunt u geïmporteerde Amazon-aanbiedingen beter afstemmen op uw [!DNL Commerce]-producten.

De eerste importbewerking wordt gestart wanneer [store integration](./store-integration.md) is voltooid. [!DNL Commerce] controleert vervolgens voortdurend op nieuwe Amazon-aanbiedingen (die niet in Amazon Sales Channel zijn gemaakt) en werkt uw [!DNL Commerce]-catalogus bij volgens de instellingen voor aanbiedingen van derden.

## Instellingen voor lijsten van derden configureren

1. Klik **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Third Party Listings]_uit.

1. Kies voor **[!UICONTROL Import Third Party Listings]** (vereist) een optie:

   - `Import Listing` - (Standaard) Kies wanneer je productinformatie uit je Amazon-aanbiedingen wilt importeren in je  [!DNL Commerce] productcatalogus. Dit is de standaardoptie en wordt aanbevolen.

   - `Do Not Import Listing` - Kies wanneer u handmatig nieuwe producten [ wilt ](https://docs.magento.com/user-guide/catalog/products.html)maken en wijs deze toe aan uw  [!DNL Commerce] catalogus voor Amazon-aanbiedingen.
   >[!NOTE]
   >De volgende optievelden zijn alleen actief wanneer deze zijn ingesteld op `Import Listing`.

1. Kies bij **[!UICONTROL Attribute That Contains Amazon Seller SKU]** het [!DNL Commerce]-kenmerk dat overeenkomt met de SKU-waarde van Amazon-verkoper.

1. Kies voor **[!UICONTROL Attribute That Contains Amazon ASIN]** het kenmerk [!DNL Commerce] dat u hebt gemaakt en pas dit aan de Amazon ASIN aan.

   >[!NOTE]
   >Zie [Kenmerken maken voor Amazon Matching](./ob-creating-magento-attributes.md) als u deze [!DNL Commerce]-kenmerken niet hebt gemaakt voor uw Amazon-aanbiedingen.

1. Klik op **[!UICONTROL Save listing settings]** als u klaar bent.

![Aanbiedingen van derden](assets/amazon-third-party-listings.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Import Third Party Listings] | Vereist. Opties:<ul><li>**[!UICONTROL Import Listing]** - (Standaard) Kies wanneer je productinformatie uit je Amazon-aanbiedingen wilt importeren in je  [!DNL Commerce] productcatalogus. </li><li>**[!UICONTROL Do Not Import Listing]** - Kies wanneer u handmatig nieuwe producten [ wilt ](https://docs.magento.com/user-guide/catalog/products.html)maken en wijs deze toe aan uw  [!DNL Commerce] catalogus voor Amazon-aanbiedingen.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Alleen actief wanneer ingesteld op `Import Listing`.<br>Kies het  [!DNL Commerce] kenmerk als overeenkomst met het Amazon-kenmerk voor de SKU van de Amazon-verkoper. Als dit kenmerk niet bestaat, zie [Amazon-productkenmerken maken voor Amazon Matching](./ob-creating-magento-attributes.md). Controleer zo nodig uw [!DNL Commerce] [kenmerken](./managing-attributes.md) en maak of bewerk een kenmerk dat aansluit op deze Amazon-gegevens. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Alleen actief wanneer ingesteld op `Import Listing`.<br>Kies het  [!DNL Commerce] kenmerk dat overeenkomt met het Amazon-kenmerk voor de Amazon ASIN. Als dit kenmerk niet bestaat, zie [Amazon-productkenmerken maken voor Amazon Matching](./ob-creating-magento-attributes.md). Controleer zo nodig uw [!DNL Commerce] [kenmerken](./managing-attributes.md) en maak of bewerk een kenmerk dat aansluit op deze Amazon-gegevens. |

**Snelle toegang**  -  [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
