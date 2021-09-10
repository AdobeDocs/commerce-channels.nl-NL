---
title: Een niet-verzonden bestelling annuleren
description: Annuleer een bestelling die in behandeling is of gedeeltelijk is verzonden (niet verzonden) via uw Amazon [!DNL Seller Central] account.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Een niet-verzonden bestelling annuleren

Amazon-orders kunnen alleen worden geannuleerd als ze de status `Unshipped` hebben. Als de bestelling in behandeling is of gedeeltelijk wordt verzonden (niet verzonden), kan de bestelling alleen worden geannuleerd via uw [!DNL Amazon Seller Central]-account. Als het item is verzonden, moeten de geretourneerde en uitgewisselde gegevens ook worden verwerkt in uw [!DNL Amazon Seller Central]-account.

>[!NOTE]
>
>Voor andere taken dan het annuleren van een bestelling:
>
>- Als u [orde invoer](./order-settings.md) toegelaten hebt, worden de orden beheerd in [[!DNL Commerce] ordeswerkschema](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.
>- Als [order import](./order-settings.md) is uitgeschakeld, moet u uw bestellingen beheren in [!DNL Amazon Seller Central].


## Een bestelling in de status `Unshipped` annuleren

1. Klik op **[!UICONTROL View Store]** op de winkelkaart.

1. Klik in de sectie _[!UICONTROL Recent Orders]_van het opslagdashboard op een bestelnummer.

   De pagina _[!UICONTROL Amazon Order Details]_wordt weergegeven.

1. Klik **[!UICONTROL Cancel Order]** in de kopbalbar.

   Deze optie wordt alleen weergegeven voor bestellingen met de status `Unshipped`.

1. Kies voor **[!UICONTROL Reason for cancellation]** een optie.

1. Klik op **[!UICONTROL Confirm]**.

   De volgorde wordt geannuleerd en de status wordt in de orderdetails bijgewerkt naar `Canceled`.

Het annuleringsbericht wordt naar uw [!DNL Amazon Seller Central]-account verzonden en de klant die aan de order is gekoppeld, wordt ook op de hoogte gesteld. De status van de corresponderende [!DNL Commerce]-volgorde, indien aanwezig, verandert in `Complete`.
