---
title: '"[!DNL Walmart] Vereisten"'
description: '"Controleer of u de vereiste[!DNL Walmart Marketplace]informatie en bronnen die met Channel Manager moeten worden geïntegreerd."'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: fffbdac54443b7b9bed8854eba8341446e78cc80
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# [!DNL Walmart] vereisten

[!DNL Channel Manager] vereist de volgende middelen en de informatie om een [!DNL Commerce] verkoopkanaal voor [!DNL Walmart Marketplace.]

* Goedkeuring om op te verkopen [!DNL Walmart] en aanmeldingsgegevens voor aanmelding bij de geregistreerde verkopersaccount

* Een API-sleutel om Adobe Commerce of Magento Open Source om te verbinden met [!DNL Walmart Marketplace]

   De [!DNL Walmart Marketplace] API-sleutel maakt de integratie mogelijk tussen [!DNL Channel Manager] voor Adobe Commerce of Magento Open Source en de Walmart Marketplace. Stel de API-sleutel in Seller Central in voordat u Kanaalbeheer aan boord gaat.

## Een verkopersaccount instellen

1. [De toepassing Walmart-verkoper verzenden](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
1. Na goedkeuring van [!DNL Walmart], [je Walmart Seller-account instellen](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

## Een [!DNL Walmart Marketplace] API-sleutel voor productie

1. Ga naar [!DNL Walmart Marketplace]om een [productie-API-sleutel voor oplossingsprovider voor Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

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

Wanneer je producten op de markt publiceert, hangt de beschikbaarheid van aanbiedingen af van de status van je [!DNL Walmart Marketplace] winkels:

* Voor live winkels worden je productaanbiedingen aangeboden en te koop aangeboden wanneer de match voltooid is.

* Voor winkels die niet live zijn, worden uw productaanbiedingen gefaseerd en niet zichtbaar voor klanten. Wanneer de [!DNL Walmart Marketplace] Winkel gaat live, gefaseerde aanbiedingen worden automatisch naar de live winkel gestuurd.

![[!DNL Walmart Seller Central] gefaseerde producten](assets/walmart-seller-central-staged.png)