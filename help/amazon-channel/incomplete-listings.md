---
title: Onvolledige Amazon-aanbiedingen
description: Het verkoopkanaal van Amazon biedt het tabblad [!UICONTROL Incomplete] om je te helpen bij het identificeren van en voldoen aan de voorwaarden om in aanmerking te komen voor onvolledige Amazon-aanbiedingen.
feature: Sales Channels, Products
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Onvolledige Amazon-aanbiedingen

Het _[!UICONTROL Incomplete]_lusje maakt een lijst van de [!DNL Commerce] catalogusproducten die aan uw Amazon geschiktheidsvereisten (die in uw [ worden bepaald lijstregels ](./listing-rules.md)) voldoen, maar die informatie missen door Amazon (zoals Amazon ASIN of een bepaalde productvoorwaarde) wordt vereist.

Er zijn vier mogelijke oorzaken voor een onvolledige aanbieding, elk geïdentificeerd door zijn status.

| Status | Reden | Handeling |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ontbrekende voorwaarde | Amazon keurt lijsten in diverse voorwaarden (zoals _Nieuw_, _Gereviseerde_ goed, _Gebruikte: Als Nieuwe_) lijst vereist een bepaalde voorwaarde. | De update vereiste info en wijst manueel [ een voorwaarde ](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) aan een lijst toe. |
| Kan niet toewijzen aan Amazon-aanbieding | Automatisch overeenkomst van deze aanbieding met uw catalogus is mislukt. Als er geen overeenkomst wordt gevonden, kan de aanbieding niet door de Sales Channel van Amazon worden beheerd | De update vereiste info en wijst manueel [ ASIN ](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) aan het catalogusproduct voor aanpassing aan de lijst toe. |
| Meerdere overeenkomsten gevonden | Automatisch overeenkomst van deze aanbieding met uw catalogus is mislukt. Als er meerdere mogelijke overeenkomsten worden gevonden, moet u de juiste overeenkomst voor uw product selecteren. | De update vereiste info en kiest manueel [ een productgelijke ](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) voor het product en de lijst. |
| Heeft varianten | Als uw product varianten heeft, zoals een t-shirt dat in verschillende grootten of kleuren beschikbaar is, moet u de variant in uw catalogus kiezen die u op de juiste wijze wilt toewijzen en aan de lijst wilt aanpassen | De update vereiste info en kiest manueel [ de correcte variant ](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) om aan deze lijst toe te wijzen en aan te passen. |

>[!NOTE]
>Wanneer onvolledige aanbiedingen correct overeenkomen met uw catalogusproducten, wordt de aanbieding verplaatst van het tabblad _[!UICONTROL Incomplete]_en op basis van uw [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) -instellingen gepubliceerd naar Amazon.

De beschikbare acties op het tabblad _[!UICONTROL Incomplete]_zijn:

Onder _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: geef aan dat u het automatische proces wilt starten om de gegevens van uw Amazon-aanbiedingen te koppelen aan uw catalogus van [!DNL Commerce] . Als producten niet automatisch overeenkomen, kunt u de [_[!UICONTROL Catalog Search]_](./catalog-search.md) -opties in de aanbiedingen opnieuw bekijken. Als aanbiedingen na het bijwerken van de _[!UICONTROL Catalog Search]_-opties niet automatisch overeenkomen, kunt u de producten handmatig afstemmen in de [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) -actie.

Onder **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_:

- **[!UICONTROL Update Required Info]**: kies wanneer aanbiedingen niet automatisch overeenkomen met uw catalogus. U kunt manueel [ catalogusproducten aan lijsten ](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) aanpassen, manueel [ toewijzen ASIN ](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) aan een catalogusgelijke, of [ toewijzen een ontbrekende voorwaarde ](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) voor lijst.

- **[!UICONTROL View Details]**: verkies om lijstdetails, met inbegrip van het [ Lijst Logboek van de Activiteit ](./product-listing-details.md#listing-activity-log) te bekijken, [ het Prijstarief van de Mededinger van de Buy Box ](./product-listing-details.md#buy-box-competitor-pricing), en [ Laagste Prijsverhoging van de Concurrent ](./product-listing-details.md#lowest-competitor-pricing). Deze handeling is alleen bedoeld voor weergave. De details van de aanbieding kunnen niet worden gewijzigd. Zie [ Details van de Mening ](./product-listing-details.md).

>[!NOTE]
>
>Als je aanbiedingen in behandeling hebt, verschijnt het aantal aanbiedingen in een bericht boven de tabbladen.

![ Onvolledige lijsten van Amazon ](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Amazon delen de homepages van het verkoopkanaal wat gemeenschappelijke [ werkruimtesecontroles ](./workspace-controls.md) die u toestaan om de gegevens aan te passen die worden getoond.

| Kolom | Beschrijving |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br> ASIN staat voor [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Condition] | De [ voorwaarde ](./product-listing-condition.md) van het product. |
| [!UICONTROL Landed Price] | De prijs van de aanbieding voor het product plus de verzendprijs. |
| [!UICONTROL Amazon Quantity] | De hoeveelheid die beschikbaar is wanneer het product actief op Amazon wordt aangeboden. |
| [!UICONTROL Status] | De status van de aanbieding, gedefinieerd door Amazon. Zie de tabel met de status hierboven. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_en selecteert u een optie:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
