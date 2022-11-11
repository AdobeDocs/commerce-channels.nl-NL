---
title: Algemene taken voor het verwerken van orders
description: Gebruik de bijbehorende [!DNL Commerce] bestellingen die zijn gemaakt voor Amazon bestellingen om orderactiviteiten en verwerking in de [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Algemene taken voor het verwerken van orders

[[!DNL Commerce] orderverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} kan uw Amazon-bestellingen beheren, zoals het per e-mail verzenden van de koper, het uitvoeren van de bestelling (verzending), het afgeven van crediteringen/terugbetalingen, het toevoegen van opmerkingen en meer. Als u uw Amazon-bestellingen wilt beheren, [**Amazon-bestellingen importeren**](./order-settings.md) instellen op `Enabled` zodat [!DNL Commerce] bestellingen worden gemaakt wanneer Amazon-bestellingen worden ontvangen. Amazon-ordergegevens worden weergegeven in het dialoogvenster *[!UICONTROL Recent Orders]* van het opslagdashboard.

Indien ingeschakeld, komt deze overeen met [!DNL Commerce] bestellingen worden gemaakt voor Amazon-bestellingen en het Amazon-ordernummer wordt weergegeven in de _[!UICONTROL Order Number]_kolom. Indien [!DNL Commerce] de orde wordt gecreeerd, klik het ordeaantal om de orde in te openen [!DNL Commerce] [orderverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} pagina. U kunt de volgorde op dezelfde manier beheren als de andere [[!DNL Commerce] orderverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}.

De [!DNL Commerce] het ordernummer wordt niet weergegeven bij het _[!UICONTROL Recent Orders]_informatie. De [!DNL Commerce] het ordernummer wordt alleen weergegeven wanneer u op het ordernummer op het opslagdashboard klikt en de volgorde opent in [[!DNL Commerce] orderverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}. Wanneer u de [!DNL Commerce] bestelling, wordt het Amazon-bestelnummer weergegeven in de *[!UICONTROL Payment & Shipping Method]*sectie. Het bevat ook opties voor *[!UICONTROL View or Cancel Amazon Order]*en *[!UICONTROL View all Amazon Orders]*, afhankelijk van de verzendstatus van de bestelling.

Zie [Een niet-verzonden bestelling annuleren](./cancel-unshipped-order.md).

![Amazon Order info in the Commerce order](assets/amazon-order-number-payment-info.png)

Bij het verwerken van een Amazon-bestelling werkt Amazon het verkoopkanaal bij en synchroniseert het de bestelgegevens met uw [!DNL Amazon Seller Central] account. Met uw uitsnijdinstellingen bepaalt u hoe vaak bestellingsgegevens worden gesynchroniseerd tussen Amazon en Amazon.

Vaak [!DNL Commerce] [orderverwerking](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} taken omvatten:

- [Handelingen ordenen](https://docs.magento.com/user-guide/sales/order-actions.html){target=&quot;_blank&quot;}
- [Zoeken in bestellingen](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [Een bestelling verwerken](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}
   - [Een bestelling weergeven](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target=&quot;_blank&quot;}
   - [Een bestelling verwerken](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target=&quot;_blank&quot;}
   - [Opdracht- en accountgegevens](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [Adresgegevens](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [Betalings- en verzendmethode](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [Geordende items controleren](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target=&quot;_blank&quot;}
- [Afgifte van een krediet/terugbetaling](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;}
- [Bestelling uitvoeren/verzenden](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;}
- [Een factuur maken](https://docs.magento.com/user-guide/sales/invoice-create.html){target=&quot;_blank&quot;}
- [Een niet-verzonden bestelling annuleren](./cancel-unshipped-order.md)

>[!NOTE]
>
>Als een order zich in `Unshipped` status, kunt u [Amazon-bestellingen annuleren](./cancel-unshipped-order.md) op de [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) pagina. Als een bestelling is verzonden, kan deze niet worden geannuleerd.

Zie [Beheer van handelsorders](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}.
