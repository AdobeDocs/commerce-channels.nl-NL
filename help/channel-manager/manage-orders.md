---
title: 'Bestellingen weergeven en beheren vanuit  [!DNL Channel Manager]'
description: De "mening en beheert  [!DNL Walmart Marketplace]  orden met  [!DNL Channel Manager]  voor Adobe Commerce en Magento Open Source."
feature: Sales Channels, Orders
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

# Bestellingen weergeven en bijhouden vanuit [!DNL Channel Manager]

[!DNL Walmart Marketplace] volgordegegevens voor [!DNL Commerce] -producten worden automatisch gesynchroniseerd met [!DNL Channel Manager] nadat [!DNL Walmart] de volgorde heeft verwerkt.

Aan de zijde van [!DNL Commerce] activeert een geslaagde synchronisatie de volgende acties:

- [!DNL Channel Manager] verzendt een ordererkenning naar Walmart.

- Er wordt een overeenkomende [!DNL Commerce] -volgorde gemaakt op basis van de Walmart-volgorde.

- De bijgewerkte ordegegevens worden weergegeven op het dashboard voor bestellingen van [!DNL Channel Manager] .

In de opslagbeheerder kunt u ordergegevens weergeven vanuit [!DNL Channel Manager] door de winkel met verkoopkanalen te openen en **[!UICONTROL Orders]** te selecteren.

![ de mening van de Orden van de Manager van het Kanaal om [!DNL Walmart Marketplace] orden ](assets/orders-dashboard-view.png){width="600" zoomable="yes"} te beheren

>[!NOTE]
>
>Het kan tot 35 minuten duren voordat een [!DNL Walmart Marketplace] -volgorde wordt weergegeven in de orderlijst van [!DNL Channel Manager] . [!DNL Walmart] vereist ongeveer 30 minuten om binnenkomende orders te verwerken en naar [!DNL Channel Manager] te verzenden. Nadat Channel Manager de bestelling heeft ontvangen, duurt het nog ongeveer vijf minuten om de bestelling te maken en weer te geven in Adobe Commerce of Magento Open Source.

## Besturingselementen voor bestellingen en kolombeschrijvingen

De volgende lijsten beschrijven de controles en de kolommen beschikbaar voor Orden.

**Controles voor[!UICONTROL Orders]**

<table>
<tr>
<td><strong>Besturing</strong></td>
<td><strong>Beschrijving</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>U kunt de weergave sorteren door een van de [!UICONTROL Order Status] -kaarten te selecteren.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Verstrekt informatie over ordefouten en terugkeerverzoeken. Als u de retourinformatie en de terugbetalingsstatus voor een bestelling wilt weergeven, selecteert u de <strong>[!UICONTROL Return requested]</strong> -tekst die u wilt openen in het [!UICONTROL Returns] -dashboard.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Als u de volgordedetails wilt weergeven, selecteert u het [!DNL Commerce] volgordenummer in de tabel [!UICONTROL Order] . Gebruik vervolgens de orderopties van [!DNL Commerce] om de volgorde te verwerken.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Als u de kanaalconfiguratie wilt wijzigen, selecteert u de referenties van de kanaalverbinding, de toegewezen kenmerken of de verzendingsidentificatoren en selecteert u het [!DNL Commerce] volgordenummer in de [!UICONTROL Order] -tabel. Gebruik vervolgens de orderopties van [!DNL Commerce] om de volgorde te verwerken.</td>
</tr>
</table>


**de beschrijvingen van de Kolom**

