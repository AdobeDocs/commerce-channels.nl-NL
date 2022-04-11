---
title: Update van voorraad en prijs
description: '''[!DNL Channel Manager] synchrone inventarisatie en prijsupdates tussen de Commerce Store en [!DNL Walmart Marketplace] zodat kunt u de bewerkingen van uw verkoopkanalen beheren vanuit de Admin van de Handel'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 30495c4e47f15c821206f7b0252b868b4e27d62d
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Inventarisatie en prijsupdates

[!DNL Channel Manager] inventarisatie en prijsstelling volgen voor producten in de [!DNL Commerce] productcatalogus en syncs updates van het verbonden verkoopkanaal en [!DNL Walmart Marketplace]. De synchronisatie zorgt ervoor dat de aanbiedingen van producten de huidige hoeveelheid en prijs van de voorraad weerspiegelen.

## Inventarisupdates

Wanneer de niveaus van de productvoorraad veranderen in [!DNL Commerce], [!DNL Channel Manager] synchroniseert updates van het verkoopkanaal en aan [!DNL Walmart Marketplace]. Het kan 10 minuten duren voordat inventarisupdates via het verkoopkanaal worden gesynchroniseerd met de [!DNL Walmart marketplace].

* **Updates van de voorraadhoeveelheid in de productcatalogus**-When [!DNL Commerce] wijziging van de voorraadhoeveelheid als gevolg van [wijzigingen in de hoeveelheid handmatige voorraad](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), terugbetalingen of annuleringen, [!DNL Channel Manager] synchroniseert de wijziging in verbonden kanalen en [!DNL Walmart Marketplace].

* **De voorraadhoeveelheid verlagen om deze weer te geven [!DNL Walmart Marketplace] orders**-Na een [!DNL Walmart Marketplace] synchronisaties bestellen naar [!DNL Channel Manager], [!DNL Channel Manager] verzendt de update naar de [!DNL Commerce] bestelsysteem. [!DNL Commerce] de voorraadhoeveelheden worden aangepast op basis van de bestelling. Vervolgens wordt het bijgewerkte aantal gesynchroniseerd met [!DNL Walmart Marketplace]. Totdat de synchronisatiebewerkingen zijn voltooid, ziet u mogelijk verschillende hoeveelheden in de verkoopkanaalaanbiedingen en [!DNL Walmart].

>[!IMPORTANT]
>
> Na een [!DNL Walmart Marketplace] synchronisaties bestellen naar [!DNL Channel Manager], inventarishoeveelheden en ordergegevens worden alleen bijgewerkt voor terugbetalingen en annuleringen die worden geïnitieerd op [!DNL Commerce]. Als een bestelling wordt terugbetaald of geannuleerd vanaf de [!DNL Walmart marketplace]de wijziging van [!DNL Commerce] de nauwkeurigheid van [!DNL Commerce] inventarishoeveelheden en ordergegevens.

## Prijsupdates

Wanneer de productprijs verandert in [!DNL Commerce], [!DNL Channel Manager] synchroniseert de update naar de [!DNL Walmart Marketplace]. Het kan maximaal vijf minuten duren voordat de prijswijziging in de [!DNL Walmart Marketplace] aanbieding.

### Prijzen voor een gepubliceerd product beheren

1. Van de [!UICONTROL Admin], selecteert u **[!UICONTROL Catalog > Products]**.
1. Zoek in het productraster het product dat u wilt bijwerken en selecteer **[!UICONTROL Edit]**.
1. Controleer en werk de prijs zo nodig bij.
1. **[!UICONTROL Save]** de wijziging.

Voor hulp bij het beheren van de productprijsconfiguratie in [!DNL Commerce], zie [Prijsbeheer](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
