---
title: Een niet-verzonden Amazon-bestelling annuleren
description: Een lopende of gedeeltelijk verzonden (niet-verzonden) bestelling via je Amazon annuleren [!DNL Seller Central] account.
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Een niet-verzonden Amazon-bestelling annuleren

Amazon-orders kunnen alleen worden geannuleerd als ze zich in een `Unshipped` status. Als de bestelling in behandeling is of gedeeltelijk wordt verzonden (niet verzonden), kan de bestelling alleen via uw [!DNL Amazon Seller Central] account. Als het object is verzonden, moeten geretourneerde en uitgewisselde gegevens ook in uw [!DNL Amazon Seller Central] Account.

>[!NOTE]
>
>Voor andere taken dan het annuleren van een bestelling:
>
>- Als u [orderimport](./order-settings.md) ingeschakeld, worden bestellingen beheerd in het dialoogvenster [[!DNL Commerce] orderwerkstroom](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).
>- Indien [orderimport](./order-settings.md) is uitgeschakeld, moet u uw bestellingen beheren in [!DNL Amazon Seller Central].

## Een bestelling annuleren in `Unshipped` status

1. Klikken **[!UICONTROL View Store]** op de winkelkaart.

1. In de _[!UICONTROL Recent Orders]_klikt u op een bestelnummer in het opslagdashboard.

   De _[!UICONTROL Amazon Order Details]_wordt weergegeven.

1. Klikken **[!UICONTROL Cancel Order]** in de koptekstbalk.

   Deze optie wordt alleen weergegeven voor opdrachten in `Unshipped` status.

1. Voor **[!UICONTROL Reason for cancellation]** kiest u een optie.

1. Klikken **[!UICONTROL Confirm]**.

   De volgorde wordt geannuleerd en de status wordt bijgewerkt naar `Canceled` in de ordergegevens.

Het annuleringsbericht wordt naar uw verzonden [!DNL Amazon Seller Central] en de klant die aan de order is gekoppeld, wordt hiervan op de hoogte gesteld. De status van de overeenkomstige [!DNL Commerce] eventuele wijzigingen in de volgorde van `Complete`.
