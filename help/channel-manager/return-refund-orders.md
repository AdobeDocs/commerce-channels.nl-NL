---
title: Terugbetalings- en terugbetalingsopdrachten
description: Instructies voor de afgifte van volledige of gedeeltelijke terugbetalingen voor terugkeerverzoeken die zijn ontvangen van [!DNL Walmart Marketplace] van [!DNL Channel Manager] voor Adobe Commerce en Magento Open Source.
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: 151cce44d1107e351a1db012e89114cf95a977e7
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Terugbetalingsopdrachten

Wanneer een koper een retournering aanvraagt voor bestellingen die zijn gekocht via [!DNL Walmart Marketplace], Walmart leidt tot een terugkeerverzoek. [!DNL Channel Manager] controleert het marktplace kanaal voor deze verzoeken en synchroniseert automatisch de informatie van het terugkeerverzoek aan de Manager van het Kanaal.

Aan de kant van de Handel, stelt het terugkeerverzoek het volgende werkschema in werking:

1. De Manager van het kanaal leidt tot een overeenkomstig terugkeerverzoek met een ontvangen status en voegt het aantal van terugkeeridentiteitskaart toe ([!UICONTROL RMA #]) aan de [!UICONTROL Returns] dashboard. Op de [!DNL Orders] dashboard, de statusdetails voor de orde verbonden aan de terugkeerupdates om a te omvatten [!UICONTROL Return requested] koppeling gebruiken om de return weer te geven en te verwerken.

1. Handelaren verwerken de aan de return gekoppelde terugbetaling door een creditcard te maken na de [Adobe Commerce-workflow voor restitutie](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow). Alle restituties worden verwerkt gebruikend de off-line methode.

1. [!DNL Channel Manager] stuurt een terugbetalingsupdate naar Walmart Marketplace zodat de retourstatus kan worden bijgewerkt met de voltooide terugbetaling van Adobe Commerce.

In opslagbeheerder, kunt u terugkeren van de Manager van het Kanaal bekijken en verwerken door de opslag van het verkoopkanaal te openen en te selecteren **[!UICONTROL Returns]**.

![De Manager van het kanaal keert dashboard terug om terugbetalingen te verwerken die van terugkeerverzoeken worden ontvangen van [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png)

>[!NOTE]
>
>U kunt alleen terugbetalingen voor verzonden bestellingen verwerken. In [!DNL Channel Manager]moet de status van de order [!UICONTROL Shipped]. In [!DNL Walmart Marketplace] Verkopersaccount, de bestelling moet [!UICONTROL Delivered].

## Retourneert besturingselementen en kolombeschrijvingen

In de volgende tabellen worden de besturingselementen en kolommen beschreven die beschikbaar zijn voor [!DNL Channel Manager] retourneert.

**Besturingselementen voor[!UICONTROL Returns]**

<table>
<tr>
<td><strong>Control</strong></td>
<td><strong>Beschrijving</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filter de weergave door een van de opties te selecteren [!UICONTROL Return Status] kaarten.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Voor retouritems met de [!UICONTROL Received] of [!UICONTROL Refunded] Als u de status hebt, kunt u de creditnota voor de terugbetaling maken of bekijken door de gekoppelde tekst te selecteren in de kolom Status Details.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Selecteer de optie [!DNL Commerce] ordernummer in het [!UICONTROL Order] tabel om de handelsorder te openen.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Om de kanaalconfiguratie te wijzigen, selecteer de geloofsbrieven van de Verbinding van het kanaal de Slimme, in kaart gebrachte attributen, of verschepende herkenningstekens, montages selecteren [!DNL Commerce] ordernummer in het [!UICONTROL Order] tabel. Gebruik vervolgens [!DNL Commerce] bestellen opties om de bestelling te verwerken.</td>
</tr>
</table>

**Kolombeschrijvingen**

<table>
<tr>
<td><strong>Veld</strong></td>
<td><strong>Beschrijving</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>Het nummer van de vergunning van de Terugkeer Merchandise verbonden aan het terugkeerverzoek dat van wordt ontvangen [!DNL Walmart Marketplace]. Dit nummer wordt gegenereerd door Walmart Marketplace [!UICONTROL Returns] wanneer het terugkeerproces in werking wordt gesteld.</td>
</tr>
<tr>
<td>[!DNL Commerce] Volgnummer</td>
<td>De [!DNL Commerce] ordernummer dat is gekoppeld aan de items die zijn opgenomen in het retourverzoek van Walmart Marketplace. U kunt de bestelgegevens weergeven door het ordernummer te selecteren.</td>
</tr>
<tr>
<td>Gevraagd</td>
<td>De datum waarop de terugkeer is aangevraagd op de [!DNL Walmart Marketplace]
omgezet in lokale tijd.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>De datum waarop de terugkeer door moet worden terugbetaald om te ontmoeten [!DNL Walmart Marketplace] [vereisten](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f) omgezet in lokale tijd.</td>
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
<td>Geeft de huidige retourstatus in het dialoogvenster [!DNL Commerce] geretourneerde werkstroom-<i>Ontvangen</i>, <i>Geretourneerd</i>, of <i>Fout</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Voor ontvangen en terugbetaalde retourzendingen bevatten de statusgegevens een koppeling naar de creditnota voor terugbetalingsverwerking. Als er een fout optreedt tijdens de [!DNL Channel Manager] synchronisatieproces tussen Adobe Commerce en [!DNL Walmart marketplace]bevat dit veld de beschrijving van de fout.</td>
</tr>
</table>

## Retourstatus

[!UICONTROL Return Status] bevat informatie over de huidige status van [!DNL Walmart Marketplace] retourverzoeken beheerd vanuit Adobe Commerce of Magento Open Source.

De statusupdates van de terugkeer komen voor wanneer [!DNL Channel Manager] ontvangt een terugkeerverzoek van [!DNL Walmart Marketplace] of wanneer de [!DNL Commerce] creditnota is gemaakt om de terugbetaling voor de geretourneerde objecten te verwerken.

Retourneert kan de volgende statussen hebben:

* **[!UICONTROL Received]**- Dit is de initiële status van het terugkeerverzoek dat van wordt ontvangen [!DNL Walmart Marketplace] opslaan. De handelaar kan de restitutie voor de teruggave verwerken door **[!UICONTROL Create credit memo]** in de [!UICONTROL Status details].

* **[!UICONTROL Refunded]**—Geeft aan dat er een creditmemo is gemaakt om de geretourneerde objecten te restitueren. Handelaren kunnen terugbetalingsgegevens bekijken door **[!UICONTROL View credit memo]** in de [!UICONTROL Status details].

* **[!UICONTROL Error]**—Terugkeer verzoeken die fouten hebben. De fouten kunnen voorkomen wanneer het terugkeerverzoek van Walmart ontbrekende of onjuiste gegevens heeft. Of, als [!DNL Channel Manager] kan de update-kennisgeving voor restitutie niet naar Walmart verzenden.

## Terugkerende scenario&#39;s

De volgende scenario&#39;s beschrijven hoe te om terugbetalingen voor verschillende types terugkeerverzoeken van uit te geven [!DNL Channel Manager].

* **Volledige terugkeer**—Als het retourverzoek van de Walmart Marketplace betrekking heeft op alle objecten in de bestelling, werkt u het aantal creditnota bij om alle objecten terug te betalen.

* **Gedeeltelijke terugkeer**- Als het retourverzoek van de Walmart Marketplace slechts voor bepaalde bestellingen geldt, werkt u het aantal creditnota&#39;s alleen bij voor de objecten die moeten worden terugbetaald.

* **Retourneren is al terugbetaald via Walmart Marketplace**- In sommige gevallen wordt een restitutie verwerkt op [!DNL Walmart Marketplace] voordat u de return verwerkt in Channel Manager. Bijvoorbeeld, als een orde van de Handel niet binnen het 48-uurs die venster wordt teruggegeven van de terugbetalingsverwerking door Walmart wordt vereist, terugkeert de Marm automatisch de orde. Als dit gebeurt, synchroniseert Channel Manager de aanvraag voor terugsturen naar Adobe Commerce nog steeds, zodat u de terugzending kunt verwerken en de creditnota kunt uitgeven. Deze workflow zorgt ervoor dat de ordergegevens in [!DNL Commerce] komt overeen met de ordergegevens in Walmart Marketplace.

>[!NOTE]
>
> Het kan maximaal vijf minuten duren voordat updates voor restitutie worden gesynchroniseerd met [!DNL Walmart Marketplace]. U kunt de huidige status van de geretourneerde waarde controleren via het menu [!DNL Channel Manager] [!UICONTROL Returns] dashboard.

## Een terugbetalingsverzoek verwerken

1. Open de [!UICONTROL Returns] dashboard voor de winkel van uw verkoopkanaal.

   * Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

   * U kunt de geretourneerde waarden bekijken door de **[!UICONTROL Returns]** tab.

      U hebt ook toegang tot de geretourneerde gegevens van het dialoogvenster [!UICONTROL Orders] pagina. Zoeken naar [!UICONTROL Shipped] orders die een retourverzoek hebben. Selecteer vervolgens de `Return requested` in de [!UICONTROL Status Details] om de aanvraag te bekijken en te verwerken.

1. Zoek in de tabel Returns een return met de opdracht *[!UICONTROL Received]* status.

1. Controleer in de kolom Objecten de lijst met orderobjecten en de hoeveelheid die u wilt terugbetalen.

1. Verwerk de terugbetaling door een creditnota te verstrekken.

   * Van de [!UICONTROL Status Details] kolom, selecteren **[!UICONTROL Create credit memo]** om de pagina met gegevens over de volgorde te openen in [!DNL Commerce].

      Als de volgorde niet is gefactureerd, wordt op de pagina Bestelling-details een foutbericht weergegeven waarin u wordt gevraagd een bestelling te maken. Selecteren **[!UICONTROL Create invoice]**. Vervolgens [de factuur maken en opslaan](https://docs.magento.com/user-guide/sales/invoices.html).

   * Selecteer op de pagina Order detail **[!UICONTROL Credit Memo]**.

   * In [!UICONTROL Items to Refund] van de [!UICONTROL Credit Memo], werkt u de **[!UICONTROL Qty to refund]** en **[!UICONTROL Return to Stock]** informatie over de items die in het retourverzoek zijn opgenomen.

      Zorg ervoor dat alleen de items worden geretourneerd die in het retourverzoek worden vermeld.

   * Als u een opmerking wilt toevoegen, voert u de tekst in het dialoogvenster **[!UICONTROL Credit Memo Comments]**

   * Selecteren **[!UICONTROL Refund Offline]**.

Na het voltooien van de restitutie, [!DNL Channel Manager] werkt de terugkeerstatus in bij [!UICONTROL Returns] dashboard naar [!UICONTROL Refunded] en synchroniseert de update naar Walmart om de terugkeerstatus op Marketplace bij te werken.


## Terugbetalingsgegevens voor een retourzending bekijken

U kunt informatie over retourverzoeken en terugbetalingsverwerking bekijken via het [!UICONTROL Returns] dashboard.

1. Open het dashboard van Terugkeren voor uw opslag van het verkoopkanaal.

   * Selecteer bij Beheer de optie **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Open de winkelweergave door het oogpictogram voor een winkel met verkoopkanalen te selecteren.

   * Selecteren **[!UICONTROL Returns]**.

1. Terugbetaalde bestellingen weergeven door de optie **[!UICONTROL Refunded]** statuskaart.

1. Terugbetalingsgegevens voor een retourzending bekijken door op **[!UICONTROL View credit memo]**.

   ![Creditnota voor terugbetaalde objecten voor een [!DNL Walmart Marketplace] bestellen](assets/refund-credit-memo-for-marketplace-order.png)

>[!NOTE]
>
>Nadat een bestelling is terugbetaald, [!UICONTROL Orders] op het dashboard worden geen retourgegevens weergegeven. Als u de retourinformatie wilt weergeven, gebruikt u de [!DNL Channel Manager] Retourneert het dashboard. Meer gedetailleerde informatie over retourneren en terugbetalen is ook beschikbaar op de pagina met gegevens over bestellingen.

## Retourfouten herstellen

Er kunnen fouten optreden wanneer de retourinformatie wordt ontvangen van [!DNL Walmart Marketplace]of wanneer [!DNL Channel Manager] synchroniseert statusupdates van [!DNL Commerce] tot [!DNL Walmart Marketplace].

Als de synchronisatiebewerking voor een retourupdate mislukt, wordt [!DNL Channel Manager] Geeft dashboard een *[!UICONTROL Error]* status voor de terugkeeringang. Om ervoor te zorgen dat de terugkeer en terugbetalingsinformatie correct in de rekening van de Marketplace van de Markeren wordt weerspiegeld, werk manueel de orde in uw [!DNL Walmart Marketplace] opslaan.
