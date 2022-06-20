---
title: '"Beheren [!DNL Walmart Marketplace] Bestellingen"'
description: '"Weergeven en beheren [!DNL Walmart Marketplace] bestellingen met [!DNL Channel Manager] voor Adobe Commerce en Magento Open Source."'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: eb57189ed866fffa064867d1de5ae9db5b32e283
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Beheren [!DNL Walmart Marketplace] orders

[!DNL Walmart Marketplace] ordergegevens voor [!DNL Commerce] producten worden automatisch gesynchroniseerd met [!DNL Channel Manager] na [!DNL Walmart] verwerkt de volgorde.

Aan de kant van de Handel, brengt een succesvolle synchronisatie de volgende acties teweeg:

- [!DNL Channel Manager] verzendt een ordererkenning naar Walmart.

- Een overeenkomstige orde van de Handel wordt gecreeerd van de orde van de Marm van de Walmart.

- De bijgewerkte ordegegevens worden weergegeven op het tabblad [!DNL Channel Manager] Orders dashboard.

In de opslagbeheerder kunt u ordegegevens weergeven vanuit [!DNL Channel Manager] door de winkel met verkoopkanalen te openen en **[!UICONTROL Orders]**.

![Weergave voor bestellingen kanaalbeheer die moet worden beheerd [!DNL Walmart Marketplace] orders](assets/orders-dashboard-view.png)

>[!NOTE]
>
>Het kan tot 35 minuten duren [!DNL Walmart Marketplace] in de [!DNL Channel Manager] orderlijst. [!DNL Walmart] vereist ongeveer 30 minuten om binnenkomende orders te verwerken en naar te sturen [!DNL Channel Manager]. Nadat Channel Manager de bestelling heeft ontvangen, duurt het nog ongeveer vijf minuten om de bestelling te maken en weer te geven in Adobe Commerce of Magento Open Source.

## Besturingselementen voor bestellingen en kolombeschrijvingen

De volgende lijsten beschrijven de controles en de kolommen beschikbaar voor Orden.

**Besturingselementen voor[!UICONTROL Orders]**
| **Control**                    | **Beschrijving**                                                                                                                                                                                                                                                                  | |—|—| | [!UICONTROL Filter orders]     | U kunt de weergave sorteren door een van de [!UICONTROL Order Status] kaarten.                                                                                                                                                                                                           | | Foutbeschrijving | Verstrekt meer gedetailleerde informatie over orden met een status van de Fout.                                                                                                                                                                                                            | | [!UICONTROL View order detail] | Selecteer de optie [!DNL Commerce] ordernummer in het [!UICONTROL Order] tabel. Gebruik vervolgens [!DNL Commerce] bestellen opties om de bestelling te verwerken.                                                                                                                    | | [!UICONTROL Channel Settings]  | Om de kanaalconfiguratie te wijzigen, selecteert de uitgezochte geloofsbrieven van de Verbinding van het Kanaal, in kaart gebrachte attributen, of verschepende herkenningstekens, montages [!DNL Commerce] ordernummer in het [!UICONTROL Order] tabel. Gebruik vervolgens [!DNL Commerce] bestellen opties om de bestelling te verwerken. |


**Kolombeschrijvingen**

