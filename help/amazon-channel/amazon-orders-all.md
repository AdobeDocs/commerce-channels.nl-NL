---
title: Amazon-bestellingen weergeven
description: Bekijk uw Amazon Marketplace-bestellingen in Adobe Commerce of Magento Open Source Admin.
feature: Sales Channels, Orders
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Amazon-bestellingen weergeven

U kunt uw Amazon-bestellingen op twee manieren weergeven: _[!UICONTROL Recent Orders]_en_[!UICONTROL All Orders]_ .

Beide opties tonen u basisordeinformatie, zoals ontvangen van Amazon, die omvat:

- Aankoopdatum
- Volgnummer
- Status
- Naam koper
- Eindtotaal
- Ordernotities

In de weergave _[!UICONTROL All Orders]_worden filteropties voor zoekopdrachten voor bestellingen toegevoegd.

>[!NOTE]
>
>Met uitzondering van de kolom _[!UICONTROL Order Notes]_wordt de tabel_[!UICONTROL Amazon orders]_ gevuld met ordergegevens die u van Amazon hebt ontvangen. De _kolom van de Nota&#39;s van de Orde_ wordt bijgewerkt door [!DNL Commerce] als ordeprocessen.

## Recente orders

U kunt uw meest recente orden in de _[!UICONTROL Recent Orders]_sectie van het [ opslagdashboard ](./amazon-store-dashboard.md) bekijken.

![ Recente Orden ](assets/amazon-recent-orders-imported.png){width="600" zoomable="yes"}

### Recente Amazon-bestellingen weergeven

1. Klik op **[!UICONTROL View Store]** op een winkelkaart.

1. Bekijk uw bestellingen in de sectie _[!UICONTROL Recent Orders]_.

1. Als u de volgordedetails wilt weergeven, klikt u op het Amazon-ordernummer in de kolom _[!UICONTROL Order Number]_.

   De pagina _[!UICONTROL Amazon Order Details]_voor de volgorde wordt geopend.

## Alle bestellingen weergeven

U kunt al uw Amazon-bestellingen weergeven op de pagina _[!UICONTROL Amazon orders]_(ook wel de_[!UICONTROL All Orders]_ -weergave genoemd). De Amazon-tabel voor bestellingen is vergelijkbaar met de sectie _[!UICONTROL Recent Orders]_van het opslagdashboard, maar u kunt al uw Amazon-bestellingen weergeven en uw lijst met bestellingen beperken met de volgende filteropties:

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![ Amazon orden ](assets/amazon-orders-list-all.png){width="600" zoomable="yes"}

### Alle Amazon-bestellingen weergeven

1. Klik op **[!UICONTROL View Store]** op een winkelkaart.

1. Klik op **[!UICONTROL All Orders]** in de sectie _[!UICONTROL Recent Orders]_.

1. Als u de lijst of zoekopdracht naar een specifiek volgnummer wilt beperken, voert u de parameters **[!UICONTROL Filter by]** in en klikt u op **[!UICONTROL Apply filters]** .

1. Als u de volgordedetails wilt weergeven, klikt u op het Amazon-ordernummer in de kolom _[!UICONTROL Order Number]_.

   De pagina _[!UICONTROL Amazon Order Details]_voor de volgorde wordt geopend.

## Filters gebruiken

U kunt filters op uw ordelijst in de _[!UICONTROL Filter by]_sectie toepassen. Maak uw selecties en klik op **[!UICONTROL Apply filters]**. De toegepaste filters verschijnen boven het orderraster.

![ Filters voor het bekijken van de orden van Amazon ](assets/amazon-orders-filter-view.png){width="600" zoomable="yes"}

### Toegepaste filters wijzigen

- In de sectie _[!UICONTROL Filter by]_kunt u filters toevoegen of wijzigen. Klik op **[!UICONTROL Apply filters]**om de volgordelijst en de filteropties die boven het raster voor bestellingen worden weergegeven bij te werken.

- U kunt filters één voor één verwijderen door op `x` voor het filter te klikken of allemaal tegelijk door op **[!UICONTROL Clear all filters]** te klikken. Als u een filter verwijdert, worden de volgordelijst en de filteropties bijgewerkt die boven het raster voor bestellingen worden weergegeven.

- Als uw ordelijst lang is, kunt u de pagineringscontroles onder het net gebruiken om meer orden te bekijken.

>[!TIP]
>
>Enkele tips voor de weergave Bestellingen:
>
>- Als u meerdere Amazon Store-integraties hebt, moet u de paginaweergave vernieuwen wanneer u overschakelt tussen de winkelweergaven om zowel de lijst met bestellingen als de pagineringsweergaven voor de huidige winkel bij te werken.
>- Bij het sorteren op kolom wordt de sortering alleen toegepast op de huidige lijstweergave. U kunt het beste uw lijst filteren en vervolgens de pagina die u bekijkt sorteren.
>- Afhankelijk van de breedte van het weergavevenster ziet u mogelijk overlappende tekst in de kolommen. Als u de kolommen voor de omloop van tekst wilt uitvouwen, verbreedt u de vensterweergave.
>- Filtreer bij filteren op _[!UICONTROL Total]_met hele getallen. Als u een decimaal getal invoert, kunnen er fouten in de resultaten optreden.

### Standaardkolommen

| Kolom | Beschrijving |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Filter by] | Alleen beschikbaar in de weergave _[!UICONTROL All Orders]_.<br> verklein de lijst van orden die op worden gebaseerd:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | De datum van de aankoop, zoals ontvangen van Amazon. |
| [!UICONTROL Order Number] | Het ordernummer dat is gegenereerd door en ontvangen van Amazon. Klik op de koppeling als u het scherm Amazon Order Details wilt weergeven. |
| [!UICONTROL Status] | De status van de bestelling, zoals ontvangen door Amazon. Opties: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | De naam van de persoon die de bestelling heeft geplaatst, zoals deze van Amazon is ontvangen. |
| [!UICONTROL Grand Total] | De totale valutawaarde van de bestelling, zoals ontvangen van Amazon. |
| [!UICONTROL Order Notes] | De meest recente handeling die is opgenomen voor de volgorde terwijl deze wordt verwerkt in [!DNL Commerce] . De informatie omvat, maar is niet beperkt tot, de fouten van de ordeinvoer en de updates van de ordeverwerking.<br>**Nota**: Dit gebied wordt bijgewerkt door [!DNL Commerce] als ordeprocessen. |
