---
title: Aanbiedingen beheren
description: De lijsten van het "verkoopkanaal voor a [!DNL Commerce]  opslag met de Manager van het Kanaal voor Adobe Commerce en Magento Open Source."beheren
feature: Sales Channels, Merchandising, Products
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Aanbiedingen beheren

Productaanbiedingen voor het verkoopkanaal van [!DNL Walmart Marketplace] beheren via de interface van Channel Manager.

De status voor een afzonderlijke vermelding geeft aan waar het product zich in de [!DNL Channel Manager] -workflow bevindt, zodat u de volgende stappen kunt bepalen en eventuele fouten kunt oplossen.

![ pagina van Lijsten voor een verbonden verkoopkanaal ](assets/listings-dashboard-view.png){width="500" zoomable="yes"}

U kunt de volgende taken uitvoeren vanuit de lijstweergave.

* Huidige aanbiedingen weergeven
* De lijsten sorteren en filteren
* Producten toevoegen
* Producten afstemmen
* Aanbiedingsstatus volgen
* Foutbeschrijving bekijken voor aanbiedingen met een foutstatus

## Objecten weergeven

1. Van Admin, ga naar [!UICONTROL **Marketing** > **Manager van het Kanaal**].

1. Selecteer in de lijst Winkel het oogpictogram in een rij met items in de winkel om de winkelweergave te openen.

1. Selecteer [!UICONTROL **Lijsten**].

1. Soort de *Lijende* mening door om het even welke kolomrubriek in de *het Lijst* lijst te selecteren.

1. Filter de *Lijende* mening door één van de kaarten van de statustelling te selecteren.

1. Herstel de soortorde en verwijder filters door **te selecteren verfrist producten**.

## [!DNL Commerce] producten toevoegen aan Channel Manager

Maak de producttoewijzing voor het [!DNL Walmart Marketplace] -kanaal door de volgende taken uit te voeren:

* [Voeg producten van uw  [!DNL Commerce]  productcatalogus aan  [!DNL Channel Manager] toe](add-products-to-channel-store.md)

