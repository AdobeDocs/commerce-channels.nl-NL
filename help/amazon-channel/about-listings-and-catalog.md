---
title: Informatie over Amazon en de handelscatalogus
description: Het verkoopkanaal van Amazon importeert je Amazon-aanbiedingen in je Commerce-achtergrond en synchroniseert voortdurend met producten en verkopen.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Over Amazon en de [!DNL Commerce] catalogus

Uw Adobe Commerce- of Magento Open Source-backend bevat een catalogus met alle producten en de bijbehorende instellingen en informatie (afbeeldingen, opties, prijzen en meer) en bestellingen en verzendconfiguraties. Uw [!DNL Amazon Seller Central] account heeft ook een catalogus en orderconfiguraties, waarbij uw verkoop strikt wordt bijgehouden via de [!DNL Amazon Marketplace].

Amazon verkoopkanaal importeert je Amazon-aanbiedingen naar je eigen locatie om je productcatalogus en verkoop beter te beheren en te bekijken. [!DNL Commerce] back-end, wordt voortdurend gesynchroniseerd met producten en verkoop, en rapporteert problemen en trends. Het steunt integratie met veelvoudige [!DNL Amazon Seller Central] accounts, die alle gegevens bijhouden via de enkele interface voor meerdere opslagronten.

## Productkenmerken

Adobe Commerce en Magento Open Source beheren catalogussynchronisaties met het gebruik van producten [attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} om productinstellingen en gegevens te definiëren. Amazon gebruikt ook kenmerken die aan boord moeten worden gezet. Tijdens [vooraf ingestelde taken](./amazon-pre-setup-tasks.md) voor Amazon-verkoopkanaal definieert u (indien nodig) aanvullende Amazon-kenmerken om ervoor te zorgen dat de producttoewijzingen correct zijn wanneer u uw Amazon-aanbiedingen importeert in uw [!DNL Commerce] catalogus. Deze kenmerken omvatten UPC, EAN, ISBN en ASIN ([!DNL Amazon Standard Identification Number]). Door aan boord te gaan, synchroniseert de producten tussen Amazon en [!DNL Commerce] catalogi die uw kenmerken gebruiken. Correcte toewijzing van uw [!DNL Commerce] en Amazon-producten zorgen voor een continue synchronisatie van productinformatie, bestellingen en inventaris.

Als deze kenmerken niet voor de catalogus zijn gemaakt of geconfigureerd, moet u een [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} en waarden aan uw producten toevoegen voordat ze worden opgenomen. Wanneer een Amazon-kenmerk wordt geïmporteerd, kan het worden gebruikt voor zoeken, navigatie, prijsregels en nog veel meer. Zie voor meer informatie over deze kenmerken [Amazon: Wat zijn UPCs, EANs, ISBNs, en ASINs?](https://www.amazon.com/gp/seller/asin-upc-isbn-info.html){target=&quot;_blank&quot;}

Na het instappen, kunt u uw productattributen en afbeeldingen van Amazon op elk ogenblik beheren en bijwerken.

## Productaanbiedingen

Een Amazon-aanbieding is een productpagina voor elk product dat je via [!DNL Amazon Marketplace], waarin productbeschrijvingen, prijzen, afbeeldingen en meer worden weergegeven die door kenmerken zijn toegewezen. Tijdens het instappen, kunt u uw vormen [!DNL Commerce] producten kunnen automatisch naar Amazon-aanbiedingen worden gepubliceerd. Je kunt je bestaande Amazon-aanbiedingen ook importeren door ze aan je te koppelen [!DNL Commerce] producten.

Wanneer je een aanbieding hebt gemaakt [!DNL Commerce] producten, worden zij ter goedkeuring aan Amazon voorgelegd. De meeste succesvolle aanbiedingen worden binnen een paar uur goedgekeurd. Als je aanbieding is goedgekeurd, wordt deze weergegeven in de [!DNL Amazon Marketplace] voor directe bestellingen door klanten. De [!DNL Amazon Sales Channel] biedt een set tabbladen om Amazon-aanbiedingen te bekijken. Afhankelijk van het probleem of de vereiste gegevens moet u uw [!DNL Amazon Seller Central] specifieke details over deze aanbiedingen opgeven.

- [Actief](./active-listings.md): Hiermee geeft u goedgekeurde productaanbiedingen weer die beschikbaar zijn via de markt.

- [Klaar voor lijst](./ready-to-list.md): Hiermee worden producten weergegeven die voldoen aan de vereisten voor aanbiedingsregels en die klaar zijn om naar Amazon te publiceren.

- [Inactief](./inactive-listings.md): Geeft producten weer die niet beschikbaar zijn op de markt omdat ze om een bepaalde reden geblokkeerd zijn (zoals een probleem met branding), gesloten zijn en opnieuw moeten worden aangeboden, enzovoort.

- [Niet-subsidiabel](./ineligible-listings.md): Als gevolg van de aanbiedingsregels wordt een product aangeboden dat niet actief op de markt kan worden aangeboden (zoals `0` aantal of verkoopdatum).

- [Onvolledig](./incomplete-listings.md): Vermeldt de producten die de vereiste informatie missen. Werk de productgegevens bij voor een andere revisie.

- [Beëindigd](./ended-listings.md): Hiermee worden productaanbiedingen weergegeven die in aanmerking komen voor aanbieding, maar die handmatig uit Amazon zijn verwijderd. Je kunt deze producten opnieuw aanbieden.

## Gegevens synchroniseren

Adobe Commerce en Magento Open Source communiceren producten en bestellen gegevens tussen uw [!DNL Amazon Seller Central] en de [!DNL Commerce] achterkant. De voortdurende updates verstrekken één enkele bron door [!DNL Commerce] om uw inventarissen te beheren en te onderhouden, orders te vervullen, verkoop te volgen, en overheadkosten en dubbel werk te verminderen. Met deze rapportage worden de meest recente gegevens vastgelegd voor het volgen van trends en het oplossen van communicatieproblemen tussen de twee systemen.

Alle synchronisatie wordt beheerd door een [snijtaak](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}, instellen om de vijf minuten in uw [Taken vooraf instellen](./amazon-pre-setup-tasks.md).
