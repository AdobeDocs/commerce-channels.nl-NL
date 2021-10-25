---
title: Een niet-verzonden bestelling annuleren
description: Een lopende of gedeeltelijk verzonden (niet-verzonden) bestelling via je Amazon annuleren [!DNL Seller Central] account.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Een niet-verzonden bestelling annuleren

Amazon-orders kunnen alleen worden geannuleerd als ze zich in een `Unshipped` status. Als de bestelling in behandeling is of gedeeltelijk wordt verzonden (niet verzonden), kan de bestelling alleen via uw [!DNL Amazon Seller Central] account. Als het object is verzonden, moeten geretourneerde en uitgewisselde gegevens ook in uw [!DNL Amazon Seller Central] Account.

>[!NOTE]
>
>Voor andere taken dan het annuleren van een bestelling:
>
>- Als u [orderimport](./order-settings.md) ingeschakeld, worden bestellingen beheerd in het dialoogvenster [[!DNL Commerce] orderwerkstroom](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.
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
