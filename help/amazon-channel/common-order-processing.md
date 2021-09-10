---
title: Algemene taken voor het verwerken van orders
description: Gebruik het corresponderende  [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Algemene taken voor het verwerken van orders

[[!DNL Commerce] Bestelverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} kan uw Amazon-bestellingen beheren, zoals het verzenden van een e-mail naar de koper, het uitvoeren van de bestelling (verzending), het afgeven van crediteringen/terugbetalingen, het toevoegen van opmerkingen en meer. Als u uw Amazon-orders wilt beheren, moet de instelling [**Amazon-orders importeren**](./order-settings.md) zijn ingesteld op `Enabled`, zodat de corresponderende [!DNL Commerce]-orders worden gemaakt wanneer Amazon-orders worden ontvangen. De de ordeinformatie van Amazon toont in *[!UICONTROL Recent Orders]* sectie van het opslagdashboard.

Als deze optie is ingeschakeld, worden corresponderende [!DNL Commerce]-orders gemaakt voor Amazon-orders en wordt het Amazon-ordernummer weergegeven in de kolom _[!UICONTROL Order Number]_. Als een overeenkomstige [!DNL Commerce] orde wordt gecreeerd, klik het ordeaantal om de orde in [!DNL Commerce] [ordeverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} pagina te openen. U kunt de orde beheren aangezien u uw andere [[!DNL Commerce] ordeverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target= &quot;_blank&quot;} doet.

Het ordernummer [!DNL Commerce] wordt niet weergegeven met de informatie _[!UICONTROL Recent Orders]_. Het [!DNL Commerce] ordeaantal toont slechts wanneer u het ordeaantal op het opslagdashboard klikt en de orde in [[!DNL Commerce] ordeverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} opent. Als u de volgorde [!DNL Commerce] weergeeft, wordt het Amazon-bestelnummer weergegeven in de sectie *[!UICONTROL Payment & Shipping Method]*. Het bevat ook opties voor *[!UICONTROL View or Cancel Amazon Order]*en *[!UICONTROL View all Amazon Orders]*, afhankelijk van de verzendstatus van de bestelling.

Zie [Een niet-verscheepte order annuleren](./cancel-unshipped-order.md).

![Amazon Order info in the Commerce order](assets/amazon-order-number-payment-info.png)

Wanneer u een Amazon-bestelling verwerkt, wordt het Amazon-verkoopkanaal bijgewerkt en worden de ordergegevens gesynchroniseerd met uw [!DNL Amazon Seller Central]-account. Met uw uitsnijdinstellingen bepaalt u hoe vaak bestellingsgegevens worden gesynchroniseerd tussen Amazon en Amazon.

De gemeenschappelijke [!DNL Commerce] [ordeverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} taken omvatten:

- [Handelingen](https://docs.magento.com/user-guide/sales/order-actions.html) bestellen{target=&quot;_blank&quot;}
- [Order Search](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [Een volgorde](https://docs.magento.com/user-guide/sales/order-processing.html) verwerken {target=&quot;_blank&quot;}
   - [Een bestelling](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order) weergeven{target=&quot;_blank&quot;}
   - [Een volgorde](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order) verwerken {target=&quot;_blank&quot;}
   - [Order- en accountgegevens](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [Adresinformatie](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [Betalings- en verzendmethode](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [Items besteld](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered) {target=&quot;_blank&quot;} controleren
- [Een creditering/teruggave](https://docs.magento.com/user-guide/sales/credit-memo-create.html) {target=&quot;_blank&quot;} afgeven
- [Een bestelling](https://docs.magento.com/user-guide/sales/shipments-create.html) laden/verzenden {target=&quot;_blank&quot;}
- [Een factuur](https://docs.magento.com/user-guide/sales/invoice-create.html) maken{target=&quot;_blank&quot;}
- [Een niet-verzonden bestelling annuleren](./cancel-unshipped-order.md)

>[!NOTE]
>
>Als een orde in `Unshipped` status is, kunt u [een orde van Amazon ](./cancel-unshipped-order.md) op [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) pagina annuleren. Als een bestelling is verzonden, kan deze niet worden geannuleerd.

Zie [Commerce Order Management](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}.
