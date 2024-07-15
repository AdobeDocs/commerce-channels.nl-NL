---
title: '[!DNL Channel Manager] Opmerkingen bij de release'
description: De recentste versieinformatie voor  [!DNL Channel Manager]  van Adobe Commerce.
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# [!DNL Channel Manager] Opmerkingen bij de release

Deze releaseopmerkingen beschrijven de eerste versie van [!DNL Channel Manager] en bevatten:

![ Nieuwe ](../assets/new.svg) Nieuwe eigenschappen
![ Vaste kwestie ](../assets/fix.svg) Oplossingen en verbeteringen
![ Bekende kwestie ](../assets/bug.svg) Bekende kwesties

Zie [ Komende Versies ](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) om over versieschema&#39;s en steun te leren.

Zie [ Beschikbaarheid van het Product ](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) om te leren welke versies van Adobe Commerce deze uitbreiding steunen.

## v2.1.0

*3 Oktober, 2023*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](../assets/new.svg) Manager van het Kanaal is nu compatibel met [ versie 2.4.7 van Adobe Commerce bèta ](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html) versies.

## v2.0.0

*Maart 20, 2023*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ de Nieuwe ](../assets/new.svg)<!--CHAN-5893--> Manager van het Kanaal is nu compatibel met versie 2.4.6 van Adobe Commerce.

## v1.1.0

*23 November, 2022*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Nieuw ](../assets/new.svg)<!--CHAN-5204--> **Keert terug en terugkeert** - u kunt de terugkeer en terugbetalingsproces van de Markt van de Markt van de Markt van de Markt nu verwerken voor orden die door een opslag van de Manager van het Kanaal van Adobe Commerce en van de Magento Open Source worden verscheept. Informatie en updates over geretourneerde waarden en terugbetalingen worden gesynchroniseerd tussen Walmart en Adobe Commerce, zodat de huidige gegevens beschikbaar zijn in zowel de [!DNL Commerce] storefront als [!DNL Walmart Marketplace] . Zie [ Terugkeer en terugbetalingsorden ](return-refund-orders.md).

![ Vaste ](../assets/fix.svg)<!--CHAN-5661--> de `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` fout die optrad wanneer het opnieuw synchroniseren van de orden van de Manager van het Kanaal gegevens gebruikend het `bin/magento saas:resync --feed orders` bevel. De fout is opgelost door de pakketafhankelijkheden van Channel Manager voor de module Verkoopgegevens exporteren bij te werken, die van `magento/module-sales-data-exporter` is gewijzigd in `magento/module-sales-orders-data-exporter` .

## v1.0.0

*Januari 14, 2022*

[!BADGE  Gesteund ]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](../assets/new.svg) Eerste versie van de Manager van het Kanaal voor algemene beschikbaarheid

