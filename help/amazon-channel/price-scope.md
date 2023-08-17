---
title: Verkoopkanaal in Amazon - Prijsbereik
description: Gebruik het prijsbereik van de Handel om prijzen volgens veelvoudige websites of globaal te beheren.
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Prijsbereik

[!DNL Commerce] verstrekt configuratie voor uw [prijsbereik](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) in te stellen `Global` of `Website`. Als de prijsstelling is ingesteld op `Global`Er is echter één prijsbron voor alle websites. Als de prijsstelling is ingesteld op `Website`, kunnen uw websites hun prijzen variëren en hebben ook een terugvalstandaard prijswaarde (zie [Prijsbereik](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html)).

Als u het prijsbereik van de catalogus wijzigt van `Global` tot `Website`, veranderen ook alle kenmerken van het prijstype in `Website`. Zie [Websites toevoegen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

Wanneer een websiteprijs wordt gekozen, zijn er twee prijsbronnen:

- De prijs van de website
- De standaardprijs (fall-back)

Voor de integratie met Amazon-verkoopkanalen, gebaseerd op uw [aanbiedingsregels](./listing-rules.md)kunt u producten van meerdere websites toewijzen aan één website [!DNL Amazon Marketplace] Land (gedefinieerd tijdens [winkelintegratie](./store-integration.md)). Deze koppeling introduceert echter de vraag welke prijs moet worden gepubliceerd als het product bestaat op meerdere websites met verschillende prijzen.
