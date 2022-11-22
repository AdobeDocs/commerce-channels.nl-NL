---
title: '''[!DNL Walmart] Vereisten'
description: '"Controleer of u de vereiste [!DNL Walmart Marketplace]informatie en bronnen die met Channel Manager moeten worden geïntegreerd.'''
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 618bbd6d6c889d555f0ff74ade3dd84b412e1e59
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# [!DNL Walmart] vereisten

[!DNL Channel Manager] vereist de volgende middelen en de informatie om een [!DNL Commerce] verkoopkanaal voor [!DNL Walmart Marketplace.]

* A [!DNL Walmart] Verkopersaccount

* Een API-sleutel om Adobe Commerce of Magento Open Source om te verbinden met [!DNL Walmart Marketplace]

   De [!DNL Walmart Marketplace] API-sleutel maakt de integratie mogelijk tussen [!DNL Channel Manager] voor Adobe [!DNL Commerce] of Magento Open Source en de Walmart Marketplace. Stel de API-sleutel in Seller Central in voordat u Kanaalbeheer aan boord gaat.

## Een [!DNL Walmart Seller] account

Ga naar de [!DNL Walmart Seller Center] om uw [Walmart-verkopersaccount](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## Een [!DNL Walmart Marketplace] API-sleutel voor productie

1. Ga naar [!DNL Walmart Marketplace] om een [productie-API-sleutel voor oplossingsprovider voor Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Maak de sleutel en configureer machtigingen:

   * Selecteer Adobe als oplossingsleverancier.

   * Stel de machtigingen in zoals weergegeven in de volgende tabel. Zie voor meer informatie [API-referenties](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) in de _Help bij Marketplace Walmart_.

   **Adobe API sleutelconfiguratie voor Walmart**

   | **Machtiging** | **Instelling** |
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

Wanneer je producten verbindt met de markt, hangt de beschikbaarheid van aanbiedingen af van de status van je [!DNL Walmart Marketplace] winkels:

* Voor live winkels worden je productaanbiedingen aangeboden en te koop aangeboden wanneer de match voltooid is.

* Voor winkels die niet live zijn, worden uw productaanbiedingen gefaseerd en niet zichtbaar voor klanten. Wanneer de [!DNL Walmart Marketplace] Winkel gaat live, gefaseerde aanbiedingen worden automatisch naar de live winkel gestuurd.

![[!DNL Walmart Seller Central] gefaseerde producten](assets/walmart-seller-central-staged.png)

>[!IMPORTANT]
>
>Na [!DNL Channel Manager] worden geïnstalleerd en geconfigureerd, worden alle voorraad-, prijs- en orderupdates automatisch gesynchroniseerd. Geen verbinding maken [!DNL Channel Manager] naar een live Marketplace-winkel van Walmart tot u andere integraties hebt uitgeschakeld die het product bijwerken en gegevens bestellen. Als u andere geïntegreerde oplossingen hebt geconfigureerd, controleert u of het aantal items en de prijzen in [!DNL Commerce] overeenkomen met de hoeveelheden in [!DNL Walmart Marketplace] voordat u verbinding maakt met een live winkel.

