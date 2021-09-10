---
title: Onvolledige aanbiedingen
description: Het verkoopkanaal van Amazon biedt het tabblad [!UICONTROL Incomplete] om u te helpen bij het identificeren van en voldoen aan geschiktheidsvereisten voor onvolledige Amazon-aanbiedingen.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Onvolledige aanbiedingen

Het tabblad _[!UICONTROL Incomplete]_bevat een lijst met de catalogusproducten [!DNL Commerce] die voldoen aan uw Amazon-geschiktheidsvereisten (gedefinieerd in uw [aanbiedingsregels](./listing-rules.md)), maar die informatie missen die Amazon vereist (zoals de Amazon ASIN of een gedefinieerde productvoorwaarde).

Er zijn vier mogelijke oorzaken voor een onvolledige aanbieding, elk geïdentificeerd door zijn status.

| Status | Reden | Handeling |
|--- |--- |--- |
| Ontbrekende voorwaarde | Amazon accepteert aanbiedingen onder verschillende omstandigheden (zoals _Nieuw_, _Gereviseerd_, _Gebruikt: Voor deze aanbieding geldt een gedefinieerde voorwaarde, net als voor Nieuwe_). | Werk vereiste informatie bij en wijs manueel [een voorwaarde ](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) aan een lijst toe. |
| Kan niet toewijzen aan Amazon-aanbieding | Automatisch overeenkomst van deze aanbieding met uw catalogus is mislukt. Als er geen overeenkomst wordt gevonden, kan de aanbieding niet worden beheerd door Amazon Sales Channel | De vereiste informatie bijwerken en [wijs manueel een ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) aan het catalogusproduct voor aanpassing aan de lijst toe. |
| Meerdere overeenkomsten gevonden | Automatisch overeenkomst van deze aanbieding met uw catalogus is mislukt. Als er meerdere mogelijke overeenkomsten worden gevonden, moet u de juiste overeenkomst voor uw product selecteren. | Werk vereiste informatie bij en kies handmatig [een productovereenkomst](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) voor het product en de lijst. |
| Heeft varianten | Als uw product varianten heeft, zoals een t-shirt dat in verschillende grootten of kleuren beschikbaar is, moet u de variant in uw catalogus kiezen die u op de juiste wijze wilt toewijzen en aan de lijst wilt aanpassen | Werk vereiste informatie bij en kies manueel [de correcte variant](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) om aan dit lijst toe te wijzen en aan te passen. |

>[!NOTE]
>Wanneer onvolledige aanbiedingen correct overeenkomen met uw catalogusproducten, wordt de aanbieding verplaatst van het tabblad _[!UICONTROL Incomplete]_en op basis van uw [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md)-instellingen gepubliceerd naar Amazon.

De beschikbare acties op het _[!UICONTROL Incomplete]_lusje omvatten:

Onder _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Kies ervoor om het automatische proces te starten voor het koppelen van de gegevens van je Amazon-aanbiedingen aan je  [!DNL Commerce] catalogus. Als producten niet automatisch overeenkomen, kunt u de [_[!UICONTROL Catalog Search]_](./catalog-search.md)-opties in de aanbiedingsbrieven opnieuw bekijken. Als aanbiedingen niet automatisch overeenkomen nadat u de _[!UICONTROL Catalog Search]_-opties hebt bijgewerkt, kunt u de producten handmatig afstemmen in de handeling [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found).

Onder **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom:

- **[!UICONTROL Update Required Info]**: Kies wanneer aanbiedingen niet automatisch overeenkomen met je catalogus. U kunt catalogusproducten handmatig [aanpassen aan aanbiedingen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), handmatig [een ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) toewijzen aan een catalogusovereenkomst of [een ontbrekende voorwaarde toewijzen](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) voor een aanbieding.

- **[!UICONTROL View Details]**: Kies ervoor om de lijstdetails, met inbegrip van het Logboek [ van de Activiteit van de ](./product-listing-details.md#listing-activity-log)Lijst, de Prijsbepaling [ van de Concurrentie van ](./product-listing-details.md#buy-box-competitor-pricing)Buy Box, en de  [Laagste Prijsverhoging](./product-listing-details.md#lowest-competitor-pricing) van de Concurrant te bekijken. Deze handeling is alleen bedoeld voor weergave. De details van de aanbieding kunnen niet worden gewijzigd. Zie [Details weergeven](./product-listing-details.md).

>[!NOTE]
>
>Als je aanbiedingen in behandeling hebt, verschijnt het aantal aanbiedingen in een bericht boven de tabbladen.

![Onvolledige Amazon-aanbiedingen](assets/amazon-incomplete-listings.png)

Amazon-homepages van verkoopkanalen hebben gemeenschappelijke [besturingselementen voor werkruimten](./workspace-controls.md) waarmee u de weergegeven gegevens kunt aanpassen.

| Kolom | Beschrijving |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br>ASIN staat voor de  [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Condition] | De [voorwaarde](./product-listing-condition.md) van het product. |
| [!UICONTROL Landed Price] | De prijs van de aanbieding voor het product plus de verzendprijs. |
| [!UICONTROL Amazon Quantity] | De hoeveelheid die beschikbaar is wanneer het product actief op Amazon wordt aangeboden. |
| [!UICONTROL Status] | De status van de aanbieding, gedefinieerd door Amazon. Zie de tabel met de status hierboven. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_en selecteert u een optie:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
