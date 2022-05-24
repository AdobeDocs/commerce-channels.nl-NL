---
title: Procesopdrachten
description: Instructies voor verzending en annulering [!DNL Walmart Marketplace] bestellingen van Adobe Commerce en Magento Open Source.
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: 6ad7a116e931408192144e4bd446fcc0055364e1
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Procesopdrachten

Als u Adobe Commerce en Magento Open Source Order Management gebruikt om uw [!DNL Commerce] winkelverkoop, kunt u verwerken [!DNL Walmart Marketplace] bestellingen van de Handel die de zelfde werkschema gebruiken.

Wanneer u een orde in Handel verwerkt, synchroniseert de Manager van het Kanaal updates aan [!DNL Walmart Marketplace]. Deze update zorgt ervoor dat de status van de bestelling en de verzendgegevens van de Handel overeenkomen met de gegevens die worden bijgehouden in het dialoogvenster [!DNL Walmart Marketplace].

* **Overbrenging van orders**-Walmart vereist een volgnummer voor alle zendingen. U kunt gedeeltelijke verzendingen maken als u geen voorraad hebt voor alle items in de volgorde. Nadat u de verzending hebt verzonden, worden de orderupdates gesynchroniseerd met [!DNL Walmart Marketplace]. Dan, brengt het Walmart klanten over de ordestatus en verzenddetails op de hoogte.

* **Opdrachten geannuleerd**-Wanneer u een [!DNL Walmart Marketplace] bestelling, vereist de Marm een annuleringsreden die in de bericht van de ordeverstoring inbegrepen is die aan de klant wordt verzonden. De reden voor annulering wordt ook weergegeven in het dialoogvenster [!DNL Commerce] betalingsgegevens.

>[!NOTE]
>
> Het kan tot vijf minuten voor orde updates synchroniseren aan [!DNL Walmart Marketplace]. Als u de status van de order wilt controleren, gaat u terug naar de [!DNL Channel Manager] Bestelpagina.

## Een bestelling verzenden

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Naar weergave [!DNL Walmart Marketplace] bestellingen, selecteer *[!UICONTROL *Orders]**.

1. In de lijst van Orden opent de orde om te verzenden door te selecteren **Handelsordernummer**.

1. Maak en verzend een verzending voor een bestelling (geheel of gedeeltelijk) door **[!UICONTROL Ship]**.

   ![Gedetailleerde weergave voor handelsorders voor een Walmart Marketplace-order](assets/order-detail-with-external-order-id.png)

   * Kies een vervoerder en voeg een trackingnummer toe door **[!UICONTROL Add tracking number]**.

      ![Gedetailleerde weergave voor handelsorders voor een Walmart Marketplace-order](assets/order-shipment-add-tracking-number.png)


   * Vul de rest van het verzendformulier naar wens in. Zie [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) voor gedetailleerde instructies.

1. Na het verzenden van de zending, volg [orderstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] om te controleren of updates zijn verzonden naar [!DNL Walmart Marketplace].

## Een bestelling annuleren

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Naar weergave [!DNL Walmart Marketplace] bestellingen, selecteer *[!UICONTROL *Orders]**.

1. Open in de tabel Orders de pagina met orderdetails door het **Handelsordernummer** voor de order om te annuleren.

   ![Gedetailleerde weergave voor handelsorders voor een Walmart Marketplace-order](assets/order-detail-with-external-order-id.png)

1. Annuleer de bestelling.

   * Selecteren **Annuleren** in het menu Order Detail.

   * Op de [!UICONTROL Cancel Order] formulier, selecteert u de **Oplossingsreden**.

   ![Gedetailleerde weergave voor handelsorders voor een Walmart Marketplace-order](assets/cancel-order-reason-selector.png)

   * Selecteren **Bestelling annuleren**.


1. Na het verzenden van de annulering volgt u de [orderstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] om te controleren of updates zijn verzonden naar [!DNL Walmart Marketplace].
