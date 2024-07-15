---
title: Algemene Amazon-taken voor orderverwerking
description: Gebruik de overeenkomstige  [!DNL Commerce]  die orden voor Amazon worden gecreeerd orden om ordeactiviteit en verwerking in [!UICONTROL Commerce] te beheren Admin.
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Algemene Amazon-taken voor orderverwerking

[ de ordeverwerking van Commerce ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) kan uw bestellingen van Amazon beheren, met inbegrip van het e-mailen van de koper, het vervullen van de orde (verschepen), het uitgeven van kredieten/terugbetalingen, het toevoegen van commentaren, en meer. Om uw orden van Amazon te beheren, moet uw [**Bevel van Amazon van de Invoer**](./order-settings.md) plaatsen aan `Enabled` worden geplaatst zodat de overeenkomstige [!DNL Commerce] orden worden gecreeerd wanneer de orden van Amazon worden ontvangen. Amazon-ordergegevens worden weergegeven in het gedeelte *[!UICONTROL Recent Orders]* van het opslagdashboard.

Als deze optie is ingeschakeld, worden corresponderende [!DNL Commerce] -orders gemaakt voor Amazon-orders en wordt het Amazon-ordernummer weergegeven in de kolom _[!UICONTROL Order Number]_. Als een overeenkomstige [!DNL Commerce] orde wordt gecreeerd, klik het ordeaantal om de orde in de [ Commerce ordeverwerking ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) pagina te openen. U kunt de orde beheren aangezien u uw andere [[!DNL Commerce]  ordeverwerking ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) doet.

Het ordernummer [!DNL Commerce] wordt niet weergegeven met de _[!UICONTROL Recent Orders]_-gegevens. Het de ordeaantal van Commerce toont slechts wanneer u het ordeaantal op het opslagdashboard klikt en de orde in [ de ordeverwerking van Commerce ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) opent. Als u de volgorde [!DNL Commerce] weergeeft, wordt het Amazon-bestelnummer weergegeven in de sectie *[!UICONTROL Payment & Shipping Method]*. Het bevat ook opties voor *[!UICONTROL View or Cancel Amazon Order]*en *[!UICONTROL View all Amazon Orders]*, afhankelijk van de verzendstatus van de bestelling.

Zie [ annuleren een niet verscheepte orde ](./cancel-unshipped-order.md).

![ info van de Orde van Amazon in de orde van Commerce ](assets/amazon-order-number-payment-info.png){width="500"}

Bij het verwerken van een Amazon-bestelling werkt Amazon het verkoopkanaal bij en synchroniseert het de bestelgegevens met uw [!DNL Amazon Seller Central] -account. Met uw uitsnijdinstellingen bepaalt u hoe vaak bestellingsgegevens worden gesynchroniseerd tussen Amazon en Amazon.

De gemeenschappelijke Commerce ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) taken van de bevelverwerking [ omvatten:

- ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions) de Acties van de orde 0}[
- [ Onderzoek van de Orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [ Proces een Orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [ Mening een Orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [ Proces een Orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [ orde en de Informatie van de Rekening ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [ Informatie van het Adres ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [ Betaling &amp; Verzendmethode ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - {de punten van het 0} Overzicht bevolen ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)[
- [ Uitgevend een krediet/terugbetaling ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [ het Verzenden/het verschepen van een orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [ creeer een factuur ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [Een niet-verzonden bestelling annuleren](./cancel-unshipped-order.md)

>[!NOTE]
>
>Als een orde in `Unshipped` status is, kunt u [ een orde van Amazon ](./cancel-unshipped-order.md) op de [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) pagina annuleren. Als een bestelling is verzonden, kan deze niet worden geannuleerd.

Zie [ Commerce Order Management ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
