---
title: Terugbetalings- en terugbetalingsopdrachten
description: Instructies voor het uitgeven van volledige of gedeeltelijke terugbetalingen voor terugkeerverzoeken die van  [!DNL Walmart Marketplace]  van  [!DNL Channel Manager]  voor Adobe Commerce en Magento Open Source worden ontvangen.
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# Terugbetalings- en terugbetalingsopdrachten

Wanneer een koper om een rendement voor bestellingen vraagt die via [!DNL Walmart Marketplace] zijn aangeschaft, maakt Walmart een aanvraag voor een retournering. [!DNL Channel Manager] bewaakt het marketingkanaal voor deze aanvragen en synchroniseert automatisch de informatie van de geretourneerde aanvraag naar Channel Manager.

Aan de Commerce-zijde wordt met de geretourneerde aanvraag de volgende workflow gestart:

1. De Manager van het kanaal leidt tot een overeenkomstig terugkeerverzoek met een ontvangen status en voegt het aantal van terugkeer identiteitskaart ([!UICONTROL RMA #]) aan het [!UICONTROL Returns] dashboard toe. Op het [!DNL Orders] dashboard worden de statusgegevens voor de volgorde die aan het retourneren is gekoppeld, bijgewerkt met een [!UICONTROL Return requested] -koppeling om het retourneren weer te geven en te verwerken.

1. De handelaren verwerken de terugbetaling verbonden aan de terugkeer door een Memo van het Krediet na het [ terugbetalingswerkschema van Adobe Commerce ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html) te creëren. Alle restituties worden verwerkt gebruikend de off-line methode.

1. [!DNL Channel Manager] verzendt een terugbetalingsupdate naar Walmart Marketplace zodat de retourstatus kan worden bijgewerkt met de voltooide restitutie van Adobe Commerce.

In de opslagbeheerder, kunt u terugkeer van de Manager van het Kanaal bekijken en verwerken door de opslag van het verkoopkanaal te openen en **[!UICONTROL Returns]** te selecteren.

![ de Manager van het Kanaal keert dashboard terug om terugbetalingen voor terugkeerverzoeken te verwerken die van [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"} worden ontvangen

>[!NOTE]
>
>U kunt alleen terugbetalingen voor verzonden bestellingen verwerken. In [!DNL Channel Manager] moet de orderstatus [!UICONTROL Shipped] zijn. In [!DNL Walmart Marketplace] Verkopersaccount moet de volgorde [!UICONTROL Delivered] zijn.

## Retourneert besturingselementen en kolombeschrijvingen

In de volgende tabellen worden de besturingselementen en kolommen beschreven die beschikbaar zijn voor [!DNL Channel Manager] retourneert.

**Controles voor[!UICONTROL Returns]**

<table>
<tr>
<td><strong>Besturing</strong></td>
<td><strong>Beschrijving</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filter de weergave door een van de [!UICONTROL Return Status] -kaarten te selecteren.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Voor geretourneerde items met de status [!UICONTROL Received] of [!UICONTROL Refunded] kunt u een creditnota voor de restitutie maken of bekijken door de gekoppelde tekst te selecteren in de kolom Statusdetails.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Als u de volgordedetails wilt weergeven, selecteert u het [!DNL Commerce] volgordenummer in de tabel [!UICONTROL Order] om de Commerce-volgorde te openen.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Als u de kanaalconfiguratie wilt wijzigen, selecteert u de referenties van de kanaalverbinding, de toegewezen kenmerken of de verzendingsidentificatoren en selecteert u het [!DNL Commerce] volgordenummer in de [!UICONTROL Order] -tabel. Gebruik vervolgens de orderopties van [!DNL Commerce] om de volgorde te verwerken.</td>
</tr>
</table>

**de beschrijvingen van de Kolom**

<table>
<tr>
<td><strong>Veld</strong></td>
<td><strong>Beschrijving</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>The Return Merchandise Authorization number associated with the return request received from [!DNL Walmart Marketplace]. Dit nummer wordt gegenereerd door Walmart Marketplace [!UICONTROL Returns] wanneer het retourproces wordt gestart.</td>
</tr>
<tr>
<td>[!DNL Commerce] Volgnummer</td>
<td>Het [!DNL Commerce] ordernummer dat is gekoppeld aan de items die zijn opgenomen in het retourverzoek van Walmart Marketplace. U kunt de bestelgegevens weergeven door het ordernummer te selecteren.</td>
</tr>
<tr>
<td>Gevraagd</td>
<td>De datum waarop de return is aangevraagd op de [!DNL Walmart Marketplace]
omgezet in lokale tijd.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>De datum waarop de return moet worden terugbetaald om te voldoen aan [!DNL Walmart Marketplace] [requirements](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f) omgezet in lokale tijd.</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>Hiermee geeft u de SKU en het aantal weer voor elk item dat in de return wordt vermeld.</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>De totale waarde die moet worden terugbetaald voor de geretourneerde items.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Wijst op de huidige terugkeerstatus in het [!DNL Commerce] terugkeerwerkschema- <i> Ontvangen </i>, <i> teruggegeven </i>, of <i> Fout </i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Voor ontvangen en terugbetaalde retourzendingen bevatten de statusgegevens een koppeling naar de creditnota voor terugbetalingsverwerking. Als er een fout optreedt tijdens het [!DNL Channel Manager] -synchronisatieproces tussen Adobe Commerce en [!DNL Walmart marketplace] , wordt in dit veld de foutbeschrijving weergegeven.</td>
</tr>
</table>

## Retourstatus

[!UICONTROL Return Status] biedt informatie over de huidige status van [!DNL Walmart Marketplace] retourverzoeken die worden beheerd vanuit Adobe Commerce of Magento Open Source.

De status van de geretourneerde waarde wordt bijgewerkt wanneer [!DNL Channel Manager] een aanvraag van [!DNL Walmart Marketplace] ontvangt of wanneer het creditmemo van [!DNL Commerce] wordt gemaakt om de terugbetaling van de geretourneerde items te verwerken.

Retourneert kan de volgende statussen hebben:

* **[!UICONTROL Received]** - Dit is de initiële status van de geretourneerde aanvraag die is ontvangen van de [!DNL Walmart Marketplace] store. De handelaar kan de terugbetaling voor de terugkeer verwerken door **[!UICONTROL Create credit memo]** in [!UICONTROL Status details] te selecteren.

* **[!UICONTROL Refunded]** - Geeft aan dat er een creditmemo is gemaakt om de geretourneerde items te restitueren. Handelaars kunnen terugbetalingsgegevens bekijken door **[!UICONTROL View credit memo]** te selecteren in [!UICONTROL Status details] .

* **[!UICONTROL Error]** - Terugkeer verzoeken die fouten hebben. De fouten kunnen voorkomen wanneer het terugkeerverzoek van Walmart ontbrekende of onjuiste gegevens heeft. Of als [!DNL Channel Manager] de update-melding voor restitutie niet naar Walmart kan verzenden.

## Terugkerende scenario&#39;s

De volgende scenario&#39;s beschrijven hoe te om terugbetalingen voor verschillende types van terugkeerverzoeken van [!DNL Channel Manager] uit te geven.

* **Volledige terugkeer** - als het de terugkeerverzoek van de Markt van de Markt van de Walmart voor alle punten in de orde is, werk het aantal van het creditmemo bij om alle punten terug te keren.

* **Gedeeltelijke terugkeer** - als het de terugkeerverzoek van de Marketplace van de Markeren van de Markt van de Markt slechts voor sommige orde punten is, werk de hoeveelheid van het creditmemo slechts voor de punten bij die moeten worden terugbetaald.

* **Terugkeer reeds teruggegeven door Marketplace van het Spoor** - in sommige gevallen, wordt een terugbetaling verwerkt op [!DNL Walmart Marketplace] alvorens u de terugkeer in de Manager van het Kanaal verwerkt. Bijvoorbeeld, als een orde van Commerce niet binnen het 48-uurs die venster wordt teruggegeven van de terugbetalingsverwerking door Walmart wordt vereist, terugkeert de Marm automatisch de orde. Als dit gebeurt, synchroniseert Channel Manager de aanvraag voor terugsturen naar Adobe Commerce nog steeds, zodat u de terugzending kunt verwerken en de creditnota kunt uitgeven. Deze workflow zorgt ervoor dat de ordergegevens in [!DNL Commerce] overeenkomen met de ordergegevens in Walmart Marketplace.

>[!NOTE]
>
> Het kan maximaal vijf minuten duren voordat updates voor restitutie worden gesynchroniseerd met [!DNL Walmart Marketplace] . U kunt de huidige retourstatus controleren via het dashboard [!DNL Channel Manager] [!UICONTROL Returns] .

## Een terugbetalingsverzoek verwerken

1. Open het dashboard van [!UICONTROL Returns] voor uw winkel van verkoopkanalen.

   * Selecteer in het menu Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** .

   * Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

   * U kunt de geretourneerde waarden bekijken door de tab **[!UICONTROL Returns]** te selecteren.

     U hebt ook toegang tot retourinformatie vanaf de pagina [!UICONTROL Orders] . Zoek naar [!UICONTROL Shipped] orders die een terugkeerverzoek hebben. Selecteer vervolgens de koppeling `Return requested` in de kolom [!UICONTROL Status Details] om de aanvraag weer te geven en te verwerken.

1. Zoek in de tabel Returns een return met de status *[!UICONTROL Received]* .

1. Controleer in de kolom Objecten de lijst met orderobjecten en de hoeveelheid die u wilt terugbetalen.

1. Verwerk de terugbetaling door een creditnota te verstrekken.

   * Selecteer in de kolom [!UICONTROL Status Details] de optie **[!UICONTROL Create credit memo]** om de pagina Order detail in [!DNL Commerce] te openen.

     Als de volgorde niet is gefactureerd, wordt op de pagina Bestelling-details een foutbericht weergegeven waarin u wordt gevraagd een bestelling te maken. Selecteer **[!UICONTROL Create invoice]** . Dan, [ creeer en bewaar de factuur ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html).

   * Selecteer **[!UICONTROL Credit Memo]** op de pagina Order detail.

   * Werk in de sectie [!UICONTROL Items to Refund] van [!UICONTROL Credit Memo] de informatie **[!UICONTROL Qty to refund]** en **[!UICONTROL Return to Stock]** bij voor de items die in de geretourneerde aanvraag zijn opgenomen.

     Zorg ervoor dat alleen de items worden geretourneerd die in het retourverzoek worden vermeld.

   * Als u een opmerking wilt toevoegen, voert u de tekst in de **[!UICONTROL Credit Memo Comments]**

   * Selecteer **[!UICONTROL Refund Offline]** .

Nadat de restitutie is voltooid, werkt [!DNL Channel Manager] de retourstatus in het [!UICONTROL Returns] dashboard bij naar [!UICONTROL Refunded] en wordt de update gesynchroniseerd naar Walmart om de retourstatus op de markt bij te werken.


## Terugbetalingsgegevens voor een retourzending bekijken

U kunt informatie over geretourneerde aanvragen en terugbetalingsverwerking bekijken vanaf het dashboard van [!UICONTROL Returns] .

1. Open het dashboard van Keert voor uw opslag van het verkoopkanaal terug.

   * Selecteer in het menu Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** .

   * Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

   * Selecteer **[!UICONTROL Returns]** .

1. Terugbetaalde bestellingen weergeven door de **[!UICONTROL Refunded]** -statuskaart te selecteren.

1. Selecteer **[!UICONTROL View credit memo]** als je terugbetalingsgegevens voor een retourzending wilt bekijken.

   ![ memo van het krediet om teruggekeerde punten voor a [!DNL Walmart Marketplace] orde ](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"} terug te keren

>[!NOTE]
>
>Nadat een bestelling is terugbetaald, bevat het dashboard van [!UICONTROL Orders] geen informatie over de geretourneerde waarde. Gebruik het dashboard [!DNL Channel Manager] Returns om informatie over de geretourneerde waarde weer te geven. Meer gedetailleerde informatie over retourneren en terugbetalen is ook beschikbaar op de pagina met gegevens over bestellingen.

## Retourfouten verhelpen

Er kunnen fouten optreden wanneer de retourinformatie wordt ontvangen van [!DNL Walmart Marketplace] of wanneer [!DNL Channel Manager] statusupdates synchroniseert van [!DNL Commerce] naar [!DNL Walmart Marketplace] .

Als de synchronisatiebewerking voor een retourupdate mislukt, wordt op het dashboard [!DNL Channel Manager] een *[!UICONTROL Error]* -status voor de geretourneerde invoer weergegeven. Werk de bestelling handmatig bij in uw [!DNL Walmart Marketplace] winkel om ervoor te zorgen dat de informatie over retournering en terugbetaling correct wordt weergegeven in het Walmart Marketplace-account.
