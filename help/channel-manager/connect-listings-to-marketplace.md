---
title: Aanbiedingen verbinden met Walmart
description: Verbind lijsten voor  [!DNL Commerce]  producten met  [!DNL Walmart Marketplace] beginnen het verkopen.'
feature: Sales Channels, Integration, Products, Tools and External Services
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---

# Aanbiedingen verbinden met Walmart

Net als andere markten biedt [!DNL Walmart] verkopers van andere leveranciers de mogelijkheid om objecten aan te bieden die door anderen worden verkocht.

- [!DNL Walmart Marketplace] gebruikt product-id&#39;s zoals UPC en GTIN om producten af te stemmen op bestaande [!DNL Walmart Marketplace] -aanbiedingen.

- Voor overeenkomende producten wordt de vermelding in de lijst Walmart Marketplace bijgewerkt met de productaanbieding van [!DNL Commerce] wanneer u een product aansluit vanuit [!DNL Channel Manager] .

- Productaanbiedingen met de laagste prijzen worden meestal als eerste weergegeven in de [!DNL Walmart Marketplace] -aanbieding, maar andere factoren, zoals revisies, beïnvloeden ook de plaatsing.

## Producten afstemmen

Wanneer u producten aanpast, stuurt Channel Manager de productgegevens naar [!DNL Walmart Marketplace] om te zoeken naar bestaande lijsten met kenmerkwaarden die overeenkomen met het toegewezen [!DNL Commerce] -productkenmerk. De criteria van de gelijke worden bepaald door de [ eigenschap-afbeelding configuratie ](map-catalog-attributes.md) voor uw opslagkanaal.

Als er een overeenkomst wordt gevonden, wordt de bestaande productaanbieding bijgewerkt en wordt je voorstel toegevoegd.

### Vereisten

Alvorens producten aan te passen, verifieer dat uw de attributenwaarden van de productcatalogus aan de vereisten van het Martard voldoen en de montages van de productattributen vormen. Zie [ de catalogusattributen van de Kaart ](map-catalog-attributes.md).

#### Producten selecteren en afstemmen

1. Open een verbonden verkoopkanaal.

1. Selecteer in **[!UICONTROL Listings]** de producten die overeenkomen met de producten in de *[!UICONTROL Draft]* -status.

   ![ selecteer producten van Lijsten en verzend voor aanpassing ](assets/products-in-marketplace-sales-channel.png){width="500" zoomable="yes"}

1. Selecteer **[!UICONTROL Match Products]** .

   Een bericht geeft het aantal producten aan dat voor matching is verzonden.

   De status voor geselecteerde producten verandert in [!UICONTROL *Verwerking*] tot de gelijke verrichting voltooit. Het kan tot 30 minuten voor Walmart Marketplace duren om de gelijke verrichting te voltooien.

### Overeenkomststatus controleren

Nadat de overeenkomst is voltooid, selecteert u de **[!UICONTROL Refresh products]** om de huidige productstatus weer te geven. *Gelijke* of *Fout*.

