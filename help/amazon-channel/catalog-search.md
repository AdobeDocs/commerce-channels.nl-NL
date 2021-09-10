---
title: Catalogus zoeken
description: 'Als u de kenmerkovereenkomst wilt instellen die u helpt in aanmerking komende producten uit de handelscatalogus toe te wijzen aan Amazon-aanbiedingen, werkt u de zoekinstellingen van de catalogus bij.'
redirect_from: /sales-channels/asc/ob-catalog-search.html: 
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 981
ht-degree: 0%

---

# Catalogus zoeken

_De instellingen voor_ zoeken naar catalogi maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via het [opslagdashboard](./amazon-store-dashboard.md).

Met deze instellingen kunt u kenmerkovereenkomsten instellen die helpen om in aanmerking komende [!DNL Commerce]-producten toe te wijzen aan Amazon-aanbiedingen. Als Amazon een kaart heeft toegewezen, activeert het acties met betrekking tot prijzen, hoeveelheden, overschrijvingen en volgorde en productsynchronisatie.

Als u deze toewijzingswaarden definieert, neemt de kans op exacte overeenkomsten toe, waardoor de noodzaak om productaanbiedingen handmatig af te stemmen, tot een minimum wordt beperkt. Als u de kenmerken toevoegt als onderdeel van uw [Taken vóór installatie](./amazon-pre-setup-tasks.md), biedt Amazon-verkoopkanaal een groter potentieel om uw producten automatisch aan elkaar te koppelen tijdens het instappen en synchroniseren van productgegevens tussen Amazon en [!DNL Commerce].

Als u alleen het Amazon ASIN-kenmerk maakt (zonder ASIN-waarden per product toe te voegen), komen uw [!DNL Commerce]-producten mogelijk niet automatisch overeen met uw Amazon-aanbiedingen. U kunt uw producten [handmatig toewijzen. ](./creating-assigning-catalog-products.md) Handmatige overeenkomsten maken echter niet de gegevenselementen die nodig zijn voor het delen en synchroniseren van uw productgegevens.

>[!IMPORTANT]
>
>Als u handmatig een product aanpast en u een ASIN-, UPC- of ander gegevenselement voor het product wilt bijwerken, moet u de gegevens op twee plaatsen bijwerken. Werk deze bij in uw [!DNL Commerce]-catalogus en in uw Amazon-aanbieding in uw [!DNL Amazon Seller Central]-account.

Het is aan te raden deze kenmerken en waarden indien beschikbaar in kaart te brengen. Het voltooien van deze toewijzing is niet vereist, maar is gunstig voor productmatching en is vereist voor een correcte catalogussynchronisatie tussen Amazon en [!DNL Commerce].

Zie [Productkenmerken maken voor Amazon Matching](./ob-creating-magento-attributes.md) als u kenmerken wilt toevoegen.

## [!UICONTROL Catalog Search]-instellingen configureren

1. Klik **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Catalog Search]_uit.

1. Kies bij **[!UICONTROL ASIN]** het productkenmerk dat u voor de Amazon ASIN-waarde hebt gemaakt.

   Een ASIN ([!DNL Amazon Standard Identification Number]) is een uniek blok van tien letters en/of aantallen die punten identificeren. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object.

1. Kies bij **[!UICONTROL EAN]** het productkenmerk dat u voor de Amazon EAN-waarde hebt gemaakt.

   Het Europese artikelnummer (EAN) is een norm voor streepjescodes, een productidentificatiecode van twaalf of dertien cijfers. Elk EAN identificeert het product, de fabrikant en zijn kenmerken op unieke wijze; Doorgaans wordt het EAN als streepjescode afgedrukt op een etiket of verpakking van het product. Amazon heeft EAN-codes nodig om de kwaliteit van de zoekresultaten en de kwaliteit van de catalogus te verbeteren. U kunt EANs van de fabrikant verkrijgen.

1. Kies bij **[!UICONTROL GCID]** het productkenmerk dat u voor de Amazon GCIN-waarde hebt gemaakt.

   De globale catalogus-id (GCID) is een id voor producten die geen UPC-code of ISBN hebben. Met het Amazon-merkregister kunt u zich registreren als merkhouder en een unieke id voor producten maken.

