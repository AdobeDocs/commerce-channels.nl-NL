---
title: Amazon-Sales Channel - [!UICONTROL Stock/Quantity]
description: Om het synchroniseren van de details van de producthoeveelheid van uw opslag van Commerce aan uw  [!DNL Amazon Seller Central]  rekening te controleren, werk de montages van de Beeld/van de Hoeveelheid bij.
feature: Sales Channels, Inventory
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# [!UICONTROL Stock/Quantity]

*[!UICONTROL Stock/Quantity]* -instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. De lijsten van montages worden betreden van het [ opslagdashboard ](./amazon-store-dashboard.md).

Deze instellingen worden gebruikt om de productkwantitatieve gegevens van uw [!DNL Commerce] winkel te synchroniseren met de hoeveelheid van uw [!DNL Amazon Seller Central] -account. Dit gereedschap is krachtig en kan worden gebruikt voor extra reclame door de koper dringend te laten zien terwijl je voorraad geordend blijft. Sommige handelaren kunnen bijvoorbeeld 150 artikelen van een bepaalde SKU in voorraad hebben in hun pakhuis en willen ervoor zorgen dat Amazon-kopers al hun voorraad kunnen kopen. Andere handelaren willen mogelijk slechts één object tegelijk aanbieden om de eindgebruiker een gevoel van schaarste te geven. Stel in dit geval de waarde *[!UICONTROL Maximum Listed Quantity]* in op `1` .

De hoeveelheid is een regionaal attribuut en gebaseerd op **[!UICONTROL Amazon Marketplace Country]** het plaatsen bepaalt tijdens [ opslagintegratie ](./store-integration.md). Wanneer de hoeveelheid van een product wordt gewijzigd, heeft de wijziging invloed op alle Amazon-aanbiedingen die die [!DNL Amazon Seller SKU] delen in uw Amazon-winkels die in hetzelfde land verkopen. Een wijziging in een gedeelde versie van [!DNL Amazon Seller SKU] in de Verenigde Staten heeft geen invloed op uw Amazon-winkels die zijn ingesteld voor een ander land. De eerste Amazon-winkel die is geïntegreerd (met de oudste aanmaakdatum) bepaalt de prioriteit in de instellingen voor de hoeveelheid.

>[!NOTE]
>
>Voor Adobe Commerce- en Magento Open Source 2.3.x-gebruikers biedt Amazon-verkoopkanalen ondersteuning voor het gebruik van de Inventory management-extensie zonder extra installatie. Zie [ het Leiden Inventaris ](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html) {target="_blank"}.

## Instellingen voor voorraad/hoeveelheid configureren {#configure-stock--quantity-settings}

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie **[!UICONTROL Stock / Quantity]** uit.

1. Voer bij **[!UICONTROL Out-of-Stock Threshold]** (verplicht) een numerieke waarde in voor de laagste hoeveelheid van een product om ervoor te zorgen dat het product in aanmerking komt voor de Amazon-aanbieding.

   De standaardwaarde is `0` . Als je [!DNL Commerce] productvoorraad lager is dan dit nummer, kan de desbetreffende Amazon-aanbieding niet worden verkocht via Amazon.

1. Voer voor **[!UICONTROL Maximum Listed Quantity]** (vereist) een numerieke waarde in voor het aantal dat je in de Amazon-aanbieding wilt weergeven.

   Met deze instelling worden al je in aanmerking komende Amazon-aanbiedingen tegen de opgegeven waarde weergegeven. Wanneer een object wordt verkocht, verandert het aantal aanbiedingen van Amazon niet. Deze waarde wordt altijd gebruikt voor de beschikbare aanbiedingshoeveelheid, zelfs als het werkelijke aantal producten hoger of lager is. Deze instelling wordt doorgaans gebruikt wanneer u de productvoorraad niet beheert. U hebt bijvoorbeeld een product met een hoeveelheid van 80 in de catalogus van [!DNL Commerce] . Als deze optie is ingesteld op `10` , wordt in de Amazon-aanbieding altijd een beschikbare hoeveelheid van `10` weergegeven. Deze hoeveelheid verandert niet wanneer het product wordt verkocht.

1. Voer voor **[!UICONTROL "Do Not Manage Stock" Quantity]** (vereist) een waarde in die in aantal moet worden weergegeven voor je Amazon-aanbiedingen.

   Amazon vereist dat je een beschikbaar aantal publiceert. Voor [!DNL Commerce] -producten die zijn ingesteld om geen voorraad te beheren maar die je wilt aanbieden op Amazon, wordt de aanbieding gepubliceerd met het beschikbare aantal dat hier wordt ingevoerd.

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ Voorraad/kwantitatieve montages ](assets/amazon-stock-quantity.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Out-of-Stock Threshold] | Voer een numerieke waarde in voor de laagste hoeveelheid van een product om het product in aanmerking te laten komen voor de Amazon-aanbieding (de standaardwaarde is `0` ).<br><br> Als uw [!DNL Commerce] -productvoorraad lager is dan dit aantal, komt de respectievelijke Amazon-aanbieding niet in aanmerking voor verkoop via Amazon. |
| [!UICONTROL Maximum Listed Quantity] | Voer een numerieke waarde in voor het aantal dat je in de Amazon-aanbieding wilt weergeven.<br><br> Wanneer een punt wordt verkocht, publiceert de Amazon aanbieding met het hier ingegaan aantal opnieuw. Deze instelling wordt doorgaans gebruikt wanneer u de productvoorraad niet beheert.<br><br> Bijvoorbeeld, gaat u de Maximumwaarde van de Aantal van de Lijst als `10` in. Het werkelijke aantal voor een product is `80` . Omdat u deze waarde op `10` hebt ingesteld, wordt in de Amazon-aanbieding altijd een beschikbare hoeveelheid van `10` weergegeven. De beschikbare hoeveelheid wordt altijd weergegeven met de gedefinieerde waarde, zelfs als het voorraadaantal lager is. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Voer een waarde in voor het weergaveaantal voor je Amazon-aanbiedingen.<br><br> Amazon vereist dat u een beschikbaar aantal publiceert. Voor [!DNL Commerce] -producten die zijn ingesteld om geen voorraad te beheren maar die je wilt aanbieden op Amazon, wordt de aanbieding gepubliceerd met het beschikbare aantal van de hier ingevoerde waarde. |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

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

Als u bijvoorbeeld *[!UICONTROL Maximum Listed Quantity]* instelt als `12` , bevat de Amazon-vermelding een hoeveelheid van 12, ook al heeft het product een [!DNL Commerce] hoeveelheid van 80:

![ Maximum vermeld kwantitatief voorbeeld 1 ](assets/amazon-max-listed-quantity.png){width="300"}

Als u *[!UICONTROL Maximum Listed Quantity]* instelt als `1` , wordt voor alle in aanmerking komende producten een hoeveelheid `1` vermeld. Wanneer een object wordt verkocht, zoekt het systeem naar het [!DNL Commerce] -product en als er extra voorraad is, vertrouwt het object op Amazon op met een hoeveelheid van `1` .

Deze optie kan nuttig zijn voor producten die doorgaans met een hoeveelheid van 1 worden geordend. Het verhoogt ook de urgentie voor de verkoper bij het bekijken van je Amazon-aanbieding.

![ Maximum vermeld kwantitatief voorbeeld 2 ](assets/amazon-max-listed-quantity-1.png){width="300"}
