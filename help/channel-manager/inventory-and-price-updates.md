---
title: Update van voorraad en prijs
description: '''[!DNL Channel Manager] synchrone inventarisatie en prijsupdates tussen de Commerce Store en [!DNL Walmart Marketplace] zodat kunt u de bewerkingen van uw verkoopkanalen beheren vanuit de Admin van de Handel'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 97128dcf45d7672e958c771f88389aba40c6e39e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Overzicht en prijzen bijwerken

[!DNL Channel Manager] inventarisatie en prijsstelling volgen voor producten in de [!DNL Commerce] productcatalogus en synchroniseert updates met het verbonden verkoopkanaal en [!DNL Walmart Marketplace]. De synchronisatiebewerking zorgt ervoor dat de huidige voorraadhoeveelheid en prijzen in de productaanbiedingen worden weergegeven.


>[!IMPORTANT]
>
>Na [!DNL Channel Manager] worden geïnstalleerd en geconfigureerd, worden alle voorraad-, prijs- en orderupdates automatisch gesynchroniseerd. Als u reeds op Walmart Marketplace of direct of door een andere integratie verkoopt, zorg ervoor om de vorige integratie onbruikbaar te maken en te verifiëren dat de voorraadniveaus en de prijzen van de voorraad in de Opslag van de Handel nauwkeurig zijn en de gegevens in aanpassen [!DNL Walmart Marketplace] voordat u verbinding maakt [!DNL Channel Manager] naar de live winkel.


## Inventarisupdates

Wanneer de niveaus van de productvoorraad veranderen in [!DNL Commerce], [!DNL Channel Manager] synchroniseert updates aan [!DNL Walmart Marketplace]. Het kan 10 minuten duren voordat inventarisupdates via het verkoopkanaal worden gesynchroniseerd met de [!DNL Walmart marketplace].

* **Updates van de voorraadhoeveelheid in de productcatalogus**—Wanneer [!DNL Commerce] wijziging van de voorraadhoeveelheid als gevolg van [wijzigingen in de hoeveelheid handmatige voorraad](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), terugbetalingen of annuleringen, [!DNL Channel Manager] synchroniseert de wijziging in verbonden kanalen en [!DNL Walmart Marketplace].

* **De voorraadhoeveelheid verlagen om deze weer te geven [!DNL Walmart Marketplace] orders**—Na een [!DNL Walmart Marketplace] synchronisaties bestellen naar [!DNL Channel Manager], [!DNL Channel Manager] verzendt de update naar de [!DNL Commerce] bestelsysteem. [!DNL Commerce] de voorraadhoeveelheden worden aangepast op basis van de bestelling. Vervolgens wordt het bijgewerkte aantal gesynchroniseerd met [!DNL Walmart Marketplace]. Totdat de synchronisatiebewerkingen zijn voltooid, ziet u mogelijk verschillende hoeveelheden in de verkoopkanaalaanbiedingen en [!DNL Walmart].

>[!IMPORTANT]
>
>Na een [!DNL Walmart Marketplace] synchronisaties bestellen naar [!DNL Channel Manager], inventarishoeveelheden en ordergegevens worden alleen bijgewerkt voor terugbetalingen en annuleringen die worden geïnitieerd op [!DNL Commerce]. Als een bestelling wordt terugbetaald of geannuleerd vanaf de [!DNL Walmart marketplace]de wijziging van [!DNL Commerce] de nauwkeurigheid van [!DNL Commerce] inventarishoeveelheden en ordergegevens.

## Prijsupdates

Wanneer de productprijs verandert in [!DNL Commerce], [!DNL Channel Manager] synchroniseert de update naar de [!DNL Walmart Marketplace]. Het kan maximaal vijf minuten duren voordat de prijswijziging in de [!DNL Walmart Marketplace] aanbieding.

### Prijzen voor een verbonden product beheren

1. Van de [!UICONTROL Admin], selecteert u **[!UICONTROL Catalog > Products]**.
1. Zoek in het productraster het product dat u wilt bijwerken en selecteer **[!UICONTROL Edit]**.
1. Controleer en werk de prijs zo nodig bij.
1. **[!UICONTROL Save]** de wijziging.

Voor hulp bij het beheren van de productprijsconfiguratie in [!DNL Commerce], zie [Prijsbeheer](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
