---
title: Op instellingen voor Amazon-aanbiedingen ingevuld door
description: Gebruik de instellingen van het venster Betaald door om te bepalen hoe de bestellingen van Amazon-aanbiedingen zijn uitgevoerd (verzonden).
feature: Sales Channels, Products
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Op instellingen voor Amazon-aanbiedingen ingevuld door

_[!UICONTROL Fulfilled By]_-instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. De lijsten van montages worden betreden van het [ opslagdashboard ](./amazon-store-dashboard.md).

Met deze instellingen wordt de partij gedefinieerd die aan bestellingen voldoet (of verzendingen). Als aan al uw bestellingen met één methode is voldaan, kiest u tussen handelaar (u) of Amazon. Als u bestellingen van uw locaties wilt uitvoeren en Amazon wilt gebruiken, kunt u het beste de derde optie gebruiken en een productkenmerk van [!DNL Commerce] configureren.

- **[!UICONTROL Fulfilled by Merchant]** - Kies of u, de handelaar, alle bestellingen uitvoert. Wanneer een bestelling wordt geplaatst, wordt de voorraad in mindering gebracht op uw catalogus van [!DNL Commerce] .

- **[!UICONTROL Fulfilled by Amazon]** - Kies of Amazon aan alle bestellingen voldoet. Met deze optie wordt de productvoorraad niet afgetrokken van uw catalogus van [!DNL Commerce] wanneer een bestelling wordt geplaatst. Voorraadvoorraad voor Amazon-bestellingen wordt opgeslagen en van hun pakhuis afgetrokken. Alvorens deze optie toe te wijzen, moet u in uw [!DNL Amazon Seller Central] rekening verifiëren dat uw producten voor _die door Amazon_ (FBA) voldoen verkiesbaar zijn. De FBA-voorraad wordt rechtstreeks beheerd via uw [!DNL Amazon Seller Central] -account. Met deze uitvoeringsmethode deelt Amazon Sales Channel geen updates van het aantal tussen [!DNL Commerce] en Amazon. Daarom zijn niet alle marketingtools die in de Quantity Settings worden beschreven, beschikbaar in Amazon-verkoopkanalen.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Als uw producten mogelijk door u en Amazon worden geleverd, wilt u wellicht een [!DNL Commerce] -productkenmerk maken met waarden voor de optie Volledig door Merchant en Volledig door Amazon. Als u deze waarde per product instelt, wordt aangegeven wie de bestellingen uitvoert.

De uitvoeringsmethode is een regionaal attribuut, en gebaseerd op **[!UICONTROL Amazon Marketplace Country]** die tijdens [ wordt bepaald opslagintegratie ](./store-integration.md). Wanneer een verandering wordt aangebracht, beïnvloedt de verandering alle aanbiedingen van Amazon die dat [!DNL Amazon Seller SKU] in uw Amazon verkoopt opslaat in het zelfde gebied (zoals die in _[!UICONTROL Amazon Marketplace Country]_tijdens [ wordt bepaald opslagintegratie ](./store-integration.md)). Een wijziging in een gedeelde [!DNL Amazon Seller SKU] in de Verenigde Staten heeft geen invloed op uw Amazon-winkels die zijn ingesteld voor een ander gebied (zoals gedefinieerd tijdens de winkelintegratie).

>[!NOTE]
>
>Wanneer Amazon (FBA) aan een bestelling voldoet en de bestelling wordt geïmporteerd, kunt u dummygegevens voor bepaalde velden in de orderdetails zien. Zie [ de Details van de Orde van Amazon ](./amazon-order-details.md).

## De [!UICONTROL Fulfilled By] -instellingen configureren {#configure-fulfilled-by-settings}

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Fulfilled By]_uit.

1. Kies bij **[!UICONTROL Product Fulfilled By]** wie aan de order voldoet (verzendt):

   - `Fulfilled by Merchant` - Merchant voldoet aan bestelling.

   - `Fulfilled by Amazon` - Amazon-pakhuis voldoet aan bestelling.

   - `Assign Fulfilled By Using Magento Product Attribute` - Een [!DNL Commerce] -kenmerk geeft aan wie de volgorde per product invult.

     Kies desgewenst het kenmerk [!DNL Commerce] dat u wilt toewijzen in **[!UICONTROL Fulfilled by Attribute]** .

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ gevuld door montages ](assets/amazon-fulfilled-by.png){width="500" zoomable="yes"}

| Veld | Beschrijving |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product Fulfilled By] | Opties:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Kies of u de bestellingen uitvoert. Wanneer een bestelling wordt geplaatst, wordt de voorraad in mindering gebracht op uw catalogus van [!DNL Commerce] . Wanneer een nieuw product wordt gecreeerd, wordt de uitvoeringsmethode van Merchant Fulfill toegewezen.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Kies of Amazon aan de bestellingen voldoet. Met deze uitvoeringsmethode wordt de productvoorraad niet afgetrokken van uw catalogus van [!DNL Commerce] wanneer een bestelling wordt geplaatst. Wanneer een product wordt gemaakt, wordt het gemaakt met _[!UICONTROL Fulfilled by Amazon (FBA)]_als het afhandelingstype. Zorg ervoor dat uw producten in aanmerking komen voor FBA-afhandeling binnen uw [!DNL Amazon Seller Central] -account. De FBA-voorraad wordt ook rechtstreeks beheerd via uw [!DNL Amazon Seller Central] -account. Met deze uitvoeringsmethode, worden de kwantitatieve updates niet gedrukt uit met betrekking tot uw [!DNL Commerce] catalogus, zodat kunt u niet enkele marketing hulpmiddelen gebruiken die in [ worden beschreven Beeld/de Montages van de Hoeveelheid ](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Kies of u een bestaand [!DNL Commerce] -kenmerk hebt dat bepaalt of het wordt vervuld door de handelaar of door Amazon. Wanneer u deze optie kiest, schakelt **[!UICONTROL Fulfilled by Attribute]** in.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Kies het kenmerk [!DNL Commerce] dat wordt gebruikt om de uitvoeringsmethode te bepalen.<br><br> Bijvoorbeeld, als het attribuut _wordt gevuld door_ en u de attributenwaarde als `Fulfilled By Merchant` of `Fulfilled By Amazon (FBA)` kiest, gebruikt het systeemgebruik die waarde als vervulingstype voor een nieuw product. Als verkoper moet u ervoor zorgen dat uw producten in aanmerking komen voor FBA-afhandeling binnen uw [!DNL Amazon Seller Central] -account. De FBA-voorraad wordt ook rechtstreeks beheerd via je Amazon-verkopersaccount.<br><br> de Opties hangen van de attributen af die u opstelling voor uw producten van Amazon. |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
