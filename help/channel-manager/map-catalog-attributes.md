---
title: Kenmerken van catalogus toewijzen
description: '''Map attributes for matching [DNL! Handel] producten naar bestaande [!DNL Walmart Marketplace] lijsten en gegevens synchroniseren tussen [!DNL Channel Manager] en [!DNL Walmart]."'
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 3f6039ad78ff500c31129bee12d65e291e226567
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Kenmerken van catalogus toewijzen

Voordat je aanbiedingen verbindt van [!DNL Commerce] tot [!DNL Walmart Marketplace], moet u ten minste één unieke id van uw [!DNL Commerce] catalogus aan het overeenkomstige herkenningsteken van Walmart.

Deze stap is vereist voor [!DNL Commerce] producten naar bestaande [!DNL Walmart] aanbiedingen en productgegevens synchroniseren tussen [!DNL Commerce] en [!DNL Walmart]. De [!DNL Commerce] product moet ten minste één productkenmerk hebben dat overeenkomt met een van de volgende product-id&#39;s (Product ID&#39;s) die vereist zijn door [!DNL Walmart].

**Vereist [!DNL Walmart] product-id&#39;s**

| **Type geaccepteerd** | **Naam** | **Doel** | **Acceptabele cijfers** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaal handelsitem | Algemeen doel, wereldwijd gebruikt | 14 cijfers |
| ISBN | International Standard Book Number | Paperback, hardcover en elektronische boeken | 10 of 13 cijfers |
| ISSN | Internationaal serienummer | Serienummer van 8 cijfers dat wordt gebruikt voor de identificatie van tijdschriften, tijdschriften, dagbladen en tijdschriften van alle soorten die worden geleverd op alle gedrukte en elektronische media | 8 cijfers |
| UPC | Universele productcode | Standaardcode voor bijhouden van detailhandel | 12 cijfers |

Als uw catalogus geen overeenkomend kenmerk heeft, [Een bestaand cataloguskenmerk toevoegen of omzetten](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## Unieke id&#39;s toewijzen

1. Van de **[!UICONTROL Listings]** of **[!UICONTROL Orders]** pagina voor de winkel van verkoopkanalen, selecteert u **[!UICONTROL Channel Settings]**.

1. Aan **[!UICONTROL Channel Settings]**, selecteert u **[!UICONTROL Map Attributes]**.

   - Zoek de [!DNL Walmart Marketplace] toe te wijzen kenmerk.

   - Selecteer het desbetreffende kenmerk in het menu [!DNL Commerce] opslagcatalogus.

      In het volgende voorbeeld worden de [!UICONTROL Walmart Marketplace UPC] aan het attribuut UPC in de productcatalogus.

      ![Kenmerken toewijzen voor productcriteria](assets/products-map-attributes-for-match.png)

   - Selecteren **[!UICONTROL Save]**.


