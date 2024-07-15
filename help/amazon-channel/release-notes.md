---
title: '[!DNL Amazon Sales Channel] opmerkingen bij de release'
description: Herzie de versienota's voor informatie over alle  [!DNL Amazon Sales Channel]  versies.
feature: Sales Channels, Release Notes
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df8bbec23d34b53a0e694c924aca5b1ed41e4d08
workflow-type: tm+mt
source-wordcount: '2010'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] releaseopmerkingen

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] kan op instanties met Magento Open Source, Adobe Commerce en Adobe Commerce worden geïnstalleerd op versie 2.3.x en 2.4.x van de wolkeninfrastructuur. De extensie wordt niet meer ondersteund op Adobe Commerce 2.1, Magento Open Source 2.2 of Magento 1.
> <br>Ondersteuning is alleen beschikbaar voor [!DNL Amazon sales channel] versies 4.0.0 en 4.1.0 in Adobe Commerce 2.3.x-versies.
> <br>[!DNL Amazon sales channel] versie 4.2.0+ is compatibel met Adobe Commerce 2.3.x-versies, maar ondersteuning is alleen beschikbaar voor Adobe Commerce 2.4.x-versies.
>

Deze releaseopmerkingen beschrijven de eerste versie van [!DNL Amazon sales channel] en bevatten:

![ Nieuwe ](../assets/new.svg) Nieuwe eigenschappen
![ Vaste kwestie ](../assets/fix.svg) Oplossingen en verbeteringen
![ Bekende kwestie ](../assets/bug.svg) Bekende kwesties

Zie [ Komende Versies ](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) voor versioning, steun, en verenigbaarheid.

Zie [ Beschikbaarheid van het Product ](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) om te leren welke versies van Adobe Commerce deze uitbreiding steunen.

## v4.5.0

*Augustus 30, 2023*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Nieuw ](../assets/new.svg) voegde de gateway Adobe.IO API, die van MAGI verandert, voor betere authentificatieveiligheid toe. `ServicesId` verstrekt een nieuwe UI om uw geloofsbrieven te beheren Adobe.IO, gelijkend op andere [ de Diensten van Adobe Commerce ](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html).

>[!NOTE]
>
>De handelaren moeten ervoor zorgen dat de [ privé en openbare API sleutels ](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html) voor productie worden bijgewerkt.


![ Vaste kwestie ](../assets/fix.svg) identificeerde een configuratie plaatsende kwestie en bevond de stroom van de ordeverwezenlijking.

## v4.4.4

*Maart 7, 2023*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Vaste kwestie ](../assets/fix.svg) Toegevoegde steun voor Adobe Commerce 2.4.6 en PHP 8.2.

![ Vaste kwestie ](../assets/fix.svg) Verminderde lawaai in logboeken.

![ Vaste kwestie ](../assets/fix.svg) Verbeterde stabiliteit van het trekken van updates.

![ Vaste kwestie ](../assets/fix.svg) vereenvoudigde het proces voor het runnen van enige actie-als trekkracht of voor het toepassen van van CLI.

![ Vaste kwestie ](../assets/fix.svg) zette het gebiedsdeel voor `magento/services-connector` bij.

![ Vaste kwestie ](../assets/fix.svg) Vaste synchronisatiekwesties in de rekeningen van het VK met ongeldige landcode.

![ Vaste kwestie ](../assets/fix.svg) Hardcoded entity_type_id voor de entiteit van het catalogusproduct veroorzaakt kwesties met de Prijs van het Magento Source.

![ Vaste kwestie ](../assets/fix.svg) Correcteerde een kwestie die rekeningen verhinderde die op een achtergrond van een andere instantie ook van UI worden geschrapt.

![ Vaste kwestie ](../assets/fix.svg) een kwestie met sommige kartregels die ordeinvoer breken.

## v4.4.3

*Maart 7, 2023*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ bevestig ](../assets/fix.svg) Toegevoegde steun voor Adobe Commerce 2.4.4.

## v4.4.2

*11 november 2021*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ bevestig ](../assets/fix.svg) Bijgewerkte gebiedsdelen om andere bijgewerkte uitbreidingen te steunen.
![ bevestig ](../assets/fix.svg) Toegevoegde steun voor PHP 8.1.

## v4.4.1

*11 november 2021*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Repareren ](../assets/fix.svg) veranderde de manier Adobe Commerce het _3} gebied van de Naam van de Gebruiker van Amazon ontvangt._ Eerder, was er een fout tijdens ordeverwezenlijking wanneer het _gebied van de Naam van de Gebruiker_ speciale karakters bevatte. Adobe Commerce ontvangt nu de _gegevens en filters van de Naam van 0} Gebruiker uit de speciale karakters zodat kan de orde met succes worden gecreeerd._

