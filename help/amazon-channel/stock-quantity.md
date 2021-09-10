---
title: Voorraad/Aantal
description: 'Als u de synchronisatie van de gegevens over de producthoeveelheid van uw winkel Commerce naar uw  [!DNL Amazon Seller Central] account wilt beheren, werkt u de instellingen voor de voorraad/hoeveelheid bij.'
redirect_from: /sales-channels/asc/ob-stock-quantity.html: 
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 771
ht-degree: 0%

---

# Voorraad/Aantal

*[!UICONTROL Stock/Quantity]* Deze instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via het [opslagdashboard](./amazon-store-dashboard.md).

Deze instellingen worden gebruikt om de productkwantitatieve gegevens van uw [!DNL Commerce]-winkel te synchroniseren met de hoeveelheid van uw [!DNL Amazon Seller Central]-account. Dit gereedschap is krachtig en kan worden gebruikt voor extra reclame door de koper dringend te laten zien terwijl je voorraad geordend blijft. Sommige handelaren kunnen bijvoorbeeld 150 artikelen van een bepaalde SKU in voorraad hebben in hun pakhuis en willen ervoor zorgen dat Amazon-kopers al hun voorraad kunnen kopen. Andere handelaren willen mogelijk slechts één object tegelijk aanbieden om de eindgebruiker een gevoel van schaarste te geven. In dit geval stelt u *[!UICONTROL Maximum Listed Quantity]* in op `1`.

De hoeveelheid is een regionaal kenmerk en is gebaseerd op de **[!UICONTROL Amazon Marketplace Country]**-instelling die tijdens [store integration](./store-integration.md) is gedefinieerd. Wanneer de hoeveelheid van een product wordt gewijzigd, heeft de wijziging invloed op alle Amazon-aanbiedingen die [!DNL Amazon Seller SKU] delen in uw Amazon-winkels die in hetzelfde land verkopen. Een wijziging in een gedeelde [!DNL Amazon Seller SKU] in de Verenigde Staten heeft geen invloed op uw Amazon-winkels die voor een ander land zijn ingesteld. De eerste Amazon-winkel die is geïntegreerd (met de oudste aanmaakdatum) bepaalt de prioriteit in de instellingen voor de hoeveelheid.

>[!NOTE]
>
>Voor Adobe Commerce en Magento Open Source 2.3.x gebruikers, steunt het verkoopkanaal van Amazon het gebruik van de uitbreiding van het Beheer van de Inventaris zonder enige extra opstelling. Zie [Inventaris beheren](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){:target=&quot;_blank&quot;}.

## Instellingen voor voorraad/hoeveelheid configureren {#configure-stock--quantity-settings}

1. Klik **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie **[!UICONTROL Stock / Quantity]** uit.

1. Voer voor **[!UICONTROL Out-of-Stock Threshold]** (verplicht) een numerieke waarde in voor de laagste hoeveelheid van een product om ervoor te zorgen dat het product in aanmerking komt voor de Amazon-vermelding.

   De standaardwaarde is `0`. Als de productvoorraad van [!DNL Commerce] lager is dan dit aantal, komt de desbetreffende Amazon-aanbieding niet in aanmerking voor verkoop via Amazon.

1. Voer voor **[!UICONTROL Maximum Listed Quantity]** (vereist) een numerieke waarde in voor het aantal dat je in de Amazon-aanbieding wilt weergeven.

   Met deze instelling worden al je in aanmerking komende Amazon-aanbiedingen tegen de opgegeven waarde weergegeven. Wanneer een object wordt verkocht, verandert het aantal aanbiedingen van Amazon niet. Deze waarde wordt altijd gebruikt voor de beschikbare aanbiedingshoeveelheid, zelfs als het werkelijke aantal producten hoger of lager is. Deze instelling wordt doorgaans gebruikt wanneer u de productvoorraad niet beheert. U hebt bijvoorbeeld een product met een hoeveelheid van 80 in uw [!DNL Commerce]-catalogus. Als de optie is ingesteld op `10`, wordt in de Amazon-aanbieding altijd een beschikbare hoeveelheid van `10` weergegeven. Deze waarde wordt niet gewijzigd wanneer het product wordt verkocht.

