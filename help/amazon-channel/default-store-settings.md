---
title: Standaardinstellingen opslaan
description: Wijzig de standaardinstellingen voor Handel om de Amazon-Sales Channel voor je winkel aan te passen.
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Standaardopslaginstellingen

Nadat je winkel is verbonden en je regel voor eerste aanbieding hebt ingesteld, kun je gegevens synchroniseren tussen Amazon en [!DNL Commerce] start. Er zijn verschillende soorten opslaginstellingen waarmee u uw winkel naar wens kunt aanpassen. De montages van de opslag worden betreden in de opslag [dashboard](./amazon-store-dashboard.md).

Opslaginstellingen zijn:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Bepaal hoe uw productcatalogus met de [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Bepalen hoe Amazon-orders worden beheerd.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Bepaal welke catalogusproducten in aanmerking komen om op Amazon te worden vermeld.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Bepaal hoe de Amazon-catalogusprijs wordt gewijzigd voor aanbiedingen die hiervoor in aanmerking komen.

- **[!UICONTROL Store reports]** - [Concurrentieprijsanalyse](./competitive-price-analysis.md) en [aanbiedingsverbeteringen](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Aanbiedingswijzigingen](./listing-changes-log.md) en [communicatiefouten](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Geef de instellingen voor de naam van e-mail- en Amazon-verkoopkanalen weer in de [!DNL Commerce] Admin.

## Enkele belangrijke standaardinstellingen

| Instelling | Standaard | Beschrijving | Locatie |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | Maakt overeenkomende [!DNL Commerce] orders bij ontvangst van nieuwe orders van Amazon, zodat orders in de [[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} workflow. Wanneer `Disabled`, Amazon bestelt importordergegevens ter controle, maar bestellingen moeten in uw [!DNL Amazon Seller Central] account. | [Orderinstellingen](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | Klantgegevens van Amazon-orders worden niet geïmporteerd in uw [!DNL Commerce] database. Geïmporteerde Amazon-bestellingen worden verwerkt als een uitcheckbewerking voor gasten. Als u uw [!DNL Commerce] de klantengegevensbestand, zou u dit het plaatsen moeten veranderen in `Build New Customer Account`. | [Orderinstellingen](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] catalogusproducten (die voldoen aan de Amazon-voorwaarden) om automatisch te publiceren naar Amazon en Amazon-aanbiedingen te maken. Als u uw producten handmatig wilt bekijken en publiceren, wijzigt u deze instelling in `Do Not Automatically List Eligible Products`. Producten die wachten op handmatige publicatie worden weergegeven op de [_Klaar voor lijst_](./ready-to-list.md) tab. | [Handelingen voor productaanbiedingen](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definieert het kenmerk Prijsbron dat wordt gebruikt als basis voor je Amazon-aanbiedingen. Als u de [!DNL Commerce] `Price` kenmerk als de basisprijs waarop uw prijsregels zijn gebaseerd, moet u deze instelling wijzigen in een ander kenmerk. | [Aanbiedingsprijs](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | De handelaar voldoet aan alle orders. Als u Fulfillment by Amazon gebruikt of een combinatie van uitvoeringsmethoden gebruikt, moet u deze instelling wijzigen. | [Betaald door](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Als al uw producten dezelfde voorwaarde zijn, kunt u een van de Amazon-voorwaardenopties selecteren om al uw producten te vertegenwoordigen. Als uw catalogus producten onder verschillende omstandigheden bevat (zoals Nieuw, Gebruikt en Gereviseerd), moet u deze instelling wijzigen in `Assign Condition Using Product Attribute` en uw [!DNL Commerce] voorwaardelementen aan je Amazon-aanbiedingsvoorwaarden. | [Aanbiedingsvoorwaarde product](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | none | Bepaal de regels die worden gebruikt om te bepalen welke producten Amazon verkoopkanaal aan Amazon publiceert. Deze regels bieden veel mogelijkheden om eenvoudige tot complexe regels te maken om producten als aanbiedingen op te nemen of uit te sluiten. | [Lijstregels](./listing-rules.md) |
| Prijsregels | none | Geef een ander kenmerk voor de Amazon-aanbiedingsprijs op dan de gedefinieerde _[!UICONTROL Magento Price Source]_in uw [Aanbiedingsprijs](./listing-price.md). Je aanbiedingsprijs (hoger of lager) afzetten tegen je_[!UICONTROL Magento Price Source]_ regels maken. | [Prijsregels](./pricing-products.md) |

Zie voor meer informatie [Opslaginstellingen](./ob-store-review.md).