## v4.4.0

*9 April, 2021*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](../assets/new.svg) Toegevoegde steun voor read-only Wijze aan de configuratie. Zie [ montages van het verkoopkanaal ](sales-channel-settings.md).

![ Repareren ](../assets/fix.svg) veranderde de gegevensstroom zodat de veelvoudige exemplaren van de zelfde instantie updates gelijktijdig kunnen halen.

![ Repareren ](../assets/fix.svg) veranderde het synchronisatieproces voor het synchroniseren van rekeningsinformatie. Er is een uitsnijdtaak toegevoegd voor synchronisatie met een externe account en dezelfde functionaliteit toegevoegd aan de CLI-opdrachten.

](../assets/fix.svg) Toegevoegde CLI bevelargumenten en vlaggen van 0} herstellen {voor nauwkeurigere controle.![

![ bevestig ](../assets/fix.svg) de Source van de AchtergrondTaken (brein) in de systeemconfiguratie.

![ Correctie ](../assets/fix.svg) de kwestie die de verwezenlijking van orden verhinderde toen de landcode aan Puerto Rico (PR) werd geplaatst.

## v4.3.0

*Maart 3, 2021*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Repareren ](../assets/fix.svg) <!--CHAN-xxxx--> de _eigenschap van de Details van de Orde_ is opnieuw ontworpen en baseert zich niet meer op het _plaatsen van de Orden van de Invoer_. De gegevens van de orde verschijnen nu in de interface van de Sales Channel van Amazon voor alle orden.

![ Repareren ](../assets/fix.svg) in het _[!UICONTROL Marketing]_menu in Admin, is de naam veranderd van_[!UICONTROL Amazon]_ in _[!UICONTROL Amazon Sales Channel]_.

![ Bekende kwestie ](../assets/bug.svg) **Belangrijk**: Bekende kwesties met Adobe Commerce 2.4.0 verenigbaarheid worden opgelost in Adobe Commerce 2.4.1 versie.

- Amazon-snijprocessen met de status `error`
- Installatie met Commerce 2.4.0 mislukt bij het maken van opslagruimten in de database
- Het maken van een product mislukt als MSI is geïnstalleerd

## v4.2.0

*Maart 3, 2021*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

Als u een eerdere [!DNL Amazon sales channel] -versie hebt geïnstalleerd en probeert uw Adobe Commerce bij te werken naar versie 2.4.0, wordt u gevraagd de extensie bij te werken voordat u de Adobe Commerce-update kunt voltooien.

![ Bekende kwestie ](../assets/bug.svg) wanneer [!DNL Amazon sales channel] 4.2.0 met versie 2.4.0 wordt geïntegreerd en [ Inventory management ](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en) wordt toegelaten, is er een bekende kwestie die de toevoeging van producten in uw catalogus van Commerce verhindert. Dit probleem wordt in een toekomstige Commerce-release opgelost.

![ Nieuw ](../assets/new.svg) [!DNL Amazon sales channel] is verbeterd om op tekst gebaseerde adresgegevens goed te keuren en het aan gestandaardiseerde adresformaten, met inbegrip van stad, staat, en postcode aan te passen. Met deze update kunnen bestellingen en verzendgegevens zonder adresfouten worden gesynchroniseerd (gesynchroniseerd) met Amazon.<br/> bijvoorbeeld, voert een verkoopster de stad, staat, postcode als `Escondido, californiA 92025-1501` in. Amazon-Sales Channel importeert de gegevens naar de standaardindeling `Escondido, CA 92025` en synchroniseert deze vervolgens terug naar Amazon in deze gestandaardiseerde indeling.

![ Nieuwe ](../assets/new.svg) Toegevoegde steun voor PHP 7.4.

![ Nieuwe ](../assets/new.svg) <!--CHAN-4334--> Toegevoegde steun voor Adobe Commerce 2.4.x. Eerdere versies zijn mogelijk compatibel met Commerce 2.4.x, maar worden niet ondersteund. Zie [ Komende versies ](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) voor versiecompatibiliteit. Amazon-Sales Channel moet worden bijgewerkt naar 4.2.0 voordat de Adobe Commerce 2.4.0-update kan worden voltooid.

![ Correctie ](../assets/fix.svg) <!--CHAN-4431--> een kwestie die _Ontkende Toegang_ fout voor klanten van het VK veroorzaakte.

![ bevestig ](../assets/fix.svg) <!--CHAN-4394--> een kwestie die de het verschepen status van Amazon aan de overeenkomstige orde van Commerce verhinderde te synchroniseren, zo &quot;vergrendelde&quot;de het verschepen status van de orde zoals `Pending` in Commerce en `Unshipped` in Amazon. Met de nieuwe gestandaardiseerde adresfunctie zijn deze verzendstatusfouten opgelost.

](../assets/fix.svg) verhelpen <!--ticket#--> bijgewerkte ordesynchronisatie (synchronisatie) om ontbroken ordeinvoer te negeren, waarbij veelvoudige synchronisatiepogingen worden verminderd en verdere invoer toe te staan om te verwerken, met de verzoeken van de ordesynchronisatie die om de vijf minuten worden voorgelegd. ![ De fouten van de synchronisatie worden nog geregistreerd in het foutenlogboek, maar duidelijk als &quot;verwerkt&quot;om verdere registrerenfuncties toe te staan. Bovendien verwijdert [!DNL Amazon sales channel] nu automatisch overtollige gegevens die zijn verzameld voor bestellingen die niet zijn gemaakt in Commerce.

