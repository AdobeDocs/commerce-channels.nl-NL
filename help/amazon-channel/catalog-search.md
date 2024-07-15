---
title: Cataloguszoekopdracht voor Amazon-aanbiedingen
description: Als u de kenmerkovereenkomst wilt instellen die u helpt in aanmerking komende Commerce-catalogusproducten toe te wijzen aan Amazon-aanbiedingen, werkt u de zoekinstellingen van de catalogus bij.
feature: Sales Channels, Search, Catalog Management, Products, Configuration
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---

# Cataloguszoekopdracht voor Amazon-aanbiedingen

_montages van het Onderzoek van de Catalogus 0} {maken deel uit van uw montages van de opslaglijst._ De lijsten van montages worden betreden van het [ opslagdashboard ](./amazon-store-dashboard.md).

Met deze instellingen kunt u kenmerkovereenkomsten instellen die helpen in aanmerking komende [!DNL Commerce] producten toe te wijzen aan Amazon-aanbiedingen. Als Amazon een kaart heeft toegewezen, activeert het acties met betrekking tot prijzen, hoeveelheden, overschrijvingen en volgorde en productsynchronisatie.

Als u deze toewijzingswaarden definieert, neemt de kans op exacte overeenkomsten toe, waardoor de noodzaak om productaanbiedingen handmatig af te stemmen, tot een minimum wordt beperkt. Toevoegend de attributen als deel van uw [ Taken van de Opstelling ](./amazon-pre-setup-tasks.md), heeft het verkoopkanaal van Amazon een hoger potentieel om uw producten tijdens het aan boord gaan en syncs productgegevens tussen Amazon en [!DNL Commerce] automatisch aan te passen.

Als u alleen het Amazon ASIN-kenmerk maakt (zonder ASIN-waarden per product toe te voegen), komen uw [!DNL Commerce] -producten mogelijk niet automatisch overeen met uw Amazon-aanbiedingen. U kunt [ manueel toewijzen ](./creating-assigning-catalog-products.md) uw producten. Handmatige overeenkomsten maken echter niet de gegevenselementen die nodig zijn voor het delen en synchroniseren van uw productgegevens.

>[!IMPORTANT]
>
>Als u handmatig een product aanpast en u een ASIN-, UPC- of ander gegevenselement voor het product wilt bijwerken, moet u de gegevens op twee plaatsen bijwerken. Werk deze bij in uw [!DNL Commerce] -catalogus en in uw Amazon-aanbieding in uw [!DNL Amazon Seller Central] -account.

Het is aan te raden deze kenmerken en waarden indien beschikbaar in kaart te brengen. Het voltooien van deze toewijzing is niet vereist, maar is gunstig voor productmatching en is vereist voor een correcte catalogussynchronisatie tussen Amazon en [!DNL Commerce].

Als u attributen wilt toevoegen, zie [ de Attributen van het Product voor Amazon het Verstemmen ](./ob-creating-magento-attributes.md) creëren.

## [!UICONTROL Catalog Search] -instellingen configureren

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Catalog Search]_uit.

1. Kies bij **[!UICONTROL ASIN]** het productkenmerk dat u voor de Amazon ASIN-waarde hebt gemaakt.

   Een ASIN ([!DNL Amazon Standard Identification Number]) is een uniek blok van tien letters en/of aantallen die punten identificeren. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object.

1. Kies bij **[!UICONTROL EAN]** het productkenmerk dat u voor de Amazon EAN-waarde hebt gemaakt.

   Het Europese artikelnummer (EAN) is een norm voor streepjescodes, een productidentificatiecode van twaalf of dertien cijfers. Elk EAN identificeert het product, de fabrikant en de kenmerken ervan op unieke wijze; doorgaans wordt het EAN op een etiket of verpakking als streepjescode gedrukt. Amazon heeft EAN-codes nodig om de kwaliteit van de zoekresultaten en de kwaliteit van de catalogus te verbeteren. U kunt EANs van de fabrikant verkrijgen.

1. Kies bij **[!UICONTROL GCID]** het productkenmerk dat u voor de Amazon GCIN-waarde hebt gemaakt.

   De globale catalogus-id (GCID) is een id voor producten die geen UPC-code of ISBN hebben. Met het Amazon-merkregister kunt u zich registreren als merkhouder en een unieke id voor producten maken.

