---
title: Update van voorraad en prijs
description: '''[!DNL Channel Manager] synchrone inventarisatie en prijsupdates tussen de Commerce Store en [!DNL Walmart Marketplace] zodat kunt u de bewerkingen van uw verkoopkanalen beheren vanuit de Admin van de Handel'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a1944052f02968c36495275cd5ddfb2ca43ce967
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Update van voorraad en prijs

[!DNL Channel Manager] volgt inventaris en tarifering voor producten in de kanaalopslag. Wanneer de voorraad of de prijs verandert, synchroniseert aan allebei [!DNL Channel Manager] en [!DNL Walmart Marketplace] om de huidige voorraadhoeveelheid en prijzen in productaanbiedingen weer te geven.

## Inventarisupdates

Wanneer de inventarisniveaus veranderen, synchroniseert de Manager van het Kanaal updates tussen de Handel en de Marketplace van de Markt van de Markt van de Markt om ervoor te zorgen dat de Manager van het Kanaal en de Markt van de Markt van de Markt van de Markt van de Markt de correcte voorraadhoeveelheid hebben.

Het kan tot 10 minuten duren voor inventarisupdates voor synchronisatie tussen Channel Manager en Marketplace.

* **Updates van de voorraadhoeveelheid in de productcatalogus**-Wanneer de voorraadhoeveelheid van de Handel verandert wegens [wijzigingen in de hoeveelheid handmatige voorraad](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), terugbetalingen of annuleringen, wordt de wijziging in verbonden kanalen gesynchroniseerd en [!DNL Walmart Marketplace].

* **De voorraad verminderen om de orders van de Marketplace van Walmart weer te geven**- Nadat de de ordesync van de Marketplace van het Spoor aan de Manager van het Kanaal, verzendt de Manager van het Kanaal de update naar het de ordesysteem van de Handel. De handel past de voorraadhoeveelheden op de orde aan. Vervolgens wordt de bijgewerkte hoeveelheid gesynchroniseerd met Walmart Marketplace. Totdat de synchronisatiebewerkingen zijn voltooid, kunnen er kwantitatieve verschillen optreden tussen Kanaalbeheer en Marketplace.

>[!IMPORTANT]
>
> Nadat een Walmart Marktorder aan de Manager van het Kanaal synchroniseert, worden de inventarishoeveelheden en de ordeinformatie bijgewerkt slechts voor terugbetalingen en annuleringen die van de Handel in werking worden gesteld. Als een bestelling wordt terugbetaald of geannuleerd van de Walmart Marketplace, verwerkt u de wijziging van de handel om de nauwkeurigheid van de inventarishoeveelheden en de ordergegevens van de handel te waarborgen.

## Prijsupdates

Wanneer de productprijs in de Handel verandert, synchroniseert de Manager van het Kanaal de update van [!DNL Commerce] productcatalogus naar [!DNL Walmart Marketplace]. Het kan tot vijf minuten duren voordat de markt de prijswijzigingen weergeeft.

### Prijzen voor een gepubliceerd product beheren

1. Van de [!UICONTROL Admin], selecteert u **[!UICONTROL Catalog > Products]**.
1. Zoek in het productraster het product dat u wilt bijwerken en selecteer **[!UICONTROL Edit]**.
1. Controleer en werk de prijs zo nodig bij.
1. **[!UICONTROL Save]** de wijziging.

Voor details over het beheren van de configuratie van de productprijs in de Handel, zie [Prijsbeheer](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
