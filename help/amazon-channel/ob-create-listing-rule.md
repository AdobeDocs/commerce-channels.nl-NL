---
title: '"Aan boord: Regel voor aanbieding maken'''
description: Wanneer u het Amazon-verkoopkanaal voor instapkaarten voltooit, maakt u de regels voor eerste aanbiedingen voor het genereren van Amazon-aanbiedingen voor uw  [!DNL Commerce] producten.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Aan boord: Aanbiedingsregel maken

Lijstregels kunnen tijdens het instappen worden gedefinieerd, maar kunnen ook op elk moment worden gewijzigd. Na aan boord gaan, kunt u tot [aanbiedingsregels](./listing-rules.md) op de opslag [dashboard](./amazon-store-dashboard.md) toegang hebben.

## Een regel voor aanbiedingen maken tijdens het instappen

1. Nadat uw opslag wordt aangesloten, klik **[!UICONTROL View Store]** voor de toegevoegde opslag.

   De opslag [dashboard](./amazon-store-dashboard.md) verschijnt met het `No products listed to Amazon` bericht.

1. Klik op **[!UICONTROL Preview and List Eligible Products]**.

   De pagina _[!UICONTROL Listing Rules]_wordt weergegeven.

1. Bepaal de gewenste voorwaarden om in aanmerking te komen voor producten die op Amazon moeten worden vermeld en klik **[!UICONTROL Preview changes]**, of klik **[!UICONTROL Preview changes]** om deze stap over te slaan.

   Zie [Voorbeeld: Definieer een voorwaarde](./ob-define-condition-example.md).

1. Je aanbiedingen bekijken in de voorvertoning van de aanbieding:

   ![Voorvertoning van aanbieding](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - Producten die op dit tabblad worden aangeboden, komen niet in aanmerking voor Amazon-aanbiedingen op basis van de huidige standaardinstellingen voor aanbiedingen.

      Niet-subsidiabele producten worden niet gepubliceerd naar Amazon. Als een product dat niet in aanmerking komt al op Amazon wordt aangeboden en u de Amazon-aanbieding aanpast aan het catalogusproduct van [!DNL Commerce], verandert de hoeveelheid voor de aanbieding van Amazon in `0` om verkoop van het product te voorkomen. Als u een aanbieding handmatig uit Amazon wilt verwijderen, raadpleegt u [Een Amazon-aanbieding beëindigen](./end-listings-manually.md). Producten die niet in aanmerking komen voor Amazon-vereisten worden hier niet vermeld. Deze producten worden vermeld op [[!UICONTROL Inactive Listings] tabel](./inactive-listings.md).

      Als u een `Ineligible`-aanbieding wilt wijzigen in een `Eligible`-aanbieding, herhaalt u dit proces en wijzigt u de aanbiedingsregels.

   - **[!UICONTROL Eligible Listings]** - Producten die op dit tabblad worden aangeboden, komen in aanmerking voor Amazon-aanbieding op basis van de huidige instelling van de aanbiedingsregel en komen in aanmerking voor Amazon-vereisten. Dit tabblad bevat de bestaande Amazon-aanbiedingen die worden geïmporteerd (als u **[!UICONTROL Import Third Party Listings]** hebt ingesteld op `Import Listing` in uw [Aanbiedingsinstellingen](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - Producten die op dit tabblad worden aangeboden, bevatten  [!DNL Commerce] catalogusproducten die nieuw in aanmerking komen voor Amazon-aanbieding op basis van de huidige instelling van de aanbiedingsregel en maken Amazon-aanbiedingen.

1. Klik op **[!UICONTROL Save and Close]** als u klaar bent.

   De opslag [dashboard](./amazon-store-dashboard.md) opent.

Nadat een winkel is ingeschakeld, wordt de informatiesync tussen [!DNL Commerce] en Amazon gestart. Uw Amazon-aanbiedingen worden geïmporteerd in [!DNL Commerce] en proberen deze af te stemmen op producten in uw [!DNL Commerce]-catalogus.

U kunt de Amazon-bestelgegevens bekijken in het gedeelte _[!UICONTROL Recent Orders]_van het winkeldashboard. Zie [Het dashboard van de opslag](./amazon-store-dashboard.md) of [Bestellingen beheren](./managing-orders.md).

>[!IMPORTANT]
>
>Er zijn enkele belangrijke winkelinstellingen (aanbiedingen, prijzen, regels, naleving, meer) met standaardwaarden voor een nieuwe winkel. Controleer uw [opslaginstellingen](./default-store-settings.md) om ervoor te zorgen dat uw winkel is ingesteld op uw specifieke behoeften.

![Volgende ](assets/btn-next.png) [**pictogramDoorgaan naar standaardwinkelinstellingen**](./default-store-settings.md)