1. Voer voor **[!UICONTROL "Do Not Manage Stock" Quantity]** (vereist) een waarde in die in aantal moet worden weergegeven voor je Amazon-aanbiedingen.

   Amazon vereist dat je een beschikbaar aantal publiceert. Voor [!DNL Commerce] producten die zijn ingesteld om geen voorraad te beheren maar die je wilt aanbieden op Amazon, wordt de aanbieding gepubliceerd met het beschikbare aantal dat hier wordt ingevoerd.

1. Klik op **[!UICONTROL Save listing settings]** als u klaar bent.

![Instellingen voor voorraad/aantal](assets/amazon-stock-quantity.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | Voer een numerieke waarde in voor de laagste hoeveelheid van een product om het product in aanmerking te laten komen voor de Amazon-aanbieding (de standaardwaarde is `0`).<br><br>Als je  [!DNL Commerce] productvoorraad lager is dan dit aantal, kan de desbetreffende Amazon-aanbieding niet worden verkocht via Amazon. |
| [!UICONTROL Maximum Listed Quantity] | Voer een numerieke waarde in voor het aantal dat je in de Amazon-aanbieding wilt weergeven.<br><br>Wanneer een object wordt verkocht, wordt de aanbieding opnieuw gepubliceerd met de hier opgegeven hoeveelheid. Deze instelling wordt doorgaans gebruikt wanneer u de productvoorraad niet beheert.<br><br>Je voert bijvoorbeeld de waarde Maximum aantal aangeboden objecten in als  `10`. De werkelijke hoeveelheid voor een product is `80`. Omdat u deze waarde hebt ingesteld op `10`, wordt in de Amazon-aanbieding altijd een beschikbare hoeveelheid van `10` weergegeven. De beschikbare hoeveelheid wordt altijd weergegeven met de gedefinieerde waarde, zelfs als het voorraadaantal lager is. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Voer een waarde in voor het weergaveaantal voor je Amazon-aanbiedingen.<br><br>Amazon vereist dat je een beschikbaar aantal publiceert. Voor [!DNL Commerce] producten die zijn ingesteld om de voorraad niet te beheren maar die je wilt aanbieden op Amazon, wordt de aanbieding gepubliceerd met de beschikbare hoeveelheid van de hier ingevoerde waarde. |

**Snelle toegang**  -  [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## Voorbeeld: Maximale vermelde hoeveelheid

Wanneer een object wordt verkocht, wordt het door de Amazon-aanbieding opnieuw op deze hoeveelheid geplaatst.

Als u bijvoorbeeld *[!UICONTROL Maximum Listed Quantity]* instelt als `12`, bevat de Amazon-vermelding een hoeveelheid van 12, ook al heeft het product een [!DNL Commerce] hoeveelheid van 80:

![Maximum aantal in de lijst, voorbeeld 1](assets/amazon-max-listed-quantity.png)

Als u *[!UICONTROL Maximum Listed Quantity]* als `1` plaatst, worden alle in aanmerking komende producten vermeld met een hoeveelheid van `1`. Wanneer een object wordt verkocht, zoekt het systeem naar het [!DNL Commerce]-product en als er nog meer voorraad is, vertrouwt het systeem het object op Amazon met een hoeveelheid van `1`.

Deze optie kan nuttig zijn voor producten die doorgaans met een hoeveelheid van 1 worden geordend. Het verhoogt ook de urgentie voor de verkoper bij het bekijken van je Amazon-aanbieding.

![Voorbeeld van maximaal aangeboden hoeveelheid 2](assets/amazon-max-listed-quantity-1.png)
