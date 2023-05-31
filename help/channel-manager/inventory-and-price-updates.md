---
title: Update van voorraad en prijs
description: '[!DNL Channel Manager] syntheseinventarisatie en prijsupdates tussen de [!DNL Commerce] opslaan en [!DNL Walmart Marketplace] zodat u de verkoopkanaalbewerkingen kunt beheren via het [!DNL Commerce] Admin'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Inventaris en prijzen bijwerken

[!DNL Channel Manager] inventarisatie en prijsstelling volgen voor producten in de [!DNL Commerce] productcatalogus en synchroniseert updates met het verbonden verkoopkanaal en [!DNL Walmart Marketplace]. De synchronisatiebewerking zorgt ervoor dat de huidige voorraadhoeveelheid en prijzen in de productaanbiedingen worden weergegeven.


>[!IMPORTANT]
>
>Na [!DNL Channel Manager] worden geïnstalleerd en geconfigureerd, worden alle voorraad-, prijs- en orderupdates automatisch gesynchroniseerd. Als u al op Marketplace verkoopt, zorg ervoor om het even welke andere integraties onbruikbaar te maken die het product en de ordegegevens bijwerken. Controleer vervolgens of de voorraadvoorraadniveaus en -prijzen in de [!DNL Commerce] opslag is nauwkeurig en komt overeen met de gegevens in [!DNL Walmart Marketplace] voordat u verbinding maakt [!DNL Channel Manager] naar de live winkel.


## Inventarisupdates

Wanneer de niveaus van de productvoorraad veranderen in [!DNL Commerce], [!DNL Channel Manager] synchroniseert updates aan [!DNL Walmart Marketplace]. Het kan 10 minuten duren voordat inventarisupdates via het verkoopkanaal worden gesynchroniseerd met de [!DNL Walmart marketplace].

* **Updates van de voorraadhoeveelheid in de productcatalogus**—Wanneer [!DNL Commerce] wijziging van de voorraadhoeveelheid als gevolg van [wijzigingen in de hoeveelheid handmatige voorraad](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html), terugbetalingen of annuleringen, [!DNL Channel Manager] synchroniseert de wijziging in verbonden kanalen en [!DNL Walmart Marketplace].

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

Voor hulp bij het beheren van de productprijsconfiguratie in [!DNL Commerce], zie [Prijsbeheer](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