| Veld | Beschrijving |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Walmart Order Number] | Het inkoopordernummer dat aan de order in het [!DNL Walmart Marketplace]. Wanneer een bestelling voor het eerst wordt geïmporteerd in [!DNL Channel Manager], alleen de [!DNL Walmart] het aantal van de orde toont. Wanneer de [!DNL Commerce] order wordt gemaakt, de [!DNL Walmart] ordernummer wordt opgeslagen in het dialoogvenster [!UICONTROL External ID] productkenmerk. |
| [!DNL Commerce] Volgnummer | Het nummer dat aan de [!DNL Commerce] bestelling gemaakt op basis van de [!DNL Walmart Marketplace] bestelling. |
| Items | Aantal bestelde objecten op [!DNL Walmart Marketplace]. |
| [!UICONTROL Order Value] | Totale kosten van de bestelde objecten. |
| [!UICONTROL Date Ordered] | De datum waarop de bestelling is ingediend op de [!DNL Walmart Marketplace]. |
| [!UICONTROL Ship By Date] | Datum waarop de bestelling moet worden verzonden door om te voldoen aan [!DNL Walmart Marketplace] eisen. |
| [!UICONTROL Deliver By Date] | Datum waarop de bestelling aan de klant moet worden geleverd om te voldoen [!DNL Walmart Marketplace] vereisten in UTC-indeling. |
| [!UICONTROL Ship Method] | De [[!DNL Walmart Marketplace] Verzendmethode](https://sellerhelp.walmart.com/s/guide?article=000007893) geselecteerd voor de volgorde. |
| [!UICONTROL Last Update At] | Tijdstempel die aangeeft wanneer de bestelgegevens het laatst zijn bijgewerkt [!DNL Channel Manager] in UTC-indeling. |
| [!UICONTROL Status] | Geeft de huidige orderstatus in het dialoogvenster [!DNL Commerce] bestelworkflow. De beginstatus van een bestelling die is geïmporteerd uit [!DNL Walmart Marketplace] is _Openen_. Er vinden extra statusupdates plaats wanneer handelsorders worden verwerkt en [!DNL Channel Manager] synchroniseert de updates voor verzending, gedeeltelijke verzending en annulering met de [!DNL Walmart Marketplace]. |
| [!UICONTROL Error Description] | Verstrekt meer gedetailleerde informatie over orden met een _[!UICONTROL Error]_status. |

## Status van bestelling


[!UICONTROL Order Status] bevat informatie over de huidige status van [!DNL Walmart Marketplace] bestellingen beheerd vanuit Adobe Commerce of Magento Open Source. De statusupdates van de orde komen voor wanneer [!DNL Channel Manager] ontvangt bijgewerkte orderinformatie van of [!DNL Walmart Marketplace] of de [!DNL Commerce] bestelsysteem. Orders kunnen de volgende statussen hebben:

- **[!UICONTROL Shipped]**-Bestellingen die zijn verzonden vanuit de [!DNL Commerce] opslaan. Wanneer de order wordt verscheept, [!DNL Channel Manager] verzendt een update naar [!DNL Walmart Marketplace] om de verzendstatus op Walmart bij te werken en het volgnummer voor de verzending te geven.

- **[!UICONTROL Partially Shipped]**—Bestellingen waarvan sommige objecten zijn gemarkeerd als verzonden en andere nog moeten worden verzonden. Wanneer items in de order worden verzonden [!DNL Channel Manager] verzendt een update naar [!DNL Walmart Marketplace] om de verzendstatus bij te werken naar een gedeeltelijke verzending via Walmart en het volgnummer van de bestelling voor de verzending op te geven.

- **[!UICONTROL Canceled]**-Bestellingen die zijn geannuleerd vanaf de [!DNL Commerce] opslaan.

   Nadat de orderannulering is voltooid, worden de [!DNL Commerce] voorraadhoeveelheid wordt bijgewerkt om geretourneerde objecten weer te geven. Vervolgens [!DNL Channel Manager] synchroniseert de update naar de [!DNL Walmart Marketplace].

- **[!UICONTROL Error]**- Orders met fouten. Fouten kunnen optreden wanneer een bewerking voor het bijwerken van een bestelling mislukt. Er treden bijvoorbeeld fouten op als [!DNL Channel Manager] kan geen nieuwe bestelling van Walmart ontvangen. Ze kunnen ook voorkomen als [!DNL Channel Manager] kan geen update voor verzending of annulering van een bestelling verzenden naar de [!DNL Walmart Marketplace]. Als een bewerking mislukt, wordt op de pagina Bestellingen een _Fout_ status van de bestelling. Zie voor meer informatie [Orderfouten herstellen](process-orders.md#fix-Shipping-and-cancelation- errors).

- **[!UICONTROL Error description]**- Verstrekt gedetailleerde informatie over ordefouten die toe te schrijven aan kwesties zoals ontbrekende informatie of ongeldige waarden, onjuiste verzenddetails, of een ontbroken orde annuleren voorkomen. Aan de hand van de beschrijving kunt u bepalen of er een fout is opgetreden in het dialoogvenster [!DNL Commerce] of op de [!DNL Walmart Marketplace].

>[!NOTE]
>
>Als orderitems in meerdere verzendingen worden verzonden, wordt de orderstatus in [!DNL Channel Manager] geeft de laatste beschikbare orderstatus weer. Als het eerste item bijvoorbeeld wordt verzonden en er geen fouten worden geretourneerd wanneer orderupdates worden gesynchroniseerd naar [!DNL Channel Manager] en [!DNL Walmart Marketplace]de [!DNL Channel Manager] orderstatus is _[!UICONTROL Partially Shipped]_.  Als een tweede object wordt verzonden en [!CKanaalbeheer] retourneert een fout. De status van de bestelling wordt bijgewerkt naar_[!UICONTROL Error]_.

## Bestellingen controleren

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** om de [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Open de archiefweergave door het oogpictogram in een rij met items in de winkel te selecteren.

1. Selecteer * om de ordergegevens weer te geven[!UICONTROL *Orders]**.

1. Informatie ophalen over de bestelling en de volgende stappen bepalen door de **[Status](#about-order-status)** kolom om informatie over de orden te krijgen.

## Bestelgegevens weergeven

Nadat een bestelling van de markt is ontvangen en in de Adobe Commerce of de Magento Open Source is geïmporteerd, gebruikt u de [!DNL Commerce] Order ID to view the order in Adobe Commerce.

Van **[!UICONTROL Orders]**, selecteert u de **[!UICONTROL Commerce Order Number]** om de [!DNL Commerce] orderdetails.

![Gedetailleerde weergave voor handelsorders voor een [!DNL Walmart Marketplace] bestellen](assets/order-detail-with-external-order-id.png)

In de winkel Commerce worden bestellingen geïmporteerd uit [!DNL Walmart Marketplace] de volgende aanvullende informatie in de ordergegevens hebben opgenomen:

- **Betalingsgegevens en verzendmethode**-Bestellingen die zijn geïmporteerd uit Walmart bevatten de volgende waarden voor betalings- en verzendvelden:

   - **[!UICONTROL Offline Channel Payment]**—Geeft aan dat de betaling van een bestelling offline wordt verwerkt door [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]**—Geeft de [!DNL Walmart Marketplace] ordernummer.

   - **[!UICONTROL Channel Shipping - Value]**-Geeft aan dat verzendkosten worden verwerkt via [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]**-Dit veld wordt alleen weergegeven als een bestelling is geïmporteerd uit [!DNL Walmart Marketplace] is geannuleerd. Tot de annuleringsredenen behoren:

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

