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
| 1 | **A handels-Voldoet orde wordt geplaatst op Amazon.** Amazon kent de status `Pending` toe totdat de creditcardgegevens van de klant zijn geverifieerd. Orders met de status `Pending` worden automatisch geïmporteerd in het Amazon-verkoopkanaal, maar worden niet weergegeven op het tabblad _[!UICONTROL Orders]_. |
| 2 | **de orde wordt geverifieerd door Amazon.** Na verificatie wijzigt Amazon de status in `Unshipped` . Met deze statuswijziging wordt de volgorde bijgewerkt in het verkoopkanaal van Amazon en weergegeven op het tabblad _[!UICONTROL Orders]_. |
| 3 | **de orddetails worden bijgewerkt.** Amazon-verkoopkanaal werkt de bestelgegevens bij met de prijs, de e-mail van de klant en de naam van de klant. Tijdens deze update maakt de Amazon-order de corresponderende [!DNL Commerce] -volgorde op de pagina voor orderbeheer. Het ordernummer [!DNL Commerce] wordt weergegeven met de ordergegevens op het tabblad _[!UICONTROL Orders]_. |
| 4 | **een nieuwe klantenrekening wordt gecreeerd.** Als dit is geconfigureerd in de instellingen voor uw bestelling en de klant niet bestaat in uw [!DNL Commerce] -database, wordt een nieuwe klant gemaakt in uw [!DNL Commerce] -database met de bijbehorende klantgegevens uit de Amazon-bestelling. Als u `No Customer Creation (guest)` kiest in de instellingen voor uw bestelling, volgt de volgorde het gastproces van [!DNL Commerce] en wordt er geen klant in uw database gemaakt. Als uw [!DNL Commerce] -systeem op dit moment is geïntegreerd met een ERP/OMS/WMS, wordt de volgorde opgehaald door de integratie van een nieuwe volgorde die binnen [!DNL Commerce] wordt geplaatst en gemaakt. |
| 5 | **de orde wordt verscheept.** Vanaf de [!DNL Commerce] pagina voor orderverwerking verzendt u de bestelling en voegt u een trackingnummer toe. Wanneer alle items zijn gemarkeerd in de status `Shipped` :<ul><li>De status van de [!DNL Commerce] -volgorde verandert in `Complete` .</li><li>De status van de Amazon-verkoopkanaalvolgorde verandert in `Shipped` .</li><li>Het trackingnummer wordt gesynchroniseerd met Amazon en de status van de bestelling in Amazon verandert in `Shipped` .</li><li>Verzendberichten worden via Amazon naar de klant verzonden, niet vanuit [!DNL Commerce] (volgens het Amazon-beleid). |

## Voorbeeld: vervuld door Amazon (FBA)

| Stap | Beschrijving |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **een Amazon-Voldoet orde wordt geplaatst op Amazon.** |
| 2 | **de orde wordt ingevoerd.** De bestelling wordt pas geïmporteerd in het verkoopkanaal van Amazon nadat aan de bestelling de status `Shipped` is toegewezen door Amazon. Aangezien Amazon over de voorraad voor dit product beschikt, voorkomt dit interferentie met het beheer van de opslagplaats/voorraad. |
| 3 | **de orddetails worden bijgewerkt.** Als gevormd in uw [ ordemontages ](./order-settings.md), leidt de orde van Amazon tot de overeenkomstige [!DNL Commerce] orde en als orde met een status van `Complete` wordt gecreeerd. |
