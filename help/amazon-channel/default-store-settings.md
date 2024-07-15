---
title: Standaardinstellingen voor winkel voor Amazon-aanbiedingen
description: Wijzig de standaard Commerce-instellingen om de Amazon-Sales Channel voor je winkel aan te passen.
role: Admin
feature: Sales Channels, Integration, Configuration
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Standaardinstellingen voor winkel voor Amazon-aanbiedingen

Nadat je winkel is verbonden en je regel voor eerste aanbieding hebt ingesteld, begint de synchronisatie van gegevens tussen Amazon en [!DNL Commerce] . Er zijn verschillende soorten opslaginstellingen waarmee u uw winkel naar wens kunt aanpassen. De montages van de opslag worden betreden op het opslag [ dashboard ](./amazon-store-dashboard.md).

Voorbeelden van opslaginstellingen:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Bepaal hoe uw productcatalogus met [!DNL Amazon Marketplace] interactie aangaat.

- [**[!UICONTROL Order settings]**](./order-settings.md) - Bepaal hoe Amazon-bestellingen worden beheerd.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Bepaal welke catalogusproducten in aanmerking komen om op Amazon te worden vermeld.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Bepaal hoe de Amazon-catalogusprijs wordt gewijzigd voor in aanmerking komende aanbiedingen.

- **[!UICONTROL Store reports]** - [ Concurrerende prijsanalyse ](./competitive-price-analysis.md) en [ het vermelden verbeteringen ](./listing-improvements.md).

- **[!UICONTROL Logs]** - [ het Lijst verandert ](./listing-changes-log.md) en [ communicatie fouten ](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Bekijk de instellingen voor de naam van de winkel van e-mail en Amazon in [!DNL Commerce] Admin.

## Enkele belangrijke standaardinstellingen

| Instelling | Standaard | Beschrijving | Locatie |
|----------------------------------------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | `Enabled` | Creeert overeenkomstige [!DNL Commerce] orden wanneer de nieuwe orden van Amazon worden ontvangen, toestaand orden om in het [[!DNL Commerce]  Orders ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) werkschema worden beheerd. Als `Disabled` , geeft Amazon opdracht tot het importeren van ordergegevens ter controle, maar de bestellingen moeten in uw [!DNL Amazon Seller Central] -account worden beheerd. | [ de Montages van de Orde ](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | Klantgegevens van Amazon-orders worden niet geïmporteerd in uw [!DNL Commerce] -database. Geïmporteerde Amazon-bestellingen worden verwerkt als een uitcheckbewerking voor gasten. Als u uw [!DNL Commerce] klantendatabase wilt samenstellen, moet u deze instelling wijzigen in `Build New Customer Account` . | [ de Montages van de Orde ](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] Met catalogusproducten (die voldoen aan de Amazon-vereisten om in aanmerking te komen voor deelname) kunt u automatisch publiceren naar Amazon en Amazon-aanbiedingen maken. Als u uw producten handmatig wilt bekijken en publiceren, wijzigt u deze instelling in `Do Not Automatically List Eligible Products` . De producten die op hand wachten publiceren verschijnen op [_Klaar om van_](./ready-to-list.md) tabel een lijst te maken. | [ Product dat Acties ](./product-listing-actions.md) aanbiedt |
| [!UICONTROL Magento Price Source] | `Price` | Definieert het kenmerk Prijsbron dat wordt gebruikt als basis voor je Amazon-aanbiedingen. Als u het kenmerk [!DNL Commerce] `Price` niet wilt gebruiken als de basisprijs waarop de prijsregels zijn gebaseerd, wijzigt u deze instelling in een ander kenmerk. | [ het Aanbieden Prijs ](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | De handelaar voldoet aan alle orders. Als u Fulfillment by Amazon gebruikt of een combinatie van uitvoeringsmethoden gebruikt, moet u deze instelling wijzigen. | [ die door ](./listing-price.md) wordt vervuld |
| [!UICONTROL Listing Product Condition] | `New` | Als al uw producten dezelfde voorwaarde zijn, kunt u een van de Amazon-voorwaardenopties selecteren om al uw producten te vertegenwoordigen. Als uw catalogus producten onder verschillende omstandigheden bevat (zoals Nieuw, Gebruikt en Gereviseerd), moet u deze instelling wijzigen in `Assign Condition Using Product Attribute` en de voorwaardelementen van [!DNL Commerce] toewijzen aan de Amazon-aanbiedingsvoorwaarden. | [ Voorwaarde van de Lijst van het Product ](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | none | Bepaal de regels die worden gebruikt om te bepalen welke producten Amazon verkoopkanaal aan Amazon publiceert. Deze regels bieden veel mogelijkheden om eenvoudige tot complexe regels te maken om producten als aanbiedingen op te nemen of uit te sluiten. | [ het Lijst Regels ](./listing-rules.md) |
| Prijsregels | none | Bepaal uw Amazon aanbiedingsprijsattribuut verschillend dan bepaald _[!UICONTROL Magento Price Source]_in uw [ Lijstprijs ](./listing-price.md). Als je de objectprijs wilt aanpassen (omhoog of omlaag) ten opzichte van de_[!UICONTROL Magento Price Source]_ -instelling, moet je regels maken. | [ het Tarief Regels ](./pricing-products.md) |

Voor meer informatie, zie [ Montages van de Opslag ](./ob-store-review.md).
