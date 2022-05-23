---
title: Procesopdrachten
description: Instructies voor verzending en annulering [!DNL Walmart Marketplace] bestellingen van Adobe Commerce en Magento Open Source.
source-git-commit: 5670639697550b2d7fee67dd29be9c6278d5782b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Procesopdrachten

Als u Adobe Commerce en Magento Open Source Order Management gebruikt om uw [!DNL Commerce] winkelverkoop, proces [!DNL Walmart Marketplace] bestellingen van de Handel die een gelijkaardige werkschema gebruiken.

Wanneer u een orde in Handel verwerkt, synchroniseert de Manager van het Kanaal updates aan [!DNL Walmart Marketplace]. Deze update zorgt ervoor dat de productinventaris en de orderstatus van de Handel overeenkomen met de gegevens die worden bijgehouden in het dialoogvenster [!DNL Walmart Marketplace] en brengt Walmart op de hoogte om orderstatus en verzendinformatie naar klanten te verzenden.

>[!NOTE]
>
> Het kan tot vijf minuten voor de orde updates synchroniseren aan [!DNL Walmart Marketplace]. Ga terug naar [!DNL Channel Manager] Bestellingen.

## Een bestelling verzenden

Wanneer u een bestelling verzendt bij Handel, gebruikt u de opdracht [[!DNL Commerce Order Management] verzendworkflow](https://docs.magento.com/user-guide/sales/order-ship.html). Nadat u de bestelling hebt verzonden, worden updates gesynchroniseerd met [!DNL Walmart Marketplace]. Dan, brengt het Walmart klanten over de ordestatus en verzenddetails op de hoogte.

**Vereiste**

Controleer vóór verzendopdrachten of de [kanaalverzendinstellingen en configuratie van de transportserver](map-shipping-carriers.md) ontmoeten [!DNL Walmart Marketplace requirements].

### De verzending maken en verzenden

Wanneer u een [!DNL Walmart Marketplace] bestellen van [!DNL Commerce], moet u een trackingnummer toevoegen. Klanten ontvangen het trackingnummer in de kennisgeving van verzending die ze ontvangen van [!DNL Walmart].

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** om de [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Naar weergave [!DNL Walmart Marketplace] bestellingen, selecteer *[!UICONTROL *Orders]**.

1. In de lijst van Orden opent de orde om te verzenden door te selecteren **Handelsordernummer**.

1. Maak en verzend een verzending voor een bestelling (geheel of gedeeltelijk) door **[!UICONTROL Ship]**.

   - Als u een vervoerder wilt kiezen en een trackingnummer wilt toevoegen, selecteert u **[!UICONTROL Add tracking number]**.

   - Vul de rest van het verzendformulier naar wens in. Zie [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) voor gedetailleerde instructies.

1. Na het verzenden van de zending, volg [orderstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] om te controleren of updates zijn verzonden naar [!DNL Walmart Marketplace].

## Een bestelling annuleren

Wanneer u een [!DNL Walmart Marketplace] order, Walmart vereist een annuleringsreden. Wanneer de orderannulering wordt bijgewerkt naar Walmart, wordt de annuleringsreden opgenomen in de annuleringskennisgeving die naar de klant wordt verzonden.

De reden voor annulering wordt ook weergegeven in het dialoogvenster [!DNL Commerce] betalingsgegevens.

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** om de [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

1. Naar weergave [!DNL Walmart Marketplace] bestellingen, selecteer *[!UICONTROL *Orders]**.

1. Open in de tabel Orders de pagina met orderdetails door het **Handelsordernummer** voor de order om te annuleren.

   ![Gedetailleerde weergave voor handelsorders voor een Walmart Marketplace-order](assets/order-detail-with-external-order-id.png)

1. Annuleer de bestelling.

   - Selecteren **Annuleren** in het menu Order Detail.

   - Selecteer in het formulier Volgorde annuleren de optie **Oplossingsreden**.

      ![Gedetailleerde weergave voor handelsorders voor een Walmart Marketplace-order](assets/order-detail-with-external-order-id.png)

   - Selecteren **Bestelling annuleren**.

1. Controleren of updates zijn verzonden naar [!DNL Walmart Marketplace] door [orderstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager].
