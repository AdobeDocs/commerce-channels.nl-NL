---
title: '''[!DNL Channel Manager] Opmerkingen bij de release'
description: De meest recente releasegegevens voor [!DNL Channel Manager] uit Adobe Commerce.
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: d3acde7aa297ba33dffa7854aa7578985ad12c9b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# [!DNL Channel Manager] Opmerkingen bij de release

In deze releaseopmerkingen wordt de eerste release van [!DNL Channel Manager] en omvatten:

![Nieuw](../assets/new.svg) Nieuwe functies
![Probleem opgelost](../assets/fix.svg) Oplossingen en verbeteringen
![Bekend probleem](../assets/bug.svg) Bekende problemen


## v2.0.0

*20 maart 2023*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Nieuw](../assets/new.svg)<!--CHAN-5893--> Channel Manager is nu compatibel met Adobe Commerce versie 2.4.6.

## v1.1.0

*23 november 2022*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Nieuw](../assets/new.svg)<!--CHAN-5204--> **Retourneert en terugbetaalt**—U kunt nu het retourproces en terugbetalingen van Walmart Marketplace verwerken voor bestellingen die via een Adobe Commerce- en Magento Open Source Channel Manager-winkel worden verzonden. De informatie en de updates over terugkeer en terugbetalingen worden gesynchroniseerd tussen Walmart en Adobe Commerce zodat de huidige gegevens in zowel [!DNL Commerce] storefront en [!DNL Walmart Marketplace]. Zie [Terugbetalingsopdrachten](return-refund-orders.md).

![Vast](../assets/fix.svg)<!--CHAN-5661--> Vaste het `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` fout die optrad bij het opnieuw synchroniseren van Channel Manager-volgordegegevens met de `bin/magento saas:resync --feed orders` gebruiken. De fout werd opgelost door de het pakketgebiedsdelen van de Manager van het Kanaal voor de module van de Exporteur van de Gegevens van de Verkoop bij te werken, die werd anders genoemd van `magento/module-sales-data-exporter` tot `magento/module-sales-orders-data-exporter`.

## v1.0.0

*14 januari 2022*

[!BADGE Compatibiliteit]{type=Informative tooltip="Compatibiliteit"}

![Nieuw](../assets/new.svg) Eerste release van Channel Manager voor algemene beschikbaarheid

