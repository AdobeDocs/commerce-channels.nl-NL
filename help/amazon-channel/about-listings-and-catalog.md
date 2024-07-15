---
title: Amazon en de Commerce-catalogus
description: Het verkoopkanaal van Amazon importeert je Amazon-aanbiedingen naar je Commerce-achtergrond en synchroniseert voortdurend met producten en verkopen.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services, Merchandising, Catalog Management
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Amazon en de [!DNL Commerce] -catalogus

Uw Adobe Commerce of Magento Open Source backend omvat een catalogus met alle producten en bijbehorende montages en informatie (beelden, opties, prijzen, en meer) en orde en verzendconfiguraties. Uw [!DNL Amazon Seller Central] -account heeft ook een catalogus en orderconfiguraties, waarbij uw verkoop strikt wordt gevolgd via [!DNL Amazon Marketplace] .

Om uw productcatalogus en verkoop beter te beheren en te bekijken via één locatie, importeert Amazon uw Amazon-aanbiedingen in uw [!DNL Commerce] -backend, synchroniseert deze voortdurend met producten en verkoop en rapporteert problemen en trends. Deze biedt ondersteuning voor integratie met meerdere [!DNL Amazon Seller Central] -accounts, waarbij alle gegevens door de enkele interface worden bijgehouden voor meerdere storefronts.

## Productkenmerken

Adobe Commerce en de Magento Open Source beheren catalogussyncs met het gebruik van product [ attributen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) om productmontages en gegevens te bepalen. Amazon gebruikt ook kenmerken die aan boord moeten worden gezet. Tijdens [ pre-opstellingstaken ](./amazon-pre-setup-tasks.md) voor de verkoopkanaal van Amazon, bepaalt u extra attributen van Amazon (indien nodig) om correcte productafbeeldingen te verzekeren wanneer het invoeren van uw aanbiedingen van Amazon in uw [!DNL Commerce] catalogus. Deze attributen omvatten UPC, EAN, ISBN, en ASIN ([!DNL Amazon Standard Identification Number]). Producten synchroniseren tussen Amazon- en [!DNL Commerce] -catalogi door uw kenmerken aan boord te nemen. Correcte mapping van uw [!DNL Commerce] - en Amazon-producten zorgt voor een continue synchronisatie van productinformatie, bestellingen en inventaris.

Als u deze attributen niet hebt die voor uw catalogus worden gecreeerd of worden gevormd, zou u a [!DNL Commerce] [ productattributen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) en waarden aan uw producten vóór het instappen moeten toevoegen. Wanneer een Amazon-kenmerk wordt geïmporteerd, kan het worden gebruikt voor zoeken, navigatie, prijsregels en nog veel meer. Zie [ wat ASIN, UPC, EAN, ISBN, SKU en Andere Streepjescodes betekenen?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number) {target="_blank"}

Na het instappen, kunt u uw productattributen en afbeeldingen van Amazon op elk ogenblik beheren en bijwerken.

## Productaanbiedingen

Een Amazon-aanbieding is een productpagina voor elk product dat u via [!DNL Amazon Marketplace] verkoopt. Hierin worden productbeschrijvingen, prijzen, afbeeldingen en meer via kenmerken in kaart gebracht. Tijdens het instappen kunt u configureren dat uw [!DNL Commerce] -producten automatisch worden gepubliceerd naar Amazon-aanbiedingen. U kunt uw bestaande Amazon-aanbiedingen ook importeren door deze toe te wijzen aan uw [!DNL Commerce] -producten.

Wanneer u een [!DNL Commerce] -aanbiedingsproduct hebt gemaakt, worden deze ter goedkeuring naar Amazon verzonden. De meeste succesvolle aanbiedingen worden binnen een paar uur goedgekeurd. Als je aanbieding is goedgekeurd, wordt deze weergegeven in de [!DNL Amazon Marketplace] voor directe bestellingen door klanten. De extensie [!DNL Amazon Sales Channel] biedt een set tabbladen om Amazon-aanbiedingen te bekijken. Afhankelijk van de uitgave of de vereiste gegevens, moet u uw [!DNL Amazon Seller Central] -account bekijken voor specifieke details over deze aanbiedingen.

- [ Actief ](./active-listings.md): Vermeldt goedgekeurde productlijsten beschikbaar door de markt.

- [ Klaar aan Lijst ](./ready-to-list.md): Maakt een lijst van producten die aan de vereisten van lijstregels voldoen en klaar om aan Amazon te publiceren.

- [ Inactief ](./inactive-listings.md): Maakt een lijst van producten die niet beschikbaar op de markt wegens het worden geblokkeerd om een specifieke reden (zoals branding kwestie), gesloten en vereist het steunen, etc. zijn.

- [ Niet in aanmerking komend ](./ineligible-listings.md): wegens de lijstregels, maakt een lijst van product dat niet actief op de markt kan worden vermeld (zoals `0` aantal of verkoopdata).

- [ Onvolledig ](./incomplete-listings.md): De producten van lijsten missen vereiste informatie. Werk de productgegevens bij voor een andere revisie.

- [ Geëindigd ](./ended-listings.md): Lijsten van productlijsten die voor lijst in aanmerking komen maar manueel uit Amazon worden verwijderd. Je kunt deze producten opnieuw aanbieden.

## Gegevens synchroniseren

Adobe Commerce en Magento Open Source communiceren product- en bestelgegevens tussen uw [!DNL Amazon Seller Central] -account en de [!DNL Commerce] backend. De continue updates bieden één bron via [!DNL Commerce] voor het beheren en onderhouden van uw inventarissen, het uitvoeren van bestellingen, het volgen van de verkoop en het verminderen van overhead en dubbel werk. Met deze rapportage worden de meest recente gegevens vastgelegd voor het volgen van trends en het oplossen van communicatieproblemen tussen de twee systemen.

Al het synchroniseren wordt beheerd door de baan van de a [ cron ](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html), reeks om elke vijf minuten in uw [ pre-Opstelling Taken ](./amazon-pre-setup-tasks.md) bij te werken.
