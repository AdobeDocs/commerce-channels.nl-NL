---
title: Een regel voor Amazon-aanbiedingen maken
description: Terwijl het voltooien van het Amazon verkoopkanaal onboarding proces, creeer de aanvankelijke lijstregels voor het produceren van de lijsten van Amazon voor uw  [!DNL Commerce]  producten.
role: Admin
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Een regel voor Amazon-aanbiedingen maken

Lijstregels kunnen tijdens het instappen worden gedefinieerd, maar kunnen ook op elk moment worden gewijzigd. Na aan boord gaan, kunt u tot de [ lijstregels ](./listing-rules.md) op het opslag [ dashboard ](./amazon-store-dashboard.md) toegang hebben.

## Een regel voor aanbiedingen maken tijdens het instappen

1. Nadat de winkel is verbonden, klikt u op **[!UICONTROL View Store]** voor de toegevoegde winkel.

   Het opslag [ dashboard ](./amazon-store-dashboard.md) verschijnt met het `No products listed to Amazon` bericht.

1. Klik op **[!UICONTROL Preview and List Eligible Products]**.

   De pagina _[!UICONTROL Listing Rules]_wordt weergegeven.

1. Bepaal de voorwaarden die u wilt stellen om in aanmerking te komen voor producten die op Amazon moeten worden aangeboden en klik op **[!UICONTROL Preview changes]** of klik op **[!UICONTROL Preview changes]** om deze stap over te slaan.

   Zie [ Voorbeeld: Bepaal een Voorwaarde ](./ob-define-condition-example.md).

1. Je aanbiedingen bekijken in de voorvertoning van de aanbieding:

   ![ het Lijst voorproef ](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]** - Producten die op dit tabblad worden aangeboden, komen niet in aanmerking voor een Amazon-aanbieding op basis van de huidige regelinstellingen voor aanbiedingen.

     Niet-subsidiabele producten worden niet gepubliceerd naar Amazon. Als een product dat niet in aanmerking komt al op Amazon wordt aangeboden en je de Amazon-aanbieding afstemt op het catalogusproduct van [!DNL Commerce] , verandert de hoeveelheid voor de Amazon-aanbieding in `0` om verkoop van het product te voorkomen. Om een lijst uit Amazon manueel te verwijderen, zie [ Eind een Amazon van lijst ](./end-listings-manually.md). Producten die niet in aanmerking komen voor Amazon-vereisten worden hier niet vermeld. Die producten zijn vermeld op het [[!UICONTROL Inactive Listings] lusje ](./inactive-listings.md).

     Als u een `Ineligible` -aanbieding wilt wijzigen in een `Eligible` -aanbieding, herhaalt u dit proces en wijzigt u de aanbiedingsregels.

   - **[!UICONTROL Eligible Listings]** - Producten die op dit tabblad worden aangeboden, komen in aanmerking voor Amazon-aanbieding op basis van de huidige instelling van de aanbiedingsregel en komen in aanmerking voor Amazon-vereisten. Dit lusje omvat uw bestaande lijsten van Amazon die worden ingevoerd (als u **[!UICONTROL Import Third Party Listings]** aan `Import Listing` in uw [ het Vermelden Montages ](./listing-settings.md) hebt geplaatst).

   - **[!UICONTROL New Listings]** - De producten die op dit tabblad worden vermeld, bevatten uw [!DNL Commerce] -catalogusproducten die nieuw in aanmerking komen voor Amazon-aanbieding op basis van de huidige instelling van de aanbiedingsregel en maken Amazon-aanbiedingen.

1. Klik op **[!UICONTROL Save and Close]** als de bewerking is voltooid.

   Het opslag [ dashboard ](./amazon-store-dashboard.md) opent.

Nadat een winkel is ingeschakeld, wordt de informatiesync tussen [!DNL Commerce] en Amazon gestart. Je Amazon-aanbiedingen worden geïmporteerd in [!DNL Commerce] en proberen deze af te stemmen op producten in je [!DNL Commerce] -catalogus.

U kunt de Amazon-ordergegevens bekijken in het gedeelte _[!UICONTROL Recent Orders]_van het winkeldashboard. Zie [ Dashboard van de Opslag ](./amazon-store-dashboard.md) of [ Orden beheren ](./managing-orders.md).

>[!IMPORTANT]
>
>Er zijn enkele belangrijke winkelinstellingen (aanbiedingen, prijzen, regels, naleving, meer) met standaardwaarden voor een nieuwe winkel. Om ervoor te zorgen dat uw opslag opstelling voor uw specifieke behoeften is, herzie uw [ opslagmontages ](./default-store-settings.md).

![ Volgende pictogram ](assets/btn-next.png) [**ga aan de Montages van de Opslag Standaard**](./default-store-settings.md)
