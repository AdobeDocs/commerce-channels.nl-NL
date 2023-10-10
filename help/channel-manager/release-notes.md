---
title: '[!DNL Channel Manager] Aanvullende informatie'
description: De meest recente releasegegevens voor [!DNL Channel Manager] uit Adobe Commerce.
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 3%

---

# [!DNL Channel Manager] Aanvullende informatie

In deze releaseopmerkingen wordt de eerste release van [!DNL Channel Manager] en omvatten:

![Nieuw](../assets/new.svg) Nieuwe functies
![Probleem opgelost](../assets/fix.svg) Oplossingen en verbeteringen
![Bekend probleem](../assets/bug.svg) Bekende problemen

Zie [Volgende releases](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) om over versieschema&#39;s en steun te leren.

Zie [Beschikbaarheid van producten](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) voor meer informatie over de Adobe Commerce-versies die deze extensie ondersteunen.

## v2.1.0

*3 oktober 2023*

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](../assets/new.svg) Kanaalbeheer is nu compatibel met [Adobe Commerce versie 2.4.7 bèta](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html) lozingen.

## v2.0.0

*20 maart 2023*

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](../assets/new.svg)<!--CHAN-5893--> Channel Manager is nu compatibel met Adobe Commerce versie 2.4.6.

## v1.1.0

*23 november 2022*

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](../assets/new.svg)<!--CHAN-5204--> **Retourneert en terugbetaalt**—U kunt nu het retourproces en terugbetalingen van Walmart Marketplace verwerken voor bestellingen die via een Adobe Commerce- en Magento Open Source Channel Manager-winkel worden verzonden. De informatie en de updates over terugkeer en terugbetalingen worden gesynchroniseerd tussen Walmart en Adobe Commerce zodat de huidige gegevens in zowel [!DNL Commerce] storefront en [!DNL Walmart Marketplace]. Zie [Terugbetalingsopdrachten](return-refund-orders.md).

![Vast](../assets/fix.svg)<!--CHAN-5661--> Vaste het `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` fout die optrad bij het opnieuw synchroniseren van Channel Manager-volgordegegevens met de `bin/magento saas:resync --feed orders` gebruiken. De fout werd opgelost door de het pakketgebiedsdelen van de Manager van het Kanaal voor de module van de Exporteur van de Gegevens van de Verkoop bij te werken, die werd anders genoemd van `magento/module-sales-data-exporter` tot `magento/module-sales-orders-data-exporter`.

## v1.0.0

*14 januari 2022*

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](../assets/new.svg) Eerste release van Channel Manager voor algemene beschikbaarheid