<table>
<tr>
<td>Veld</td>
<td>Beschrijving</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>Het inkoopordernummer dat aan de order in de [!DNL Walmart Marketplace] is toegewezen. Wanneer een volgorde voor het eerst wordt geïmporteerd in [!DNL Channel Manager] , wordt alleen het ordernummer [!DNL Walmart] weergegeven. Wanneer de [!DNL Commerce] -volgorde wordt gemaakt, wordt het [!DNL Walmart] -ordernummer opgeslagen in het [!UICONTROL External ID] -productkenmerk.</td>
</tr>
<tr>
<td>[!DNL Commerce] Volgnummer</td>
<td>Het nummer dat is toegewezen aan de [!DNL Commerce] -volgorde die is gemaakt op basis van de [!DNL Walmart Marketplace] -volgorde.</td>
</tr>
<tr>
<td>Items</td>
<td>Aantal items dat op [!DNL Walmart Marketplace] is geordend.</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>Totale kosten van de bestelde objecten.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>De datum waarop de order naar de [!DNL Walmart Marketplace] is geconverteerd naar de lokale tijdzone.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>De datum waarop de bestelling moet worden verzonden om te voldoen aan [!DNL Walmart Marketplace] -vereisten die zijn omgezet in de lokale tijdzone.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>De datum waarop de order aan de klant moet worden geleverd om te voldoen aan [!DNL Walmart Marketplace] -vereisten die zijn omgezet in de lokale tijdzone.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>De [[!DNL Walmart Marketplace] Verzendmethode] (https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29 geselecteerd voor de bestelling.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Tijdstempel die de laatste keer aangeeft dat de ordegegevens zijn bijgewerkt, wordt omgezet in [!DNL Channel Manager] naar lokale tijdzone.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Geeft de huidige orderstatus in de [!DNL Commerce] bestelworkflow aan. De beginstatus van een bestelling die wordt geïmporteerd uit [!DNL Walmart Marketplace] is _Open_. Er vinden extra statusupdates plaats wanneer [!DNL Commerce] -orders worden verwerkt en [!DNL Channel Manager] de verzending, gedeeltelijke verzending en annulering van updates naar [!DNL Walmart Marketplace] kan synchroniseren.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Verstrekt meer gedetailleerde informatie over orden met fouten of terugbetalingsverzoeken.</td>
</tr>
</table>

## Status van bestelling

[!UICONTROL Order Status] biedt informatie over de huidige status van [!DNL Walmart Marketplace] -orders die worden beheerd vanuit Adobe Commerce of Magento Open Source. De status van de bestelling wordt bijgewerkt wanneer [!DNL Channel Manager] bijgewerkte bestelgegevens ontvangt van het [!DNL Walmart Marketplace] - of [!DNL Commerce] -bestelsysteem. Orders kunnen de volgende statussen hebben:

- **[!UICONTROL Shipped]** - Bestellingen die zijn verzonden vanuit de [!DNL Commerce] store. Wanneer de bestelling wordt verzonden, verzendt [!DNL Channel Manager] een update naar [!DNL Walmart Marketplace] om de verzendstatus op Walmart bij te werken en het volgnummer van de bestelling voor de verzending op te geven. Nadat een orde is verscheept, kunnen de orde punten gedeeltelijk of volledig worden terugbetaald als het Martly een vorm van de Vergunning van de Goederen van de Terugkeer uitgeeft. Zie [ Keert terug en terugkeert ](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]** - Bestellingen waarvan sommige items zijn gemarkeerd als verzonden en andere wachten op verzending. Wanneer items in het orderschip door [!DNL Channel Manager] worden verzonden, wordt een update naar [!DNL Walmart Marketplace] verzonden om de verzendstatus bij te werken naar _[!DNL Partially Shipped]_on Walmart en het volgnummer voor de verzending te geven.

- **[!UICONTROL Canceled]** - Bestellingen die zijn geannuleerd in de [!DNL Commerce] store.

  Nadat de orderannulering is voltooid, wordt de voorraad van [!DNL Commerce] bijgewerkt om de geretourneerde items weer te geven. Vervolgens synchroniseert [!DNL Channel Manager] de update naar de map [!DNL Walmart Marketplace] .

- **[!UICONTROL Return requested]** - Als Walmart Marketplace om retournering vraagt voor orderitems die zijn verzonden, wordt een `Return requested` -koppeling weergegeven in de kolom [!UICONTROL Status details] . Als u de koppeling selecteert, wordt het dashboard van [!UICONTROL Returns] geopend en wordt de geretourneerde waarde weergegeven en wordt het terugbetalingsproces beheerd.

- **[!UICONTROL Error]** - Orders met fouten. Fouten kunnen optreden wanneer een bewerking voor het bijwerken van een bestelling mislukt. Er treden bijvoorbeeld fouten op als [!DNL Channel Manager] geen nieuwe bestelling van Walmart kan ontvangen. Ze kunnen zich ook voordoen als [!DNL Channel Manager] geen verzending van een bestelling of annulering naar de [!DNL Walmart Marketplace] kan verzenden. Als een verrichting ontbreekt, toont de pagina van Orden een _status van de Fout_ voor de orde. Voor details, zie [ de ordefouten van de Oplossing ] (proces-orders.md#fix-verscheepte-en-annulering-fouten).

- **[!UICONTROL Status details]** - Verstrekt meer informatie over ordefouten die toe te schrijven aan kwesties zoals ontbrekende informatie of ongeldige waarden, onjuiste verzenddetails, of een ontbroken ordevernietiging voorkomen. Aan de hand van de beschrijving kunt u bepalen of er een fout is opgetreden bij de [!DNL Commerce] -instantie of bij [!DNL Walmart Marketplace] .

>[!NOTE]
>
>Als orderitems in meerdere verzendingen worden verzonden, geeft de status van de bestelling in [!DNL Channel Manager] de status van de laatste bestelling weer. Als het eerste item bijvoorbeeld wordt verzonden en er geen fouten worden geretourneerd wanneer orderupdates worden gesynchroniseerd naar [!DNL Channel Manager] en [!DNL Walmart Marketplace] , is de status van de [!DNL Channel Manager] volgorde _[!UICONTROL Partially Shipped]_. Als een tweede item wordt verzonden en [!DNL Channel Manager] een fout retourneert, wordt de status van de bestelling bijgewerkt naar_[!UICONTROL Error]_ .

## Bestellingen controleren

1. Selecteer in de beheerdersruimte **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** om de pagina [!UICONTROL Channel Manager Marketplace Stores] te openen.

1. Open de archiefweergave door het oogpictogram in een rij met items in de winkel te selecteren.

1. Om ordeinformatie te bekijken, selecteer * [!UICONTROL *Orders] **.

1. Krijg informatie over de orde en bepaal volgende stappen door de **[kolom van de Status](#order-status)** te controleren.

## Bestelgegevens controleren

Nadat een bestelling van Marketplace is ontvangen en in uw winkel met verkoopkanalen is geïmporteerd, gebruikt u de bestelling-id [!DNL Commerce] om de ordergegevens in Adobe Commerce weer te geven.

Selecteer in **[!UICONTROL Orders]** de **[!UICONTROL Commerce Order Number]** om de [!DNL Commerce] -orderdetails te openen.

![ het detailmening van de Orde van Commerce voor a [!DNL Walmart Marketplace] orde ](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

In de Commerce-winkel bevatten bestellingen die zijn geïmporteerd uit [!DNL Walmart Marketplace] de volgende aanvullende informatie die in de ordergegevens is opgenomen:

- **de Informatie van de Betaling &amp; Verzendmethode** - Bestellingen die van Walmart worden ingevoerd omvatten volgende waarden voor betaling en verschepende gebieden:

   - **[!UICONTROL Offline Channel Payment]** - Geeft aan dat de bestelling offline wordt verwerkt door [!DNL Walmart Marketplace] .

   - **[!UICONTROL External Order Number]** - Geeft het [!DNL Walmart Marketplace] ordernummer weer.

   - **[!UICONTROL Channel Shipping - Value]** - Geeft aan dat verzendkosten worden verwerkt via [!DNL Walmart Marketplace] .

   - **[!UICONTROL Cancellation Reason]** - Dit veld wordt alleen weergegeven als een volgorde die is geïmporteerd uit [!DNL Walmart Marketplace] , wordt geannuleerd. De annuleringsredenen zijn onder meer:

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **Gangschikte Punten** - deze sectie maakt een lijst van de ordepunten op alle orden van Commerce. De kolom [!UICONTROL Qty] bevat de statusgeschiedenis voor orderitems. Als een bestelling bijvoorbeeld is gefactureerd, verzonden en terugbetaald, kunt u de statusovergangen zien.

  [!DNL Walmart Marketplace] orden ](assets/order-detail-status-history.png){width="600" zoomable="yes"} van de orde van het Detail bevolen puntenstatusgeschiedenis van de orde ![

U kunt de factuur van het object en de terugbetalingsgegevens weergeven door de opties [!UICONTROL Invoice] en [!UICONTROL Credit Memo] in het navigatiemenu te selecteren. U kunt het creditmemo ook rechtstreeks openen via het dashboard [[!UICONTROL Returns]](return-refund-orders.md) in uw winkel met verkoopkanalen.