- **[!UICONTROL Match]** geeft aan dat het product is gevonden. Je productaanbod was verbonden met een bestaande Walmart Marketplace-aanbieding. Als de [ opslag van de Marktplaats niet actief ](walmart-requirements.md#walmart-marketplace-store-status) is, *[!UICONTROL Staged for Match]* wordt getoond in de *[!UICONTROL Status detail]* kolom. Producten met een status worden automatisch verbonden wanneer de [!DNL Walmart Marketplace] store wordt geactiveerd.

- **[!UICONTROL Error]** geeft aan dat de overeenkomst is mislukt door een van de volgende problemen:

   - [!DNL Channel Manager] kan niet verzenden voor overeenkomst vanwege een verbindingsprobleem.

   - Er is geen overeenkomst gevonden.

   - Overeenkomst gevonden, maar de lijst kan niet worden verbonden omdat [!DNL Walmart Marketplace] een foutcode heeft geretourneerd. Zie **[!UICONTROL Error Description]** voor informatie over de kwestie.

### Aanbieding controleren op Walmart

Nadat u producten hebt gevonden, controleert u de bijgewerkte productlijst en de productgegevens, de prijs en het voorraadaantal op het [[!UICONTROL Walmart Marketplace Seller Account Items] dashboard ](https://seller.walmart.com/items-and-inventory/manage-items) om het bijgewerkte product te bekijken.

### Problemen met overeenkomende productfouten oplossen

Als de overeenkomende bewerking met het product een fout oplevert, wordt het foutbericht weergegeven in de kolom *[!UICONTROL Status detail]* in de productlijst van [!UICONTROL Channel Manager] .

Gangbare geretourneerde fouten zijn onjuist opgemaakte product-id-waarden of ontbrekende vereiste kenmerken.

#### ID-waarden van product corrigeren

| Type | Beschrijving | Voorbeeld |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, het 12-cijferige getal inclusief controlecijfer. </br></br> als uw UPC minder dan 12 cijfers heeft, zoals UPC-E die 8 cijfers is, voeg beëindigende nul toe om aan het vereiste te voldoen. | Wijzigen van `45678912345` in `045678912345` |
| GTIN | GTIN-14, het 14-cijferige getal inclusief controlecijfer. </br></br> als uw GTIN minder dan 14 cijfers heeft, voeg belangrijke nul </br> toe om aan het vereiste te voldoen. | `456789123456` wijzigen in `0045678912345` |
| EAN | GTIN-13, het 13-cijferige getal inclusief controlecijfer. </br></br> als uw EAN minder dan 13 cijfers heeft, voeg belangrijke </br> nullen toe om aan het vereiste te voldoen. | Wijzigen van `4567891234` in `0004567891234` |

Voor details over de foutencodes van de Marketplace van de Markt van de Markt, zie de [ Hulp van de Markeren van de Verkoper ](https://sellerhelp.walmart.com/s/guide?article=000005844).

## Nieuwe productaanbiedingen uploaden

Voor producten die geen gelijke op Marketplace hebben, gebruik een sjabloon van de de productcategorie van het Walmart product Excel om productaanbiedingen bulksgewijs te uploaden. U vult de sjabloon Slim met de catalogusgegevens van het product die u uit uw [!DNL Commerce] -instantie hebt geëxporteerd.

Voor nieuwe productaanbiedingen raadpleegt u de productcatalogus om ervoor te zorgen dat producten die je op de Marketplace wilt verkopen, de kenmerken hebben die vereist zijn voor aanbiedingen op de Marketplace-markt.

**Marketplace lijsten-Attribuut van de Markt de Markt vereisten**

| **Attribuut** | **Niveau van de Vereiste** |
|--------------------------|-----------------------|
| SKU | Vereist |
| Productnaam | Vereist |
| Type product-id | Vereist |
| Product-id | Vereist |
| Merk | Vereist |
| Korte beschrijving | Vereist |
| Verkoopprijs | Vereist |
| Beschrijving van site | Vereist |
| URL hoofdafbeelding | Vereist |
| Verzendgewicht | Vereist |
| Belangrijkste kenmerken | Aanbevolen |
| Modelnummer | Aanbevolen |
| Naam fabrikant | Aanbevolen |
| Onderdeelnummer fabrikant | Aanbevolen |
| Grootte | Aanbevolen |
| Kleur | Aanbevolen |
| URL hoofdafbeelding | Optioneel |
| URL van extra afbeelding | Optioneel |
| Fabrikant | Optioneel |

### Vereisten

- Verifieer dat u aan de [ vereisten van het Smarm ](walmart-requirements.md) voldoet.

- Controleer in uw productcatalogus van [!DNL Commerce] of de catalogusconfiguratie voor de producten die op Walmart Marketplace moeten worden aangeboden, alle vereiste kenmerken heeft en voldoet aan de richtlijnen voor Inhoud van de Marketplace van Walmart.

- Controleer of de uitsnijdtaak wordt uitgevoerd om de exportbewerking te voltooien.

   - Voor op-gebouwinstanties, zie [ uitsnede ](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/configure-cron-jobs.html) vormen en in werking stellen.

   - Voor de infrastructuur van de wolk van de Adobe, zie [ banen van de opstelling cron ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/properties/crons-property.html).

### Het te uploaden productgegevensbestand maken

1. Van uw [ Marm Verkoper rekening van de Verkoper ](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), download een malplaatje van de productlijst van het Centrum van de Verkoper van de Mara.

   - Selecteer **[!UICONTROL Add Items]** op de pagina Items van de productcatalogus. Selecteer vervolgens **[!UICONTROL Add items in bulk]** .

     ![ voegt punten in bulkoptie in de het puntconfiguratie van de Marketplace van de Markt toe ](assets/walmart-seller-account-add-items-bulk.png){width="600" zoomable="yes"}

   - Selecteer **[!UICONTROL Full Setup]** op de downloadpagina. Selecteer vervolgens een objectcategorie en download de rubrieksjabloon.

     ![ de optie van het de categoriemalplaatje van de Download in de het puntconfiguratie van de Marketplace van de Markt ](assets/walmart-seller-account-full-setup-download.png){width="600" zoomable="yes"}

   - Controleer of de sjabloon de vereiste en aanbevolen kenmerken voor de productaanbieding bevat.

1. Selecteer in [!DNL Commerce] Beheer de productgegevens die u wilt exporteren van uw Adobe [!DNL Commerce] -site.

   - Van Admin, uitgezochte [!UICONTROL **Systeem** > Overdracht van Gegevens > **de Uitvoer**].

   - Voor de [!UICONTROL Export] pagina op het [!UICONTROL Entity Type] gebied, uitgezochte [!UICONTROL **Producten**].

   - Configureer in de tabel [!UICONTROL Entity Attributes] de selectiecriteria voor de export van productgegevens.

     Gebruik filters om de kenmerkwaarden te selecteren en te configureren die van toepassing zijn op de productcategorieën waarin u verkoopt. Zorg ervoor dat u de vereiste en aanbevolen kenmerken van Walmart opneemt. (Zie [ Gegevens van de Uitvoer ](https://experienceleague.adobe.com/docs/commerce-admin/systems/data-transfer/data-export.html) in de Gids van de Gebruiker van de Adobe [!DNL Commerce] voor gedetailleerde instructies.)

     Om een attribuut van de uitvoer weg te laten, selecteer [!UICONTROL **uitsluiten**] checkbox aan het begin van de rij.

1. De rol aan het eind van de attributenlijst en selecteert [!UICONTROL **gaat**] verder om de gegevensuitvoer te beginnen.

   Het CSV-exportbestand wordt verwerkt via een berichtwachtrij met gebruik van snijtaken en opgeslagen in de `var/export/folder` . (Zie [ berichtrijen ](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/message-queues/manage-message-queues.html) in de *Gids van de Configuratie* beheren.)

1. Open het malplaatje van Excel voor de het productcategorie van de Marketplace van de Markt van de Markt, en gebruik de macromogelijkheden van Excel om de uitgevoerde productgegevens in het malplaatje van Excel samen te voegen.

1. Upload het Excel-bestand met de geëxporteerde productgegevens.

   - Terugkeer naar de pagina van de Punten van de Catalogus van het Product in het [ Centrum van de Verkoper van de Marge ](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - Selecteer [!UICONTROL **punten** toevoegen > **punten in bulk**] toevoegen.
   - Sleep de voltooide spreadsheet aan de Upload sectie.
   - Selecteer [!UICONTROL **voorleggen**].
   - Selecteer het [!UICONTROL  **Diervoer van de Activiteit**] om vooruitgang te bekijken.

Voor volledige instructies, zie [ Punten in Bulk toevoegen Gebruikend Volledige Spec van het Punt ](https://sellerhelp.walmart.com/s/guide?article=000007680) in de [!DNL *Slimme Hulp van de Verkoper van de Markeren*].
