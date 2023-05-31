---
title: '''[!DNL Amazon Sales Channel] opmerkingen vrijgeven'
description: Lees de opmerkingen bij de release voor meer informatie over alle [!DNL Amazon Sales Channel] lozingen.
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '1933'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] releaseopmerkingen

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] kan worden geïnstalleerd op instanties met Magento Open Source, Adobe Commerce en Adobe Commerce op versie 2.3.x en 2.4.x van de wolkeninfrastructuur. De extensie wordt niet meer ondersteund in Adobe Commerce 2.1, Magento Open Source 2.2 of Magento 1.
> <br>Ondersteuning is beschikbaar voor [!DNL Amazon sales channel]  Alleen versies 4.0.0 en 4.1.0 op Adobe Commerce 2.3.x.
> <br>[!DNL Amazon sales channel] versie 4.2.0+ is compatibel met Adobe Commerce 2.3.x-versies, maar ondersteuning is alleen beschikbaar voor Adobe Commerce 2.4.x-versies.

In deze releaseopmerkingen wordt de eerste release van [!DNL Amazon sales channel] en omvatten:

![Nieuw](../assets/new.svg) Nieuwe functies
![Probleem opgelost](../assets/fix.svg) Oplossingen en verbeteringen
![Bekend probleem](../assets/bug.svg) Bekende problemen

Zie [Volgende releases](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) voor versioning, ondersteuning en compatibiliteit.

## v4.4.4

*7 maart 2023*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Probleem opgelost](../assets/fix.svg) Extra ondersteuning voor Adobe Commerce 2.4.6 en PHP 8.2.

![Probleem opgelost](../assets/fix.svg) Minder ruis in logboeken.

![Probleem opgelost](../assets/fix.svg) Verbeterde stabiliteit bij het ophalen van updates.

![Probleem opgelost](../assets/fix.svg) Vereenvoudigd het proces voor het runnen van enige actie-als trekkracht of voor het toepassen van van CLI.

![Probleem opgelost](../assets/fix.svg) Bijgewerkt gebiedsdeel voor `magento/services-connector`.

![Probleem opgelost](../assets/fix.svg) Correctie van problemen met synchronisatie in Britse accounts met ongeldige landcode.

![Probleem opgelost](../assets/fix.svg) Hardcoded entity_type_id for catalog product entity cause issues with Magento Price Source.

![Probleem opgelost](../assets/fix.svg) Correctie een kwestie verhinderend rekeningen die op een achtergrond van een andere instantie worden geschrapt van UI eveneens.

![Probleem opgelost](../assets/fix.svg) Probleem verholpen met bepaalde regels voor winkelwagentjes die het importeren van bestellingen verbreken.

## v4.4.3

*7 maart 2023*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Repareren](../assets/fix.svg) Extra ondersteuning voor Adobe Commerce 2.4.4.

## v4.4.2

*11 november 2021*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Repareren](../assets/fix.svg) Bijgewerkte afhankelijkheden ter ondersteuning van andere bijgewerkte extensies.
![Repareren](../assets/fix.svg) Toegevoegde ondersteuning voor PHP 8.1.

## v4.4.1

*11 november 2021*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Repareren](../assets/fix.svg) De manier waarop Adobe Commerce de _Gebruikersnaam_ veld uit Amazon. Er is eerder een fout opgetreden tijdens het maken van de bestelling toen de _Gebruikersnaam_ veld bevat speciale tekens. Adobe Commerce ontvangt nu de _Gebruikersnaam_ gegevens en filters uit de speciale karakters zodat kan de orde met succes worden gecreeerd.

## v4.4.0

*9 april 2021*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Nieuw](../assets/new.svg) Toegevoegde steun voor read-only Wijze aan de configuratie. Zie [verkoopkanaalinstellingen](sales-channel-settings.md).

![Repareren](../assets/fix.svg) De gegevensstroom is gewijzigd, zodat meerdere kopieën van dezelfde instantie gelijktijdig updates kunnen ophalen.

![Repareren](../assets/fix.svg) Het synchronisatieproces voor het synchroniseren van accountgegevens is gewijzigd. Er is een uitsnijdtaak toegevoegd voor synchronisatie met een externe account en dezelfde functionaliteit toegevoegd aan de CLI-opdrachten.

![Repareren](../assets/fix.svg) Toegevoegde CLI bevelargumenten en vlaggen voor nauwkeurigere controle.

![Repareren](../assets/fix.svg) Correcteerde de Bron van de Taken van de Achtergrond (kroon) in de systeemconfiguratie.

![Repareren](../assets/fix.svg) Correctie van het probleem dat het aanmaken van orders verhinderde toen de landcode op Puerto Rico (PR) werd ingesteld.

## v4.3.0

*3 maart 2021*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Repareren](../assets/fix.svg) <!--CHAN-xxxx-->De _Bestelgegevens_ is opnieuw ontworpen en is niet meer afhankelijk van de _Orders importeren_ instellen. De gegevens van de orde verschijnen nu in de interface van de Sales Channel van Amazon voor alle orden.

![Repareren](../assets/fix.svg) In de _[!UICONTROL Marketing]_in Beheer is de naam gewijzigd van_[!UICONTROL Amazon]_ tot _[!UICONTROL Amazon Sales Channel]_.

![Bekend probleem](../assets/bug.svg) **Belangrijk**: Bekende problemen met Adobe Commerce 2.4.0-compatibiliteit worden opgelost in de Adobe Commerce 2.4.1-release.

- Amazon-snijprocessen in `error` state
- Installatie met Commerce 2.4.0 mislukt bij het maken van opslagruimten in de database
- Het maken van een product mislukt als MSI is geïnstalleerd

## v4.2.0

*3 maart 2021*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

Als u een [!DNL Amazon sales channel] geïnstalleerde versie en poging om uw Adobe Commerce bij te werken naar versie 2.4.0, wordt u gevraagd de extensie bij te werken voordat u de Adobe Commerce-update kunt voltooien.

![Bekend probleem](../assets/bug.svg) Wanneer [!DNL Amazon sales channel] 4.2.0 is geïntegreerd met versie 2.4.0 en [Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en) is ingeschakeld, is er een bekend probleem dat het toevoegen van producten in uw handelscatalogus verhindert. Deze kwestie zal in een toekomstige mededeling van de Handel worden behandeld.

![Nieuw](../assets/new.svg) [!DNL Amazon sales channel] is verbeterd voor het accepteren van op tekst gebaseerde adresgegevens en het aanpassen aan gestandaardiseerde adresnotaties, zoals plaats, provincie en postcode. Met deze update kunnen bestellingen en verzendgegevens zonder adresfouten worden gesynchroniseerd (gesynchroniseerd) met Amazon.<br/>Een winkelier voert bijvoorbeeld de plaats, de staat en de postcode in als `Escondido, californiA 92025-1501`. Amazon Sales Channel importeert en stemt overeen met de standaardnotatie `Escondido, CA 92025`en synchroniseert het vervolgens terug naar Amazon in deze gestandaardiseerde indeling.

![Nieuw](../assets/new.svg) Extra ondersteuning voor PHP 7.4.

![Nieuw](../assets/new.svg) <!--CHAN-4334-->Extra ondersteuning voor Adobe Commerce 2.4.x. Eerdere versies zijn mogelijk compatibel met Commerce 2.4.x, maar worden niet ondersteund. Zie [Volgende releases](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) voor versiecompatibiliteit. Amazon Sales Channel moet worden bijgewerkt naar 4.2.0 voordat de Adobe Commerce 2.4.0-update kan worden voltooid.

![Repareren](../assets/fix.svg) <!--CHAN-4431-->Correctie van een probleem dat een _Toegang geweigerd_ fout voor klanten in het Verenigd Koninkrijk.

![Repareren](../assets/fix.svg) <!--CHAN-4394-->Correctie van een probleem waardoor de verzendstatus van Amazon niet kon worden gesynchroniseerd met de corresponderende handelsorder, waardoor de verzendstatus van de order als &quot;vergrendeld&quot; werd `Pending` in de handel en `Unshipped` in Amazon. Met de nieuwe gestandaardiseerde adresfunctie zijn deze verzendstatusfouten opgelost.

![Repareren](../assets/fix.svg) <!--ticket#-->De bijgewerkte synchronisatie van de orde (synchronisatie) om ontbroken ordeinvoer te negeren, waarbij veelvoudige synchronisatiepogingen worden verminderd en verdere invoer toe te staan om te verwerken, met de verzoeken van de ordesynchronisatie die om de vijf minuten worden voorgelegd. De fouten van de synchronisatie worden nog geregistreerd in het foutenlogboek, maar duidelijk als &quot;verwerkt&quot;om verdere registrerenfuncties toe te staan. Ook, [!DNL Amazon sales channel] verwijdert nu automatisch overtollige gegevens die voor orden worden verzameld die er niet in slagen om in de Handel tot stand te brengen.

![Repareren](../assets/fix.svg) Bijgewerkte foutenregistratie om meer informatie voor uncaught uitzondering en de fouten van de uitbreidingsupdate te verzamelen.

![Repareren](../assets/fix.svg) <!--ticket#-->Correctie van een probleem dat de eerste synchronisatie van de _laagste prijs_ gegevens die moeten mislukken omdat een _prijs_ waarde.

![Repareren](../assets/fix.svg) <!--CHAN-4410-->Correctie van problemen die filterfouten in de _Amazon-orders_ weergeven wanneer het veld voor het datumbereik leeg blijft.

![Repareren](../assets/fix.svg) <!--CHAN-4439-->Correctie van een probleem dat fouten met betrekking tot de voorraad en de uitvoeringssync veroorzaakte. Met de extensie worden nu de waarden voor het aantal decimalen weergegeven voordat ze met Amazon worden gesynchroniseerd.<br/> Wanneer een handelaar bijvoorbeeld handmatig een hoeveelheid van `2.5`, wordt de waarde met de extensie omlaag gedraaid naar `2` en synchroniseert de bijgewerkte hoeveelheid vervolgens met Amazon.

## v4.1.0

*7 mei 2020*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Nieuw](../assets/new.svg) <!--4247, 4230-->Veranderde het proces van de ordeinvoer om zich aan de ordevereisten van de Handel te richten. Met deze wijzigingen worden problemen verholpen die ertoe hebben geleid dat de handel de corresponderende volgorde voor een geïmporteerde order niet kon maken. Zie [Bestellingen beheren](managing-orders.md) voor informatie over orderblokkers en oplossingen.

![Nieuw](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->De _Recente bestellingen_ sectie van het opslagdashboard en toegevoegd een nieuwe _Alle bestellingen_ een weergave waarin al uw Amazon-bestellingen worden weergegeven, inclusief filteropties en paginering voor het weergeven van meer bestellingen. Zie [Amazon Store Dashboard](amazon-store-dashboard.md) en [Amazon-bestellingen weergeven](amazon-orders-all.md).

![Nieuw](../assets/new.svg) De _[!UICONTROL Order Notes]_kolom van het opnieuw ontworpen_[!UICONTROL Amazon Orders]_ tabel in beide _[!UICONTROL Recent Orders]_en_[!UICONTROL All Orders]_ weergaven. _[!UICONTROL Order Notes]_de handelaar te laten weten dat er een probleem is met de invoer van de order . Zie [Amazon-bestellingen weergeven](amazon-orders-all.md).

![Nieuw](../assets/new.svg) <!--CHAN-4013-->Bijgewerkte parameters voor de productvoorwaarde die moeten worden uitgelijnd met de [Amazon vernieuwd](https://sell.amazon.com/programs/renewed) programma. Zie [Vernieuwde producten](renewed-products.md).

![Nieuw](../assets/new.svg) <!--CHAN-3680-->Bijgewerkt [Amazon-bestellingsgegevens](amazon-order-details.md) &quot;generieke gegevens&quot; op te nemen voor orders die door Amazon worden uitgevoerd. Zie [Betaald door](fulfilled-by.md).

![Repareren](../assets/fix.svg) <!--CHAN-4069-->Correctie van een probleem dat de vervorming van pictogrammen op de winkelkaart veroorzaakte.

![Repareren](../assets/fix.svg) <!--CHAN-4165-->Correctie van een fout die de _Aanmelden_ scherm verschijnt na de sessietijden uit.

![Repareren](../assets/fix.svg) <!--CHAN-4211-->Correctie van een probleem waardoor de bestellingsbelasting van Amazon niet in de nieuwe handelsorder kon worden ingevoerd.

![Repareren](../assets/fix.svg) <!--CHAN-4234-->Correctie een kwestie die opbrengsttotalen veroorzaakte die op het opslagdashboard worden getoond om orden in te omvatten `Canceled` of `Error` status.

![Repareren](../assets/fix.svg) <!--CHAN-4326-->Correctie van een probleem dat fouten met het importeren van orders veroorzaakte die waren gekoppeld aan extensies van derden die gebruikten _Magento Shipping_ methoden om orders te maken.

![Repareren](../assets/fix.svg) <!--CHAN-4357-->Correctie van een probleem dat fouten veroorzaakte bij het uitvoeren van de kroonsynchronisatie. Een slot is toegevoegd op het CLI bevel dat twee kroonbanen verhindert tezelfdertijd te synchroniseren.

![Repareren](../assets/fix.svg) Bijgewerkt inhoudsveiligheidsbeleid voor steun met Versie 2.3.5 van de Handel.

## v4.0.0

*25 maart 2020*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 wordt niet ondersteund voor Adobe Commerce 2.3.5. Voor ondersteuning met Adobe Commerce 2.3.5 voert u een upgrade uit naar Amazon Sales Channel 4.1.0.

![Nieuw](../assets/new.svg) Nieuwe [Amazon Sales Channel](amazon-sales-channel-home.md) homepage met verbeterde &quot;kaartweergave&quot; voor je winkelgegevens.

![Nieuw](../assets/new.svg) Nieuwe [opslagdashboard](amazon-store-dashboard.md) met informatie over aanbiedingen, recente bestellingen en winkelinstellingen.

![Nieuw](../assets/new.svg) Introductie van een eenvoudigere, gestroomlijnde [onboarding](amazon-onboarding-home.md) en [standaardopslaginstellingen](default-store-settings.md) om uw winkels sneller te integreren.

![Bekend probleem](../assets/bug.svg) <!--CHAN-4102--> Wanneer [kenmerken maken](managing-attributes.md) voor het importeren van afbeeldingen uit aanbiedingen en **Winkelweergaven** is ingesteld op `All Store Views (Global)`Er is een bekend probleem dat voorkomt dat afbeeldingen worden geïmporteerd in alle winkelweergaven. Als u de instelling voor **Winkelweergaven (om waarden te importeren in)** naar een specifieke winkel, worden de afbeeldingen geïmporteerd voor die winkel.

## v3.0.1

*11 november 2019*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Repareren](../assets/fix.svg) **Instellingen numeriek veld**: <!--CHAN-3779-->Velden waarvoor een numerieke waarde nodig is, zijn bijgewerkt en bevatten alleen numerieke tekens. Voorbeeld: Instellingen voor prijsregel > veld Hoeveelheid aanpassing

![Repareren](../assets/fix.svg) **Koppelingen in gebruikershandleiding**: <!--CHAN-3778-->Onjuist _Handboek_ koppelingen zijn gecorrigeerd.

![Repareren](../assets/fix.svg) **Amazon-aanbiedingen dupliceren**: <!--CHAN-3593-->Een eerder gemelde uitgave die dubbele Amazon-aanbiedingen veroorzaakt, is nu gecorrigeerd. Vóór deze release werd bij het importeren van aanbiedingen de landcode voor het Amazon-gebied toegevoegd aan SKU-waarden. De lijst kwam met het cataloguspunt overeen, maar de uitbreiding leidde tot een nieuwe, dubbele lijst met toegevoegde SKU. Met deze release wijzigt de extensie de SKU voor geïmporteerde aanbiedingen niet en worden er geen wijzigingen aangebracht in bestaande aanbiedingen. U kunt de [!UICONTROL End Listing(s)] op Amazon om dubbele aanbiedingen te verwijderen.

## v3.0.0

*7 oktober 2019*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Nieuw](../assets/new.svg) **Amazon UK Marketplace Nu beschikbaar**: Gebruikers kunnen de markt van het Verenigd Koninkrijk kiezen bij het maken en integreren van een Commerce-winkel. Deze upgrade naar het Verenigd Koninkrijk biedt extra ondersteuning voor:

- [Amazon BTW-berekeningsservice](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [Productbelastingcode](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} informatie.

![Nieuw](../assets/new.svg) **Verbeterde logboekregistratie**: <!--CHAN-3642, 3672-->Geïmplementeerd **Foutopsporingsregistratie inschakelen** functie om aanvullende synchronisatiegegevens te verzamelen wanneer het oplossen van problemen nodig is. Zie de [Sales Channel-instellingen](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html) onderwerp in de Verwijzing van de Configuratie.

![Repareren](../assets/fix.svg) **Productcatalogus**: <!--CHAN-3687-->Correctie van een probleem dat ervoor zorgde dat afbeeldingen die met een Amazon-lijst zijn geïmporteerd, niet konden worden toegepast op het corresponderende product uit de handelscatalogus.

![Repareren](../assets/fix.svg) **Maken van bestelling**: <!--CHAN-3708-->Correctie van een probleem dat ervoor zorgde dat Commerce geen orders kon maken voor een Amazon-order die niet overeenkwam met een product uit de handelscatalogus.

![Bekend probleem](../assets/bug.svg) **Amazon-aanbiedingen dupliceren**: <!--CHAN-3593-->Deze kwestie veroorzaakt de catalogus om een punt voor een ingevoerde lijst tot stand te brengen, gebruikend zelfde SKU maar met een gebiedscode die op het eind wordt toegevoegd. Amazon verwerkt de gewijzigde SKU vervolgens als een nieuw object en maakt een aanbieding. Dit probleem zal in een toekomstige release worden opgelost.

## v2.0.0

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

>[!NOTE]
>
>Versie 1.0.0 was alleen beschikbaar in beperkte versie.

![Nieuw](../assets/new.svg)  **Vereenvoudigd on-boarding en onderhoud**: Voeg en integreer met uw Amazon-verkopersaccount toe via een stapsgewijs proces met gedetailleerde instructies die beschikbaar zijn via de beheerder. Houd uw winkels, accounts en producten die u hebt aangeboden via één dashboard bij.

![Nieuw](../assets/new.svg)  **Ondersteuning voor meerdere accounts**: Beheer en controleer meerdere Amazon-merken en -verkoopgebieden via de beheerfunctie.

![Nieuw](../assets/new.svg)  **Intelligente prijzen**: Stel automatische prijsstellingsregels in om de kans op de gekozen Buy Box te vergroten. Prijzen instellen om zich dynamisch aan te passen aan de huidige prijs van Buy Box, of de laagste prijs van de concurrent. Stel limieten in voor de prijsaanpassing om je marge te beschermen.

![Nieuw](../assets/new.svg)  **Aanbiedingsbeheer**: Automatiseer productaanbiedingen en synchroniseer je handelscatalogus met de Amazon Marketplace aan de hand van aanbiedingsregels. Voeg specifieke overschrijvingen toe om uw aanbod nauwkeurig te regelen. Al je aanbiedingen rechtstreeks vanuit de beheerder volgen en beheren.

![Nieuw](../assets/new.svg)  **Consistent Inventory management**: Houd je voorraad voor Handel en Amazon constant gesynchroniseerd.

![Nieuw](../assets/new.svg)  **Bestel- en uitvoeringsbeheer**: Houd Amazon-bestellingen bij via het dashboard, met naadloze communicatie en inventarisupdates. Volledige en trackbestelling die door Amazon wordt uitgevoerd, waaraan de handelaar heeft voldaan of een combinatie van methoden.

![Bekend probleem](../assets/bug.svg)  Er kunnen langere wachttijden optreden voor het bijwerken van de producthoeveelheden. Het synchroniseren van updates voor het aantal producten kan ~twee uur duren.

![Bekend probleem](../assets/bug.svg)  Geïmporteerde orders kunnen van het type _Eerste_ of _Premium_ bestellingen. Je moet deze bestellingen verifiëren in je Amazon-verkopersaccount.

![Bekend probleem](../assets/bug.svg)  Niet-subsidiabele gebundelde producten kunnen worden weergegeven als in aanmerking komend voor aanbieding op Amazon. Een van de producten in het gebundelde product is mogelijk niet in aanmerking komende producten. Als u problemen ondervindt, controleert u de geschiktheidsstatus voor gebundelde producten.

![Bekend probleem](../assets/bug.svg)  Bij gebruik van Inventory management for Commerce 2.3.x wordt een gedeeltelijke herindex van aandelen mogelijk niet geactiveerd wanneer een order wordt gemaakt. De verkoopbare hoeveelheid wordt per uur opnieuw berekend, waardoor tijdens dit update-interval oververkopen kan optreden.
