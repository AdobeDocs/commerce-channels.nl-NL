---
title: Amazon-verkoopkanaal - [!UICONTROL Listing Rules]
description: Met aanbiedingsregels kun je de Commerce-catalogusproducten bepalen die als Amazon Marketplace-aanbiedingen worden gepubliceerd.
feature: Sales Channels, Products
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# [!UICONTROL Listing Rules]

U kunt tot de lijstregels voor opslag in het [ opslagdashboard ](./amazon-store-dashboard.md) toegang hebben.

De aanbiedingsregels bepalen de regels om te bepalen welke producten Amazon verkoopt aan Amazon. Deze regels bieden veel mogelijkheden om eenvoudige tot complexe regels te maken om producten als aanbiedingen op te nemen of uit te sluiten. Elke regel bestaat uit voorwaarden die de voorwaarden bepalen waaraan producten moeten voldoen om in aanmerking te komen voor een productlijst.

Je aanbiedingsregels worden voortdurend gesynchroniseerd met je catalogus van [!DNL Commerce] . Als je nieuwe [!DNL Commerce] -producten toevoegt die voldoen aan de voorwaarden om in aanmerking te komen voor aanbieding, worden de producten automatisch verwerkt voor aanbieding op Amazon.

- Als je alle producten naar een Amazon-aanbieding wilt publiceren, moet je geen voorwaarden voor je aanbieding definiëren.

- Als je wilt beperken welke catalogusproducten naar Amazon worden gepubliceerd, definieert je de regelvoorwaarden voor aanbiedingen. Het bepalen van de voorwaarden voor uw Amazon lijstregels volgt de zelfde logica en het proces zoals het bepalen van de voorwaarden voor [ Regels van de Prijs van de Kar ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

- Als je aanbiedingsregels een product uitsluiten, verandert de status om in aanmerking te komen voor dat product in `Ineligible` . Niet-subsidiabele producten worden niet gepubliceerd naar Amazon.

- Als een product dat niet in aanmerking komt al op Amazon wordt aangeboden en je de Amazon-aanbieding afstemt op het catalogusproduct van [!DNL Commerce] , verandert de hoeveelheid voor de Amazon-aanbieding in `0` om verkoop van het product te voorkomen. De lijsten van Amazon kunnen [ manueel worden verwijderd ](./end-listings-manually.md).

De veranderingen in aantal en geschiktheidsstatus beïnvloeden alle aanbiedingen die het SKU van de Verkoper van Amazon in marktplaatsen delen die voor opslag bestaan die in het zelfde gebied (zoals die in _[!UICONTROL Amazon Marketplace Country]_tijdens [ wordt bepaald opslagintegratie ](./store-integration.md) verkopen). Een wijziging van een gedeelde [!DNL Amazon Seller SKU] in een regio heeft echter geen invloed op de Amazon-aanbiedingen van het product in een ander land.

![ Lijstregels ](assets/ob-listing-rules.png){width="600" zoomable="yes"}

## Instellingen voor aanbiedingsregels configureren

1. Klik op **[!UICONTROL Listing Rules]** op het opslagdashboard.

1. Bepaal de voorwaarden die je wilt stellen om in aanmerking te komen voor producten die op Amazon worden aangeboden.

Zie [ Voorbeeld: Bepaal een Voorwaarde ](./ob-define-condition-example.md).

| Veld | Beschrijving |
|-------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Websites] | De beschikbare opties hangen van de [ websites ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) af u opstelling in uw [!DNL Commerce] configuratie hebt. Selecteer de website voor de in aanmerking komende producten die op Amazon worden vermeld. Er kan slechts één website worden geselecteerd, omdat voor elke website een unieke Amazon-winkel nodig is die in Amazon-verkoopkanalen is gemaakt. |
| [!UICONTROL Conditions] | Hiermee definieert u de [!DNL Commerce] -kenmerken voor productgeschiktheid in uw Amazon-regio. Zie [ Voorbeeld: Bepaal een Voorwaarde ](./ob-define-condition-example.md). |

## Functie Voorwaarden

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

