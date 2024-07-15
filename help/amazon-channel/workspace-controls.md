---
title: Amazon-verkoopkanaal - Workspace-controles
description: De Sales Channel van Amazon biedt besturingselementen in de werkruimte waarmee u lijsten kunt zoeken, informatie kunt bekijken en eenvoudig handelingen kunt toepassen.
feature: Sales Channels
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Workspace-besturingselementen

De het verkoopkanaal van Amazon [ homepage ](./amazon-sales-channel-home.md) heeft sommige gemeenschappelijke werkruimtesecontroles met inbegrip van Filters, StandaardMening, Kolommen, en de Uitvoer. Niet alle pagina&#39;s hebben dezelfde besturingsopties.

![ de controlevoorbeelden van de Sales Channel van Amazon ](assets/amazon-workspace-controls.png){width="600" zoomable="yes"}

## Handelingen

De kiezer van _[!UICONTROL Actions]_bevat een lijst met acties die beschikbaar zijn voor een gebruiker voor een pagina. Wanneer u deze optie kiest, wordt de actie toegepast op alle geselecteerde items. Als u een actie wilt toepassen op een specifiek item, schakelt u het selectievakje in de eerste kolom van elk item in en kiest u een optie onder_[!UICONTROL Actions]_ .

Wanneer de kiezer bijvoorbeeld op de pagina _[!UICONTROL Attributes]_wordt weergegeven, bevat deze de handeling_[!UICONTROL Re-import Product Attribute Values]_ . Als u deze handeling kiest, wordt de bijbehorende [!DNL Amazon Seller Central] -account gepingeld en worden de [!DNL Commerce] -gegevens vernieuwd voor elk van de Amazon-opslagitems die in de linkerkolom zijn gecontroleerd.

![ het menuvoorbeeld van Acties ](assets/amazon-sales-channel-home-actions-option.png){width="500"}

## Filters

In het besturingselement _[!UICONTROL Filters]_worden opties weergegeven voor het verfijnen van de gegevens in de tabel. Filteropties zijn gebaseerd op de kolommen die zijn geselecteerd in het besturingselement Kolommen. De opties van de filter tonen slechts kolommen die in de controle van Kolommen worden toegelaten.

Besturingselementen voor filters kunnen dynamische kalenders bevatten voor het beperken van gegevens voor opgegeven datums, vervolgkeuzemenu&#39;s voor kolommen met vooraf gedefinieerde selecties en tekstvelden met vrije tekst die aangepaste gegevens kunnen bevatten.

In het volgende voorbeeld worden de instellingen getoond voor het filteren van de lijst met orders, zodat alleen orders worden weergegeven die aan de volgende criteria voldoen:

- tussen 2.1.2019 en 2.7.2019 geplaatste orders, en
- bestellingen met een koper met de naam `Smith` en
- Orders met de status `Shipped` .

Wanneer u filteropties hebt ingesteld, klikt u op **[!UICONTROL Apply Filters]** om de vermelde gegevens te filteren. Klik op Annuleren om het besturingselement Filters af te sluiten zonder het toe te passen.

![ de controlevoorbeeld van Filters ](assets/workspace-controls-filters.png){width="600" zoomable="yes"}

Nadat u filters op uw gegevens toepast, zal **[!UICONTROL Active Filters]** informatie verschijnen. U kunt het ![ Duidelijke pictogram van filters ](assets/x-icon-clear-filters.png) klikken om een specifieke filteroptie te ontruimen of **[!UICONTROL Clear All]** te klikken om alle toegepaste filters te ontruimen.

![ Actief filtervoorbeeld ](assets/applied-filters-line.png){width="700"}

## Weergave

De controle van de Mening is gebaseerd op de standaardkolommen voor pagina, zo wordt het genoemd de StandaardMening. U kunt beschikbare kolommen toevoegen of verwijderen gebruikend de controle van Kolommen. Wanneer u uw kolommen aanpast, kunt u de mening als douanemening in de controle van de Mening dan bewaren.

Wanneer u kolommen hebt toegevoegd of uit de paginaweergave verwijderd:

1. Klik op **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]** .

1. Voer een naam in voor weergave.

1. Klik op het pijlpictogram om de aangepaste weergave op te slaan.

![ de controlevoorbeeld van de Mening ](assets/workspace-controls-view.png)

In dit voorbeeld, wordt de _kolom van identiteitskaart van de Orde_ toegevoegd in de controle van de Kolom en als douanemening bewaard. Bericht dat na de naam van de douanemening werd bewaard, veranderde de naam van de Mening van _StandaardMening_ in de ingegaan naam.

U kunt schakelen tussen de weergaven door de gewenste weergave te selecteren in het menu _[!UICONTROL View]_.

Als u de naam van de aangepaste weergave wilt verwijderen of wijzigen, klikt u op het potloodpictogram. U kunt vervolgens een andere naam invoeren of op het prullenbakpictogram klikken om de aangepaste weergave te verwijderen. De standaardweergave kan niet worden verwijderd.

## Kolommen

Met het besturingselement Kolommen kunt u kolommen met gegevens toevoegen aan of verwijderen uit de paginaweergave. Elke Amazon-pagina met verkoopkanalen heeft een vooraf ingestelde combinatie van gegevenskolommen, maar op de meeste pagina&#39;s zijn extra kolommen beschikbaar. Als er geen extra kolommen beschikbaar zijn, kunt u nog steeds standaardkolommen uit de weergave verwijderen.

In het volgende voorbeeld ziet u een besturingselement Kolommen. De geselecteerde opties komen overeen met de kolomkoppen die op de pagina worden weergegeven.

- Schakel het selectievakje in om een gegevenskolom aan de pagina toe te voegen.
- Schakel het selectievakje niet in als u een gegevenskolom van de pagina wilt verwijderen.

![ de controlevoorbeeld van Kolommen ](assets/workspace-controls-columns.png){width="400"}

Wijzigingen in selectievakje worden direct weergegeven. Als u wijzigingen aanbrengt en de pagina afsluit, keert de pagina terug naar de standaardkolomweergave. Voor veranderingen die u regelmatig aanbrengt, kunt u de kolomveranderingen als douanemening in de controle van de Mening bewaren. Dan kunt u in de controle van de Mening van een knevel voorzien zonder het moeten kolommen toevoegen of manueel verwijderen.

U kunt op **[!UICONTROL Reset]** klikken om de standaardinstellingen weer in te stellen. U kunt ook op **[!UICONTROL Cancel]** klikken om de opties weer in te stellen zonder uw wijzigingen.

## Exporteren

Met de optie Exporteren kunt u de gegevens exporteren naar een gegevensbestand dat niet kan worden geïmporteerd naar een externe software of afzonderlijke database. De geëxporteerde gegevens zijn beperkt tot de weergegeven gegevens. Indien nodig, zorg ervoor dat u kolommen toevoegt of verwijdert alvorens de controle van de Uitvoer te gebruiken.

Als u uw gegevens wilt exporteren, kiest u een optie voor de exportindeling en klikt u op **[!UICONTROL Export]** .

- CSV - een kommagescheiden waardebestand dat normale tekstgegevens bevat
- Excel XML - een op XML-Gebaseerde, spreadsheetgegevensformaat (typisch gebruikt voor de gebruikers van Excel)

Het gegenereerde gegevensbestand wordt automatisch voor downloads opgeslagen naar de door u aangewezen map.

![ de controle van de Uitvoer ](assets/workspace-controls-export.png){width="250"}