![ bevestig ](../assets/fix.svg) Bijgewerkt foutenregistreren om meer informatie voor uncaught uitzondering en uitbreidingsupdatefouten te verzamelen.

![ Repareerde ](../assets/fix.svg) <!--ticket#--> een kwestie die de aanvankelijke synchronisatie van de _laagste prijs_ gegevens om wegens een ontbrekende _prijs_ waarde veroorzaakte te ontbreken.

](../assets/fix.svg) Correcte 1} <!--CHAN-4410--> kwesties die het filtreren fouten in de _Amazon orden_ mening veroorzaakte wanneer het gebied van de datumwaaier leeg wordt verlaten.![

![ bevestig ](../assets/fix.svg) <!--CHAN-4439--> een kwestie die op hoeveelheid betrekking hebbende voorraad en de fouten van de uitvoeringssynchronisatie veroorzaakte. Met de extensie worden nu de waarden voor het aantal tekens afgerond die zijn ingevoerd als een decimaal voordat ze worden gesynchroniseerd met Amazon.<br/> Wanneer een handelaar bijvoorbeeld handmatig een hoeveelheid `2.5` invoert, wordt de waarde door de extensie afgerond naar `2` en wordt de bijgewerkte hoeveelheid gesynchroniseerd met Amazon.

## v4.1.0

*7 Mei, 2020*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Nieuw ](../assets/new.svg) <!--4247, 4230--> veranderde het proces van de ordeinvoer om met de ordevereisten van Commerce te richten. Deze wijzigingen verhelpen problemen die ervoor zorgen dat Commerce de corresponderende volgorde voor een geïmporteerde order niet kan maken. Zie [ Orden ](managing-orders.md) voor informatie over ordeblokkers en oplossingen beheren.