- Voeg geen voorwaarden toe als alle producten binnen de geselecteerde websites in aanmerking komen.
- Er is een complexe reeks back-end processen om direct met Amazon-systemen te communiceren. Op basis van het aantal objecten dat je probeert aan te bieden en de manier waarop het druk is met Amazon-systemen (zoals &#39;Zwarte Vrijdag&#39;), kan het enige tijd duren voordat je objecten op Amazon worden aangeboden.

Voor meer informatie over voorwaarden, zie [ beschrijf de Voorwaarden ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

## Voorvertoning van aanbiedingsregel

Wanneer je de definities van je voorwaarden wijzigt voor je aanbiedingsregels, kun je op **[!UICONTROL Preview Changes]** klikken om de wijzigingen in je regels toe te passen en te bekijken wat de gevolgen zijn voor je aanbiedingen. Verifieer je aanbiedingen in deze voorvertoningsfunctie voordat je wijzigingen in de aanbiedingsregel opslaat.

Je Amazon-aanbiedingen worden vergeleken met je regels en voorwaarden. U kunt dan controleren:

- Welke producten naar een status die niet in aanmerking komt, worden verplaatst op basis van uw huidige [!DNL Amazon Seller Central] -account
- Welke producten van een staat die niet in aanmerking komt, naar een status terugkeren die in aanmerking komt
- Welke producten zijn Nieuwe Amazon-aanbiedingen en worden aan je Amazon-aanbieding toegevoegd vanuit in aanmerking komende [!DNL Commerce] producten

Met Voorvertoning van aanbieding kun je je potentiële Amazon-aanbiedingen bekijken en de regels voor aanbiedingen aanpassen.

Je potentiële Amazon-aanbiedingen worden op de pagina _[!UICONTROL Listing Preview]_in een van de volgende drie tabbladen ingevuld:

- **[!UICONTROL Ineligible Listings]** - Aangeboden producten komen niet in aanmerking voor Amazon-aanbieding op basis van de huidige aanbiedingsregels en -voorwaarden.

  Niet-subsidiabele producten worden niet gepubliceerd naar Amazon. Als een product dat niet in aanmerking komt al op Amazon wordt aangeboden en je de Amazon-aanbieding afstemt op het catalogusproduct van [!DNL Commerce] , verandert de hoeveelheid voor de Amazon-aanbieding in `0` om verkoop van het product te voorkomen. Om een lijst manueel te verwijderen, zie [ Eind een Amazon van lijst ](./end-listings-manually.md). Producten die niet in aanmerking komen voor Amazon-vereisten worden hier niet vermeld. Die producten zijn vermeld op het [ Inactieve lusje van Lijsten ](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - Aangeboden producten komen in aanmerking voor Amazon-aanbieding op basis van de huidige aanbiedingsregels en -voorwaarden en komen ook in aanmerking voor Amazon-vereisten. Deze lijst omvat uw bestaande lijsten van Amazon die (als u **de Lijsten van de Derde van de Invoer** geplaatst aan `Import Listing` in [ het Lijsten van Montages ](./third-party-listing-settings.md) hebt ingevoerd).

- **[!UICONTROL New Listings]** - De aangeboden producten bevatten de catalogusproducten van [!DNL Commerce] die nieuw in aanmerking komen voor Amazon-aanbieding op basis van de huidige aanbiedingsregels en -voorwaarden, en maken en publiceren nieuwe Amazon-aanbiedingen.

### Je voorbeeld van een aanbieding bekijken

1. Klik op **[!UICONTROL Listing Rules]** op het opslagdashboard.

1. Bekijk of voeg uw [ lijstregels ](./listing-rules.md) toe.

1. Wijzig uw [ Voorwaarden van de Regel van de Lijst ](./ob-define-condition-example.md).

1. Klik op **[!UICONTROL Preview Changes]**.

1. Bekijk en bevestig je aanbiedingen op de tabbladen _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_ en _[!UICONTROL New Listings]_.

1. Klik op **[!UICONTROL Save and close]** als je aanbiedingen aan je verwachtingen voldoen.

   Als je aanbiedingen niet zoals verwacht worden weergegeven, klik je op **[!UICONTROL Back]** en wijzig je regels en voorwaarden totdat je aanbiedingen aan je verwachtingen voldoen.

![ de voorproef van de lijstregel ](assets/amazon-listing-rule-preview.png){width="600" zoomable="yes"}

### Records met aanbiedingsvoorbeelden

| Veld | Beschrijving |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product ID] | Het unieke, opeenvolgende nummer dat aan een catalogusproduct van [!DNL Commerce] wordt toegewezen wanneer het wordt toegevoegd. |
| [!UICONTROL Thumbnail] | Geeft een miniatuur van de hoofdafbeelding van het product weer. |
| [!UICONTROL Name] | De naam van het product, dat in het [!DNL Commerce] [ wordt geleid productennet ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html). |
| [!UICONTROL Type] | Het type product dat wordt beheerd in het productraster van [!DNL Commerce] . |
| [!UICONTROL Attribute Set] | De naam van de kenmerkenreeks die als malplaatje voor het product wordt gebruikt, die in het [!DNL Commerce] productnet wordt beheerd. |
| [!UICONTROL SKU] | De unieke Stock Keeping Unit die aan het product wordt toegewezen, die in het [!DNL Commerce] productnet wordt beheerd. |
| [!UICONTROL Visibility] | Geeft aan waar het product zichtbaar is en wordt beheerd in het productraster van [!DNL Commerce] . Opties:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Status | Geeft de status van het product aan, beheerd in het productraster van [!DNL Commerce] . Opties: `Enabled` / `Disabled` |

![ het van de lijst voorproefwerkschema ](assets/listing-preview-flowchart.png){width="500" zoomable="yes"}
