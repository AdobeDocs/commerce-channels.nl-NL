---
title: Verkoopkanaal van Amazon - [!UICONTROL Listing Rules]
description: Met de aanbiedingsregels van het gebruik bepaalt u de catalogusproducten die als Amazon Marketplace-aanbiedingen worden gepubliceerd.
feature: Sales Channels, Products
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 0%

---

# [!UICONTROL Listing Rules]

Je hebt toegang tot de aanbiedingsregels voor winkelobjecten in het dialoogvenster [opslagdashboard](./amazon-store-dashboard.md).

De aanbiedingsregels bepalen de regels om te bepalen welke producten Amazon verkoopt aan Amazon. Deze regels bieden veel mogelijkheden om eenvoudige tot complexe regels te maken om producten als aanbiedingen op te nemen of uit te sluiten. Elke regel bestaat uit voorwaarden die de voorwaarden bepalen waaraan producten moeten voldoen om in aanmerking te komen voor een productlijst.

Je aanbiedingsregels worden voortdurend gesynchroniseerd met je [!DNL Commerce] catalogus. Wanneer u nieuwe [!DNL Commerce] producten die voldoen aan de voorwaarden om in aanmerking te komen voor je aanbieding, worden de producten automatisch verwerkt voor aanbieding op Amazon.

- Als je alle producten naar een Amazon-aanbieding wilt publiceren, moet je geen voorwaarden voor je aanbieding definiëren.

- Als je wilt beperken welke catalogusproducten naar Amazon worden gepubliceerd, definieert je de regelvoorwaarden voor aanbiedingen. Als je de voorwaarden voor je Amazon-aanbiedingsregels definieert, volg je dezelfde logica en hetzelfde proces als de voorwaarden definiëren voor [Lijnen met winkelprijzen](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

- Als een product volgens de aanbiedingsregels niet in aanmerking komt, verandert de status van dat product in `Ineligible`. Niet-subsidiabele producten worden niet gepubliceerd naar Amazon.

- Als een product dat niet in aanmerking komt al op Amazon wordt aangeboden en je de Amazon-aanbieding afstemt op je [!DNL Commerce] catalogusproduct, de hoeveelheid voor de Amazon-aanbieding verandert in `0` om verkoop van het product te voorkomen. Amazon-aanbiedingen kunnen [handmatig verwijderd](./end-listings-manually.md).

Wijzigingen in aantal en status van geschiktheid beïnvloeden alle aanbiedingen die de SKU van de verkoper van Amazon delen op markten die bestaan voor winkels die in dezelfde regio verkopen (zoals gedefinieerd in _[!UICONTROL Amazon Marketplace Country]_tijdens [winkelintegratie](./store-integration.md)). Een wijziging in een gedeelde [!DNL Amazon Seller SKU] in één regio heeft dit geen invloed op de Amazon-aanbiedingen van het product in een ander land.

![Aanbiedingsregels](assets/ob-listing-rules.png){width="600" zoomable="yes"}

## Instellingen voor aanbiedingsregels configureren

1. Klikken **[!UICONTROL Listing Rules]** op het opslagdashboard.

1. Bepaal de voorwaarden die je wilt stellen om in aanmerking te komen voor producten die op Amazon worden aangeboden.

Zie [Voorbeeld: een voorwaarde definiëren](./ob-define-condition-example.md).

| Veld | Beschrijving |
|-------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Websites] | Welke opties beschikbaar zijn, is afhankelijk van de [websites](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) u hebt ingesteld in uw [!DNL Commerce] configuratie. Selecteer de website voor de in aanmerking komende producten die op Amazon worden vermeld. Er kan slechts één website worden geselecteerd, omdat voor elke website een unieke Amazon-winkel nodig is die in Amazon-verkoopkanalen is gemaakt. |
| [!UICONTROL Conditions] | Hiermee definieert u de [!DNL Commerce] -kenmerken voor producten die in uw Amazon-regio in aanmerking komen. Zie [Voorbeeld: een voorwaarde definiëren](./ob-define-condition-example.md). |

## Functie Voorwaarden

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

