---
title: Niet in aanmerking komende Amazon-aanbiedingen
description: Het verkoopkanaal van Amazon biedt het tabblad [!UICONTROL Ineligible] om je te helpen objecten te beheren die niet in aanmerking komen als een aanbieding op basis van je huidige aanbiedingsregels.
feature: Sales Channels, Products
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Niet in aanmerking komende Amazon-aanbiedingen

Het tabblad _[!UICONTROL Ineligible]_bevat een lijst met alle producten die momenteel op Amazon zijn gepubliceerd, maar die niet in aanmerking komen voor een aanbieding op basis van de huidige aanbiedingsregels. Als een vorig product verkiesbaar was en de lijstregels worden gewijzigd om het nu niet in aanmerking te nemen, daalt de hoeveelheid verbonden aan een product aan 0 en het product wordt duidelijk als_ niet in aanmerking komend _. Deze blijft echter wel aanwezig op uw [!DNL Amazon Seller Account] .

Om een product uit het _[!UICONTROL Ineligible]_lusje te bewegen, kunt u [ uw lijstregels ](./listing-rules.md) wijzigen om uw producten toe te staan om in aanmerking te komen.

De beschikbare acties op het tabblad _[!UICONTROL Ineligible]_zijn:

Onder _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: kies ervoor alle geselecteerde aanbiedingen te verwijderen uit de [!DNL Amazon Marketplace] . Zie [ een Amazon het Vermelden ](./end-listings-manually.md) beëindigen.

- **[!UICONTROL Edit Listing Overrides]**: verander de overschrijvingsinstellingen voor de vermelding. Zie [ met voeten treedt ](./overrides.md) of [ uitgeven of verwijderen een opheffing ](./creating-editing-overrides.md#edit-override-single-listing).

Onder **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_:

- **[!UICONTROL View Details]**: verkies om lijstdetails, met inbegrip van het [ Lijst Logboek van de Activiteit ](./product-listing-details.md#listing-activity-log) te bekijken, [ het Prijstarief van de Mededinger van de Buy Box ](./product-listing-details.md#buy-box-competitor-pricing), en [ Laagste Prijsverhoging van de Concurrent ](./product-listing-details.md#lowest-competitor-pricing). Deze handeling is alleen bedoeld voor weergave. De details van de aanbieding kunnen niet worden gewijzigd. Zie [ Details van de Mening ](./product-listing-details.md).

- **[!UICONTROL Create Override]**: maak een overschrijving en pas deze toe op deze aanbieding. Zie [ een opheffing ](./creating-editing-overrides.md) creëren.

- **[!UICONTROL Edit Assigned ASIN]**: kies ervoor om de ASIN te wijzigen die aan uw catalogusproduct is toegewezen. Deze actie wordt gebruikt als een product in uw catalogus aan verkeerde ASIN werd aangepast. Zie [ een Toegewezen ASIN ](./edit-assigned-asin.md) uitgeven.

- **[!UICONTROL Create Alias Seller SKU]**: maak een Alias-SKU die u kunt gebruiken om een Amazon-aanbieding te maken van hetzelfde catalogusproduct. Zie [ een Alias Seller SKU ](./create-alias-seller-sku.md) creëren.

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: kies ervoor om de uitvoeringsmethode te wijzigen die aan de volgorde is gekoppeld. Zie [ vormen gevuld door montages ](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: verwijder de vermelding uit de [!DNL Amazon Marketplace] . Zie [ een Amazon het Vermelden ](./end-listings-manually.md) beëindigen.

>[!NOTE]
>Als je aanbiedingen in behandeling hebt, wordt het aantal aanbiedingen weergegeven in een bericht boven de tabbladen.

![ Niet in aanmerking komende lijsten van Amazon ](assets/amazon-ineligible-listings.png){width="600" zoomable="yes"}

Amazon delen de homepages van het verkoopkanaal wat gemeenschappelijke [ werkruimtesecontroles ](./workspace-controls.md) die u toestaan om de gegevens aan te passen die worden getoond.

## Standaardkolommen

| Kolom | Beschrijving |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br> ASIN staat voor [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Condition] | De [ voorwaarde ](./product-listing-condition.md) van het product. |
| [!UICONTROL Landed Price] | De prijs van de aanbieding voor het product plus de verzendprijs. |
| [!UICONTROL Amazon Quantity] | De hoeveelheid die beschikbaar is wanneer het product actief op Amazon wordt aangeboden. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_en selecteert u een optie:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[ creeer Opheffing ](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
