---
title: Workflows voor Amazon-tegoeden
description: Voor een bestelling uit een Amazon-aanbieding wordt een specifieke volgorde aangehouden, van het verzenden van bestellingen tot verzending.
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Workflows voor Amazon-vervulling

## Voorbeeld: voldaan door handelaar

| Stap | Beschrijving |
|----|----|
| 1 | **Op Amazon wordt een order geplaatst die voldoet aan de eisen van de handel.** Amazon kent een status van toe  `Pending` totdat de creditcardgegevens van de klant zijn geverifieerd. Orders in de status `Pending` worden automatisch geïmporteerd in Amazon-verkoopkanaal, maar worden niet weergegeven op het tabblad _[!UICONTROL Orders]_. |
| 2 | **De bestelling wordt geverifieerd door Amazon.** Na verificatie wijzigt Amazon de status in  `Unshipped`. Met deze statuswijziging wordt de volgorde bijgewerkt in Amazon-verkoopkanaal en weergegeven op het tabblad _[!UICONTROL Orders]_. |
| 1 | **De ordergegevens worden bijgewerkt.** Amazon-verkoopkanaal werkt de bestelgegevens bij met de prijs, de e-mail van de klant en de naam van de klant. Tijdens deze update maakt de Amazon-order de corresponderende [!DNL Commerce]-volgorde op de pagina voor orderbeheer. Het ordernummer [!DNL Commerce] wordt weergegeven met de orderinformatie op het tabblad _[!UICONTROL Orders]_. |
| 4 | **Er wordt een nieuwe klantenaccount gemaakt.** Indien geconfigureerd in uw orderinstellingen en de klant niet bestaat in uw  [!DNL Commerce] database, wordt een nieuwe klant gemaakt in uw  [!DNL Commerce] database met de bijbehorende klantgegevens uit de Amazon-order. Als u `No Customer Creation (guest)` in uw ordemontages kiest, volgt de orde het [!DNL Commerce] gastproces en creeert geen klant in uw gegevensbestand. Als uw [!DNL Commerce]-systeem op dit moment is geïntegreerd met een ERP/OMS/WMS, wordt de volgorde opgehaald door de integratie van een nieuwe volgorde die binnen [!DNL Commerce] wordt geplaatst en gemaakt. |
| 5 | **De bestelling wordt verzonden.** Vanaf de pagina voor  [!DNL Commerce] orderverwerking verzendt u de bestelling en voegt u een trackingnummer toe. Wanneer alle items zijn gemarkeerd in de status `Shipped`:<ul><li>De status van de [!DNL Commerce] orde verandert in `Complete`.</li><li>De status van de Amazon-verkoopkanaalvolgorde verandert in `Shipped`.</li><li>Het trackingnummer wordt gesynchroniseerd met Amazon en de status van de bestelling in Amazon wordt gewijzigd in `Shipped`.</li><li>Verzendberichten worden naar de klant verzonden via Amazon, niet vanuit [!DNL Commerce] (volgens het beleid van Amazon). |

## Voorbeeld: vervuld door Amazon (FBA)

| Stap | Beschrijving |
|---|---|
| 3 | **Op Amazon wordt een volgorde geplaatst die voldoet aan Amazon.** |
| 2 | **De volgorde wordt geïmporteerd.** De bestelling wordt pas geïmporteerd in het verkoopkanaal van Amazon als aan de bestelling de  `Shipped` status door Amazon is toegewezen. Aangezien Amazon over de voorraad voor dit product beschikt, voorkomt dit interferentie met het beheer van de opslagplaats/voorraad. |
| 3 | **De ordergegevens worden bijgewerkt.** Indien geconfigureerd in uw  [orderinstellingen](./order-settings.md), maakt de Amazon-volgorde de corresponderende  [!DNL Commerce] volgorde en wordt deze gemaakt als een volgorde met de status  `Complete`. |
