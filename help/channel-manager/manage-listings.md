---
title: Aanbiedingen beheren
description: Aanbiedingen in verkoopkanalen beheren voor een [!DNL Commerce] Opslaan met Channel Manager voor Adobe Commerce en Magento Open Source.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 61d72e655a9f9eaefddd7561e0bc5fe36da69577
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Aanbiedingen beheren

Productaanbiedingen beheren voor de [!DNL Walmart Marketplace] verkoopkanaal van [!UICONTROL Listings] in de weergave Kanaalopslag. De status van een afzonderlijke aanbieding geeft aan waar het product zich bevindt in de [!DNL Channel Manager] zodat u de volgende stappen kunt bepalen en eventuele fouten kunt oplossen.

De status van een afzonderlijke aanbieding geeft aan waar het product zich bevindt in de [!DNL Channel Manager] zodat u de volgende stappen kunt bepalen en eventuele fouten kunt oplossen.

![Pagina met aanbiedingen voor een verbonden verkoopkanaal](assets/product-listing-landing.png)

U kunt de volgende taken uitvoeren vanuit de lijstweergave.

* Huidige aanbiedingen weergeven
* De lijsten sorteren en filteren
* Producten toevoegen
* Producten afstemmen
* Aanbiedingsstatus volgen

## Objecten weergeven

1. Ga vanuit de beheerder naar [!UICONTROL **Marketing** > Kanalen > **Kanaalbeheer**].

1. Selecteer in de lijst Kanaalwinkel het potloodpictogram in de rij met items in de winkel om de winkelweergave te openen.

1. Selecteren [!UICONTROL **Aanbiedingen**].

1. Sorteer de *Aanbieding* weergeven door een kolomkop te selecteren in het dialoogvenster *Aanbieding* tabel.

1. Filter de *Aanbieding* door een van de statustelkaarten te selecteren.

1. De sorteervolgorde herstellen en filters verwijderen door **Producten vernieuwen**.

## Commerce-producten toevoegen aan Channel Manager

Creeer het productassortiment voor het kanaal van de Marketplace van de Markeren van de Markt door de volgende taken te voltooien:

* [Producten uit uw productcatalogus voor handel toevoegen aan Channel Manager](add-products-to-connected-channel.md)

