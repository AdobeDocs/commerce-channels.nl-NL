---
title: Aanbiedingen verbinden met Walmart
description: '''Aanbiedingen verbinden voor [!DNL Commerce] producten naar [!DNL Walmart Marketplace]om te beginnen met verkopen.'''
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: bc2e14714e9b532263c480395da28b31b4c3797c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Aanbiedingen verbinden met Walmart

Zoals andere markten, [!DNL Walmart] biedt verkopers van derden de mogelijkheid om objecten aan te bieden die door anderen worden verkocht.

- [!DNL Walmart Marketplace] gebruikt product-id&#39;s zoals UPC en GTIN om producten af te stemmen op bestaande [!DNL Walmart Marketplace] aanbiedingen.

- Voor overeenkomende producten wordt de vermelding in de lijst Walmart Marketplace bijgewerkt met de vermelding [!DNL Commerce] productaanbod wanneer u een product aansluit van [!DNL Channel Manager].

- Meestal worden productaanbiedingen met de laagste prijzen het eerst weergegeven in de [!DNL Walmart Marketplace] aanbiedingen, maar andere factoren zoals revisies hebben ook invloed op plaatsing.

## Producten afstemmen

Wanneer u producten aanpast, verzendt de Manager van het Kanaal de productgegevens naar [!DNL Walmart Marketplace] naar bestaande aanbiedingen met kenmerkwaarden zoeken die overeenkomen met de toegewezen waarden [!DNL Commerce] productkenmerk. Overeenkomstcriteria worden bepaald door de [configuratie voor kenmerktoewijzing](map-catalog-attributes.md) voor uw winkelkanaal.

Als er een overeenkomst wordt gevonden, wordt de bestaande productaanbieding bijgewerkt en wordt je voorstel toegevoegd.

### Vereisten

Alvorens producten aan te passen, verifieer dat uw de attributenwaarden van de productcatalogus aan de vereisten van het Martard voldoen en de montages van de productattributen vormen. Zie [Kenmerken van catalogus toewijzen](map-catalog-attributes.md).

#### Producten selecteren en afstemmen

1. Open een verbonden verkoopkanaal.

1. Van **[!UICONTROL Listings]**, selecteer de producten die overeenkomen met de producten in *[!UICONTROL Draft]* status.

   ![Producten uit aanbiedingen selecteren en verzenden voor overeenkomst](assets/products-in-marketplace-sales-channel.png)

1. Selecteren **[!UICONTROL Match Products]**.

   Een bericht geeft het aantal producten aan dat voor matching is verzonden.

   ![Producten naar het verbonden verkoopkanaal verzenden](assets/products-submitted-for-matching.png)

   De status van geselecteerde producten verandert in [!UICONTROL *Verwerking*] totdat de overeenkomende bewerking is voltooid. Het kan tot 30 minuten voor Walmart Marketplace duren om de gelijke verrichting te voltooien.

### Overeenkomststatus controleren

Nadat de overeenkomst voltooit, selecteer **[!UICONTROL Refresh products]** om de huidige productstatus weer te geven. *Overeenkomst* of *Fout*.

- **[!UICONTROL Match]** geeft aan dat het product is gevonden. Je productaanbod was verbonden met een bestaande Walmart Marketplace-aanbieding. Als de [Marktarchief is niet actief](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]* wordt weergegeven in het dialoogvenster *[!UICONTROL Status detail]* kolom. Producten in het werkgebied worden automatisch aangesloten wanneer de [!DNL Walmart Marketplace] store is geactiveerd.

- **[!UICONTROL Error]** geeft aan dat de overeenkomende bewerking is mislukt door een van de volgende problemen:

   - [!DNL Channel Manager] kan niet verzenden voor overeenkomst vanwege een verbindingsprobleem.

   - Er is geen overeenkomst gevonden.

   - Overeenkomst gevonden, maar de aanbieding kan niet worden verbonden omdat [!DNL Walmart Marketplace] heeft een foutcode geretourneerd. Zie de **[!UICONTROL Error Description]** voor meer informatie over deze kwestie.

### Aanbieding controleren op Walmart