1. Kies voor **[!UICONTROL ISBN]** het productkenmerk dat u voor de Amazon ISBN-waarde hebt gemaakt.

   Het ISBN (International Standard Book Number) is een unieke streepjescode ter identificatie van een handelsportefeuille. Elke ISBN-code identificeert een boek op unieke wijze. Een ISBN heeft of tien of 13 cijfers. Alle ISBN die na 1 januari 2007 worden toegewezen hebben 13 cijfers.

1. Kies bij **[!UICONTROL UPC]** het productkenmerk dat u voor de Amazon UPC-waarde hebt gemaakt.

   De Universal Product Code (UPC) is een streepjescode van 12 cijfers die veel wordt gebruikt voor detailverpakkingen in de Verenigde Staten.

1. Kies voor **[!UICONTROL General Search]** het productkenmerk dat u wilt gebruiken voor een algemene zoekovereenkomst.

   Dit kenmerk kunt u selecteren om de [!DNL Commerce]-producten af te stemmen op de desbetreffende Amazon-vermelding. Bij de algemene zoekopdracht worden trefwoordzoekopdrachten uit de catalogus gebruikt. Als dusdanig, wordt het geadviseerd om een [!DNL Commerce] attribuut te gebruiken dat relevante sleutelwoorden, zoals product SKU of productnaam draagt. Algemene zoekopdracht kan veel mogelijke overeenkomsten opleveren. In dergelijke gevallen kunt u de juiste Amazon-aanbieding selecteren uit de mogelijke overeenkomsten. Een algemene selectie voor dit veld is `Product Name`.

1. Klik op **[!UICONTROL Save listing settings]** als u klaar bent.

![Catalogus zoeken](assets/amazon-catalog-search.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br>ASIN staat voor de  [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL EAN (European Article Number)] | Een 12- of 13-cijferige productidentificatiecode. Het Europese artikelnummer (EAN) is een norm voor streepjescodes, een productidentificatiecode van twaalf of dertien cijfers. Elk EAN identificeert het product, de fabrikant en zijn kenmerken op unieke wijze; Doorgaans wordt het EAN als streepjescode afgedrukt op een etiket of verpakking van het product. Amazon heeft EAN-codes nodig om de kwaliteit van de zoekresultaten en de kwaliteit van de catalogus te verbeteren. U kunt EANs van de fabrikant verkrijgen. |
| [!UICONTROL GCID (Global Catalog Identifier)] | De globale catalogus-id (GCID) is een id voor producten die geen UPC-code of ISBN hebben. Met het Amazon-merkregister kunt u zich registreren als merkeigenaar en een unieke id maken voor producten die geen UPC of ISBN hebben. |
| [!UICONTROL ISBN (International Standard Book Number)] | Een unieke streepjescode voor een handelsportefeuille van 10 of 13 cijfers. Het ISBN (International Standard Book Number) is een unieke streepjescode ter identificatie van een handelsportefeuille. Elke ISBN-code identificeert een boek op unieke wijze. Een ISBN heeft of tien of 13 cijfers. Alle ISBN die na 1 januari 2007 worden toegewezen hebben 13 cijfers. |
| UPC (Universal Product Code) | Een streepjescode van 12 cijfers. De Universal Product Code (UPC) is een streepjescode van 12 cijfers die veel wordt gebruikt voor detailverpakkingen in de Verenigde Staten. |
| [!UICONTROL General Search] | Selecteer een kenmerk. Dit kenmerk kunt u selecteren om de [!DNL Commerce]-producten af te stemmen op de desbetreffende Amazon-vermelding. Bij de algemene zoekopdracht worden trefwoordzoekopdrachten uit de catalogus gebruikt. Als dusdanig, wordt het geadviseerd om een [!DNL Commerce] attribuut te gebruiken dat relevante sleutelwoorden, zoals product SKU of productnaam draagt. Algemene zoekopdracht kan veel mogelijke overeenkomsten opleveren. In dergelijke gevallen kunt u de juiste Amazon-aanbieding selecteren uit de mogelijke overeenkomsten. Een algemene selectie voor dit veld is `Product Name`. |

**Snelle toegang**  -  [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