* [Productovereenkomst configureren](map-product-attributes-for-matching.md#configure-product-attribute-settings)

## Producten publiceren naar Walmart

U kunt productaanbiedingen maken op de Marketplace van het type Walmart met productmatching of door handmatig productaanbiedingen voor nieuwe producten te uploaden. Zie voor instructies [Aanbiedingen publiceren naar Walmart Marketplace](publish-listings-to-marketplace.md) zoals beschreven in de volgende onderwerpen:

* **[Producten afstemmen op Walmart](publish-listings-to-marketplace.md)**-Publiceer productaanbiedingen van je kanaal naar [!DNL Walmart Marketplace] door bestaande aanbiedingen die hetzelfde product verkopen bij te werken. Overeenkomstcriteria worden bepaald door de [configuratie voor kenmerktoewijzing](map-product-attributes-for-matching.md) voor uw kanaal.

* **[Nieuwe aanbiedingen handmatig uploaden](publish-listings-to-marketplace.md#upload-new-product-listings)-**-Voor producten die niet overeenkomen met een bestaande aanbieding op Marketplace, gebruikt u een Excel-sjabloon voor de Walmart-productcategorie om productaanbiedingen in bulk te uploaden.

## Besturingselementen voor lijsten en kolombeschrijvingen

In de volgende tabellen worden de besturingselementen en kolommen beschreven die beschikbaar zijn voor [!UICONTROL Listings].

**Besturingselementen voor[!UICONTROL Listings]**

| **Control** | **Beschrijving** |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Hiermee opent u de [!UICONTROL Admin Product Catalog] pagina voor het selecteren van producten die u aan uw [!DNL Walmart Marketplace] assorment, of om productattributen bij te werken om aan de vereisten van de de lijstaanbieding van de Marketplace van het Markeren te voldoen. |
| [!UICONTROL Match products on Walmart] | Nadat u een of meer producten in de conceptstatus hebt geselecteerd, selecteert u Producten afstemmen op Walmart om te controleren op productaanbiedingen die aan een bestaand product kunnen worden toegevoegd [!DNL Walmart Marketplace] aanbieding. |
| [!UICONTROL Refresh products] | Werk de weergave bij met de meest recente aanbieding en status. Met dit besturingselement wordt ook de standaardsorteervolgorde van de lijstweergave hersteld en worden eventuele filters verwijderd. |
| [!UICONTROL Filter by *Status*] | Alleen aanbiedingen met een specifieke status weergeven door een van de statustelkaarten boven de tabel met aanbiedingen te selecteren. Gebruik de *Producten vernieuwen* om het filter te verwijderen. |
| [!UICONTROL Sort products] | Wijzig de sorteervolgorde voor de aanbieding door een kolomkop te selecteren. |


**Kolombeschrijvingen**

| **Veld** | **Beschrijving** |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Naam van het product van de [!DNL Commerce] opslagcatalogus. |
| [!UICONTROL SKU (Unique ID)] | Het toegewezen kenmerk dat wordt gebruikt om producten op de markt aan te passen. Deze veldnaam is afhankelijk van de configuratie van het toegewezen kenmerk voor [!DNL Channel Manager] aanbiedingen. In dit geval gebruikt de productmatchingbewerking de SKU van de [!DNL Commerce] catalogus om een [!DNL Walmart Marketplace]  Een aanbieding maken met een SKU-waarde die overeenkomt met de SKU-waarde van de [!DNL Commerce] productkenmerken. |
| [!UICONTROL  Quantity] | De hoeveelheid voorraad beschikbaar in Adobe Commerce of Magento Open Source. |
| [!UICONTROL Price] | De productprijs van de [!DNL Commerce] opslagcatalogus. Updates van catalogusprijzen worden gesynchroniseerd naar Channel Manager en vervolgens verzonden naar [!DNL Walmart Marketplace]  zodat de aangeboden objecten de huidige prijs aangeven. |
| [!UICONTROL Status] | Geeft de huidige orderstatus in het dialoogvenster [!DNL Commerce] bestelworkflow. De status wordt bijgewerkt wanneer u producten toevoegt aan [!DNL Channel Manager] en wanneer u producten op de markt aanpast. Als een bewerking mislukt, wordt een foutstatus weergegeven. Nadat u de fout hebt verholpen, [!DNL Channel Manager] probeert de bewerking opnieuw en werkt de status bij. |
| [!UICONTROL Status Detail] | Verstrekt extra informatie voor producten met *Fout* of *Overeenkomst* status. |

### Over aanbiedingsstatus

In de werkruimte van de aanbieding geeft het label Status aan waar een product zich in het dialoogvenster [!DNL Channel Manager] zodat u de volgende stappen kunt bepalen en fouten kunt oplossen. Aanbiedingen kunnen de volgende statuslabels hebben:

* **[!UICONTROL Draft]**-Identificeert producten die niet zijn [ingediend bij [!DNL Walmart] voor matching](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**-Identificeert producten die worden ingediend voor matching op de [!DNL Walmart Marketplace]. Producten blijven in *Verwerking* status tot de [!DNL Walmart] retourneert een HTTP-statusbericht dat aangeeft of de overeenkomst is gelukt of dat er een fout is opgetreden. Het kan tot 30 minuten duren voor de gelijke verrichting op [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identificeert producten die met succes werden aangepast [!DNL Walmart].

   Er treedt een overeenkomst op wanneer de waarde-UPC-code van het productkenmerk bijvoorbeeld overeenkomt met de UPC-waarde in een bestaand[!DNL Walmart Marketplace] aanbieding. Wanneer een product aanpast, wordt de het productaanbieding van de Handel toegevoegd aan de bestaande aanbieding van het Marsmarm.

   Controleer de [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) dashboard om de bijgewerkte productlijst te bekijken en de productgegevens, de prijs en de voorraad te controleren.

* **[!UICONTROL Match - Match in Stage]**-Identificeert producten die overeenkomen met [!DNL Walmart] die pas gepubliceerd kunnen worden na de [!DNL Walmart Marketplace] de winkel is live. Producten met deze status publiceren automatisch wanneer de [!DNL Walmart Marketplace] winkel gaat live.

* **[!UICONTROL Error]**-Identificeert producten die niet aan een bestaand [!DNL Walmart Marketplace] aanbieding. Foutgegevens weergeven door de muisaanwijzer op de knop *Fout* statuslabel.

   Nadat u de fout hebt verholpen, dient u het product opnieuw in voor overeenkomst. Zie [Problemen met overeenkomende productfouten oplossen](publish-listings-to-marketplace.md#troubleshoot-product-match-errors).
