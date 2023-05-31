---
title: Amazon-bestellingen weergeven
description: Bekijk uw Amazon Marketplace-bestellingen in Adobe Commerce of Magento Open Source Admin.
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Amazon-bestellingen weergeven

Er zijn twee manieren om uw Amazon-bestellingen weer te geven: _[!UICONTROL Recent Orders]_en_[!UICONTROL All Orders]_.

Beide opties tonen u basisordeinformatie, zoals ontvangen van Amazon, die omvat:

- Aankoopdatum
- Volgnummer
- Status
- Naam koper
- Eindtotaal
- Ordernotities

_[!UICONTROL All Orders]_de mening voegt het filtreren opties voor ordeonderzoeken toe.

>[!NOTE]
>
>Met uitzondering van de _[!UICONTROL Order Notes]_de_[!UICONTROL Amazon orders]_ tabel is gevuld met ordergegevens die zijn ontvangen van Amazon. De _Ordernotities_ kolom wordt bijgewerkt door [!DNL Commerce] als de ordeprocessen.

## Recente orders

U kunt uw meest recente bestellingen weergeven in het dialoogvenster _[!UICONTROL Recent Orders]_van de [opslagdashboard](./amazon-store-dashboard.md).

![Recente bestellingen](assets/amazon-recent-orders-imported.png){width="600" zoomable="yes"}

### Recente Amazon-bestellingen weergeven

1. Klikken **[!UICONTROL View Store]** op een winkelkaart.

1. Je bestellingen bekijken in het dialoogvenster _[!UICONTROL Recent Orders]_sectie.

1. Klik op het Amazon-ordernummer in het dialoogvenster _[!UICONTROL Order Number]_kolom.

   De _[!UICONTROL Amazon Order Details]_pagina voor de bestelling wordt geopend.

## Alle bestellingen weergeven

U kunt al uw Amazon-bestellingen weergeven op de _[!UICONTROL Amazon orders]_pagina (ook wel de_[!UICONTROL All Orders]_ weergave). De tabel Amazon Orders is vergelijkbaar met de tabel _[!UICONTROL Recent Orders]_in het winkeldashboard, maar hiermee kunt u al uw Amazon-bestellingen weergeven en uw lijst met bestellingen beperken met de volgende filteropties:

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon-orders](assets/amazon-orders-list-all.png){width="600" zoomable="yes"}

### Alle Amazon-bestellingen weergeven

1. Klikken **[!UICONTROL View Store]** op een winkelkaart.

1. Klikken **[!UICONTROL All Orders]** in de _[!UICONTROL Recent Orders]_sectie.

1. Als u de lijst of de zoekopdracht naar een specifiek ordernummer wilt beperken, voert u de opdracht **[!UICONTROL Filter by]** parameters en klik op **[!UICONTROL Apply filters]**.

1. Klik op het Amazon-ordernummer in het dialoogvenster _[!UICONTROL Order Number]_kolom.

   De _[!UICONTROL Amazon Order Details]_pagina voor de bestelling wordt geopend.

## Filters gebruiken

U kunt filters toepassen op uw orderlijst in het dialoogvenster _[!UICONTROL Filter by]_sectie. Maak uw selecties en klik op **[!UICONTROL Apply filters]**. De toegepaste filters verschijnen boven het orderraster.

![Filters voor het weergeven van Amazon-orders](assets/amazon-orders-filter-view.png){width="600" zoomable="yes"}

### Toegepaste filters wijzigen

- U kunt filters toevoegen aan of wijzigen in het dialoogvenster _[!UICONTROL Filter by]_sectie. Klikken **[!UICONTROL Apply filters]**om de ordelijst en de filteropties bij te werken die boven het orderraster worden weergegeven.

- U kunt filters één voor één verwijderen door op de knop `x` voor het filter of alles tegelijk door op **[!UICONTROL Clear all filters]**. Als u een filter verwijdert, worden de volgordelijst en de filteropties bijgewerkt die boven het raster voor bestellingen worden weergegeven.

- Als uw ordelijst lang is, kunt u de pagineringscontroles onder het net gebruiken om meer orden te bekijken.

>[!TIP]
>
>Enkele tips voor de weergave Bestellingen:
>
>- Als u meerdere Amazon Store-integraties hebt, moet u de paginaweergave vernieuwen wanneer u overschakelt tussen de winkelweergaven om zowel de lijst met bestellingen als de pagineringsweergaven voor de huidige winkel bij te werken.
>- Bij het sorteren op kolom wordt de sortering alleen toegepast op de huidige lijstweergave. U kunt het beste uw lijst filteren en vervolgens de pagina die u bekijkt sorteren.
>- Afhankelijk van de breedte van het weergavevenster ziet u mogelijk overlappende tekst in de kolommen. Als u de kolommen voor de omloop van tekst wilt uitvouwen, verbreedt u de vensterweergave.
>- Wanneer filteren op _[!UICONTROL Total]_, filtreer met hele getallen. Als u een decimaal getal invoert, kunnen er fouten in de resultaten optreden.


### Standaardkolommen

| Kolom | Beschrijving |
|---|---|
| [!UICONTROL Filter by] | Alleen beschikbaar in het dialoogvenster _[!UICONTROL All Orders]_weergeven.<br>Versmal de lijst met bestellingen op basis van:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | De datum van de aankoop, zoals ontvangen van Amazon. |
| [!UICONTROL Order Number] | Het ordernummer dat is gegenereerd door en ontvangen van Amazon. Klik op de koppeling als u het scherm Amazon Order Details wilt weergeven. |
| [!UICONTROL Status] | De status van de bestelling, zoals ontvangen door Amazon. Opties: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | De naam van de persoon die de bestelling heeft geplaatst, zoals deze van Amazon is ontvangen. |
| [!UICONTROL Grand Total] | De totale valutawaarde van de bestelling, zoals ontvangen van Amazon. |
| [!UICONTROL Order Notes] | De meest recente handeling die is opgenomen voor de volgorde waarin deze wordt verwerkt in [!DNL Commerce]. De informatie omvat, maar is niet beperkt tot, de fouten van de ordeinvoer en de updates van de ordeverwerking.<br>**Opmerking**: Dit veld wordt bijgewerkt door [!DNL Commerce] als de ordeprocessen. |
