---
title: Algemene Amazon-taken voor orderverwerking
description: Gebruik de bijbehorende [!DNL Commerce] bestellingen die zijn gemaakt voor Amazon bestellingen om orderactiviteiten en verwerking in de [!UICONTROL Commerce] Admin.
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Algemene Amazon-taken voor orderverwerking

[Bewerking van handelsorders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) kan uw Amazon-bestellingen beheren, zoals het per e-mail verzenden van de koper, het voldoen aan de bestelling (verzending), het afgeven van crediteringen/terugbetalingen, het toevoegen van opmerkingen en meer. Als u uw Amazon-bestellingen wilt beheren, [**Amazon-bestellingen importeren**](./order-settings.md) instellen op `Enabled` zodat [!DNL Commerce] bestellingen worden gemaakt wanneer Amazon-bestellingen worden ontvangen. Amazon-ordergegevens worden weergegeven in het dialoogvenster *[!UICONTROL Recent Orders]* van het opslagdashboard.

Indien ingeschakeld, komt deze overeen met [!DNL Commerce] bestellingen worden gemaakt voor Amazon-bestellingen en het Amazon-ordernummer wordt weergegeven in de _[!UICONTROL Order Number]_kolom. Indien [!DNL Commerce] de orde wordt gecreeerd, klik het ordeaantal om de orde in te openen [Bewerking van handelsorders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) pagina. U kunt de volgorde op dezelfde manier beheren als de andere [[!DNL Commerce] orderverwerking](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

De [!DNL Commerce] het ordernummer wordt niet weergegeven bij het _[!UICONTROL Recent Orders]_informatie. Het de ordeaantal van de Handel toont slechts wanneer u het ordeaantal op het opslagdashboard klikt en de orde opent in [Bewerking van handelsorders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order). Wanneer u de [!DNL Commerce] bestelling, wordt het Amazon-bestelnummer weergegeven in de *[!UICONTROL Payment & Shipping Method]*sectie. Het bevat ook opties voor *[!UICONTROL View or Cancel Amazon Order]*en *[!UICONTROL View all Amazon Orders]*, afhankelijk van de verzendstatus van de bestelling.

Zie [Een niet-verzonden bestelling annuleren](./cancel-unshipped-order.md).

![Amazon Order info in the Commerce order](assets/amazon-order-number-payment-info.png){width="500"}

Bij het verwerken van een Amazon-bestelling werkt Amazon het verkoopkanaal bij en synchroniseert het de bestelgegevens met uw [!DNL Amazon Seller Central] account. Met uw uitsnijdinstellingen bepaalt u hoe vaak bestellingsgegevens worden gesynchroniseerd tussen Amazon en Amazon.

Gemeenschappelijke handel [orderverwerking](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) tot de taken behoren :

- [Handelingen ordenen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [Zoeken in bestellingen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [Een bestelling verwerken](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [Een bestelling weergeven](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [Een bestelling verwerken](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [Opdracht- en accountgegevens](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [Adresgegevens](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [Betalings- en verzendmethode](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [Geordende items controleren](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [Afgifte van een krediet/terugbetaling](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [Bestelling uitvoeren/verzenden](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [Een factuur maken](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [Een niet-verzonden bestelling annuleren](./cancel-unshipped-order.md)

>[!NOTE]
>
>Als een order zich in `Unshipped` status, kunt u [Amazon-bestellingen annuleren](./cancel-unshipped-order.md) op de [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) pagina. Als een bestelling is verzonden, kan deze niet worden geannuleerd.

Zie [Beheer van handelsorders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
