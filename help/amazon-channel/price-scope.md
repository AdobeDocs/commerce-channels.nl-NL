---
title: Prijsbereik
description: Gebruik het prijsbereik van de Handel om prijzen volgens veelvoudige websites of globaal te beheren.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Prijsbereik

[!DNL Commerce] verstrekt configuratie voor uw  [het tarief werkingsgebied](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target= &quot;_blank&quot;} om aan  `Global` of  `Website`. worden geplaatst. Als de prijs wordt ingesteld op `Global`, is er één prijsbron voor alle websites. Als de prijsstelling is ingesteld op `Website`, kunnen uw websites hun prijzen variëren en hebben ze ook een standaardprijswaarde voor fallback. Zie [Catalogusprijs](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;} in de gebruikershandleiding voor de kernhandel.

Als u het prijsbereik van de catalogus wijzigt van `Global` in `Website`, veranderen alle kenmerken van het prijstype ook in `Website`. Zie [Websites toevoegen](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){:target=&quot;_blank&quot;}.

Wanneer een websiteprijs wordt gekozen, zijn er twee prijsbronnen:

- De prijs van de website
- De standaardprijs (fall-back)

Voor de integratie van Amazon-verkoopkanalen, op basis van uw [aanbiedingsregels](./listing-rules.md), kunt u producten van meerdere websites toewijzen aan één [!DNL Amazon Marketplace]-land (gedefinieerd tijdens [winkelintegratie](./store-integration.md)). Deze koppeling introduceert echter de vraag welke prijs moet worden gepubliceerd als het product bestaat op meerdere websites met verschillende prijzen.
