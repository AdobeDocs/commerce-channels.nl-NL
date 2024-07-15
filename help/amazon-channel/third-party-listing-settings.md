---
title: Amazon-Sales Channel - [!UICONTROL Third-party Listings]
description: Werk de aanbiedingsinstellingen van derden bij om te bepalen of je Commerce-catalogus producten uit je bestaande Amazon Seller Central-aanbiedingen importeert.
feature: Sales Channels, Products
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

De instellingen voor aanbiedingen van derden maken deel uit van de aanbiedingsinstellingen van je winkel. De lijsten van montages worden betreden van het [ opslagdashboard ](./amazon-store-dashboard.md).

Deze instellingen bepalen of in de catalogus van [!DNL Commerce] producten uit bestaande [!DNL Amazon Seller Central] -aanbiedingen worden geïmporteerd. Het wordt aanbevolen om aanbiedingen uit Amazon te importeren om ervoor te zorgen dat alle aanbiedingen overeenkomende [!DNL Commerce] -producten hebben. Wanneer je aanbiedingen deel uitmaken van je catalogus in [!DNL Commerce] , kun je al je producten uit één catalogus beheren en de Amazon-verkoopkanaalfuncties gebruiken. Deze functies zijn onder andere het uitvoeren van bestellingen en het beheren van bestellingen met Amazon, intelligente prijsaanpassingen en beheer van hoeveelheden.

Als je je Amazon-aanbiedingen importeert, importeert Amazon je Amazon-aanbiedingen naar je catalogus van [!DNL Commerce] en probeert ze aan te passen aan bestaande producten. Als er niet automatisch een overeenkomst wordt gevonden, kunt u de Amazon-aanbieding als een nieuw [!DNL Commerce] product importeren of de aanbieding handmatig aan een product aanpassen.

Als je je Amazon-aanbiedingen wilt importeren, kies dan de [!DNL Commerce] -kenmerken met waarden voor Amazon Seller SKU en Amazon ASIN. Als u [!DNL Commerce] [ productattributen ](./ob-creating-magento-attributes.md) niet hebt, denk na creërend en toewijzend hen. Door deze kenmerken toe te wijzen, kunt u geïmporteerde Amazon-aanbiedingen op de juiste wijze afstemmen op uw [!DNL Commerce] -producten.

De aanvankelijke lijst voert in werking wanneer [ opslagintegratie ](./store-integration.md) volledig is. Vervolgens controleert [!DNL Commerce] voortdurend op nieuwe Amazon-aanbiedingen (die niet in de Sales Channel van Amazon zijn gemaakt) en werkt je [!DNL Commerce] -catalogus bij op basis van de instellingen voor aanbiedingen van derden.

## Instellingen voor lijsten van derden configureren

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Third Party Listings]_uit.

1. Kies bij **[!UICONTROL Import Third Party Listings]** (vereist) een optie:

   - `Import Listing` - (Standaard) Kies wanneer u productinformatie uit uw Amazon-aanbiedingen wilt importeren in uw productcatalogus van [!DNL Commerce] . Dit is de standaardoptie en wordt aanbevolen.

   - `Do Not Import Listing` - kies wanneer u wilt manueel [ creëren en nieuwe producten ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) aan uw [!DNL Commerce] catalogus voor uw aanbiedingen van Amazon toewijzen.

   >[!NOTE]
   >De volgende optievelden zijn alleen actief wanneer deze zijn ingesteld op `Import Listing` .

1. Kies bij **[!UICONTROL Attribute That Contains Amazon Seller SKU]** het kenmerk [!DNL Commerce] dat overeenkomt met de SKU-waarde van Amazon-verkoper.

1. Kies bij **[!UICONTROL Attribute That Contains Amazon ASIN]** het kenmerk [!DNL Commerce] dat u hebt gemaakt en pas dit aan de Amazon ASIN-code aan.

   >[!NOTE]
   >Als u deze [!DNL Commerce] attributen voor uw lijsten van Amazon niet creeerde, zie [ Creërend Attributen voor het Vergelijken van Amazon ](./ob-creating-magento-attributes.md).

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ lijsten van derden ](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Third Party Listings] | Vereist. Opties:<ul><li>**[!UICONTROL Import Listing]** - (Standaard) Kies wanneer u productinformatie uit uw Amazon-aanbiedingen wilt importeren in uw productcatalogus van [!DNL Commerce] . </li><li>**[!UICONTROL Do Not Import Listing]** - kies wanneer u wilt manueel [ creëren en nieuwe producten ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) aan uw [!DNL Commerce] catalogus voor uw aanbiedingen van Amazon toewijzen.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Alleen actief wanneer ingesteld op `Import Listing` .<br> kies het [!DNL Commerce] attribuut als gelijke aan het attribuut van Amazon voor Amazon Seller SKU. Als dit attribuut niet bestaat, zie [ Creërend de Attributen van het Product van Amazon voor Amazon het Matching ](./ob-creating-magento-attributes.md). Indien nodig, herzie uw [!DNL Commerce] [ attributen ](./managing-attributes.md) en creeer of geef een attribuut uit om aan deze gegevens van Amazon aan te passen. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Alleen actief wanneer ingesteld op `Import Listing` .<br> kies het [!DNL Commerce] attribuut dat aan het attribuut van Amazon voor Amazon ASIN aanpast. Als dit attribuut niet bestaat, zie [ Creërend de Attributen van het Product van Amazon voor Amazon het Matching ](./ob-creating-magento-attributes.md). Indien nodig, herzie uw [!DNL Commerce] [ attributen ](./managing-attributes.md) en creeer of geef een attribuut uit om aan deze gegevens van Amazon aan te passen. |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
