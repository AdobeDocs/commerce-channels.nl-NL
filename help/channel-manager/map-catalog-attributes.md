---
title: Kenmerken van catalogus toewijzen
description: Kenmerken toewijzen voor overeenkomsten [DNL! Handel] producten naar bestaande [!DNL Walmart Marketplace] lijsten en gegevens synchroniseren tussen [!DNL Channel Manager] en [!DNL Walmart].
source-git-commit: dfe56db25bb569ad70fb1036d539797bbb126dd5
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Kenmerken van catalogus toewijzen

Voordat u aanbiedingen publiceert vanuit [!DNL Commerce] tot [!DNL Walmart Marketplace], moet u ten minste één unieke id van uw [!DNL Commerce] catalogus aan het overeenkomstige herkenningsteken van Walmart.
Deze stap is vereist voor [!DNL Commerce] producten naar bestaande [!DNL Walmart] aanbiedingen en productgegevens synchroniseren tussen [!DNL Commerce] en [!DNL Walmart].

Voor productmatching moet het product van de Handel ten minste één productkenmerk hebben dat één van de volgende product-id&#39;s (Product ID&#39;s) aanpast die door [!DNL Walmart].

**Vereiste product-id&#39;s van Walmart**

| **Type geaccepteerd** | **Naam** | **Doel** | **Acceptabele cijfers** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaal handelsitem | Algemeen doel, wereldwijd gebruikt | 14 cijfers |
| ISBN | International Standard Book Number | Paperback, hardcover en elektronische boeken | 10 of 13 cijfers |
| ISSN | Internationaal serienummer | Serienummer van 8 cijfers dat wordt gebruikt voor de identificatie van tijdschriften, tijdschriften, dagbladen en tijdschriften van alle soorten die worden geleverd op alle gedrukte en elektronische media | 8 cijfers |
| UPC | Universele productcode | Standaardcode voor bijhouden van detailhandel | 12 cijfers |

Als in uw catalogus geen kenmerk voorkomt dat overeenkomt met een van deze typen, [Een bestaand cataloguskenmerk toevoegen of omzetten](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## Unieke id&#39;s toewijzen

1. Op de [!UICONTROL Listings] pagina voor de winkel van verkoopkanalen, selecteert u **[!UICONTROL Settings]**.

   - Zoek het kenmerk Walmart Marketplace dat u wilt toewijzen.

   - Selecteer het desbetreffende kenmerk in het menu [!DNL Commerce] opslagcatalogus.

      In het volgende voorbeeld wordt het kenmerk UPC van de Marketplace Walmart gekoppeld aan het kenmerk UPC in de productcatalogus.
   ![Kenmerken toewijzen voor productcriteria](assets/products-map-attributes-for-match.png)

   - Selecteren **[!UICONTROL Save]**.


## Toegewezen kenmerkconfiguratie bijwerken

Wijzig de product-id van de Handel voor overeenkomende producten door de toegewezen kenmerkinstellingen bij te werken.

Bijvoorbeeld, in plaats van passende producten die op de het productkenmerkcode van UPC van de Handel worden gebaseerd, kunt u aanpassen gebaseerd op SKU. U kunt ook aanvullende kenmerken toewijzen om de overeenkomst te verbeteren.

1. Van de **[!UICONTROL Listings]**, selecteert u **[!UICONTROL Settings]**.

1. Voor de de attributenvorm van de Kaart, verander de in kaart gebrachte attributenconfiguratie zoals nodig.
