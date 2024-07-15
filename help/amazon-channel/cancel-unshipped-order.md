---
title: Een niet-verzonden Amazon-bestelling annuleren
description: Annuleer een hangende of gedeeltelijk verscheepte (niet verscheepte) orde door uw Amazon  [!DNL Seller Central]  rekening.
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Een niet-verzonden Amazon-bestelling annuleren

Amazon-orders kunnen alleen worden geannuleerd als ze de status `Unshipped` hebben. Als de bestelling in behandeling is of gedeeltelijk wordt verzonden (niet verzonden), kan de bestelling alleen worden geannuleerd via uw [!DNL Amazon Seller Central] -account. Als het item is verzonden, moeten geretourneerde en uitgewisselde gegevens ook worden verwerkt in uw [!DNL Amazon Seller Central] -account.

>[!NOTE]
>
>Voor andere taken dan het annuleren van een bestelling:
>
>- Als u ](./order-settings.md) toegelaten de ordeinvoer [ hebt, worden de orden beheerd in het [[!DNL Commerce]  werkschema van orden ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).
>- Als [ orde de invoer ](./order-settings.md) gehandicapt is, moet u uw orden binnen beheren [!DNL Amazon Seller Central].

## Een bestelling in de status `Unshipped` annuleren

1. Klik op **[!UICONTROL View Store]** op de winkelkaart.

1. Klik in de sectie _[!UICONTROL Recent Orders]_van het opslagdashboard op een bestelnummer.

   De pagina _[!UICONTROL Amazon Order Details]_wordt weergegeven.

1. Klik op **[!UICONTROL Cancel Order]** in de koptekstbalk.

   Deze optie wordt alleen weergegeven voor bestellingen met de status `Unshipped` .

1. Kies bij **[!UICONTROL Reason for cancellation]** een optie.

1. Klik op **[!UICONTROL Confirm]**.

   De volgorde wordt geannuleerd en de status wordt in de orderdetails bijgewerkt naar `Canceled` .

Het annuleringsbericht wordt verzonden naar uw [!DNL Amazon Seller Central] account, en de klant die aan de order is gekoppeld, wordt ook op de hoogte gesteld. De status van de corresponderende [!DNL Commerce] -volgorde, indien van toepassing, verandert in `Complete` .
