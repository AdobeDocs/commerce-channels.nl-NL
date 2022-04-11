---
title: Productovereenkomst configureren
description: Kenmerken toewijzen voor het afstemmen van producten van de Handel op bestaande aanbiedingen van de Marketplace van de Markt
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: e6368d30e16ccffcb1dfc64bdd56561116934b54
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Productovereenkomst configureren

Voordat u een aanbieding publiceert naar Walmart Marketplace, moet u ten minste één unieke identificatie uit uw productcataloguskenmerken toewijzen aan een van de vereiste productid&#39;s van de Marketplace. Deze stap is vereist om producten op de Marketplace van het Markeren van de Markt van het Markeren aan te passen.

Voor productmatching moet het product van de Handel minstens één van de volgende product Identifiers (Product IDs) in de catalogusattributen hebben.

**Vereiste product-id&#39;s van Walmart**

| **Type geaccepteerd** | **Naam** | **Doel** | **Acceptabele cijfers** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaal handelsitem | Algemeen doel, wereldwijd gebruikt | 14 cijfers |
| ISBN | International Standard Book Number | Paperback, hardcover en elektronische boeken | 10 of 13 cijfers |
| ISSN | Internationaal serienummer | Serienummer van 8 cijfers dat wordt gebruikt voor de identificatie van tijdschriften, tijdschriften, dagbladen en tijdschriften van alle soorten die worden geleverd op alle gedrukte en elektronische media | 8 cijfers |
| ISBN | International Standard Book Number | Paperback, hardcover en elektronisch | 12 cijfers |

Als u een ander type product-id-kenmerk in uw catalogus hebt, zet u dit om in een van de vereiste typen. Dan, kaart het aan het overeenkomstige attribuut van de Marketplace van de Markt van de Markt in de configuratie van de Lijst voor de opslag van de Manager van het Kanaal.

## Instellingen voor productkenmerken configureren

1. Op de [!UICONTROL Listings] pagina voor het verbonden verkoopkanaal, selecteer één of meerdere producten in *Concept* status.

1. Selecteren **[!UICONTROL Settings]**.

   - Zoek het kenmerk Walmart Marketplace dat u wilt toewijzen.

   - Selecteer het overeenkomstige kenmerk in de opslagcatalogus.

      In het volgende voorbeeld wordt het kenmerk UPC van de Marketplace Walmart gekoppeld aan het kenmerk UPC in de productcatalogus.
   ![Kenmerken toewijzen voor productcriteria](assets/products-map-attributes-for--match.png)

   - Selecteren **[!UICONTROL Save]**.


## Toegewezen kenmerkconfiguratie bijwerken

Wijzig de product-id van de Handel voor overeenkomende producten door de toegewezen kenmerkinstellingen bij te werken.

Bijvoorbeeld, in plaats van passende producten die op de het productkenmerkcode van UPC van de Handel worden gebaseerd, kunt u aanpassen gebaseerd op SKU. U kunt ook aanvullende kenmerken toewijzen om de overeenkomst te verbeteren.

1. Van de **[!UICONTROL Listings]**, selecteert u **[!UICONTROL Settings]**.

1. Voor de de attributenvorm van de Kaart, verander de in kaart gebrachte attributenconfiguratie zoals nodig.
