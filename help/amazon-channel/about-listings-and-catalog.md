---
title: Informatie over Amazon en de handelscatalogus
description: Het verkoopkanaal van Amazon importeert je Amazon-aanbiedingen in je Commerce-achtergrond en synchroniseert voortdurend met producten en verkopen.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Informatie over Amazon en de [!DNL Commerce]-catalogus

De Adobe Commerce of Magento Open Source backend omvat een catalogus met alle producten en bijbehorende montages en informatie (beelden, opties, prijzen, en meer) en orde en verzendconfiguraties. Uw [!DNL Amazon Seller Central]-account heeft ook een catalogus en orderconfiguraties, waarbij uw verkoop strikt wordt gevolgd via [!DNL Amazon Marketplace].

Om uw productcatalogus en verkoop beter te beheren en te bekijken via één locatie, importeert Amazon uw Amazon-aanbiedingen in uw [!DNL Commerce]-backend, synchroniseert deze voortdurend met producten en verkoop en rapporteert problemen en trends. Het steunt integraties met veelvoudige [!DNL Amazon Seller Central] rekeningen, die alle gegevens door de enige interface voor veelvoudige storefronts volgen.

## Productkenmerken

Adobe de Handel en Magento Open Source beheren catalogussyncs met het gebruik van product [attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} om productmontages en gegevens te bepalen. Amazon gebruikt ook kenmerken die aan boord moeten worden gezet. Tijdens [vooraf ingestelde taken](./amazon-pre-setup-tasks.md) voor Amazon-verkoopkanaal definieert u (indien nodig) extra Amazon-kenmerken om ervoor te zorgen dat de producttoewijzingen correct zijn wanneer u uw Amazon-aanbiedingen importeert in uw [!DNL Commerce]-catalogus. Deze attributen omvatten UPC, EAN, ISBN, en ASIN ([!DNL Amazon Standard Identification Number]). Producten synchroniseren tussen Amazon en [!DNL Commerce] catalogi met behulp van uw kenmerken door aan boord te gaan. Correcte mapping van uw [!DNL Commerce]- en Amazon-producten zorgt voor een continue synchronisatie van productinformatie, bestellingen en inventaris.

Als u deze attributen niet hebt die voor uw catalogus worden gecreeerd of worden gevormd, zou u [!DNL Commerce] [productattribuut](https://docs.magento.com/user-guide/catalog/product-attributes.html){target= &quot;_blank&quot;} en waarden aan uw producten vóór aan boord gaan moeten toevoegen. Wanneer een Amazon-kenmerk wordt geïmporteerd, kan het worden gebruikt voor zoeken, navigatie, prijsregels en nog veel meer. Zie [Amazon voor meer informatie over deze kenmerken: Wat zijn UPCs, EANs, ISBNs, en ASINs?](https://www.amazon.com/gp/seller/asin-upc-isbn-info.html){target=&quot;_blank&quot;}

Na het instappen, kunt u uw productattributen en afbeeldingen van Amazon op elk ogenblik beheren en bijwerken.

## Productaanbiedingen

Een Amazon-aanbieding is een productpagina voor elk product dat u via [!DNL Amazon Marketplace] verkoopt. Hierin worden productbeschrijvingen, prijzen, afbeeldingen en meer via kenmerken in kaart gebracht. Tijdens het instappen kunt u configureren dat uw [!DNL Commerce]-producten automatisch worden gepubliceerd naar Amazon-aanbiedingen. U kunt uw bestaande Amazon-aanbiedingen ook importeren door deze toe te wijzen aan uw [!DNL Commerce]-producten.

Wanneer u een aanbieding [!DNL Commerce] producten hebt gecreeerd, worden zij voorgelegd aan Amazon voor goedkeuring. De meeste succesvolle aanbiedingen worden binnen een paar uur goedgekeurd. Als je aanbieding is goedgekeurd, wordt deze weergegeven in de [!DNL Amazon Marketplace] voor directe bestellingen door klanten. De extensie [!DNL Amazon Sales Channel] biedt een set tabbladen om Amazon-lijsten te bekijken. Afhankelijk van de uitgave of de vereiste gegevens moet u uw [!DNL Amazon Seller Central]-account controleren voor specifieke details over deze aanbiedingen.

- [Actief](./active-listings.md): Hiermee geeft u goedgekeurde productaanbiedingen weer die beschikbaar zijn via de markt.

- [Klaar om aan te bieden](./ready-to-list.md): Hiermee worden producten weergegeven die voldoen aan de vereisten voor aanbiedingsregels en die klaar zijn om naar Amazon te publiceren.

- [Inactief](./inactive-listings.md): Geeft producten weer die niet beschikbaar zijn op de markt omdat ze om een bepaalde reden geblokkeerd zijn (zoals een probleem met branding), gesloten zijn en opnieuw moeten worden aangeboden, enzovoort.

- [Niet-subsidiabel](./ineligible-listings.md): Als gevolg van de aanbiedingsregels worden producten aangeboden die niet actief op de markt kunnen worden aangeboden (zoals  `0` aantal- of verkoopdatums).

- [Onvolledig](./incomplete-listings.md): Vermeldt de producten die de vereiste informatie missen. Werk de productgegevens bij voor een andere revisie.

- [Beëindigd](./ended-listings.md): Hiermee worden productaanbiedingen weergegeven die in aanmerking komen voor aanbieding, maar die handmatig uit Amazon zijn verwijderd. Je kunt deze producten opnieuw aanbieden.

## Gegevens synchroniseren

Adobe Handel en Magento Open Source communiceren product- en ordergegevens tussen uw [!DNL Amazon Seller Central]-account en de [!DNL Commerce]-back-end. De continue updates bieden één bron via [!DNL Commerce] voor het beheren en onderhouden van uw inventarissen, het uitvoeren van bestellingen, het volgen van de verkoop en het verminderen van overhead en dubbel werk. Met deze rapportage worden de meest recente gegevens vastgelegd voor het volgen van trends en het oplossen van communicatieproblemen tussen de twee systemen.

Al het synchroniseren wordt beheerd door [cron baan](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}, die wordt geplaatst om de vijf minuten in uw [Taken van de Opstelling ](./amazon-pre-setup-tasks.md) bij te werken.
