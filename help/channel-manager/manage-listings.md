---
title: Aanbiedingen beheren
description: '''Aanbiedingen in verkoopkanalen beheren voor een [!DNL Commerce] Opslaan met Channel Manager voor Adobe Commerce en Magento Open Source.'''
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 638ba8c595652e66aa5f15f5207855c6d2b872d7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Aanbiedingen beheren

Productaanbiedingen beheren voor de [!DNL Walmart Marketplace] verkoopkanaal van de UI van de Manager van het Kanaal.

De status van een afzonderlijke aanbieding geeft aan waar het product zich bevindt in de [!DNL Channel Manager] zodat u de volgende stappen kunt bepalen en eventuele fouten kunt oplossen.

![Pagina met aanbiedingen voor een verbonden verkoopkanaal](assets/listings-dashboard-view.png)

U kunt de volgende taken uitvoeren vanuit de lijstweergave.

* Huidige aanbiedingen weergeven
* De lijsten sorteren en filteren
* Producten toevoegen
* Producten afstemmen
* Aanbiedingsstatus volgen
* Foutbeschrijving bekijken voor aanbiedingen met een foutstatus

## Objecten weergeven

1. Ga vanuit de beheerder naar [!UICONTROL **Marketing** > **Kanaalbeheer**].

1. Selecteer in de lijst Winkel het oogpictogram in de rij Winkelitem om de winkelweergave te openen.

1. Selecteren [!UICONTROL **Aanbiedingen**].

1. Sorteer de *Aanbieding* weergeven door een kolomkop te selecteren in het dialoogvenster *Aanbieding* tabel.

1. Filter de *Aanbieding* door een van de statustelkaarten te selecteren.

1. De sorteervolgorde herstellen en filters verwijderen door **Producten vernieuwen**.

## Toevoegen [!DNL Commerce] producten naar Channel Manager

Maak de productassortiment voor de [!DNL Walmart Marketplace] kanaal door de volgende taken uit te voeren:

* [Producten toevoegen van uw [!DNL Commerce] productcatalogus naar [!DNL Channel Manager]](add-products-to-channel-store.md)

