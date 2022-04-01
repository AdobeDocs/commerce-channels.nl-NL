---
title: Bestellingen beheren
description: Aanbiedingen in verkoopkanalen beheren voor een [!DNL Commerce] Opslaan met Channel Manager voor Adobe Commerce en Magento Open Source.
source-git-commit: d1de3bb8873ea6bd141914c083b023def07999fd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Aanbiedingen beheren

Productaanbiedingen voor een verbonden kanaal beheren vanuit[!UICONTROL Listings] in de weergave Kanaalopslag.

De werkruimte Aanbiedingen bevat de producten die je kunt aanbieden op de Marketplace van Walmart en biedt de tools voor het beheren van aanbiedingen. De status van een afzonderlijke aanbieding geeft aan waar het product zich bevindt in de [!DNL Channel Manager] zodat u de volgende stappen kunt bepalen en fouten kunt oplossen.

![Pagina met aanbiedingen voor een verbonden verkoopkanaal](assets/products-submit-for-matching.png)

## Aanbiedingen bekijken

1. Ga vanuit de beheerder naar [!UICONTROL **Marketing** > Kanalen > **Kanaalbeheer**].

1. Selecteer in de lijst Kanaalwinkel het potloodpictogram in de rij met items in de winkel om de winkelweergave te openen.

1. Selecteren [!UICONTROL **Aanbiedingen**].


## Producten publiceren naar Walmart

U kunt productaanbiedingen maken op de Marketplace van het type Walmart met productmatching of door handmatig productaanbiedingen voor nieuwe producten te uploaden. Zie voor instructies [Aanbiedingen publiceren naar Walmart Marketplace](publish-listings-to-marketplace.md) zoals beschreven in de volgende onderwerpen:

* **[Producten afstemmen op Walmart](publish-listings-to-marketplace.md)**-Publiceer productaanbiedingen van je kanaal naar [!DNL Walmart Marketplace] door bestaande aanbiedingen die hetzelfde product verkopen bij te werken. Overeenkomstcriteria worden bepaald door de [kenmerktoewijzingsconfiguratie](map-product-attributes-for-matching.md) voor uw kanaal.

* **Nieuwe aanbiedingen handmatig uploaden**-Voor producten die niet overeenkomen met een bestaande aanbieding op Marketplace, gebruikt u een Excel-sjabloon voor de Walmart-productcategorie om productaanbiedingen in bulk te uploaden.

## Informatie over besturingselementen voor lijsten en informatie

**Besturingselementen voor[!UICONTROL Listings]**

| **Kenmerk** | **Vereiste niveau** |
|---------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Producten vernieuwen | Werkt de weergave bij met de meest recente lijst en statusgegevens. |
| Producten toevoegen | Hiermee opent u de [!UICONTROL  Admin Product Catalog] pagina voor het selecteren van producten die u aan uw [!DNL Walmart Marketplace] assorment, of om productattributen bij te werken om aan de vereisten van de de lijstaanbieding van de Marketplace van het Markeren te voldoen. |
| Producten afstemmen op Walmart | Nadat u een of meer producten in de conceptstatus hebt geselecteerd, selecteert u Producten afstemmen op Walmart om te controleren op productaanbiedingen die aan een bestaand product kunnen worden toegevoegd[!DNL Walmart Marketplace] aanbieding. |


**Kolombeschrijvingen**

| **Veld** | **Beschrijving** |
|-----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Productnaam | Naam van het product van de [!DNL Commerce] opslagcatalogus. |
| SKU (unieke id) | Het toegewezen kenmerk dat wordt gebruikt om producten op de markt aan te passen. Deze veldnaam is afhankelijk van de configuratie van het toegewezen kenmerk voor [!DNL Channel Manager] aanbiedingen. In dit geval gebruikt de productmatchingbewerking de SKU van de [!DNL Commerce] catalogus om een [!DNL Walmart Marketplace]  Een aanbieding met een waarde SKU die de waarde SKU van de het productattributen van de Handel aanpast. |
| Aantal | De hoeveelheid voorraad beschikbaar in Adobe Commerce of Magento Open Source. |
| Prijs | De productprijs van de [!DNL Commerce] opslagcatalogus. Updates van catalogusprijzen worden gesynchroniseerd naar Channel Manager en vervolgens verzonden naar [!DNL Walmart Marketplace]  zodat de aangeboden objecten de huidige prijs aangeven. |
| Status | Geeft de huidige orderstatus in het dialoogvenster [!DNL Commerce] bestelworkflow. De status wordt bijgewerkt wanneer u producten toevoegt aan [!DNL Channel Manager] en wanneer u producten op de markt aanpast. Als een bewerking mislukt, wordt de status Fout weergegeven. Nadat u de fout hebt verholpen, [!DNL Channel Manager] probeert de bewerking opnieuw en werkt de status bij. |


### Over aanbiedingsstatus

In de werkruimte van de aanbieding geeft het label Status aan waar een product zich in het dialoogvenster [!DNL Channel Manager] zodat u de volgende stappen kunt bepalen en fouten kunt oplossen. Productstatus*.

* **[!UICONTROL Draft]**-Identificeert producten die niet zijn [ingediend bij [!DNL Walmart] voor matching](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**-Identificeert producten die worden ingediend voor matching op de [!DNL Walmart Marketplace]. Producten blijven in *Verwerking* status tot de [!DNL Walmart Marketplace] retourneert een HTTP-statusbericht dat aangeeft of de overeenkomst is gelukt of dat er een fout is opgetreden. Het kan tot 30 minuten duren voor de gelijke verrichting op [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identificeert producten die met succes op Walmart werden ontmoet.

   Er treedt een overeenkomst op wanneer de waarde-UPC-code van het productkenmerk bijvoorbeeld overeenkomt met de UPC-waarde in een bestaand[!DNL Walmart Marketplace] aanbieding. Wanneer een product aanpast, wordt de het productaanbieding van de Handel toegevoegd aan de bestaande aanbieding van het Marsmarm.

   Controleer de [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) dashboard om de bijgewerkte productlijst te bekijken en de productgegevens, de prijs en de voorraad te controleren.


* **[!UICONTROL Error]**-Identificeert producten die niet aan een bestaand [!DNL Walmart Marketplace] aanbieding. Foutgegevens weergeven door de muisaanwijzer op de knop *Fout* statuslabel.

   Nadat u de fout hebt verholpen, dient u het product opnieuw in voor overeenkomst. Zie [Problemen met overeenkomende productfouten oplossen](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.sz6eji8z9vzy).

* **[!UICONTROL Error - Match in Stage]**-Identificeert producten die overeenkomen met [!DNL Walmart] die pas gepubliceerd kunnen worden na de [!DNL Walmart Marketplace] de winkel is live. Producten met deze status publiceren automatisch wanneer de [!DNL Walmart Marketplace] winkel gaat live.



