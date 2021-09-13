---
title: Betaald door
description: Gebruik de instellingen van het venster Betaald door om te bepalen hoe de bestellingen van Amazon-aanbiedingen zijn uitgevoerd (verzonden).
redirect_from: /sales-channels/asc/ob-fulfilled-by.html: 
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 0
ht-degree: 0%

---

# Betaald door

_[!UICONTROL Fulfilled By]_Deze instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via het [opslagdashboard](./amazon-store-dashboard.md).

Met deze instellingen wordt de partij gedefinieerd die aan bestellingen voldoet (of verzendingen). Als aan al uw bestellingen met één methode is voldaan, kiest u tussen handelaar (u) of Amazon. Als u bestellingen van uw locaties wilt uitvoeren en Amazon wilt gebruiken, kunt u het beste de derde optie gebruiken en een [!DNL Commerce]-productkenmerk configureren.

- **[!UICONTROL Fulfilled by Merchant]** - Kies of u, de handelaar, alle bestellingen uitvoert. Wanneer een bestelling wordt geplaatst, wordt de voorraad afgetrokken van uw [!DNL Commerce] catalogus.

- **[!UICONTROL Fulfilled by Amazon]** - Kies of Amazon aan alle bestellingen voldoet. Met deze optie wordt de productvoorraad niet afgetrokken van uw [!DNL Commerce]-catalogus wanneer een bestelling wordt geplaatst. Voorraadvoorraad voor Amazon-bestellingen wordt opgeslagen en van hun pakhuis afgetrokken. Voordat u deze optie toewijst, moet u in uw [!DNL Amazon Seller Central]-account controleren of uw producten in aanmerking komen voor _Betaald door Amazon_ (FBA)-tegoed. De FBA-inventarisatie wordt rechtstreeks beheerd via uw [!DNL Amazon Seller Central]-account. Met deze uitvoeringsmethode deelt Amazon Sales Channel geen updates voor het aantal pixels tussen [!DNL Commerce] en Amazon. Daarom zijn niet alle marketingtools die in de Quantity Settings worden beschreven, beschikbaar in Amazon-verkoopkanalen.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Als uw producten door u en Amazon kunnen worden vervuld, kunt u een  [!DNL Commerce] productkenmerk met waarden voor Fulfill door Merchant en Fulfill door Amazon maken. Als u deze waarde per product instelt, wordt aangegeven wie de bestellingen uitvoert.

De uitvoeringsmethode is een regionaal kenmerk en is gebaseerd op de instelling **[!UICONTROL Amazon Marketplace Country]** die tijdens [store integration](./store-integration.md) is gedefinieerd. Wanneer een wijziging wordt aangebracht, heeft de wijziging invloed op alle Amazon-aanbiedingen die [!DNL Amazon Seller SKU] in uw Amazon delen en die in hetzelfde gebied verkopen (zoals gedefinieerd in _[!UICONTROL Amazon Marketplace Country]_tijdens [winkelintegratie](./store-integration.md)). Een wijziging in een gedeelde [!DNL Amazon Seller SKU] in de Verenigde Staten heeft geen invloed op uw Amazon-winkels die zijn ingesteld voor een ander gebied (zoals gedefinieerd tijdens de winkelintegratie).

>[!NOTE]
>
>Wanneer Amazon (FBA) aan een bestelling voldoet en de bestelling wordt geïmporteerd, kunt u dummygegevens voor bepaalde velden in de orderdetails zien. Zie [Amazon Order Details](./amazon-order-details.md).

## De [!UICONTROL Fulfilled By]-instellingen configureren {#configure-fulfilled-by-settings}

1. Klik **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Fulfilled By]_uit.

1. Kies voor **[!UICONTROL Product Fulfilled By]** wie aan de order voldoet (schepen):

   - `Fulfilled by Merchant` - Merchant voldoet aan order.

   - `Fulfilled by Amazon` - Amazon-entrepot voldoet aan de voorwaarden.

   - `Assign Fulfilled By Using Magento Product Attribute` - Een  [!DNL Commerce] kenmerk geeft aan wie voldoet aan de volgorde per product.

      Kies desgewenst het [!DNL Commerce]-kenmerk dat u wilt toewijzen in **[!UICONTROL Fulfilled by Attribute]**.

1. Klik op **[!UICONTROL Save listing settings]** als u klaar bent.

![Betaald door instellingen](assets/amazon-fulfilled-by.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | Opties:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Kies of u aan de bestellingen voldoet. Wanneer een bestelling wordt geplaatst, wordt de voorraad afgetrokken van uw [!DNL Commerce] catalogus. Wanneer een nieuw product wordt gecreeerd, wordt de uitvoeringsmethode van Merchant Fulfill toegewezen.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Kies of Amazon aan de bestellingen voldoet. Met deze uitvoeringsmethode wordt de productvoorraad niet afgetrokken van uw [!DNL Commerce]-catalogus wanneer een bestelling wordt geplaatst. Wanneer een product wordt gecreeerd, wordt het gecreeerd met _[!UICONTROL Fulfilled by Amazon (FBA)]_als vervulingstype. Zorg ervoor dat uw producten in aanmerking komen voor FBA-afhandeling binnen uw [!DNL Amazon Seller Central]-account. De FBA-inventarisatie wordt ook rechtstreeks beheerd via uw [!DNL Amazon Seller Central]-account. Met deze uitvoeringsmethode worden updates van het aantal niet uitgeduwd ten opzichte van uw [!DNL Commerce] catalogus, zodat kunt u niet enkele marketinghulpmiddelen gebruiken die in [Stock/Quantity Settings](./stock-quantity.md) worden beschreven.</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Kies of u een bestaand  [!DNL Commerce] kenmerk hebt dat bepaalt of het wordt vervuld door de handelaar of door Amazon. Als u **[!UICONTROL Fulfilled by Attribute]** kiest, wordt deze ingeschakeld.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Kies het [!DNL Commerce] attribuut dat wordt gebruikt om de uitvoeringsmethode te bepalen.<br><br>Als het kenmerk bijvoorbeeld  _vol_ bytes is en u kiest de kenmerkwaarde als  _[!UICONTROL Fulfilled By Merchant]_of_[!UICONTROL Fulfilled By Amazon (FBA)]_, gebruikt het systeem die waarde als het afhandelingstype voor een nieuw product. Als verkoper moet u ervoor zorgen dat uw producten in aanmerking komen voor FBA-afhandeling binnen uw [!DNL Amazon Seller Central]-account. De FBA-voorraad wordt ook rechtstreeks beheerd via je Amazon-verkopersaccount.<br><br>Welke opties beschikbaar zijn, is afhankelijk van de kenmerken die u instelt voor uw Amazon-producten. |

**Snelle toegang**  -  [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
