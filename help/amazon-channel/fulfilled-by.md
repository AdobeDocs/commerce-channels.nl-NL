---
title: Betaald door
description: Use the Fulfilled By settings to determine how the orders from Amazon listings are fulfilled (shipped).
redirect_from: /sales-channels/asc/ob-fulfilled-by.html
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Betaald door

_[!UICONTROL Fulfilled By]_settings are part of your store listing settings. Lijstinstellingen zijn toegankelijk via de [opslagdashboard](./amazon-store-dashboard.md).

Met deze instellingen wordt de partij gedefinieerd die aan bestellingen voldoet (of verzendingen). Als aan al uw bestellingen met één methode is voldaan, kiest u tussen handelaar (u) of Amazon. Als u bestellingen van uw locaties wilt uitvoeren en Amazon wilt gebruiken, kunt u het beste de derde optie gebruiken en een [!DNL Commerce] productkenmerk.

- **[!UICONTROL Fulfilled by Merchant]** - Kies of u, de handelaar, alle bestellingen uitvoert. Wanneer een bestelling wordt geplaatst, wordt de voorraad van uw [!DNL Commerce] catalogus.

- **[!UICONTROL Fulfilled by Amazon]** - Kies of Amazon aan alle bestellingen voldoet. With this option, product inventory is not deducted from your [!DNL Commerce] catalog when an order is placed. Voorraadvoorraad voor Amazon-bestellingen wordt opgeslagen en van hun pakhuis afgetrokken. Voordat u deze optie kunt toewijzen, moet u controleren in uw [!DNL Amazon Seller Central] omdat je producten in aanmerking komen voor _Betaald door Amazon_ (FBA). FBA inventory is directly managed through your [!DNL Amazon Seller Central] Account. Met deze uitvoeringsmethode deelt Amazon Sales Channel geen updates over hoeveelheden tussen [!DNL Commerce] en Amazon. Therefore, not all marketing tools described in the Quantity Settings are available to you in Amazon sales channel.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Als je en Amazon aan je producten voldoen, kun je een [!DNL Commerce] productkenmerk met waarden voor Fulfill by Merchant en Fulfill van Amazon. Setting this value per product indicates who fulfills the orders.

The fulfillment method is a regional attribute, and based on the **[!UICONTROL Amazon Marketplace Country]** setting defined during [store integration](./store-integration.md). Wanneer een wijziging wordt aangebracht, heeft de wijziging invloed op alle Amazon-aanbiedingen die dat delen [!DNL Amazon Seller SKU] in je Amazon winkels in hetzelfde gebied (zoals gedefinieerd in _[!UICONTROL Amazon Marketplace Country]_tijdens [winkelintegratie](./store-integration.md)). Een wijziging in een gedeelde [!DNL Amazon Seller SKU] in de Verenigde Staten heeft geen invloed op uw Amazon-winkels die zijn ingesteld voor een ander gebied (zoals gedefinieerd tijdens de winkelintegratie).

>[!NOTE]
>
>Wanneer Amazon (FBA) aan een bestelling voldoet en de bestelling wordt geïmporteerd, kunt u dummygegevens voor bepaalde velden in de orderdetails zien. See [Amazon Order Details](./amazon-order-details.md).

## Configure the [!UICONTROL Fulfilled By] settings {#configure-fulfilled-by-settings}

1. Click **[!UICONTROL Listing Settings]** on the store dashboard.

1. Expand the _[!UICONTROL Fulfilled By]_section.

1. For **[!UICONTROL Product Fulfilled By]**, choose who fulfills (ships) the order:

   - `Fulfilled by Merchant` - Merchant fulfills order.

   - `Fulfilled by Amazon` - Amazon warehouse fulfills order.

   - `Assign Fulfilled By Using Magento Product Attribute` - A [!DNL Commerce] attribute indicates who fulfills the order per product.

      If chosen, choose the [!DNL Commerce] attribute you want to map in **[!UICONTROL Fulfilled by Attribute]**.

1. Klik op **[!UICONTROL Save listing settings]**.

![Fulfilled By settings](assets/amazon-fulfilled-by.png)

| Veld | Description |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | Opties:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Choose if you fulfill the orders. Wanneer een bestelling wordt geplaatst, wordt de voorraad van uw [!DNL Commerce] catalogus. When a new product is created, the fulfillment method of Merchant Fulfilled is assigned.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Kies of Amazon aan de bestellingen voldoet. Met deze uitvoeringsmethode wordt de productvoorraad niet afgetrokken van uw [!DNL Commerce] catalogus wanneer een bestelling wordt geplaatst. Wanneer een product wordt gemaakt, wordt het gemaakt met _[!UICONTROL Fulfilled by Amazon (FBA)]_als het afhandelingstype. Zorg ervoor dat uw producten in aanmerking komen voor FBA-conformiteit binnen uw [!DNL Amazon Seller Central] account. FBA inventory is also directly managed through your [!DNL Amazon Seller Central] account. Met deze uitvoeringsmethode worden updates van het aantal niet uitgeduwd ten opzichte van uw [!DNL Commerce] catalogus, dus u kunt niet een aantal marketinggereedschappen gebruiken die worden beschreven in [Instellingen voor voorraad/hoeveelheid](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Kies een bestaande [!DNL Commerce] attribuut dat bepaalt of het door de handelaar wordt vervuld of door Amazon wordt vervuld. Indien gekozen, **[!UICONTROL Fulfilled by Attribute]** schakelt.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Kies de optie [!DNL Commerce] kenmerk dat wordt gebruikt om de uitvoeringsmethode te bepalen.<br><br>Als het kenmerk bijvoorbeeld _Betaald door_ en u kiest de kenmerkwaarde als _[!UICONTROL Fulfilled By Merchant]_of_[!UICONTROL Fulfilled By Amazon (FBA)]_, gebruikt het systeem die waarde als het afhandelingstype voor een nieuw product. As a merchant, you should ensure that your products are eligible for FBA fulfillment within your [!DNL Amazon Seller Central] account. De FBA-voorraad wordt ook rechtstreeks beheerd via je Amazon-verkopersaccount.<br><br>Options depend on the attributes you set up for your Amazon products. |

**Quick Access** - [!UICONTROL Listing Settings] sections

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
