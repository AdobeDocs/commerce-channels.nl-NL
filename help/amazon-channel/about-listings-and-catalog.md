---
title: Amazon en de handelscatalogus
description: Het verkoopkanaal van Amazon importeert je Amazon-aanbiedingen in je Commerce-achtergrond en synchroniseert voortdurend met producten en verkopen.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services, Merchandising, Catalogs
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Amazon en [!DNL Commerce] Catalogus

Uw Adobe Commerce of Magento Open Source backend omvat een catalogus met alle producten en bijbehorende montages en informatie (beelden, opties, prijzen, en meer) en orde en verzendconfiguraties. Uw [!DNL Amazon Seller Central] account heeft ook een catalogus en orderconfiguraties, waarbij uw verkoop strikt wordt bijgehouden via de [!DNL Amazon Marketplace].

Amazon verkoopkanaal importeert je Amazon-aanbiedingen naar je eigen locatie om je productcatalogus en verkoop beter te beheren en te bekijken. [!DNL Commerce] back-end, wordt voortdurend gesynchroniseerd met producten en verkoop, en rapporteert problemen en trends. Het steunt integratie met veelvoudige [!DNL Amazon Seller Central] accounts, die alle gegevens bijhouden via de enkele interface voor meerdere opslagronten.

## Productkenmerken

Adobe Commerce en Magento Open Source beheren catalogussyncs met het gebruik van producten [attributes](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) om productinstellingen en gegevens te definiëren. Amazon gebruikt ook kenmerken die aan boord moeten worden gezet. Tijdens [vooraf ingestelde taken](./amazon-pre-setup-tasks.md) voor Amazon-verkoopkanaal definieert u (indien nodig) aanvullende Amazon-kenmerken om ervoor te zorgen dat de producttoewijzingen correct zijn wanneer u uw Amazon-aanbiedingen importeert in uw [!DNL Commerce] catalogus. Deze kenmerken omvatten UPC, EAN, ISBN en ASIN ([!DNL Amazon Standard Identification Number]). Door aan boord te gaan, synchroniseert de producten tussen Amazon en [!DNL Commerce] catalogi die uw kenmerken gebruiken. Correcte toewijzing van uw [!DNL Commerce] en Amazon-producten zorgen voor een continue synchronisatie van productinformatie, bestellingen en inventaris.

Als u deze kenmerken niet hebt gemaakt of geconfigureerd voor uw catalogus, moet u een [!DNL Commerce] [productkenmerk](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) en waarden aan uw producten vóór aan boord nemen. Wanneer een Amazon-kenmerk wordt geïmporteerd, kan het worden gebruikt voor zoeken, navigatie, prijsregels en nog veel meer. Zie [Wat betekenen ASIN, UPC, EAN, ISBN, SKU en andere streepjescodes?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

Na het instappen, kunt u uw productattributen en afbeeldingen van Amazon op elk ogenblik beheren en bijwerken.

## Productaanbiedingen

Een Amazon-aanbieding is een productpagina voor elk product dat je via [!DNL Amazon Marketplace], waarin productbeschrijvingen, prijzen, afbeeldingen en meer worden weergegeven die door kenmerken zijn toegewezen. Tijdens het instappen, kunt u uw vormen [!DNL Commerce] producten kunnen automatisch naar Amazon-aanbiedingen worden gepubliceerd. Je kunt je bestaande Amazon-aanbiedingen ook importeren door ze aan je te koppelen [!DNL Commerce] producten.

Wanneer je een aanbieding hebt gemaakt [!DNL Commerce] producten, worden zij ter goedkeuring aan Amazon voorgelegd. De meeste succesvolle aanbiedingen worden binnen een paar uur goedgekeurd. Als je aanbieding is goedgekeurd, wordt deze weergegeven in de [!DNL Amazon Marketplace] voor directe bestellingen door klanten. De [!DNL Amazon Sales Channel] biedt een set tabbladen om Amazon-aanbiedingen te bekijken. Afhankelijk van het probleem of de vereiste gegevens moet u uw [!DNL Amazon Seller Central] specifieke details over deze aanbiedingen opgeven.

- [Actief](./active-listings.md): Hiermee geeft u een lijst weer met goedgekeurde productaanbiedingen die op de markt beschikbaar zijn.

- [Klaar voor lijst](./ready-to-list.md): Hier worden producten weergegeven die voldoen aan de vereisten voor aanbiedingsregels en die klaar zijn om te worden gepubliceerd naar Amazon.

- [Inactief](./inactive-listings.md): Vermeldt producten die niet beschikbaar zijn op de markt omdat ze om een bepaalde reden worden geblokkeerd (zoals een probleem met branding), zijn gesloten en moeten worden gebruikt, enzovoort.

- [Niet-subsidiabel](./ineligible-listings.md): Vanwege de aanbiedingsregels wordt een lijst weergegeven met producten die niet actief op de markt kunnen worden aangeboden (zoals `0` aantal of verkoopdatum).

- [Onvolledig](./incomplete-listings.md): Hier worden producten weergegeven waarvoor vereiste gegevens ontbreken. Werk de productgegevens bij voor een andere revisie.

- [Afgelopen](./ended-listings.md): Hiermee geeft u een lijst weer met productaanbiedingen die in aanmerking komen voor aanbieding, maar die handmatig uit Amazon zijn verwijderd. Je kunt deze producten opnieuw aanbieden.

## Gegevens synchroniseren

Adobe Commerce en Magento Open Source communiceren product- en bestelgegevens tussen uw [!DNL Amazon Seller Central] en de [!DNL Commerce] achterkant. De voortdurende updates verstrekken één enkele bron door [!DNL Commerce] om uw inventarissen te beheren en te onderhouden, orders te vervullen, verkoop te volgen, en overheadkosten en dubbel werk te verminderen. Met deze rapportage worden de meest recente gegevens vastgelegd voor het volgen van trends en het oplossen van communicatieproblemen tussen de twee systemen.

Alle synchronisatie wordt beheerd door een [snijtaak](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html), wordt ingesteld om de vijf minuten in uw [Taken vooraf instellen](./amazon-pre-setup-tasks.md).