1. Kies bij **[!UICONTROL ISBN]** het productkenmerk dat u voor de Amazon ISBN-waarde hebt gemaakt.

   Het ISBN (International Standard Book Number) is een unieke streepjescode ter identificatie van een handelsportefeuille. Elke ISBN-code identificeert een boek op unieke wijze. Een ISBN heeft of tien of 13 cijfers. Alle ISBN die na 1 januari 2007 worden toegewezen hebben 13 cijfers.

1. Kies bij **[!UICONTROL UPC]** het productkenmerk dat u voor de Amazon UPC-waarde hebt gemaakt.

   De Universal Product Code (UPC) is een streepjescode van 12 cijfers die veel wordt gebruikt voor detailverpakkingen in de Verenigde Staten.

1. Kies bij **[!UICONTROL General Search]** het productkenmerk dat u wilt gebruiken voor een algemene zoekovereenkomst.

   Dit kenmerk kunt u selecteren om [!DNL Commerce] -producten af te stemmen op de juiste Amazon-vermelding. Bij de algemene zoekopdracht worden trefwoordzoekopdrachten uit de catalogus gebruikt. Daarom wordt aangeraden een attribuut [!DNL Commerce] te gebruiken dat relevante trefwoorden draagt, zoals de product-SKU of de productnaam. Algemene zoekopdracht kan veel mogelijke overeenkomsten opleveren. In dergelijke gevallen kunt u de juiste Amazon-aanbieding selecteren uit de mogelijke overeenkomsten. Een algemene selectie voor dit veld is `Product Name` .

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ het Onderzoek van de Catalogus ](assets/amazon-catalog-search.png){width="500" zoomable="yes"}

| Veld | Beschrijving |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br> ASIN staat voor [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL EAN (European Article Number)] | Een productidentificatiecode van 12 of 13 cijfers. Het Europese artikelnummer (EAN) is een norm voor streepjescodes, een productidentificatiecode van twaalf of dertien cijfers. Elk EAN identificeert het product, de fabrikant en de kenmerken ervan op unieke wijze; doorgaans wordt het EAN op een etiket of verpakking als streepjescode gedrukt. Amazon heeft EAN-codes nodig om de kwaliteit van de zoekresultaten en de kwaliteit van de catalogus te verbeteren. U kunt EANs van de fabrikant verkrijgen. |
| [!UICONTROL GCID (Global Catalog Identifier)] | De globale catalogus-id (GCID) is een id voor producten die geen UPC-code of ISBN hebben. Met het Amazon-merkregister kunt u zich registreren als merkeigenaar en een unieke id maken voor producten die geen UPC of ISBN hebben. |
| [!UICONTROL ISBN (International Standard Book Number)] | Een unieke streepjescode voor een handelsportefeuille van 10 of 13 cijfers. Het ISBN (International Standard Book Number) is een unieke streepjescode ter identificatie van een handelsportefeuille. Elke ISBN-code identificeert een boek op unieke wijze. Een ISBN heeft of tien of 13 cijfers. Alle ISBN die na 1 januari 2007 worden toegewezen hebben 13 cijfers. |
| UPC (Universal Product Code) | Een streepjescode van 12 cijfers. De Universal Product Code (UPC) is een streepjescode van 12 cijfers die veel wordt gebruikt voor detailverpakkingen in de Verenigde Staten. |
| [!UICONTROL General Search] | Selecteer een kenmerk. Dit kenmerk kunt u selecteren om [!DNL Commerce] -producten af te stemmen op de juiste Amazon-vermelding. Bij de algemene zoekopdracht worden trefwoordzoekopdrachten uit de catalogus gebruikt. Daarom wordt aangeraden een attribuut [!DNL Commerce] te gebruiken dat relevante trefwoorden draagt, zoals de product-SKU of de productnaam. Algemene zoekopdracht kan veel mogelijke overeenkomsten opleveren. In dergelijke gevallen kunt u de juiste Amazon-aanbieding selecteren uit de mogelijke overeenkomsten. Een algemene selectie voor dit veld is `Product Name` . |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
