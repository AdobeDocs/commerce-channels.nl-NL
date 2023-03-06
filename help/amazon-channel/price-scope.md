---
title: Prijsbereik
description: Gebruik het prijsbereik van de Handel om prijzen volgens veelvoudige websites of globaal te beheren.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Prijsbereik

[!DNL Commerce] verstrekt configuratie voor uw [prijsbereik](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} to be set to `Global` or `Website`. If pricing is set to `Global`, there is a single price source for all websites. If pricing is set to `Website`, your websites can vary their pricing across and also have a fallback default pricing value. See [Catalog Price](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} in de kerngids voor de gebruiker van de Handel.

Als u het prijsbereik van de catalogus wijzigt van `Global` tot `Website`, veranderen ook alle kenmerken van het prijstype in `Website`. Zie [Websites toevoegen](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target="_blank"}.

Wanneer een websiteprijs wordt gekozen, zijn er twee prijsbronnen:

- De prijs van de website
- De standaardprijs (fall-back)

Voor de integratie met Amazon-verkoopkanalen, gebaseerd op uw [aanbiedingsregels](./listing-rules.md)kunt u producten van meerdere websites toewijzen aan één website [!DNL Amazon Marketplace] Land (gedefinieerd tijdens [winkelintegratie](./store-integration.md)). Deze koppeling introduceert echter de vraag welke prijs moet worden gepubliceerd als het product bestaat op meerdere websites met verschillende prijzen.