* [Kenmerken van catalogus toewijzen](map-catalog-attributes.md#configure-product-attribute-settings)

## Producten afstemmen op [!DNL Walmart]

U kunt productaanbiedingen maken op de [!DNL Walmart Marketplace] met productmatching of door handmatig productaanbiedingen voor nieuwe producten te uploaden.

* **[Producten afstemmen op Walmart](connect-listings-to-marketplace.md)**—Verbind productaanbiedingen van uw kanaal met [!DNL Walmart Marketplace] door bestaande aanbiedingen die hetzelfde product verkopen bij te werken. Overeenkomstcriteria worden bepaald door de [configuratie voor kenmerktoewijzing](map-catalog-attributes.md) voor uw kanaal.

* **[Nieuwe aanbiedingen handmatig uploaden](connect-listings-to-marketplace.md#upload-new-product-listings)**—Voor producten die niet overeenkomen met een bestaande aanbieding op [!DNL Walmart Marketplace], gebruikt u een [!DNL Walmart] productcategorie Excel-sjabloon om productaanbiedingen bulksgewijs te uploaden.

## Besturingselementen voor lijsten en kolombeschrijvingen

In de volgende tabellen worden de besturingselementen en kolommen beschreven die beschikbaar zijn voor [!UICONTROL Listings].

**Besturingselementen voor[!UICONTROL Listings]**

| **Control** | **Beschrijving** |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Hiermee opent u de [!UICONTROL Admin Product Catalog] pagina voor het selecteren van producten die u aan uw [!DNL Walmart Marketplace] assorment, of om productattributen bij te werken om aan de vereisten van de de lijstaanbieding van de Marketplace van het Markeren te voldoen. |
| [!UICONTROL Match products on Walmart] | Nadat u een of meer producten in de conceptstatus hebt geselecteerd, selecteert u Producten afstemmen op [!DNL Walmart] om te controleren op productaanbiedingen die kunnen worden toegevoegd aan een bestaande [!DNL Walmart Marketplace] aanbieding. |
| [!UICONTROL Refresh products] | Werk de weergave bij met de meest recente aanbieding en status. Met dit besturingselement wordt ook de standaardsorteervolgorde van de lijstweergave hersteld en worden eventuele filters verwijderd. |
| [!UICONTROL Filter by *Status*] | Alleen aanbiedingen met een specifieke status weergeven door een van de statustelkaarten boven de tabel met aanbiedingen te selecteren. Gebruik de *Producten vernieuwen* om het filter te verwijderen. |
| [!UICONTROL Sort products] | Wijzig de sorteervolgorde voor de aanbieding door een kolomkop te selecteren. |


**Kolombeschrijvingen**

| **Veld** | **Beschrijving** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Naam van het product van de [!DNL Commerce] opslagcatalogus. |
| [!UICONTROL SKU (Unique ID)] | De SKU die aan het product in [!DNL Commerce] catalogus. |
| [!UICONTROL  Quantity] | De hoeveelheid voorraad beschikbaar in Adobe Commerce of Magento Open Source. |
| [!UICONTROL Price] | De productprijs van de [!DNL Commerce] opslagcatalogus. Updates van catalogusprijzen worden gesynchroniseerd naar Channel Manager en vervolgens verzonden naar [!DNL Walmart Marketplace]  zodat de aangeboden objecten de huidige prijs aangeven. |
| [!UICONTROL Status] | Geeft de huidige orderstatus in het dialoogvenster [!DNL Commerce] bestelworkflow. De status wordt bijgewerkt wanneer u producten toevoegt aan [!DNL Channel Manager] en wanneer u producten op de markt aanpast. Als een bewerking mislukt, wordt een foutstatus weergegeven. Nadat u de fout hebt verholpen, [!DNL Channel Manager] probeert de bewerking opnieuw en werkt de status bij. |
| [!UICONTROL Error Description] | Biedt aanvullende foutinformatie voor producten met een `[!DNL Error]` status. |
| [!UICONTROL Status Detail] | Verstrekt extra informatie voor producten met *Fout* of *Overeenkomst* status. |

### Over aanbiedingsstatus

In de werkruimte van de aanbieding geeft het label Status aan waar een product zich in het dialoogvenster [!DNL Channel Manager] zodat u de volgende stappen kunt bepalen en fouten kunt oplossen. Aanbiedingen kunnen de volgende statuslabels hebben:

* **[!UICONTROL Draft]**-Identificeert producten die niet zijn [ingediend bij [!DNL Walmart] voor matching](connect-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**—Identificeert producten die worden ingediend voor matching op de [!DNL Walmart Marketplace]. Producten blijven in *Verwerking* status tot de [!DNL Walmart] retourneert een HTTP-statusbericht dat aangeeft of de overeenkomst is gelukt of dat er een fout is opgetreden. Het kan tot 30 minuten duren voor de gelijke verrichting op [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identificeert producten die met succes werden aangepast [!DNL Walmart].

   Er is een overeenkomst wanneer de waarde van het productkenmerk (bijvoorbeeld de UPC-code) overeenkomt met de UPC-waarde in een bestaand kenmerk [!DNL Walmart Marketplace] aanbieding. Wanneer een product overeenkomt, wordt het aanbod van het product van de Handel toegevoegd aan de bestaande aanbieding.

   Controleer de [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) dashboard om de bijgewerkte productlijst te bekijken en de productgegevens, de prijs en de voorraad te controleren.

* **[!UICONTROL Match - Match in Stage]**—Identificeert producten die overeenkomen met [!DNL Walmart] die niet kunnen worden aangesloten tot de [!DNL Walmart Marketplace] de winkel is live. Producten met deze status maken automatisch verbinding wanneer de [!DNL Walmart Marketplace] winkel gaat live.

* **[!UICONTROL Error]**—Identificeert producten die niet aan een bestaand [!DNL Walmart Marketplace] aanbieding.

* **[!UICONTROL Error description]**—Geeft gedetailleerde informatie over de lijstfout.

   Nadat u de fout hebt verholpen, dient u het product opnieuw in voor overeenkomst. Zie [Problemen met overeenkomende productfouten oplossen](connect-listings-to-marketplace.md#troubleshoot-product-match-errors).