- Voeg geen voorwaarden toe als alle producten binnen de geselecteerde websites in aanmerking komen.
- Er is een complexe reeks back-end processen om direct met Amazon-systemen te communiceren. Op basis van het aantal objecten dat je probeert aan te bieden en de manier waarop het druk is met Amazon-systemen (zoals &#39;Zwarte Vrijdag&#39;), kan het enige tijd duren voordat je objecten op Amazon worden aangeboden.

Zie voor meer informatie over voorwaarden [Beschrijf de Voorwaarden](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

## Voorvertoning van aanbiedingsregel

Wanneer je de definities van je voorwaarden wijzigt voor je aanbiedingsregels, kun je klikken op **[!UICONTROL Preview Changes]** om de wijzigingen in je regels toe te passen en te bekijken wat de gevolgen voor je aanbiedingen zijn. Verifieer je aanbiedingen in deze voorvertoningsfunctie voordat je wijzigingen in de aanbiedingsregel opslaat.

Je Amazon-aanbiedingen worden vergeleken met je regels en voorwaarden. U kunt dan controleren:

- Welke producten op basis van uw huidige situatie naar een status komen die niet in aanmerking komt [!DNL Amazon Seller Central] account
- Welke producten van een staat die niet in aanmerking komt, naar een status terugkeren die in aanmerking komt
- Welke producten zijn Nieuwe Amazon-aanbiedingen en worden aan je Amazon-aanbieding toegevoegd vanuit je in aanmerking komende producten [!DNL Commerce] producten

Met Voorvertoning van aanbieding kun je je potentiële Amazon-aanbiedingen bekijken en de regels voor aanbiedingen aanpassen.

Je potentiële Amazon-aanbiedingen worden ingevuld op het tabblad _[!UICONTROL Listing Preview]_pagina in een van de drie tabbladen:

- **[!UICONTROL Ineligible Listings]** - Aangeboden producten komen niet in aanmerking voor Amazon-aanbieding op basis van de huidige aanbiedingsregels en -voorwaarden.

  Niet-subsidiabele producten worden niet gepubliceerd naar Amazon. Als een product dat niet in aanmerking komt al op Amazon wordt aangeboden en je de Amazon-aanbieding afstemt op je [!DNL Commerce] catalogusproduct, de hoeveelheid voor de Amazon-aanbieding verandert in `0` om verkoop van het product te voorkomen. Als u een aanbieding handmatig wilt verwijderen, raadpleegt u [Een Amazon-aanbieding beëindigen](./end-listings-manually.md). Producten die niet in aanmerking komen voor Amazon-vereisten worden hier niet vermeld. Deze producten zijn opgenomen in de [Tabblad Niet-actieve aanbiedingen](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - Aangeboden producten komen in aanmerking voor Amazon-aanbieding op basis van de huidige aanbiedingsregels en -voorwaarden en komen ook in aanmerking voor Amazon-vereisten. Deze lijst bevat de bestaande Amazon-aanbiedingen die worden geïmporteerd (als je **Aanbiedingen van derden importeren** instellen op `Import Listing` in [Aanbiedingsinstellingen](./third-party-listing-settings.md)).

- **[!UICONTROL New Listings]** - De vermelde producten omvatten uw [!DNL Commerce] catalogiseer producten die nieuw in aanmerking komen voor Amazon-aanbieding op basis van de huidige aanbiedingsregels en -voorwaarden en maak en publiceer nieuwe Amazon-aanbiedingen.

### Je voorbeeld van een aanbieding bekijken

1. Klikken **[!UICONTROL Listing Rules]** op het opslagdashboard.

1. Uw bekijken of toevoegen [aanbiedingsregels](./listing-rules.md).

1. Wijzig uw [Voorwaarden voor aanbiedingsregels](./ob-define-condition-example.md).

1. Klik op **[!UICONTROL Preview Changes]**.

1. Je aanbiedingen bekijken en bevestigen in het dialoogvenster _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_, en _[!UICONTROL New Listings]_tabs.

1. Als je aanbiedingen aan je verwachtingen voldoen, klik je op **[!UICONTROL Save and close]**.

   Als je aanbiedingen niet zoals verwacht worden weergegeven, klikt u op **[!UICONTROL Back]** en wijzig je regels en voorwaarden totdat je aanbiedingen aan je verwachtingen voldoen.

![Voorvertoning van aanbiedingsregel](assets/amazon-listing-rule-preview.png){width="600" zoomable="yes"}

### Records met aanbiedingsvoorbeelden

| Veld | Beschrijving |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product ID] | Het unieke, opeenvolgende nummer dat aan een [!DNL Commerce] catalogusproduct wanneer het wordt toegevoegd. |
| [!UICONTROL Thumbnail] | Geeft een miniatuur van de hoofdafbeelding van het product weer. |
| [!UICONTROL Name] | De naam van het product, beheerd in de [!DNL Commerce] [productraster](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html). |
| [!UICONTROL Type] | Het type product, beheerd in de [!DNL Commerce] productraster. |
| [!UICONTROL Attribute Set] | De naam van de kenmerkenreeks die als malplaatje voor het product wordt gebruikt, in wordt beheerd [!DNL Commerce] productraster. |
| [!UICONTROL SKU] | De unieke voorraadbewaareenheid die aan het product wordt toegewezen, die in [!DNL Commerce] productraster. |
| [!UICONTROL Visibility] | Geeft aan waar het product zichtbaar is en wordt beheerd in het dialoogvenster [!DNL Commerce] productraster. Opties:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Status | Geeft de status van het product aan, beheerd in de [!DNL Commerce] productraster. Opties: `Enabled` / `Disabled` |

![Workflow voor voorvertoningen](assets/listing-preview-flowchart.png){width="500" zoomable="yes"}
