---
title: Verkoopkanaal in Amazon - Prijsbereik
description: Met het prijsbereik van Commerce kunt u de prijzen op meerdere websites of wereldwijd beheren.
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Prijsbereik

[!DNL Commerce] verstrekt configuratie voor uw [ tariferend werkingsgebied ](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) dat aan `Global` of `Website` moet worden geplaatst. Als de prijs is ingesteld op `Global` , is er één prijsbron voor alle websites. Als de tarifering aan `Website` wordt geplaatst, kunnen uw websites hun tarifering over variëren en ook een fallback standaardwaarde van de prijsstelling hebben (zie [ het werkingsgebied van de Prijs ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html)).

Als u het prijsbereik van de catalogus wijzigt van `Global` in `Website` , veranderen alle kenmerken van het prijstype ook in `Website` . Zie [ Toevoegend Websites ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

Wanneer een websiteprijs wordt gekozen, zijn er twee prijsbronnen:

- De prijs van de website
- De standaardprijs (fall-back)

Voor de integratie van het het verkoopkanaal van Amazon, die op uw [ het vermelden regels ](./listing-rules.md) wordt gebaseerd, kunt u producten van veelvoudige websites in één enkel [!DNL Amazon Marketplace] Land in kaart brengen (tijdens [ wordt bepaald opslagintegratie ](./store-integration.md)). Deze koppeling introduceert echter de vraag welke prijs moet worden gepubliceerd als het product bestaat op meerdere websites met verschillende prijzen.