* [Kenmerken van catalogus toewijzen](map-catalog-attributes.md#configure-product-attribute-settings)

## Producten afstemmen op [!DNL Walmart]

U kunt productaanbiedingen op [!DNL Walmart Marketplace] maken door producten op elkaar af te stemmen of door handmatig productaanbiedingen voor nieuwe producten te uploaden.

* **[de producten van de Gelijke Gelijke op Marm](connect-listings-to-marketplace.md)** - verbind productlijsten van uw kanaal met [!DNL Walmart Marketplace] door bestaande lijsten bij te werken die het zelfde product verkopen. De criteria van de gelijke worden bepaald door de [ eigenschap-afbeelding configuratie ](map-catalog-attributes.md) voor uw kanaal.

* **[uploadt manueel nieuwe lijsten](connect-listings-to-marketplace.md#upload-new-product-listings)** - voor producten die geen bestaande lijst op [!DNL Walmart Marketplace] aanpassen, gebruik een [!DNL Walmart] malplaatje van de productcategorie Excel aan bulkupload productlijsten.

## Besturingselementen voor lijsten en kolombeschrijvingen

In de volgende tabellen worden de besturingselementen en kolommen beschreven die beschikbaar zijn voor [!UICONTROL Listings] .

**Controles voor[!UICONTROL Listings]**

| **Controle** | **Beschrijving** |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Hiermee opent u de pagina [!UICONTROL Admin Product Catalog] waarin u producten kunt selecteren die u wilt toevoegen aan uw [!DNL Walmart Marketplace] -assortiment of productkenmerken kunt bijwerken om te voldoen aan de vereisten voor de aanbieding in de handelsplaats van Walmart. |
| [!UICONTROL Match products on Walmart] | Nadat u een of meer producten met de status [!UICONTROL Draft] hebt geselecteerd, selecteert u [!UICONTROL Match products on Walmart] om te controleren op productaanbiedingen die aan een bestaande [!DNL Walmart Marketplace] -lijst kunnen worden toegevoegd. |
| [!UICONTROL Refresh products] | Werk de weergave bij met de meest recente aanbieding en status. Met dit besturingselement wordt ook de standaardsorteervolgorde van de lijstweergave hersteld en worden eventuele filters verwijderd. |
| [!UICONTROL Filter by *Status*] | Alleen aanbiedingen met een specifieke status weergeven door een van de statuskaarten boven de tabel met aanbiedingen te selecteren. Verwijder het filter door **[!UICONTROL Refresh products]** te selecteren. |
| [!UICONTROL Sort products] | Wijzig de sorteervolgorde voor de aanbieding door een kolomkop te selecteren. |


**de beschrijvingen van de Kolom**

| **Gebied** | **Beschrijving** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Naam van het product uit de [!DNL Commerce] winkelcatalogus. |
| [!UICONTROL SKU (Unique ID)] | De SKU die aan het product in de [!DNL Commerce] catalogus wordt toegewezen. |
| [!UICONTROL  Quantity] | De hoeveelheid voorraad beschikbaar in Adobe Commerce of Magento Open Source. |
| [!UICONTROL Price] | De prijs van het product in de winkelcatalogus van [!DNL Commerce] . Updates van catalogusprijzen worden gesynchroniseerd naar Channel Manager en vervolgens verzonden naar [!DNL Walmart Marketplace] zodat de huidige prijs wordt weergegeven in de aangeboden items. |
| [!UICONTROL Status] | Geeft de huidige orderstatus in de [!DNL Commerce] bestelworkflow aan. De status wordt bijgewerkt wanneer u producten aan [!DNL Channel Manager] toevoegt en wanneer u producten op de markt aanpast. Als een bewerking mislukt, wordt een foutstatus weergegeven. Nadat u de fout hebt verholpen, probeert [!DNL Channel Manager] de bewerking opnieuw en wordt de status bijgewerkt. |
| [!UICONTROL Error Description] | Bevat aanvullende foutinformatie voor producten met een `[!DNL Error]` -status. |

### Over aanbiedingsstatus

In de werkruimte van de Lijst, toont het etiket van de Status waar een product in [!DNL Channel Manager] werkschema is zodat kunt u volgende stappen bepalen en fouten oplossen. Aanbiedingen kunnen de volgende statuslabels hebben:

* **[!UICONTROL Draft]** - identificeert producten die niet [ aan  [!DNL Walmart]  voor aanpassing ](connect-listings-to-marketplace.md#match-products) zijn voorgelegd.

* **[!UICONTROL Processing]** - Identificeert producten die worden verzonden voor overeenkomst op [!DNL Walmart Marketplace]. De producten blijven in *Verwerking* status tot [!DNL Walmart] een de statusbericht terugkeert van HTTP dat erop wijst of de gelijke, of als er een fout was. Het kan tot 30 minuten duren voordat de match-bewerking op de [!DNL Walmart Marketplace] is voltooid.

* **[!UICONTROL Match]** - Identificeert producten die op [!DNL Walmart] met succes werden aangepast.

  Er treedt een overeenkomst op wanneer de waarde van het productkenmerk, bijvoorbeeld UPC-code, overeenkomt met de waarde UPC in een bestaande [!DNL Walmart Marketplace] -lijst. Wanneer een product overeenkomt, wordt het Commerce-productaanbod aan de bestaande aanbieding toegevoegd.

  Controleer het [[!UICONTROL Walmart Marketplace Seller Account Items] ](https://seller.walmart.com/items-and-inventory/manage-items) dashboard om de bijgewerkte productlijst te herzien en productdetails, prijs, en inventarishoeveelheid te verifiëren.

* **[!UICONTROL Match - Match in Stage]** - Identificeert producten die overeenkomen met [!DNL Walmart] en die pas kunnen worden verbonden als de [!DNL Walmart Marketplace] -winkel live is. Producten met deze status maken automatisch verbinding wanneer de [!DNL Walmart Marketplace] store live gaat.

* **[!UICONTROL Error]** - Identificeert producten die niet overeenkomen met een bestaande [!DNL Walmart Marketplace] -lijst.

* **[!UICONTROL Error description]** - Geeft gedetailleerde informatie over de lijstfout.

  Nadat u de fout hebt verholpen, dient u het product opnieuw in voor overeenkomst. Zie [ problemen oplossen van de fouten van de productgelijke ](connect-listings-to-marketplace.md#troubleshoot-product-match-errors).
