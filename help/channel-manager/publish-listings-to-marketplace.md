---
title: Aanbiedingen publiceren naar Walmart
description: Publiceer aanbiedingen voor Commerce-producten naar Walmart Marketplace om te beginnen met verkopen.
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: a10ab3f7fa7049e48d83a942f6c5441d8147b12c
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Aanbiedingen publiceren naar Walmart

Net als andere markten biedt Walmart verkopers van derden de mogelijkheid om objecten aan te bieden die door anderen worden verkocht.

Het platform gebruikt product-id&#39;s zoals UPC en GTIN om overeen te komen met items die al te koop zijn.
Voor gematchte producten wordt de bestaande lijst van de Marketplace van het Markeren bijgewerkt om de het productaanbod van de Handel te omvatten.

Doorgaans komen producten met de laagste prijzen eerst voor in de resultaten, maar andere factoren zoals recensies beïnvloeden ook de plaatsing.

## Producten afstemmen

Wanneer u producten aanpast, stuurt de Manager van het Kanaal de productgegevens naar Marketplace van de Markt van de Markt van de Markt om naar bestaande lijsten met attributenwaarden te zoeken die de in kaart gebrachte het productattribuut van de Handel aanpassen. Overeenkomstcriteria worden bepaald door de [kenmerktoewijzingsconfiguratie](map-product-attributes-for-matching.md) voor uw winkelkanaal.

Als er een overeenkomst wordt gevonden, wordt de bestaande productaanbieding bijgewerkt en wordt je voorstel toegevoegd.

### Vereisten

Alvorens producten aan te passen, verifieer dat uw de attributenwaarden van de productcatalogus voldoen aan de vereisten van het Martard en attributenmontages vormen. Zie [Productovereenkomst configureren](map-product-attributes-for-matching.md)

#### Producten selecteren en afstemmen

1. Open een verbonden verkoopkanaal.

1. Van **[!UICONTROL Listings]**, selecteer de producten die overeenkomen met de producten in *[!UICONTROL Draft]* status.

   ![Producten uit aanbiedingen selecteren en verzenden voor overeenkomst](assets/products-in-marketplace-sales-channel.png)

1. Selecteren **[!UICONTROL Match Products]**.

   Een bericht geeft het aantal producten aan dat voor matching is verzonden.

   ![Producten naar het verbonden verkoopkanaal verzenden](assets/products-submit-for-matching.png)

   De status van geselecteerde producten verandert in [!UICONTROL *Verwerking*] totdat de overeenkomende bewerking is voltooid. Het kan tot 30 minuten voor Walmart Marketplace duren om de gelijke verrichting te voltooien.

### Overeenkomststatus controleren

1. Selecteren **Producten vernieuwen** om de meest recente productstatus bij te werken.

