---
title: Amazon Sales Channel - [!UICONTROL Third-party Listings]
description: Werk de aanbiedingsinstellingen van derden bij om te bepalen of in de handelscatalogus producten uit je bestaande Amazon Seller Central-aanbiedingen worden geïmporteerd.
feature: Sales Channels, Products
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

De instellingen voor aanbiedingen van derden maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via de [opslagdashboard](./amazon-store-dashboard.md).

Deze instellingen bepalen of uw [!DNL Commerce] uit catalogus geïmporteerde producten uit uw bestaande [!DNL Amazon Seller Central] aanbiedingen. Het wordt aanbevolen om aanbiedingen uit Amazon te importeren om ervoor te zorgen dat alle aanbiedingen overeenkomen [!DNL Commerce] producten. Wanneer je aanbiedingen deel uitmaken van je [!DNL Commerce] -catalogus, kunt u al uw producten uit één catalogus beheren en gebruikmaken van Amazon-verkoopkanaalfuncties. Deze functies zijn onder andere het uitvoeren van bestellingen en het beheren van bestellingen met Amazon, intelligente prijsaanpassingen en beheer van hoeveelheden.

Wanneer het is geconfigureerd om je Amazon-aanbiedingen te importeren, importeert Amazon je Amazon-aanbiedingen naar je [!DNL Commerce] catalogus, proberen deze aan te passen aan bestaande producten. Als er niet automatisch een overeenkomst wordt gevonden, kunt u de Amazon-aanbieding als een nieuwe aanbieding importeren [!DNL Commerce] of de aanbieding handmatig aan een product aanpassen.

Als je je Amazon-aanbiedingen wilt importeren, kies dan de optie [!DNL Commerce] kenmerken met waarden voor Amazon Seller SKU en Amazon ASIN. Als u [!DNL Commerce] [productkenmerken](./ob-creating-magento-attributes.md), kunt u ze maken en toewijzen. Door deze kenmerken toe te wijzen, kunt u geïmporteerde Amazon-aanbiedingen op de juiste wijze afstemmen op je [!DNL Commerce] producten.

De eerste aanbieding wordt geïmporteerd wanneer [winkelintegratie](./store-integration.md) is voltooid. Hierna en op basis van uw instellingen voor uitsnijden, [!DNL Commerce] controleert voortdurend op nieuw toegevoegde Amazon-aanbiedingen (die niet in Amazon Sales Channel zijn gemaakt) en werkt je [!DNL Commerce] catalogi uitvoeren op basis van de instellingen voor aanbiedingen van derden.

## Instellingen voor lijsten van derden configureren

1. Klikken **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Breid uit _[!UICONTROL Third Party Listings]_sectie.

1. Voor **[!UICONTROL Import Third Party Listings]** (vereist) kiest u een optie:

   - `Import Listing` - (Standaard) Kies wanneer je productinformatie uit je Amazon-aanbiedingen wilt importeren in je [!DNL Commerce] productcatalogus. Dit is de standaardoptie en wordt aanbevolen.

   - `Do Not Import Listing` - Kies wanneer u handmatig wilt [nieuwe producten maken en toewijzen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) aan uw [!DNL Commerce] catalogus voor je Amazon-aanbiedingen.

   >[!NOTE]
   >De volgende optievelden zijn alleen actief wanneer deze zijn ingesteld op `Import Listing`.

1. Voor **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, kiest u de [!DNL Commerce] -kenmerk dat overeenkomt met de Amazon Seller SKU-waarde.

1. Voor **[!UICONTROL Attribute That Contains Amazon ASIN]**, kiest u de [!DNL Commerce] -kenmerk dat u hebt gemaakt en dat hiermee overeenkomt met de Amazon ASIN.

   >[!NOTE]
   >Als u deze niet hebt gemaakt [!DNL Commerce] kenmerken voor je Amazon-aanbiedingen, zie [Kenmerken maken voor Amazon Matching](./ob-creating-magento-attributes.md).

1. Klik op **[!UICONTROL Save listing settings]**.

![Aanbiedingen van derden](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Third Party Listings] | Vereist. Opties:<ul><li>**[!UICONTROL Import Listing]** - (Standaard) Kies wanneer je productinformatie uit je Amazon-aanbiedingen wilt importeren in je [!DNL Commerce] productcatalogus. </li><li>**[!UICONTROL Do Not Import Listing]** - Kies wanneer u handmatig wilt [nieuwe producten maken en toewijzen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) aan uw [!DNL Commerce] catalogus voor je Amazon-aanbiedingen.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Alleen actief wanneer ingesteld op `Import Listing`.<br>Kies de optie [!DNL Commerce] -kenmerk als een overeenkomst met het Amazon-kenmerk voor de SKU van de Amazon-verkoper. Als dit kenmerk niet bestaat, raadpleegt u [Amazon-productkenmerken voor Amazon Matching maken](./ob-creating-magento-attributes.md). Controleer indien nodig uw [!DNL Commerce] [attributes](./managing-attributes.md) en maak of bewerk een kenmerk dat aansluit bij deze Amazon-gegevens. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Alleen actief wanneer ingesteld op `Import Listing`.<br>Kies de optie [!DNL Commerce] kenmerk dat overeenkomt met het Amazon-kenmerk voor de Amazon ASIN. Als dit kenmerk niet bestaat, raadpleegt u [Amazon-productkenmerken voor Amazon Matching maken](./ob-creating-magento-attributes.md). Controleer indien nodig uw [!DNL Commerce] [attributes](./managing-attributes.md) en maak of bewerk een kenmerk dat aansluit bij deze Amazon-gegevens. |

**Snelle toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