Nadat je producten hebt gevonden, kun je de bijgewerkte productlijst bekijken en de productgegevens, prijs en voorraadhoeveelheid van de [[!UICONTROL Walmart Marketplace Seller Account Items] dashboard](https://seller.walmart.com/items-and-inventory/manage-items) om het bijgewerkte product te beoordelen.

### Problemen met overeenkomende productfouten oplossen

Als de productvergelijkingsbewerking mislukt vanwege een fout, wordt het foutbericht weergegeven in het dialoogvenster *[!UICONTROL Status detail]* in de [!UICONTROL Channel Manager] productaanbieding.

Gangbare geretourneerde fouten zijn onjuist opgemaakte product-id-waarden of ontbrekende vereiste kenmerken.

#### ID-waarden van product corrigeren

| Type | Beschrijving | Voorbeeld |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, het 12-cijferige getal inclusief controlecijfer. </br></br>Als uw UPC minder dan 12 cijfers, zoals UPC-E heeft die 8 cijfers is, voeg beëindigende nullen toe om aan het vereiste te voldoen. | Wijzigen van `45678912345` tot `045678912345` |
| GTIN | GTIN-14, het 14-cijferige getal inclusief controlecijfer. </br></br>Als de GTIN uit minder dan 14 cijfers bestaat, voegt u voorloopnullen toe </br>om aan deze eis te voldoen. | Wijzigen `456789123456` tot `0045678912345` |
| EAN | GTIN-13, het 13-cijferige getal inclusief controlecijfer. </br></br>Als uw EAN minder dan 13 cijfers heeft, voeg belangrijke </br>nullen om aan de vereiste te voldoen. | Wijzigen van `4567891234` tot `0004567891234` |

Voor meer informatie over de foutcodes van Walmart Marketplace raadpleegt u de [Help bij Walmart Seller](https://sellerhelp.walmart.com/s/guide?article=000005844).

## Nieuwe productaanbiedingen uploaden

Voor producten die geen gelijke op Marketplace hebben, gebruik een sjabloon van de de productcategorie van het Walmart product Excel om productaanbiedingen bulksgewijs te uploaden. U bevolkt het malplaatje van de Marm gebruikend de gegevens van de productcatalogus die uit uw worden uitgevoerd [!DNL Commerce] -instantie.

Voor nieuwe productaanbiedingen raadpleegt u de productcatalogus om ervoor te zorgen dat producten die je op de Marketplace wilt verkopen, de kenmerken hebben die vereist zijn voor aanbiedingen op de Marketplace-markt.

**Marketplace-aanbiedingen met kenmerk van Walmart**

| **Kenmerk** | **Vereiste niveau** |
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

- Controleren of u voldoet aan de [Walmart-vereisten](walmart-requirements.md).

- In uw [!DNL Commerce] de productcatalogus, verifieert dat de catalogusconfiguratie voor de producten om op Marketplace van het Markeren te vermelden alle vereiste attributen heeft en aan de Richtlijnen van de Inhoud van de Markt van het Markeren voldoet.

- Controleer of de uitsnijdtaak wordt uitgevoerd om de exportbewerking te voltooien.

   - Zie voor informatie op locatie [Uitsnede configureren en uitvoeren](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   - Voor Adobe cloud-infrastructuur raadpleegt u [Uitsnijdtaken instellen](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### Het te uploaden productgegevensbestand maken

1. Van uw [Walmart-verkopersaccount](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), download een productaanbiedingstemplate via het Walmart-winkelcentrum.

   - Selecteer op de pagina Items in productcatalogus de optie **[!UICONTROL Add Items]**. Selecteer vervolgens **[!UICONTROL Add items in bulk]**.

      ![Voeg punten in bulkoptie toe optie in de het puntconfiguratie van de Marketplace van de Markeren](assets/walmart-seller-account-add-items-bulk.png)

   - Selecteer op de downloadpagina de optie **[!UICONTROL Full Setup]**. Selecteer vervolgens een objectcategorie en download de rubrieksjabloon.

      ![Categoriesjabloonoptie downloaden in de configuratie van items in de Marketplace-indeling van het programma](assets/walmart-seller-account-full-setup-download.png)

   - Controleer of de sjabloon de vereiste en aanbevolen kenmerken voor de productaanbieding bevat.

1. Van de [!DNL Commerce] Admin, selecteer de productgegevens om van uw Adobe uit te voeren [!DNL Commerce] site.

   - Selecteer bij Beheer de optie [!UICONTROL **Systeem** > Gegevensoverdracht > **Exporteren**].

   - Op de [!UICONTROL Export] pagina in de [!UICONTROL Entity Type] veld, selecteren [!UICONTROL **Producten**].

   - In de [!UICONTROL Entity Attributes] de lijst, vormt de selectiecriteria voor de uitvoer van productgegevens.
   ![De productgegevenspagina exporteren in het dialoogvenster [!UICONTROL [!DNL Commerce] Admin]](assets/walmart-seller-account-full-setup-download.png)

   Gebruik filters om de kenmerkwaarden te selecteren en te configureren die van toepassing zijn op de productcategorieën waarin u verkoopt. Zorg ervoor dat u de vereiste en aanbevolen kenmerken van Walmart opneemt (zie [Gegevens exporteren](https://docs.magento.com/user-guide/system/data-export.html) in de Adobe [!DNL Commerce] Gebruikershandleiding voor gedetailleerde instructies.)

   Als u een kenmerk wilt weglaten uit het exportbestand, selecteert u de optie [!UICONTROL **Uitsluiten**] Schakel het selectievakje aan het begin van de rij in.

1. Naar het einde van de tabel met kenmerken bladeren en [!UICONTROL **Doorgaan**] om de gegevensexport te starten.

   Het CSV-exportbestand wordt verwerkt via een wachtrij met snijtaken en opgeslagen in de `var/export/folder`. (Zie [Berichtenrijen beheren](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) in de *Handleiding voor ontwikkelaars van handel*.)

1. Open het malplaatje van Excel voor de het productcategorie van de Marketplace van de Markt van de Markt, en gebruik de macromogelijkheden van Excel om de uitgevoerde productgegevens in het malplaatje van Excel samen te voegen.

1. Upload het Excel-bestand met de geëxporteerde productgegevens.

   - Terug naar de pagina Items in de productcatalogus in het dialoogvenster [Walmart Seller Center](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - Selecteren [!UICONTROL **Items toevoegen** > **Objecten bulksgewijs toevoegen**].
   - Sleep de voltooide spreadsheet aan de Upload sectie.
   - Selecteren [!UICONTROL **Verzenden**].
   - Selecteer [!UICONTROL  **Activiteitsfeed**] om de voortgang te bekijken.

Voor volledige instructies, zie [Items in bulk toevoegen met de specificaties Volledig item](https://sellerhelp.walmart.com/s/guide?article=000007680) in de [!DNL *Help bij Walmart Seller*].
