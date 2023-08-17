---
title: Amazon-Sales Channel - [!UICONTROL Stock/Quantity]
description: De synchronisatie van de gegevens over de hoeveelheid producten van je winkel voor Koophandel met je [!DNL Amazon Seller Central] de voorraad/hoeveelheid-instellingen bijwerken.
feature: Sales Channels, Inventory
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# [!UICONTROL Stock/Quantity]

*[!UICONTROL Stock/Quantity]* Deze instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via de [opslagdashboard](./amazon-store-dashboard.md).

Met deze instellingen synchroniseert u de productkwantitatieve gegevens via uw [!DNL Commerce] opslaan naar de hoeveelheid op je [!DNL Amazon Seller Central] account. Dit gereedschap is krachtig en kan worden gebruikt voor extra reclame door de koper dringend te laten zien terwijl je voorraad geordend blijft. Sommige handelaren kunnen bijvoorbeeld 150 artikelen van een bepaalde SKU in voorraad hebben in hun pakhuis en willen ervoor zorgen dat Amazon-kopers al hun voorraad kunnen kopen. Andere handelaren willen mogelijk slechts één object tegelijk aanbieden om de eindgebruiker een gevoel van schaarste te geven. In dit geval stelt u de *[!UICONTROL Maximum Listed Quantity]* tot `1`.

Hoeveelheid is een regionaal kenmerk en is gebaseerd op de **[!UICONTROL Amazon Marketplace Country]** definiëren tijdens [winkelintegratie](./store-integration.md). Wanneer de hoeveelheid van een product wordt gewijzigd, heeft de wijziging invloed op alle Amazon-aanbiedingen die dat delen [!DNL Amazon Seller SKU] in je Amazon-winkels die in hetzelfde land verkopen. Een wijziging in een gedeelde [!DNL Amazon Seller SKU] in de Verenigde Staten heeft geen invloed op je Amazon-winkels die voor een ander land zijn ingesteld. De eerste Amazon-winkel die is geïntegreerd (met de oudste aanmaakdatum) bepaalt de prioriteit in de instellingen voor de hoeveelheid.

>[!NOTE]
>
>Voor Adobe Commerce- en Magento Open Source 2.3.x-gebruikers biedt Amazon-verkoopkanalen ondersteuning voor het gebruik van de Inventory management-extensie zonder extra installatie. Zie [Inventaris beheren](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}.

## Instellingen voor voorraad/hoeveelheid configureren {#configure-stock--quantity-settings}

1. Klikken **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie **[!UICONTROL Stock / Quantity]** uit.

1. Voor **[!UICONTROL Out-of-Stock Threshold]** (vereist), voert u een numerieke waarde in voor de laagste hoeveelheid van een product om ervoor te zorgen dat het product in aanmerking komt voor de Amazon-aanbieding.

   De standaardwaarde is `0`. Als uw [!DNL Commerce] De voorraad van het product is lager dan dit aantal. De desbetreffende Amazon-aanbieding komt niet in aanmerking voor verkoop via Amazon.

1. Voor **[!UICONTROL Maximum Listed Quantity]** (vereist) voert u een numerieke waarde in voor het aantal dat je in de Amazon-aanbieding wilt weergeven.

   Met deze instelling worden al je in aanmerking komende Amazon-aanbiedingen tegen de opgegeven waarde weergegeven. Wanneer een object wordt verkocht, verandert het aantal aanbiedingen van Amazon niet. Deze waarde wordt altijd gebruikt voor de beschikbare aanbiedingshoeveelheid, zelfs als het werkelijke aantal producten hoger of lager is. Deze instelling wordt doorgaans gebruikt wanneer u de productvoorraad niet beheert. U hebt bijvoorbeeld een product met een hoeveelheid van 80 in uw [!DNL Commerce] catalogus. Met ingesteld op `10`, de Amazon-aanbieding geeft altijd een beschikbare hoeveelheid weer van `10` en verandert niet wanneer het product wordt verkocht.

1. Voor **[!UICONTROL "Do Not Manage Stock" Quantity]** (vereist), voer een waarde in die in aantal moet worden weergegeven voor je Amazon-aanbiedingen.

   Amazon vereist dat je een beschikbaar aantal publiceert. Voor [!DNL Commerce] producten die zijn ingesteld om geen voorraad te beheren maar die je wilt aanbieden op Amazon, worden gepubliceerd met de beschikbare hoeveelheid die hier wordt ingevoerd.

1. Klik op **[!UICONTROL Save listing settings]**.

![Instellingen voor voorraad/aantal](assets/amazon-stock-quantity.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Out-of-Stock Threshold] | Voer een numerieke waarde in voor de laagste hoeveelheid van een product om het product in aanmerking te laten komen voor de Amazon-aanbieding (standaard is `0`).<br><br>Als uw [!DNL Commerce] De voorraad van het product is lager dan dit aantal. De desbetreffende Amazon-aanbieding komt niet in aanmerking voor verkoop via Amazon. |
| [!UICONTROL Maximum Listed Quantity] | Voer een numerieke waarde in voor het aantal dat je in de Amazon-aanbieding wilt weergeven.<br><br>Wanneer een object wordt verkocht, wordt de aanbieding opnieuw gepubliceerd met de hier opgegeven hoeveelheid. Deze instelling wordt doorgaans gebruikt wanneer u de productvoorraad niet beheert.<br><br>Je voert bijvoorbeeld de waarde Maximum aantal aangeboden objecten in als `10`. De werkelijke hoeveelheid voor een product is `80`. Omdat u deze waarde hebt ingesteld op `10`, de Amazon-aanbieding geeft altijd een beschikbare hoeveelheid weer van `10`. De beschikbare hoeveelheid wordt altijd weergegeven met de gedefinieerde waarde, zelfs als het voorraadaantal lager is. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Voer een waarde in voor het weergaveaantal voor je Amazon-aanbiedingen.<br><br>Amazon vereist dat je een beschikbaar aantal publiceert. Voor [!DNL Commerce] producten die zijn ingesteld om geen voorraad te beheren maar die je op Amazon wilt aanbieden, worden gepubliceerd met een beschikbare hoeveelheid van de hier ingevoerde waarde. |

**Snelle toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## Voorbeeld: Maximale aangeboden hoeveelheid

Wanneer een object wordt verkocht, wordt het door de Amazon-aanbieding opnieuw op deze hoeveelheid geplaatst.

Als u bijvoorbeeld *[!UICONTROL Maximum Listed Quantity]* als `12`In de Amazon-aanbieding wordt een hoeveelheid van 12 getoond, ook al heeft het product een [!DNL Commerce] hoeveelheid van 80:

![Maximum aantal in de lijst, voorbeeld 1](assets/amazon-max-listed-quantity.png){width="300"}

Als u uw *[!UICONTROL Maximum Listed Quantity]* als `1`alle in aanmerking komende producten met een hoeveelheid `1`. Wanneer een object wordt verkocht, zoekt het systeem naar je [!DNL Commerce] -product en als er nog meer voorraad is, wordt het object op Amazon opnieuw aangeboden met een hoeveelheid `1`.

Deze optie kan nuttig zijn voor producten die doorgaans met een hoeveelheid van 1 worden geordend. Het verhoogt ook de urgentie voor de verkoper bij het bekijken van je Amazon-aanbieding.

![Voorbeeld van maximaal aangeboden hoeveelheid 2](assets/amazon-max-listed-quantity-1.png){width="300"}
