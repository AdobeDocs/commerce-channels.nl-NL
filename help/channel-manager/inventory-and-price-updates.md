---
title: Update van voorraad en prijs
description: '"[!DNL Channel Manager] syncs inventariseren en prijsupdates tussen de  [!DNL Commerce]  opslag en  [!DNL Walmart Marketplace]  zodat u uw verrichtingen van het verkoopkanaal van  [!DNL Commerce]  Admin kunt beheren'
feature: Sales Channels, Merchandising, Inventory, Tools and External Services
role: Leader, Admin, User
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Inventaris en prijzen bijwerken

[!DNL Channel Manager] volgt de inventaris en de prijzen van producten in de [!DNL Commerce] productcatalogus en synchroniseert updates naar het verbonden verkoopkanaal en [!DNL Walmart Marketplace] . De synchronisatiebewerking zorgt ervoor dat de huidige voorraadhoeveelheid en prijzen in de productaanbiedingen worden weergegeven.


>[!IMPORTANT]
>
>Nadat [!DNL Channel Manager] is geïnstalleerd en geconfigureerd, worden alle voorraad-, prijs- en orderupdates automatisch gesynchroniseerd. Als u al op Marketplace verkoopt, zorg ervoor om het even welke andere integraties onbruikbaar te maken die het product en de ordegegevens bijwerken. Controleer vervolgens of de voorraadniveaus en -prijzen in de [!DNL Commerce] winkel nauwkeurig zijn en overeenkomen met de gegevens in [!DNL Walmart Marketplace] voordat u een verbinding tot stand brengt met de live winkel. [!DNL Channel Manager]


## Inventarisupdates

Wanneer de niveaus van de productinventaris in [!DNL Commerce] veranderen, [!DNL Channel Manager] synchroniseert updates aan [!DNL Walmart Marketplace]. Het kan 10 minuten duren voordat inventarisupdates via het verkoopkanaal worden gesynchroniseerd met de [!DNL Walmart marketplace] .

* **Updates aan voorraadhoeveelheid in productcatalogus** - wanneer [!DNL Commerce] voorraadhoeveelheid wegens [ de veranderingen van het handvoorraadaantal ](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html) verandert, terugbetaalt, of annuleert, [!DNL Channel Manager] synchroniseert de verandering in verbonden kanalen en [!DNL Walmart Marketplace].

* **Verminder voorraadhoeveelheid om [!DNL Walmart Marketplace] orden** te wijzen - na a [!DNL Walmart Marketplace] orde syncs aan [!DNL Channel Manager], [!DNL Channel Manager] verzendt de update naar het [!DNL Commerce] ordesysteem. [!DNL Commerce] past de voorraadhoeveelheden aan op basis van de orde. Vervolgens wordt het bijgewerkte aantal gesynchroniseerd met [!DNL Walmart Marketplace] . Totdat de synchronisatiebewerkingen zijn voltooid, ziet u mogelijk verschillende hoeveelheden in de verkoopkanaallijsten en [!DNL Walmart] .

>[!IMPORTANT]
>
>Nadat een [!DNL Walmart Marketplace] bestelling is gesynchroniseerd met [!DNL Channel Manager] , worden de inventarishoeveelheden en de ordergegevens alleen bijgewerkt voor terugbetalingen en annuleringen die worden gestart vanuit [!DNL Commerce] . Als een order wordt terugbetaald of geannuleerd uit [!DNL Walmart marketplace] , verwerkt u de wijziging van [!DNL Commerce] om de nauwkeurigheid van de inventarishoeveelheden en ordergegevens van [!DNL Commerce] te garanderen.

## Prijsupdates

Wanneer de prijs van het product verandert in [!DNL Commerce] , synchroniseert [!DNL Channel Manager] de update naar de [!DNL Walmart Marketplace] . Het kan maximaal vijf minuten duren voordat de prijswijziging in de [!DNL Walmart Marketplace] -aanbieding wordt weergegeven.

### Prijzen voor een verbonden product beheren

1. Selecteer in het menu [!UICONTROL Admin] de optie **[!UICONTROL Catalog > Products]** .
1. Zoek in het productraster het product dat u wilt bijwerken en selecteer **[!UICONTROL Edit]** .
1. Controleer en werk de prijs zo nodig bij.
1. **[!UICONTROL Save]** de wijziging.

Voor hulp met het beheren van de configuratie van de productprijs in [!DNL Commerce], zie [ Prijsbeheer ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
