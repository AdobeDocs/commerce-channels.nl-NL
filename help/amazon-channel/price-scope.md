---
title: Prijsbereik
description: Gebruik het prijsbereik van de Handel om prijzen volgens veelvoudige websites of globaal te beheren.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Prijsbereik

[!DNL Commerce] verstrekt configuratie voor uw [prijsbereik](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target=&quot;_blank&quot;} in te stellen op `Global` of `Website`. Als de prijsstelling is ingesteld op `Global`Er is echter één prijsbron voor alle websites. Als de prijsstelling is ingesteld op `Website`Uw websites kunnen hun prijzen variëren en hebben ook een terugvalstandaardwaarde voor de standaardprijzen. Zie [Catalogusprijs](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target=&quot;_blank&quot;} in de core Commerce-gebruikershandleiding.

Als u het prijsbereik van de catalogus wijzigt van `Global` tot `Website`, veranderen ook alle kenmerken van het prijstype in `Website`. Zie [Websites toevoegen](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target=&quot;_blank&quot;}.

Wanneer een websiteprijs wordt gekozen, zijn er twee prijsbronnen:

- De prijs van de website
- De standaardprijs (fall-back)

Voor de integratie met Amazon-verkoopkanalen, gebaseerd op uw [aanbiedingsregels](./listing-rules.md)kunt u producten van meerdere websites toewijzen aan één website [!DNL Amazon Marketplace] Land (gedefinieerd tijdens [winkelintegratie](./store-integration.md)). Deze koppeling introduceert echter de vraag welke prijs moet worden gepubliceerd als het product bestaat op meerdere websites met verschillende prijzen.