1. Controleer de productstatus.

   Nadat de overeenkomst is voltooid, kan de status *Overeenkomst* of *Fout*.

   * **[!UICONTROL Match]** geeft aan dat het product is gevonden. Je productaanbod is gepubliceerd naar een bestaande Walmart Marketplace-aanbieding.

   * **[!UICONTROL Error]** Hiermee wordt een van de volgende items aangegeven:

      * Er is een fout opgetreden en de overeenkomende bewerking is mislukt.

      * Er is geen overeenkomst gevonden.

      * Overeenkomst gevonden, maar product gepubliceerd als gefaseerd omdat [Marktarchief is niet actief](walmart-prerequisites.md#walmart-marketplace-store-status).

### Aanbieding controleren op Walmart

Nadat je producten hebt gevonden, kun je de bijgewerkte productlijst bekijken en de productgegevens, prijs en voorraadhoeveelheid van de [[!UICONTROL Walmart Marketplace Seller Account Items] dashboard](https://seller.walmart.com/items-and-inventory/manage-items) om het bijgewerkte product te beoordelen.

### Problemen met overeenkomende productfouten oplossen

Als de verrichting van de productgelijke ontbreekt, keert de Marketplace van de Markt van de Markeren een foutencode terug en de Manager van het Kanaal toont de foutenstatus in de informatie van de productlijst.

Geef de details van foutberichten weer door de muisaanwijzer op de knop **Fout** statuslabel. Gangbare geretourneerde fouten zijn onjuist opgemaakte product-id-waarden of ontbrekende vereiste kenmerken.

#### ID-waarden van product corrigeren

| Type | Beschrijving | Voorbeeld |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, het 12-cijferige getal inclusief controlecijfer. </br></br>Als uw UPC minder dan 12 cijfers, zoals UPC-E heeft die 8 cijfers is, voeg beëindigende nullen toe om aan het vereiste te voldoen. | Wijzigen van `45678912345` tot `045678912345` |
| GTIN | GTIN-14, het 14-cijferige getal inclusief controlecijfer. </br></br>Als de GTIN uit minder dan 14 cijfers bestaat, voegt u voorloopnullen toe </br>om aan deze eis te voldoen. | Wijzigen `456789123456` tot `0045678912345` |
| EAN | GTIN-13, het 13-cijferige getal inclusief controlecijfer. </br></br>Als uw EAN minder dan 13 cijfers heeft, voeg belangrijke </br>nullen om aan de vereiste te voldoen. | Wijzigen van `4567891234` tot `0004567891234` |

Voor meer informatie over de foutcodes van Walmart Marketplace raadpleegt u de [Help bij Walmart Seller](https://sellerhelp.walmart.com/s/guide?article=000005844).

## Nieuwe productaanbiedingen uploaden

Voor producten die geen gelijke op Marketplace hebben, gebruik een sjabloon van de de productcategorie van het Walmart product Excel om productaanbiedingen bulksgewijs te uploaden. U bevolkt het malplaatje van de Marm gebruikend de gegevens van de productcatalogus die van uw instantie van de Handel worden uitgevoerd.

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

* Controleren of u voldoet aan de [Walmart-voorwaarden](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.k2lo9voad1gx).

* Controleer in uw productcatalogus van de Handel of de catalogusconfiguratie voor de producten die op de Walmart Marketplace worden aangeboden, alle vereiste kenmerken heeft en voldoet aan de richtlijnen voor Inhoud van de Marketplace van het type Walmart.

* Controleer of de uitsnijdtaak wordt uitgevoerd om de exportbewerking te voltooien.

   * Zie voor informatie op locatie [Uitsnede configureren en uitvoeren](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   * Voor Adobe cloud-infrastructuur raadpleegt u [Uitsnijdtaken instellen](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### Het te uploaden productgegevensbestand maken

1. Van uw [Walmart-verkopersaccount](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), download een productaanbiedingstemplate via het Walmart-winkelcentrum.

   * Selecteer op de pagina Items in productcatalogus de optie **[!UICONTROL Add Items]**. Selecteer vervolgens **[!UICONTROL Add items in bulk]**.

      ![Voeg punten in bulkoptie toe optie in de het puntconfiguratie van de Marketplace van de Markeren](assets/walmart-seller-account-add-items-bulk.png)

   * Selecteer op de downloadpagina de optie **[!UICONTROL Full Setup]**. Selecteer vervolgens een objectcategorie en download de rubrieksjabloon.

      ![Categoriesjabloonoptie downloaden in de configuratie van items in de Marketplace-indeling van het programma](assets/walmart-seller-account-full-setup-download.png)

   * Controleer of de sjabloon de vereiste en aanbevolen kenmerken voor de productaanbieding bevat.

1. Van de [!DNL Commerce] Beheer, selecteer de productgegevens die u wilt exporteren van uw Adobe Commerce-site.

   * Selecteer bij Beheer de optie [!UICONTROL **Systeem** > Gegevensoverdracht > **Exporteren**].

   * Op de [!UICONTROL Export] pagina in de [!UICONTROL Entity Type] veld, selecteren [!UICONTROL **Producten**].

   * In de [!UICONTROL Entity Attributes] de lijst, vormt de selectiecriteria voor de uitvoer van productgegevens.
   ![De productgegevenspagina exporteren in het dialoogvenster [!UICONTROL Commerce Admin]](assets/walmart-seller-account-full-setup-download.png)

   Gebruik filters om de kenmerkwaarden te selecteren en te configureren die van toepassing zijn op de productcategorieën waarin u verkoopt. Zorg ervoor dat u de vereiste en aanbevolen kenmerken van Walmart opneemt (zie [Gegevens exporteren](https://docs.magento.com/user-guide/system/data-export.html) in de Adobe Commerce-gebruikershandleiding voor gedetailleerde instructies.)

   Als u een kenmerk wilt weglaten uit het exportbestand, selecteert u de optie [!UICONTROL **Uitsluiten**] Schakel het selectievakje aan het begin van de rij in.

1. Naar het einde van de tabel met kenmerken bladeren en [!UICONTROL **Doorgaan**] om de gegevensexport te starten.

   Het CSV-exportbestand wordt verwerkt via een wachtrij met snijtaken en opgeslagen in de `var/export/folder`. (Zie [Berichtenrijen beheren](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) in de *Handleiding voor ontwikkelaars van handel*.)

1. Open het malplaatje van Excel voor de het productcategorie van de Marketplace van de Markt van de Markt, en gebruik de macromogelijkheden van Excel om de uitgevoerde productgegevens in het malplaatje van Excel samen te voegen.

1. Upload het Excel-bestand met de geëxporteerde productgegevens.

   * Terug naar de pagina Items in de productcatalogus in het dialoogvenster [Walmart Seller Center](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   * Selecteren [!UICONTROL **Items toevoegen** > **Objecten bulksgewijs toevoegen**].
   * Sleep de voltooide spreadsheet aan de Upload sectie.
   * Selecteren [!UICONTROL **Verzenden**].
   * Selecteer [!UICONTROL  **Activiteitsfeed**] om de voortgang te bekijken.

Voor volledige instructies, zie [Items in bulk toevoegen met de specificaties Volledig item](https://sellerhelp.walmart.com/s/guide?article=000007680) in de [!DNL *Help bij Walmart Seller*].
