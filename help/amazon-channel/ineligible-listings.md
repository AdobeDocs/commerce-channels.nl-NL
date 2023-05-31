---
title: Niet in aanmerking komende Amazon-aanbiedingen
description: Amazon-verkoopkanaal biedt [!UICONTROL Ineligible] om je te helpen objecten te beheren, komen niet in aanmerking als een aanbieding op basis van je huidige aanbiedingsregels.
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Niet in aanmerking komende Amazon-aanbiedingen

De _[!UICONTROL Ineligible]_bevat een lijst met alle producten die momenteel op Amazon zijn gepubliceerd maar die niet in aanmerking komen voor een aanbieding op basis van de huidige aanbiedingsregels. Als een eerder product in aanmerking kwam en de aanbiedingsregels zijn gewijzigd om het nu niet in aanmerking te laten komen, daalt de hoeveelheid die aan een product is gekoppeld tot 0 en wordt het product gemarkeerd als_ niet-subsidiabel _. Het is echter nog steeds aanwezig op uw [!DNL Amazon Seller Account].

Een product uit de _[!UICONTROL Ineligible]_tabblad, kunt u [Je aanbiedingsregels wijzigen](./listing-rules.md) om uw producten in aanmerking te laten komen.

De beschikbare acties op de _[!UICONTROL Ineligible]_include:

Onder _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: Kies ervoor om alle geselecteerde aanbiedingen te verwijderen uit de [!DNL Amazon Marketplace]. Zie [Een Amazon-aanbieding beëindigen](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: Kies of u de overschrijvingsinstellingen voor de aanbieding wilt wijzigen. Zie [Overschrijvingen](./overrides.md) of [Een overschrijving bewerken of verwijderen](./creating-editing-overrides.md#edit-override-single-listing).

Onder **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom:

- **[!UICONTROL View Details]**: Kies ervoor om de details van de aanbieding weer te geven, inclusief de [Logboek met aanbiedingsactiviteiten](./product-listing-details.md#listing-activity-log), [Prijsstelling voor Buy Box-concurrent](./product-listing-details.md#buy-box-competitor-pricing), en [Laagste concurrerende Prijs](./product-listing-details.md#lowest-competitor-pricing). Deze handeling is alleen bedoeld voor weergave. De details van de aanbieding kunnen niet worden gewijzigd. Zie [Details weergeven](./product-listing-details.md).

- **[!UICONTROL Create Override]**: Kies of u een overschrijving wilt maken en deze op deze aanbieding wilt toepassen. Zie [Een overschrijving maken](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: Kies of u de ASIN wilt wijzigen die aan het catalogusproduct is toegewezen. Deze actie wordt gebruikt als een product in uw catalogus aan verkeerde ASIN werd aangepast. Zie [Een toegewezen ASIN bewerken](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: Maak een Alias-SKU die u kunt gebruiken om een Amazon-aanbieding te maken van hetzelfde catalogusproduct. Zie [Een SKU voor Alias Seller maken](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: Kies of u de uitvoeringsmethode wilt wijzigen die aan de volgorde is gekoppeld. Zie [Instellingen Volledig ingevuld door configureren](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: Kies of u de aanbieding wilt verwijderen uit de [!DNL Amazon Marketplace]. Zie [Een Amazon-aanbieding beëindigen](./end-listings-manually.md).

>[!NOTE]
>Als je aanbiedingen in behandeling hebt, wordt het aantal aanbiedingen weergegeven in een bericht boven de tabbladen.

![Niet in aanmerking komende Amazon-aanbiedingen](assets/amazon-ineligible-listings.png){width="600" zoomable="yes"}

Homepages van Amazon-verkoopkanalen delen [besturingselementen voor werkruimte](./workspace-controls.md) waarmee u de weergegeven gegevens kunt aanpassen.

## Standaardkolommen

| Kolom | Beschrijving |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br>ASIN staat voor de [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Condition] | De [voorwaarde](./product-listing-condition.md) van het product. |
| [!UICONTROL Landed Price] | De prijs van de aanbieding voor het product plus de verzendprijs. |
| [!UICONTROL Amazon Quantity] | De hoeveelheid die beschikbaar is wanneer het product actief op Amazon wordt aangeboden. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom en selecteer een optie:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[Overschrijven maken](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
