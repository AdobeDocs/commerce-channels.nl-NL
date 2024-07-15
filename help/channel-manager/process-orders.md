---
title: Procesvolgorde
description: "Instructies voor het verschepen en het annuleren van  [!DNL Walmart Marketplace]  bevelen van Adobe Commerce en Magento Open Source."
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Procesvolgorde

Nadat [!DNL Walmart Marketplace] orden zijn erkend en met succes verzonden naar [!DNL Channel Manager], gebruikt u [ Commerce Order Management ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace) om de orde te verwerken.

Channel Manager synchroniseert updates naar [!DNL Walmart Marketplace] om ervoor te zorgen dat de orderstatus en de verzendgegevens van [!DNL Commerce] overeenkomen met de gegevens die worden bijgehouden in de [!DNL Walmart Marketplace] .

* **de zendingen van de Orde** - Marm vereist een volgend aantal voor alle transporten. Als bepaalde items niet in voorraad zijn, kunt u gedeeltelijke verzendingen maken om items te verzenden die momenteel beschikbaar zijn. Nadat u de verzending hebt verzonden, worden de orderupdates gesynchroniseerd met [!DNL Walmart Marketplace] . Vervolgens brengt Walmart klanten op de hoogte van de status van de bestelling en de verzendgegevens.

* **de annuleringen van de Orde** - wanneer u a [!DNL Walmart Marketplace] orde annuleert, vereist de Marm van de Volgorde een annuleringsreden die in de bericht inbegrepen is van de ordeverstoring die naar de klant wordt verzonden. De reden voor annulering wordt ook weergegeven in de betalingsgegevens van de bestelling van [!DNL Commerce] . Nadat u de annulering hebt verzonden, worden inventarisupdates gesynchroniseerd met [!DNL Walmart Marketplace] . Vervolgens brengt Walmart klanten op de hoogte van de status van de bestelling en de verzendgegevens.

  In de winkel moet u de volledige bestelling annuleren. In [!DNL Commerce] zijn gedeeltelijke annuleringen niet toegestaan.

* **verzoek van de Terugbetaling** - als een terugkeer van de Marketplace van het Walmart voor een verscheepte orde wordt gevraagd, omvat [!UICONTROL Status details] een verbinding aan de terugkeer. De terugkeer en de terugbetalingen worden beheerd van [ Keert ](return-refund-orders.md) dashboard terug.

Wanneer Commerce-orders worden verwerkt en [!DNL Channel Manager] verzendingen, gedeeltelijke verzending en annuleringen van updates naar [!DNL Walmart Marketplace] correct synchroniseert, is de verwerking van de bestelling voltooid. De verzoeken van de terugkeer en de terugbetalingen voor verscheepte orden worden beheerd van [ Keert ](return-refund-orders.md) dashboard terug.

>[!NOTE]
>
> Het kan maximaal vijf minuten duren voordat de volgorde van de updates wordt gesynchroniseerd met [!DNL Walmart Marketplace] . Ga terug naar de pagina [!DNL Channel Manager] Bestellingen om de status van de bestelling te controleren.

## Een bestelling verzenden

1. Selecteer in het menu Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** .

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Selecteer **[!UICONTROL Orders]** als u [!DNL Walmart Marketplace] -bestellingen wilt weergeven.

1. In de lijst van Orden, open de orde om te verzenden door **[!UICONTROL Commerce Order Number]** te selecteren.

1. Selecteer **[!UICONTROL Ship]** om een verzending voor een bestelling of een deel ervan te maken en te verzenden.

   ![ het detailmening van de Orde van Commerce voor a [!DNL Walmart Marketplace] orde ](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * Selecteer **[!UICONTROL Add tracking number]** en kies een verzendende vervoerder en voeg een trackingnummer toe.

     ![ het detailmening van de Orde van Commerce voor a [!DNL Walmart Marketplace] orde ](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * Vul de rest van het verzendformulier in. Zie [[!DNL Shipping an Order] ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html) voor gedetailleerde instructies.

1. Na het voorleggen van de zending, spoor de [ ordestatus ](manage-orders.md#about-order-status) in [!DNL Channel Manager] om te verifiëren dat de updates werden verzonden naar [!DNL Walmart Marketplace].

Nadat een bestelling is verzonden, kunt u volledige of gedeeltelijke terugbetalingen van [!DNL Channel Manager] verwerken voor items die in de bestelling zijn opgenomen op basis van aanvragen die u van [!DNL Walmart Marketplace] hebt ontvangen. Zie [ Terugkeer en terugbetalingsorden ](return-refund-orders.md).

## Een bestelling annuleren

1. Selecteer in het menu Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** .

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Als u [!DNL Walmart Marketplace] -bestellingen wilt weergeven, selecteert u * [!UICONTROL Orders] **.

1. In de lijst van Orden, open de [ orde detailpagina ](manage-orders.md#view-order-detail) door **[!UICONTROL Commerce Order Number]** voor de orde te selecteren om te annuleren.

   ![ het detailmening van de Orde van Commerce voor a [!DNL Walmart Marketplace] orde ](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. Annuleer de bestelling.

   * Selecteer **annuleren** van het menu van het Detail van de Orde.

   * Selecteer in het [!UICONTROL Cancel Order] -formulier de **[!UICONTROL Cancellation reason]** .

   ![ het detailmening van de Orde van Commerce voor a [!DNL Walmart Marketplace] orde ](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * Selecteer **[!UICONTROL Cancel Order]** .

1. Na het voorleggen van de annulering, spoor de [ ordestatus ](manage-orders.md#about-order-status) in [!DNL Channel Manager] om te verifiëren dat de updates werden verzonden naar [!DNL Walmart Marketplace].

## Orderfouten herstellen

Er kunnen fouten optreden tijdens het synchronisatieproces van de bestelling vanuit [!DNL Walmart Marketplace] of tijdens het proces voor het bijwerken van de bestelling voor verzendingen, gedeeltelijke verzendingen en annuleringen.

Als de synchronisatieverrichting voor een verzending, gedeeltelijke verzending, of annuleringsupdate ontbreekt, toont de [!DNL Channel Manager] pagina van Orden een _2} status van de Fout {voor de orde._ Werk de volgorde handmatig bij in uw [!DNL Walmart Marketplace] -winkel om ervoor te zorgen dat informatie over verzending en annulering van bestellingen correct wordt weergegeven in het Walmart Marketplace-account.


