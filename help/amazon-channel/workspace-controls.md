---
title: Besturingselementen werkruimte
description: Amazon Sales Channel biedt besturingselementen in de werkruimte waarmee u lijsten kunt zoeken, informatie kunt bekijken en eenvoudig handelingen kunt toepassen.
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Besturingselementen werkruimte

Het verkoopkanaal van Amazon [homepage](./amazon-sales-channel-home.md) bevat enkele algemene besturingselementen voor werkruimten, zoals Filters, Standaardweergave, Kolommen en Exporteren. Niet alle pagina&#39;s hebben dezelfde besturingsopties.

![Voorbeelden van besturingselementen voor de Amazon-werkruimte](assets/amazon-workspace-controls.png)

## Handelingen

De _[!UICONTROL Actions]_biedt een lijst met acties die beschikbaar zijn voor een gebruiker voor een pagina. Wanneer u deze optie kiest, wordt de actie toegepast op alle geselecteerde items. Als u een actie wilt toepassen op een specifiek item, schakelt u het selectievakje in de eerste kolom van elk item in en kiest u een optie onder_[!UICONTROL Actions]_.

Wanneer de kiezer bijvoorbeeld wordt weergegeven op het tabblad _[!UICONTROL Attributes]_pagina, bevat de_[!UICONTROL Re-import Product Attribute Values]_ handeling. Als u deze handeling kiest, wordt de bijbehorende [!DNL Amazon Seller Central] en vernieuwt de [!DNL Commerce] gegevens voor elk van de Amazon-winkelitems die in de linkerkolom worden gecontroleerd.

![Voorbeeld van het menu Handelingen](assets/amazon-sales-channel-home-actions-option.png)

## Filters

De _[!UICONTROL Filters]_In het besturingselement ziet u opties voor het versmallen van de gegevens in de tabel. Filteropties zijn gebaseerd op de kolommen die zijn geselecteerd in het besturingselement Kolommen. De opties van de filter tonen slechts kolommen die in de controle van Kolommen worden toegelaten.

Besturingselementen voor filters kunnen dynamische kalenders bevatten voor het beperken van gegevens voor opgegeven datums, vervolgkeuzemenu&#39;s voor kolommen met vooraf gedefinieerde selecties en tekstvelden met vrije tekst die aangepaste gegevens kunnen bevatten.

In het volgende voorbeeld worden de instellingen getoond voor het filteren van de lijst met orders, zodat alleen orders worden weergegeven die aan de volgende criteria voldoen:

- orders geplaatst tussen 2/01/2019 en 2/07/2019, en
- Bestellingen met een koper met de naam `Smith`, en
- Orders met de status `Shipped`.

Wanneer u filteropties hebt ingesteld, klikt u op **[!UICONTROL Apply Filters]** om de vermelde gegevens te filteren. Klik op Annuleren om het besturingselement Filters af te sluiten zonder het toe te passen.

![Voorbeeld van filterbesturing](assets/workspace-controls-filters.png)

Nadat u filters op uw gegevens toepast, **[!UICONTROL Active Filters]** de informatie wordt weergegeven. U kunt op de knop ![Filterpictogram wissen](assets/x-icon-clear-filters.png) pictogram om een specifieke filteroptie te wissen of klik op **[!UICONTROL Clear All]** om alle toegepaste filters te wissen.

![Voorbeeld van actieve filters](assets/applied-filters-line.png)

## Weergave

De controle van de Mening is gebaseerd op de standaardkolommen voor pagina, zo wordt het genoemd de StandaardMening. U kunt beschikbare kolommen toevoegen of verwijderen gebruikend de controle van Kolommen. Wanneer u uw kolommen aanpast, kunt u de mening als douanemening in de controle van de Mening dan bewaren.

Wanneer u kolommen hebt toegevoegd of uit de paginaweergave verwijderd:

1. Klikken **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**.

1. Voer een naam in voor weergave.

1. Klik op het pijlpictogram om de aangepaste weergave op te slaan.

![Voorbeeld van besturing weergeven](assets/workspace-controls-view.png)

In dit voorbeeld wordt _Order-id_ kolom wordt toegevoegd in de controle van de Kolom en als douanemening bewaard. De naam van de weergave is gewijzigd van _Standaardweergave_ op de ingevoerde naam.

U kunt schakelen tussen de weergaven door de gewenste weergave te selecteren in het dialoogvenster _[!UICONTROL View]_-menu.

Als u de naam van de aangepaste weergave wilt verwijderen of wijzigen, klikt u op het potloodpictogram. U kunt vervolgens een andere naam invoeren of op het prullenbakpictogram klikken om de aangepaste weergave te verwijderen. De standaardweergave kan niet worden verwijderd.

## Kolommen

Met het besturingselement Kolommen kunt u kolommen met gegevens toevoegen aan of verwijderen uit de paginaweergave. Elke Amazon-pagina met verkoopkanalen heeft een vooraf ingestelde combinatie van gegevenskolommen, maar op de meeste pagina&#39;s zijn extra kolommen beschikbaar. Als er geen extra kolommen beschikbaar zijn, kunt u nog steeds standaardkolommen uit de weergave verwijderen.

In het volgende voorbeeld ziet u een besturingselement Kolommen. De geselecteerde opties komen overeen met de kolomkoppen die op de pagina worden weergegeven.

- Schakel het selectievakje in om een gegevenskolom aan de pagina toe te voegen.
- Als u een gegevenskolom van de pagina wilt verwijderen, schakelt u het selectievakje niet in.

![Kolommen, controlevoorbeeld](assets/workspace-controls-columns.png)

Wijzigingen in selectievakje worden direct weergegeven. Als u wijzigingen aanbrengt en de pagina afsluit, keert de pagina terug naar de standaardkolomweergave. Voor veranderingen die u regelmatig aanbrengt, kunt u de kolomveranderingen als douanemening in de controle van de Mening bewaren. Dan kunt u in de controle van de Mening van een knevel voorzien zonder het moeten kolommen toevoegen of manueel verwijderen.

U kunt op **[!UICONTROL Reset]** om de opties weer in te stellen op de standaardinstellingen, of u kunt op **[!UICONTROL Cancel]** om af te sluiten zonder uw wijzigingen.

## Exporteren

Met de optie Exporteren kunt u de gegevens exporteren naar een gegevensbestand dat niet kan worden geïmporteerd naar een externe software of afzonderlijke database. De geëxporteerde gegevens zijn beperkt tot de weergegeven gegevens. Indien nodig, zorg ervoor dat u kolommen toevoegt of verwijdert alvorens de controle van de Uitvoer te gebruiken.

Kies een optie voor de exportindeling als u uw gegevens wilt exporteren en klik op **[!UICONTROL Export]**.

- CSV - een kommagescheiden waardebestand dat normale tekstgegevens bevat
- Excel XML - een op XML-Gebaseerde, spreadsheetgegevensformaat (typisch gebruikt voor de gebruikers van Excel)

Het gegenereerde gegevensbestand wordt automatisch voor downloads opgeslagen naar de door u aangewezen map.

![Exportcontrole](assets/workspace-controls-export.png)
