---
title: Workflows voor Amazon-vervulling
description: Voor een bestelling uit een Amazon-aanbieding wordt een specifieke volgorde aangehouden, van het verzenden van bestellingen tot verzending.
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Workflows voor Amazon-vervulling

## Voorbeeld: vervuld door handelaar

| Stap | Beschrijving |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Op Amazon wordt een order geplaatst die voldoet aan de eisen van de handel.** Amazon wijst de status van `Pending` totdat de creditcardgegevens van de klant zijn geverifieerd. Orders in `Pending` status wordt automatisch geïmporteerd in het verkoopkanaal van Amazon, maar wordt niet weergegeven op _[!UICONTROL Orders]_tab. |
| 2 | **De bestelling wordt geverifieerd door Amazon.** Na verificatie wijzigt Amazon de status in `Unshipped`. Met deze statuswijziging wordt de bestelling bijgewerkt in Amazon-verkoopkanaal en wordt deze weergegeven in het dialoogvenster _[!UICONTROL Orders]_tab. |
| 3 | **De ordergegevens worden bijgewerkt.** Amazon-verkoopkanaal werkt de bestelgegevens bij met de prijs, de e-mail van de klant en de naam van de klant. Tijdens deze update maakt de Amazon-order de bijbehorende [!DNL Commerce] volgorde op de pagina voor orderbeheer. De [!DNL Commerce] het ordernummer wordt weergegeven met de orderinformatie op de _[!UICONTROL Orders]_tab. |
| 4 | **Er wordt een nieuwe klantenaccount gemaakt.** Indien geconfigureerd in uw orderinstellingen en de klant niet bestaat in uw [!DNL Commerce] database, wordt een nieuwe klant gemaakt in uw [!DNL Commerce] database die de overeenkomstige klantgegevens uit de Amazon-bestelling gebruikt. Als u `No Customer Creation (guest)` in uw orderinstellingen volgt de volgorde [!DNL Commerce] gastproces en geen klant in uw gegevensbestand creëren. Op dit punt, als [!DNL Commerce] -systeem is geïntegreerd met een ERP/OMS/WMS, wordt de bestelling opgehaald bij de integratie van een nieuwe bestelling die binnen wordt geplaatst en gemaakt [!DNL Commerce]. |
| 5 | **De bestelling wordt verzonden.** Van de [!DNL Commerce] Als u een pagina voor de verwerking van bestellingen wilt bestellen, verzendt u de bestelling en voegt u een trackingnummer toe. Wanneer alle items zijn gemarkeerd in een `Shipped` status:<ul><li>De status van de [!DNL Commerce] orderwijzigingen in `Complete`.</li><li>De status van de Amazon-verkoopkanaalorder verandert in `Shipped`.</li><li>Het trackingnummer wordt gesynchroniseerd met Amazon en de status van de bestelling in Amazon verandert in `Shipped`.</li><li>Verzendberichten worden naar de klant verzonden via Amazon, niet vanuit [!DNL Commerce] (per beleid voor Amazon). |

## Voorbeeld: vervuld door Amazon (FBA)

| Stap | Beschrijving |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Op Amazon wordt een volgorde geplaatst die voldoet aan Amazon.** |
| 2 | **De volgorde wordt geïmporteerd.** De bestelling wordt pas geïmporteerd in het verkoopkanaal van Amazon als aan de bestelling de volgende voorwaarden zijn toegewezen: `Shipped` status door Amazon. Aangezien Amazon over de voorraad voor dit product beschikt, voorkomt dit interferentie met het beheer van de opslagplaats/voorraad. |
| 3 | **De ordergegevens worden bijgewerkt.** Indien geconfigureerd in uw [orderinstellingen](./order-settings.md), maakt de Amazon-order de bijbehorende [!DNL Commerce] bestellen en aanmaken als een bestelling met de status `Complete`. |
