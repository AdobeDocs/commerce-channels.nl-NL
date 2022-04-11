---
title: Walmart-vereisten
description: Verifieer dat u de vereiste Marketplace informatie en de middelen van de Markt van de Markt hebt om met de Manager van het Kanaal te integreren.
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: e6368d30e16ccffcb1dfc64bdd56561116934b54
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Walmart-voorwaarden

De Manager van het kanaal vereist de volgende middelen en de informatie om een de verkoopkanaal van de Handel voor de Marketplace van de Markt van de Markt te vormen.

* Goedkeuring om te verkopen op Walmart en aanmeldingsgegevens voor de geregistreerde verkopersaccount

* Een API-sleutel om Adobe Commerce of Magento Open Source te verbinden met Walmart Marketplace

   De Walmart Marketplace API sleutel laat de integratie tussen de Manager van het Kanaal voor Adobe Commerce of Magento Open Source en de Marketplace van de Markeren toe. Stel de API-sleutel in Seller Central in voordat u Kanaalbeheer aan boord gaat.

## Een verkopersaccount instellen

1. [De toepassing Walmart-verkoper verzenden](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
1. Na goedkeuring door Walmart, [je Walmart Seller-account instellen](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

## Een Walmart Marketplace Production API-sleutel genereren

1. Ga naar Walmart Marketplace om een [productie-API-sleutel voor oplossingsprovider voor Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

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

## Status van Walmart Marketplace Store

Wanneer u producten aan Marketplace publiceert, hangt de beschikbaarheid van lijsten van de status van uw winkels van de Marketplace van de Markt van de Markt van de Markt van de Markt af:

* Voor live winkels worden je productaanbiedingen aangeboden en te koop aangeboden wanneer de match voltooid is.

* Voor winkels die niet live zijn, worden uw productaanbiedingen gefaseerd en niet zichtbaar voor klanten. Wanneer de winkel live gaat, worden gefaseerde aanbiedingen automatisch naar de live winkel gestuurd.

![[!DNL Walmart Seller Central] gefaseerde producten](assets/walmart-seller-central-staged.png)
