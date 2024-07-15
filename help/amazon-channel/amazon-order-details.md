---
title: Amazon-ordergegevens
description: Bekijk details voor je Amazon Marketplace-bestellingen in Adobe Commerce of Magento Open Source Admin.
feature: Sales Channels, Orders
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon-ordergegevens

![ de ordedetails van Amazon ](assets/amazon-order-details-header.png){width="600" zoomable="yes"}

## Amazon-ordergegevens weergeven

1. Klik op **[!UICONTROL View Store]** op de winkelkaart.

1. Klik in de sectie _[!UICONTROL Recent Orders]_op een bestelnummer.

   De pagina _[!UICONTROL Amazon Order Details]_wordt geopend.

>[!NOTE]
>
>Als u orde invoert die in uw [ wordt toegelaten de Montages van de Orde ](./order-settings.md) en de orde wordt [ vervuld door Amazon (FBA) ](./fulfilled-by.md), kunt u dummygegevens voor sommige gebieden in de ordedetails zien. Amazon verzendt de volgende gegevens voor FBA-orders niet.
>
> - `AddressType`
> - `AddressLine1`
> - `AddressLine2`
> - `AddressLine3`
> - `BuyerName`
> - `Phone`
> - `PurchaseOrderNumber`
> - `RecipientName`
> - `CustomizedURL`
> - `GiftMessageText`

### Tabblad Bestelling en verzendgegevens

Het tabblad _[!UICONTROL Order and Shipping Details]_bevat gedetailleerde ordegegevens, zoals ontvangen van Amazon.

>[!IMPORTANT]
>
>Amazon accepteert niet-standaard adresgegevens die niet kunnen worden geïmporteerd in Amazon-verkoopkanalen, waardoor de land-/landcodes voor sommige bestellingen niet correct kunnen worden bijgewerkt. Om adresfouten te corrigeren, zijn de volgende velden bewerkbaar in de volgordedetails:
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`
>
>Vergeet niet om **te klikken sparen Orde** na het aanbrengen van uitgeeft.

![ orde en Verzenddetails ](assets/amazon-order-details.png){width="600" zoomable="yes"}

### Items bestellen, tabblad

Op het tabblad _[!UICONTROL Order Items]_worden alle items weergegeven die zijn gekoppeld aan de Amazon-volgorde, zoals deze zijn ontvangen van Amazon.

![ de Details van het Punt van de Orde ](assets/amazon-order-item-details.png){width="600" zoomable="yes"}

### Tabblad Tekstspatiëring

Op het tabblad _[!UICONTROL Tracking]_vindt u informatie over het bijhouden van de Amazon-volgorde.

![ het Volgen details ](assets/amazon-order-tracking-details.png){width="600" zoomable="yes"}
