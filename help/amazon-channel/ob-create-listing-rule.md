---
title: Een regel voor Amazon-aanbiedingen maken
description: Wanneer je het Amazon-verkoopkanaal voor instapkaarten voltooit, moet je de regels voor eerste aanbiedingen maken voor het genereren van Amazon-aanbiedingen voor je [!DNL Commerce] producten.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Een regel voor Amazon-aanbiedingen maken

Lijstregels kunnen tijdens het instappen worden gedefinieerd, maar kunnen ook op elk moment worden gewijzigd. Na het instappen, kunt u tot [aanbiedingsregels](./listing-rules.md) in de winkel [dashboard](./amazon-store-dashboard.md).

## Een regel voor aanbiedingen maken tijdens het instappen

1. Klik op **[!UICONTROL View Store]** voor de toegevoegde winkel.

   De winkel [dashboard](./amazon-store-dashboard.md) wordt weergegeven met de `No products listed to Amazon` bericht.

1. Klikken **[!UICONTROL Preview and List Eligible Products]**.

   De _[!UICONTROL Listing Rules]_wordt weergegeven.

1. Bepaal de gewenste voorwaarden om in aanmerking te komen voor producten die op Amazon worden aangeboden en klik **[!UICONTROL Preview changes]** of klik op **[!UICONTROL Preview changes]** om deze stap over te slaan.

   Zie [Voorbeeld: Een voorwaarde definiëren](./ob-define-condition-example.md).

1. Je aanbiedingen bekijken in de voorvertoning van de aanbieding:

   ![Voorvertoning van aanbieding](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]** - Producten die op dit tabblad worden aangeboden, komen niet in aanmerking voor Amazon-aanbiedingen op basis van de huidige standaardinstellingen voor aanbiedingen.

      Niet-subsidiabele producten worden niet gepubliceerd naar Amazon. Als een product dat niet in aanmerking komt al op Amazon wordt aangeboden en je de Amazon-aanbieding afstemt op je [!DNL Commerce] catalogusproduct, de hoeveelheid voor de Amazon-aanbieding verandert in `0` om verkoop van het product te voorkomen. Als je een aanbieding handmatig uit Amazon wilt verwijderen, raadpleegt u [Een Amazon-aanbieding beëindigen](./end-listings-manually.md). Producten die niet in aanmerking komen voor Amazon-vereisten worden hier niet vermeld. Deze producten zijn opgenomen in de [[!UICONTROL Inactive Listings] tab](./inactive-listings.md).

      Als u een `Ineligible` aanbieding aan een `Eligible` aanbieden, dit proces herhalen en je aanbiedingsregels wijzigen.

   - **[!UICONTROL Eligible Listings]** - Producten die op dit tabblad worden aangeboden, komen in aanmerking voor Amazon-aanbieding op basis van de huidige instelling van de aanbiedingsregel en komen in aanmerking voor Amazon-vereisten. Dit tabblad bevat de bestaande Amazon-aanbiedingen die zijn geïmporteerd (als je **[!UICONTROL Import Third Party Listings]** instellen op `Import Listing` in uw [Aanbiedingsinstellingen](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - Producten die op dit tabblad worden vermeld, omvatten uw [!DNL Commerce] catalogusproducten die nieuw in aanmerking komen voor Amazon-aanbieding op basis van de huidige instelling van de regel voor aanbiedingen en maak Amazon-aanbiedingen.

1. Klik op **[!UICONTROL Save and Close]**.

   De winkel [dashboard](./amazon-store-dashboard.md) wordt geopend.

Nadat het aan boord gaan van een winkel is voltooid, wordt de informatie gesynchroniseerd tussen [!DNL Commerce] en Amazon wordt gestart. Je Amazon-aanbiedingen worden geïmporteerd in [!DNL Commerce] en proberen te passen met producten in uw [!DNL Commerce] Catalogus.

U kunt uw Amazon-ordergegevens bekijken in het dialoogvenster _[!UICONTROL Recent Orders]_van het opslagdashboard. Zie [Winkeldashboard](./amazon-store-dashboard.md) of [Bestellingen beheren](./managing-orders.md).

>[!IMPORTANT]
>
>Er zijn enkele belangrijke winkelinstellingen (aanbiedingen, prijzen, regels, naleving, meer) met standaardwaarden voor een nieuwe winkel. Om ervoor te zorgen dat uw winkel is ingesteld op uw specifieke behoeften, raadpleegt u uw [opslaginstellingen](./default-store-settings.md) .

![Volgende pictogram](assets/btn-next.png) [**Doorgaan met standaardwinkelinstellingen**](./default-store-settings.md)