![ Nieuw ](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324--> werkte de _Recente Orden_ sectie van het opslagdashboard bij en voegde een nieuwe _Alle Orden_ mening toe die al uw orden van Amazon, met inbegrip van filteropties en paginering voor het bekijken van meer orden toont. Zie [ het Dashboard van de Opslag van Amazon ](amazon-store-dashboard.md) en [ de Orden van Amazon van de Mening ](amazon-orders-all.md).

![ Nieuw ](../assets/new.svg) voegde de _[!UICONTROL Order Notes]_kolom van de opnieuw ontworpen_[!UICONTROL Amazon Orders]_ lijst in zowel _[!UICONTROL Recent Orders]_als_[!UICONTROL All Orders]_ meningen toe. _[!UICONTROL Order Notes]_laat de handelaar weten dat er een probleem is met de import van de order. Zie {de Orden van Amazon van 0} Mening ](amazon-orders-all.md).[

![ Nieuwe ](../assets/new.svg) <!--CHAN-4013--> bijgewerkte parameters van de productvoorwaarde om met [ Amazon te richten vernieuwde ](https://sell.amazon.com/programs/renewed) programma. Zie [ Vernieuwde Producten ](renewed-products.md).

![ Nieuwe ](../assets/new.svg) <!--CHAN-3680--> bijgewerkte [ de Details van de Orde van Amazon ](amazon-order-details.md) om &quot;generische gegevens&quot;voor orden te omvatten die door Amazon worden vervuld. Zie [ die door ](fulfilled-by.md) wordt gevuld.

![ Repareerde ](../assets/fix.svg) <!--CHAN-4069--> een kwestie die de vervorming van pictogrammen op de opslagkaart veroorzaakte.

![ Repareerde ](../assets/fix.svg) <!--CHAN-4165--> een fout die het _Login_ scherm verhinderde na de zittingstijden uit te verschijnen.

![ bevestig ](../assets/fix.svg) <!--CHAN-4211--> een kwestie verhinderde het de ordebelastingbedrag van Amazon in de nieuwe orde van Commerce in te voeren.

![ bevestig ](../assets/fix.svg) <!--CHAN-4234--> een kwestie die opbrengsttotalen veroorzaakte die op het opslagdashboard worden getoond om orden in `Canceled` of `Error` status te omvatten.

![ Repareerde ](../assets/fix.svg) <!--CHAN-4326--> een kwestie die orde invoerfouten verbonden aan derdeuitbreidingen veroorzaakte die _Magento Shipping_ methodes gebruiken om orden tot stand te brengen.

![ Repareer ](../assets/fix.svg) <!--CHAN-4357--> corrigeerde een kwestie die fouten wanneer het runnen van kroonsynchronisatie veroorzaakte. Een slot is toegevoegd op het CLI bevel dat twee kroonbanen verhindert tezelfdertijd te synchroniseren.

![ verbeter ](../assets/fix.svg) Bijgewerkt inhoudsveiligheidsbeleid voor steun met versie 2.3.5 van Commerce.

## v4.0.0

*Maart 25, 2020*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 wordt niet ondersteund voor Adobe Commerce 2.3.5. Upgrade naar Amazon Sales Channel 4.1.0 voor ondersteuning met Adobe Commerce 2.3.5.

![ Nieuw ](../assets/new.svg) introduceerde een nieuwe [ Sales Channel van Amazon ](amazon-sales-channel-home.md) homepage met betere &quot;kaartmening&quot;voor uw opslaginformatie.

![ Nieuw ](../assets/new.svg) introduceerde een nieuw [ opslagdashboard ](amazon-store-dashboard.md) met lijst, recente orden, en opslag plaatsende informatie.

![ Nieuw ](../assets/new.svg) introduceerde een eenvoudigere, gestroomlijnde [ onboarding proces ](amazon-onboarding-home.md) en [ standaard opslagmontages ](default-store-settings.md) om uw opslag te krijgen sneller geïntegreerd.

![ Bekende kwestie ](../assets/bug.svg) <!--CHAN-4102--> wanneer [ het creëren van attributen ](managing-attributes.md) voor het invoeren van beelden van lijsten en **de Bekende Mening van de Opslag** aan `All Store Views (Global)` wordt geplaatst, bestaat een bekende kwestie verhinderend beelden in alle opslagmeningen in te voeren. Als u het plaatsen voor **Mening van de Opslag verandert (om waarden in in) in te voeren** aan een specifieke opslag, de beeldinvoer voor die opslag.

## v3.0.1

*11 november 2019*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

](../assets/fix.svg) herstellen **** de Montages van het Numerieke Gebied ![ <!--CHAN-3779--> die een op numeric-based waarde vereisen zijn bijgewerkt om numerieke karakters slechts goed te keuren. Voorbeeld: Instellingen prijsregel > Veld Aanpassingsbedrag

](../assets/fix.svg) herstellen **de Verbindingen van de Gids van de Gebruiker**: <!--CHAN-3778--> Onjuiste _Gids van de Gebruiker_ de verbindingen zijn verbeterd.![

](../assets/fix.svg) **Duidelijke Lijsten van Amazon** herstellen: <!--CHAN-3593--> A eerder gemelde kwestie die dubbele lijsten van Amazon veroorzaakt wordt nu verbeterd. ![ Vóór deze release werd bij het importeren van aanbiedingen de landcode voor het Amazon-gebied toegevoegd aan SKU-waarden. De lijst kwam met het cataloguspunt overeen, maar de uitbreiding leidde tot een nieuwe, dubbele lijst met toegevoegde SKU. Met deze release wijzigt de extensie de SKU voor geïmporteerde aanbiedingen niet en worden er geen wijzigingen aangebracht in bestaande aanbiedingen. Met de optie [!UICONTROL End Listing(s)] Op Amazon kunt u dubbele aanbiedingen verwijderen.

## v3.0.0

*7 Oktober, 2019*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](../assets/new.svg) **nu Beschikbare Marketplace van Amazon UK**: De gebruikers kunnen de markt van het Verenigd Koninkrijk kiezen wanneer het creëren van en het integreren van een opslag van Commerce. Deze upgrade naar het Verenigd Koninkrijk biedt extra ondersteuning voor:

- [ de Dienst van de Berekening van de BTW Amazon ](https://sell.amazon.co.uk/learn/vat-resources) {target="_blank"}

- ](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US) {target="_blank"} informatie van de Code van de Belasting van het 0} Product {.[

![ Nieuw ](../assets/new.svg) **Verbeterde het Registreren**: <!--CHAN-3642, 3672--> Geïmporteerde **laat Debug het Registreren** eigenschap toe om extra synchronisatiegegevens te verzamelen wanneer het oplossen van problemen nodig is. Zie het [ onderwerp van de Montages van Sales Channel ](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html) in de Verwijzing van de Configuratie.

![ bevestig ](../assets/fix.svg) **Catalogus van het Product**: <!--CHAN-3687--> Correcte een kwestie die beelden die met een lijst van Amazon werden ingevoerd verhinderde worden toegepast op het overeenkomstige de catalogusproduct van Commerce.

![ verbeter ](../assets/fix.svg) **creatie van de Orde**: <!--CHAN-3708--> Correcteerde een kwestie die Commerce verhinderde orden voor een orde van Amazon tot stand te brengen die niet met een de catalogusproduct van Commerce aanpast.

![ Bekende kwestie ](../assets/bug.svg) **dupliceert de Lijsten van Amazon**: <!--CHAN-3593--> Deze kwestie veroorzaakt de catalogus om een punt voor een ingevoerde lijst tot stand te brengen, gebruikend zelfde SKU maar met een gebiedscode die op het eind wordt toegevoegd. Amazon verwerkt de gewijzigde SKU vervolgens als een nieuw object en maakt een aanbieding. Dit probleem zal in een toekomstige release worden opgelost.

## v2.0.0

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

>[!NOTE]
>
>Versie 1.0.0 was alleen beschikbaar in beperkte versie.

![ Nieuw ](../assets/new.svg) **Vereenvoudigd Onboarding en Onderhoud**: voeg en integreer met uw rekening van de Verkoper van Amazon door een geleidelijke proces met gedetailleerde instructies beschikbaar door Admin toe. Houd uw winkels, accounts en producten die u hebt aangeboden via één dashboard bij.

![ Nieuwe ](../assets/new.svg) **Veelvoudige Steun van de Rekening**: beheer en controleer veelvoudige merken Amazon en marktplaatsgebieden door Admin.

![ Nieuwe ](../assets/new.svg) **Intelligente Prijsstelling**: Plaats geautomatiseerde het opnieuw bepalen regels om uw kansen voor de behandelde Buy Box te verhogen. Prijzen instellen om zich dynamisch aan te passen aan de huidige prijs van Buy Box, of de laagste prijs van de concurrent. Stel limieten in voor de prijsaanpassing om je marge te beschermen.

![ Nieuw ](../assets/new.svg) **het Lijstbeheer**: Automatiseer productlijsten en synchroniseer uw catalogus van Commerce aan de Marketplace van Amazon gebruikend lijstregels. Voeg specifieke overschrijvingen toe om uw aanbod nauwkeurig te regelen. Al je aanbiedingen rechtstreeks vanuit de beheerder volgen en beheren.

![ Nieuwe ](../assets/new.svg) **Consistente Inventory management**: houd uw Commerce en Amazon inventarishoeveelheden in constante synchronisatie.

![ Nieuw ](../assets/new.svg) **de Orde en het Beheer van de Uitvoering**: De orden van Amazon van het spoor door het dashboard, met naadloze mededeling en inventarisupdates. Volledige en trackbestelling die door Amazon wordt uitgevoerd, waaraan de handelaar heeft voldaan of een combinatie van methoden.

![ Bekende kwestie ](../assets/bug.svg) u kunt langere wachttijden ontmoeten om producthoeveelheden bij te werken. Het synchroniseren van updates voor het aantal producten kan ~twee uur duren.

![ Bekende kwestie ](../assets/bug.svg) Geïmporteerde orden kunnen een type van _eerste_ of _Premium_ orden hebben. Je moet deze bestellingen verifiëren in je Amazon-verkopersaccount.

![ Bekende kwestie ](../assets/bug.svg) De Niet in aanmerking komende gebundelde producten kunnen als In aanmerking komend voor lijst op Amazon tonen. Een van de producten in het gebundelde product is mogelijk niet in aanmerking komende producten. Als u problemen ondervindt, controleert u de geschiktheidsstatus voor gebundelde producten.

![ Bekende kwestie ](../assets/bug.svg) wanneer het gebruiken van Inventory management voor Commerce 2.3.x, kan een gedeeltelijke voorraadherdex niet teweegbrengen wanneer een orde wordt gecreeerd. De verkoopbare hoeveelheid wordt per uur opnieuw berekend, waardoor tijdens dit update-interval oververkopen kan optreden.
