---
title: '[!DNL Walmart] Vereisten'
description: "Verifieer dat u de vereiste  [!DNL Walmart Marketplace] informatie en middelen hebt om met de Manager van het Kanaal te integreren."
role: Leader, Admin, Developer
feature: Sales Channels, Install, User Account, Tools and External Services
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# [!DNL Walmart] Vereisten

[!DNL Channel Manager] vereist de volgende bronnen en informatie om een [!DNL Commerce] verkoopkanaal voor [!DNL Walmart Marketplace.] te configureren

* Een [!DNL Walmart] verkopersaccount

* Een API-sleutel om Adobe Commerce of Magento Open Source met te verbinden [!DNL Walmart Marketplace]

  Met de API-sleutel [!DNL Walmart Marketplace] kunt u [!DNL Channel Manager] for Adobe [!DNL Commerce] of Magento Open Source integreren met de Marketplace van Walmart. Stel de API-sleutel in Seller Central in voordat u Kanaalbeheer aan boord gaat.

## Een [!DNL Walmart Seller] -account instellen

Ga naar [!DNL Walmart Seller Center] aan opstelling uw [ rekening van de Verkoper van de Markeren ](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## Een [!DNL Walmart Marketplace] productie-API-sleutel genereren

1. Ga naar [!DNL Walmart Marketplace] om de productie API van de a [ oplossingsleverancier voor Adobe ](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey) te produceren.

1. Maak de sleutel en configureer machtigingen:

   * Selecteer Adobe als oplossingsleverancier.

   * Stel de machtigingen in zoals weergegeven in de volgende tabel. Voor details, zie [ API Geloofsbrieven ](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) in de _Hulp van de Verkoper van de Markt van de Markt van de Markt van de Markt_.

   **Adobe API zeer belangrijke configuratie voor Walmart**

   | **Toestemming** | **Plaatsende** |
   |----------------|-------------|
   | Inhoud | Volledige toegang |
   | Feeds ophalen | Alleen weergeven |
   | Inventaris | Volledige toegang |
   | Items | Volledige toegang |
   | Laagtijd | Volledige toegang |
   | Volgorde | Volledige toegang |
   | Prijs | Volledige toegang |
   | Rapporten | Alleen weergeven |
   | Retourneert | Volledige toegang |
   | Regels | Volledige toegang |
   | Verzending | Volledige toegang |

## [!DNL Walmart Marketplace] Winkelstatus

Wanneer u producten op de markt aansluit, hangt de beschikbaarheid van aanbiedingen af van de status van uw [!DNL Walmart Marketplace] -winkels:

* Voor live winkels worden je productaanbiedingen aangeboden en te koop aangeboden wanneer de match voltooid is.

* Voor winkels die niet live zijn, worden uw productaanbiedingen gefaseerd en niet zichtbaar voor klanten. Wanneer de winkel van [!DNL Walmart Marketplace] live gaat, worden gefaseerde aanbiedingen automatisch naar de live winkel gestuurd.

![[!DNL Walmart Seller Central] Gelaagde producten ](assets/walmart-seller-central-staged.png){width="600" zoomable="yes"}

>[!IMPORTANT]
>
>Nadat [!DNL Channel Manager] is geïnstalleerd en geconfigureerd, worden alle voorraad-, prijs- en orderupdates automatisch gesynchroniseerd. Verbind [!DNL Channel Manager] niet met een live Marketplace winkel tot u andere integraties hebt uitgeschakeld die het product bijwerken en gegevens bestellen. Als u andere integraties hebt geconfigureerd, controleert u of het aantal items en de prijzen in [!DNL Commerce] overeenkomen met de hoeveelheden in [!DNL Walmart Marketplace] voordat u verbinding maakt met een live winkel.

