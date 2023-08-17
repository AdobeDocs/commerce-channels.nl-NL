---
title: Procesvolgorde
description: '''Instructies voor verzending en annulering [!DNL Walmart Marketplace] bestellingen van Adobe Commerce en Magento Open Source. "'
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Procesvolgorde

Na [!DNL Walmart Marketplace] bestellingen zijn bevestigd en met succes verzonden naar [!DNL Channel Manager], gebruikt u [Beheer van handelsorders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace) om de bestelling te verwerken.

Kanaalbeheer synchroniseert updates met [!DNL Walmart Marketplace] om ervoor te zorgen dat de status van de bestelling en de verzendgegevens van [!DNL Commerce] komt overeen met de gegevens die in het [!DNL Walmart Marketplace].

* **Overbrenging van orders**-Walmart vereist een volgnummer voor alle zendingen. Als bepaalde items niet in voorraad zijn, kunt u gedeeltelijke verzendingen maken om items te verzenden die momenteel beschikbaar zijn. Nadat u de verzending hebt verzonden, worden de orderupdates gesynchroniseerd met [!DNL Walmart Marketplace]. Vervolgens brengt Walmart klanten op de hoogte van de status van de bestelling en de verzendgegevens.

* **Opdrachten geannuleerd**-Wanneer u een [!DNL Walmart Marketplace] bestelling, vereist de Marm een annuleringsreden die in de bericht van de ordeverstoring inbegrepen is die aan de klant wordt verzonden. De reden voor annulering wordt ook weergegeven in het dialoogvenster [!DNL Commerce] betalingsgegevens. Nadat u de annulering hebt verzonden, worden inventarisupdates gesynchroniseerd met [!DNL Walmart Marketplace]. Vervolgens brengt Walmart klanten op de hoogte van de status van de bestelling en de verzendgegevens.

  In de winkel moet u de volledige bestelling annuleren. [!DNL Commerce] staat gedeeltelijke annuleringen niet toe.

* **Terugbetalingsaanvraag**- Als een Marketplace van het Walmart voor een verscheepte orde wordt gevraagd, [!UICONTROL Status details] bevat een koppeling naar de return. Retouren en terugbetalingen worden beheerd via de [Retourneert](return-refund-orders.md) dashboard.

Wanneer handelsorders worden verwerkt en [!DNL Channel Manager] synchroniseert de updates voor verzending, gedeeltelijke verzending en annulering met de [!DNL Walmart Marketplace], is de verwerking van de bestelling voltooid. Terugbetalingsverzoeken en terugbetalingen voor verzonden bestellingen worden beheerd via de [Retourneert](return-refund-orders.md) dashboard.

>[!NOTE]
>
> Het kan maximaal vijf minuten duren voordat de volgorde van updates wordt gesynchroniseerd met [!DNL Walmart Marketplace]. Als u de status van de order wilt controleren, gaat u terug naar de [!DNL Channel Manager] Bestelpagina.

## Een bestelling verzenden

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Naar weergave [!DNL Walmart Marketplace] bestellingen, selecteren **[!UICONTROL Orders]**.

1. In de lijst van Orden opent de orde om te verzenden door te selecteren **[!UICONTROL Commerce Order Number]**.

1. Maak en verzend een verzending voor een bestelling (geheel of gedeeltelijk) door **[!UICONTROL Ship]**.

   ![Gedetailleerde weergave voor handelsorders voor een [!DNL Walmart Marketplace] bestellen](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * Kies een vervoerder en voeg een trackingnummer toe door **[!UICONTROL Add tracking number]**.

     ![Gedetailleerde weergave voor handelsorders voor een [!DNL Walmart Marketplace] bestellen](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * Vul de rest van het verzendformulier in. Zie [[!DNL Shipping an Order]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html) voor gedetailleerde instructies.

1. Na het verzenden van de zending, traceer [orderstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] om te controleren of updates zijn verzonden naar [!DNL Walmart Marketplace].

Nadat een bestelling is verzonden, kunt u volledige of gedeeltelijke terugbetalingen van [!DNL Channel Manager] voor items die in de bestelling zijn opgenomen op basis van terugkeerverzoeken ontvangen van [!DNL Walmart Marketplace]. Zie [Terugbetalingsopdrachten](return-refund-orders.md).

## Een bestelling annuleren

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Naar weergave [!DNL Walmart Marketplace] bestellingen, selecteer *[!UICONTROL Orders]**.

1. In de lijst van Orden, open [detailpagina bestellen](manage-orders.md#view-order-detail) door de **[!UICONTROL Commerce Order Number]** voor de order om te annuleren.

   ![Gedetailleerde weergave voor handelsorders voor een[!DNL Walmart Marketplace]bestellen](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. Annuleer de bestelling.

   * Selecteren **Annuleren** in het menu Order Detail.

   * Op de [!UICONTROL Cancel Order] formulier, selecteert u de **[!UICONTROL Cancellation reason]**.

   ![Gedetailleerde weergave voor handelsorders voor een [!DNL Walmart Marketplace] bestellen](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * Selecteren **[!UICONTROL Cancel Order]**.

1. Na het verzenden van de annulering volgt u de [orderstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] om te controleren of updates zijn verzonden naar [!DNL Walmart Marketplace].

## Orderfouten herstellen

Fouten kunnen optreden tijdens het synchronisatieproces van de bestelling vanaf [!DNL Walmart Marketplace]of tijdens het proces voor het bijwerken van de volgorde voor overbrengingen, gedeeltelijke overbrengingen en annuleringen.

Als de synchronisatiebewerking voor een verzending, gedeeltelijke verzending of annuleringsupdate mislukt, wordt [!DNL Channel Manager] Op de pagina Bestellingen wordt een _Fout_ status van de bestelling. Om ervoor te zorgen dat de informatie van de verzending en de orde annuleren in de rekening van de Marketplace van de Markeren correct wordt weerspiegeld, werk manueel de orde in uw [!DNL Walmart Marketplace] opslaan.


