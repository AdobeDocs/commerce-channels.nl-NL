---
title: 'Bestellingen weergeven en beheren vanuit [!DNL Channel Manager]'
description: '''Weergeven en beheren [!DNL Walmart Marketplace] bestellingen met [!DNL Channel Manager] voor Adobe Commerce en Magento Open Source."'
feature: Sales Channels, Orders
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Bestellingen weergeven en bijhouden via [!DNL Channel Manager]

[!DNL Walmart Marketplace] ordergegevens voor [!DNL Commerce] producten worden automatisch gesynchroniseerd met [!DNL Channel Manager] na [!DNL Walmart] verwerkt de volgorde.

Op de [!DNL Commerce] Als de synchronisatie succesvol is, worden de volgende acties geactiveerd:

- [!DNL Channel Manager] verzendt een ordererkenning naar Walmart.

- A corresponderend [!DNL Commerce] order wordt gecreeerd van de orde van het Walmart.

- De bijgewerkte ordegegevens worden weergegeven op het tabblad [!DNL Channel Manager] Orders dashboard.

In de opslagbeheerder kunt u ordegegevens weergeven vanuit [!DNL Channel Manager] door de winkel met verkoopkanalen te openen en **[!UICONTROL Orders]**.

![Weergave voor bestellingen kanaalbeheer die moet worden beheerd [!DNL Walmart Marketplace] orders](assets/orders-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Het kan tot 35 minuten duren [!DNL Walmart Marketplace] in de [!DNL Channel Manager] orderlijst. [!DNL Walmart] vereist ongeveer 30 minuten om binnenkomende orders te verwerken en naar te sturen [!DNL Channel Manager]. Nadat Channel Manager de bestelling heeft ontvangen, duurt het nog ongeveer vijf minuten om de bestelling te maken en weer te geven in Adobe Commerce of Magento Open Source.

## Besturingselementen voor bestellingen en kolombeschrijvingen

De volgende lijsten beschrijven de controles en de kolommen beschikbaar voor Orden.

**Besturingselementen voor[!UICONTROL Orders]**

<table>
<tr>
<td><strong>Control</strong></td>
<td><strong>Beschrijving</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>De weergave sorteren door een van de [!UICONTROL Order Status] kaarten.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Verstrekt informatie over ordefouten en terugkeerverzoeken. Als u de retourgegevens en de terugbetalingsstatus van een bestelling wilt bekijken, selecteert u de optie <strong>[!UICONTROL Return requested]</strong> tekst om de [!UICONTROL Returns] dashboard.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Selecteer de optie [!DNL Commerce] ordernummer in het [!UICONTROL Order] tabel. Gebruik vervolgens [!DNL Commerce] bestellen opties om de bestelling te verwerken.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Om de kanaalconfiguratie te wijzigen, selecteer de geloofsbrieven van de Verbinding van het kanaal de Slimme, in kaart gebrachte attributen, of verschepende herkenningstekens, montages selecteren [!DNL Commerce] ordernummer in het [!UICONTROL Order] tabel. Gebruik vervolgens [!DNL Commerce] bestellen opties om de bestelling te verwerken.</td>
</tr>
</table>


**Kolombeschrijvingen**

<table>
<tr>
<td>Veld</td>
<td>Beschrijving</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>Het inkoopordernummer dat aan de order in het [!DNL Walmart Marketplace]. Wanneer een bestelling voor het eerst wordt geïmporteerd in [!DNL Channel Manager], alleen de [!DNL Walmart] het aantal van de orde toont. Wanneer de [!DNL Commerce] order wordt gemaakt, de [!DNL Walmart] ordernummer wordt opgeslagen in het dialoogvenster [!UICONTROL External ID] productkenmerk.</td>
</tr>
<tr>
<td>[!DNL Commerce] Volgnummer</td>
<td>Het nummer dat aan de [!DNL Commerce] bestelling gemaakt op basis van de [!DNL Walmart Marketplace] bestelling.</td>
</tr>
<tr>
<td>Items</td>
<td>Aantal bestelde objecten op [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>Totale kosten van de bestelde objecten.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>De datum waarop de order bij de [!DNL Walmart Marketplace] omgezet in de lokale tijdzone.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>De datum waarop de bestelling moet worden verzonden door om te voldoen aan [!DNL Walmart Marketplace] vereisten omgezet in de lokale tijdzone.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>De datum waarop de bestelling aan de klant moet worden geleverd om te voldoen [!DNL Walmart Marketplace] vereisten omgezet in de lokale tijdzone.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>De [[!DNL Walmart Marketplace] Verzendmethode](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29 geselecteerd voor de bestelling.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Tijdstempel die aangeeft wanneer de bestelgegevens het laatst zijn bijgewerkt [!DNL Channel Manager] omgezet in lokale tijdzone.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Geeft de huidige orderstatus in het dialoogvenster [!DNL Commerce] bestelworkflow. De beginstatus van een bestelling die is geïmporteerd uit [!DNL Walmart Marketplace] is _Open_. Aanvullende statusupdates vinden plaats wanneer [!DNL Commerce] bestellingen worden verwerkt en [!DNL Channel Manager] synchroniseert de updates voor verzending, gedeeltelijke verzending en annulering met de [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Verstrekt meer gedetailleerde informatie over orden met fouten of terugbetalingsverzoeken.</td>
</tr>
</table>

## Status van bestelling

[!UICONTROL Order Status] bevat informatie over de huidige status van [!DNL Walmart Marketplace] bestellingen beheerd vanuit Adobe Commerce of Magento Open Source. De statusupdates van de orde komen voor wanneer [!DNL Channel Manager] ontvangt bijgewerkte orderinformatie van of [!DNL Walmart Marketplace] of de [!DNL Commerce] bestelsysteem. Orders kunnen de volgende statussen hebben:

- **[!UICONTROL Shipped]**—Bestellingen die zijn verzonden vanuit de [!DNL Commerce] opslaan. Wanneer de order wordt verscheept, [!DNL Channel Manager] verzendt een update naar [!DNL Walmart Marketplace] om de verzendstatus op Walmart bij te werken en het volgnummer voor de verzending te geven. Nadat een orde is verscheept, kunnen de orde punten gedeeltelijk of volledig worden terugbetaald als het Martly een vorm van de Vergunning van de Goederen van de Terugkeer uitgeeft. Zie [Retourneert en terugbetaalt](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]**—Bestellingen waarvan sommige objecten zijn gemarkeerd als verzonden en andere nog moeten worden verzonden. Wanneer items in de order worden verzonden [!DNL Channel Manager] verzendt een update naar [!DNL Walmart Marketplace] om de verzendstatus bij te werken naar _[!DNL Partially Shipped]_op Walmart en geef het volgnummer van de bestelling voor de zending op.

- **[!UICONTROL Canceled]**—Bestellingen die zijn geannuleerd van de [!DNL Commerce] opslaan.

  Nadat de orderannulering is voltooid, worden de [!DNL Commerce] voorraadhoeveelheid wordt bijgewerkt om geretourneerde objecten weer te geven. Vervolgens [!DNL Channel Manager] synchroniseert de update naar de [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]**—Als Walmart Marketplace om een rendement voor bestellingen vraagt die zijn verzonden, `Return requested` de verbindingsvertoningen in [!UICONTROL Status details] kolom. Als u de koppeling selecteert, wordt het dialoogvenster [!UICONTROL Returns] dashboard om de teruggave te bekijken en het terugbetalingsproces te beheren.

- **[!UICONTROL Error]**—Orders met fouten. Fouten kunnen optreden wanneer een bewerking voor het bijwerken van een bestelling mislukt. Er treden bijvoorbeeld fouten op als [!DNL Channel Manager] kan geen nieuwe bestelling van Walmart ontvangen. Ze kunnen ook voorkomen als [!DNL Channel Manager] kan geen update voor verzending of annulering van een bestelling verzenden naar de [!DNL Walmart Marketplace]. Als een bewerking mislukt, wordt op de pagina Bestellingen een _Fout_ status van de bestelling. Zie voor meer informatie [Orderfouten herstellen](process-orders.md#fix-Shipping-and-cancelation- errors).

- **[!UICONTROL Status details]**- Verstrekt meer informatie over ordefouten die toe te schrijven aan kwesties zoals ontbrekende informatie of ongeldige waarden, onjuiste verzenddetails, of een ontbroken orde annuleren voorkomen. Aan de hand van de beschrijving kunt u bepalen of er een fout is opgetreden in het dialoogvenster [!DNL Commerce] of op de [!DNL Walmart Marketplace].

>[!NOTE]
>
>Als orderitems in meerdere verzendingen worden verzonden, wordt de orderstatus in [!DNL Channel Manager] geeft de laatst beschikbare orderstatus weer. Als het eerste item bijvoorbeeld wordt verzonden en er geen fouten worden geretourneerd wanneer orderupdates worden gesynchroniseerd naar [!DNL Channel Manager] en [!DNL Walmart Marketplace]de [!DNL Channel Manager] orderstatus is _[!UICONTROL Partially Shipped]_. Als een tweede object wordt verzonden en [!DNL Channel Manager] retourneert een fout. De status van de bestelling wordt bijgewerkt naar_[!UICONTROL Error]_.

## Bestellingen controleren

1. Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** om de [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Open de archiefweergave door het oogpictogram in een rij met items in de winkel te selecteren.

1. Selecteer * om de ordergegevens weer te geven[!UICONTROL *Orders]**.

1. Informatie ophalen over de bestelling en de volgende stappen bepalen door de **[Status](#order-status)** kolom.

## Bestelgegevens controleren

Nadat een bestelling van de markt is ontvangen en in uw verkoopkanaalwinkel is geïmporteerd, kunt u de [!DNL Commerce] Order ID to view the order detail in Adobe Commerce.

Van **[!UICONTROL Orders]**, selecteert u de **[!UICONTROL Commerce Order Number]** om de [!DNL Commerce] orderdetails.

![Gedetailleerde weergave voor handelsorders voor een [!DNL Walmart Marketplace] bestellen](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

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

- **Geordende objecten**—Deze sectie maakt een lijst van de ordepunten op alle orden van de Handel. De [!UICONTROL Qty] bevat de statushistorie voor orderitems. Als een bestelling bijvoorbeeld is gefactureerd, verzonden en terugbetaald, kunt u de statusovergangen zien.

  ![Status historie van geordende items voor ordergegevens [!DNL Walmart Marketplace] orders](assets/order-detail-status-history.png){width="600" zoomable="yes"}

Je kunt de gegevens van de objectfactuur en de restitutie bekijken door de [!UICONTROL Invoice] en [!UICONTROL Credit Memo] in het navigatiemenu. U kunt het creditmemo ook rechtstreeks openen vanuit de [[!UICONTROL Returns]](return-refund-orders.md) dashboard in uw verkoopkanaalwinkel.
