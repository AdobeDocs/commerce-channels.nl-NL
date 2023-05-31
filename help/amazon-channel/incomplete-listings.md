---
title: Onvolledige Amazon-aanbiedingen
description: Amazon-verkoopkanaal biedt [!UICONTROL Incomplete] om je te helpen bepalen welke objecten in aanmerking komen voor je onvolledige Amazon-aanbiedingen en om aan deze voorwaarden te voldoen.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Onvolledige Amazon-aanbiedingen

De _[!UICONTROL Incomplete]_wordt weergegeven [!DNL Commerce] catalogusproducten die voldoen aan uw Amazon-vereisten (gedefinieerd in uw [aanbiedingsregels](./listing-rules.md)), maar ontbreekt de door Amazon vereiste informatie (zoals de Amazon ASIN of een bepaalde productvoorwaarde).

Er zijn vier mogelijke oorzaken voor een onvolledige aanbieding, elk geïdentificeerd door zijn status.

| Status | Reden | Handeling |
|--- |--- |--- |
| Ontbrekende voorwaarde | Amazon accepteert aanbiedingen onder verschillende voorwaarden (zoals _Nieuw_, _Gereviseerd_, _Gebruikt: Als nieuw_) vereist een bepaalde voorwaarde. | Vereiste gegevens bijwerken en handmatig [een voorwaarde toewijzen](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) aan een aanbieding. |
| Kan niet toewijzen aan Amazon-aanbieding | Automatisch overeenkomst van deze aanbieding met uw catalogus is mislukt. Als er geen overeenkomst wordt gevonden, kan de aanbieding niet worden beheerd door Amazon Sales Channel | Vereiste gegevens bijwerken en handmatig [een ASIN toewijzen](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) op het catalogusproduct voor overeenkomende objecten met de aanbieding. |
| Meerdere overeenkomsten gevonden | Automatisch overeenkomst van deze aanbieding met uw catalogus is mislukt. Als er meerdere mogelijke overeenkomsten worden gevonden, moet u de juiste overeenkomst voor uw product selecteren. | Vereiste gegevens bijwerken en handmatig [een productovereenkomst kiezen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) voor het product en de aanbieding. |
| Heeft varianten | Als uw product varianten heeft, zoals een t-shirt dat in verschillende grootten of kleuren beschikbaar is, moet u de variant in uw catalogus kiezen die u op de juiste wijze wilt toewijzen en aan de lijst wilt aanpassen | Vereiste gegevens bijwerken en handmatig [de juiste variant kiezen](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) om deze aanbieding toe te wijzen en aan te passen. |

>[!NOTE]
>Als onvolledige aanbiedingen correct overeenkomen met je catalogusproducten, wordt de aanbieding verplaatst van _[!UICONTROL Incomplete]_en worden gepubliceerd naar Amazon op basis van uw [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) instellingen.

De beschikbare acties op de _[!UICONTROL Incomplete]_include:

Onder _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Kies ervoor om de automatische procedure te starten voor het koppelen van de gegevens van je Amazon-aanbiedingen aan je [!DNL Commerce] catalogus. Als producten niet automatisch overeenkomen, kunt u uw [_[!UICONTROL Catalog Search]_](./catalog-search.md) opties in de lijsten met aanbiedingen. Als aanbiedingen niet automatisch overeenkomen na het bijwerken van je _[!UICONTROL Catalog Search]_kunt u producten handmatig afstemmen in het dialoogvenster [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) handeling.

Onder **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom:

- **[!UICONTROL Update Required Info]**: Kies wanneer aanbiedingen niet automatisch overeenkomen met je catalogus. U kunt handmatig [catalogusproducten aan aanbiedingen koppelen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), handmatig [een ASIN toewijzen](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) in een catalogusovereenkomst, of [Een ontbrekende voorwaarde toewijzen](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) voor aanbieding.

- **[!UICONTROL View Details]**: Kies ervoor om de details van de aanbieding weer te geven, inclusief de [Logboek met aanbiedingsactiviteiten](./product-listing-details.md#listing-activity-log), [Prijsstelling voor Buy Box-concurrent](./product-listing-details.md#buy-box-competitor-pricing), en [Laagste concurrerende Prijs](./product-listing-details.md#lowest-competitor-pricing). Deze handeling is alleen bedoeld voor weergave. De details van de aanbieding kunnen niet worden gewijzigd. Zie [Details weergeven](./product-listing-details.md).

>[!NOTE]
>
>Als je aanbiedingen in behandeling hebt, verschijnt het aantal aanbiedingen in een bericht boven de tabbladen.

![Onvolledige Amazon-aanbiedingen](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Homepages van Amazon-verkoopkanalen delen [besturingselementen voor werkruimte](./workspace-controls.md) waarmee u de weergegeven gegevens kunt aanpassen.

| Kolom | Beschrijving |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br>ASIN staat voor de [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Condition] | De [voorwaarde](./product-listing-condition.md) van het product. |
| [!UICONTROL Landed Price] | De prijs van de aanbieding voor het product plus de verzendprijs. |
| [!UICONTROL Amazon Quantity] | De hoeveelheid die beschikbaar is wanneer het product actief op Amazon wordt aangeboden. |
| [!UICONTROL Status] | De status van de aanbieding, gedefinieerd door Amazon. Zie de tabel met de status hierboven. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom en selecteer een optie:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
