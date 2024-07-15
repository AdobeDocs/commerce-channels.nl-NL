---
title: Kenmerken van catalogus toewijzen
description: 'Map attributes for matching [DNL! Commerce] producten aan bestaande  [!DNL Walmart Marketplace]  lijsten en het synchroniseren van gegevens tussen  [!DNL Channel Manager]  en  [!DNL Walmart].'
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Kenmerken van catalogus toewijzen

Voordat u aanbiedingen van [!DNL Commerce] tot [!DNL Walmart Marketplace] verbindt, moet u ten minste één unieke id uit uw catalogus van [!DNL Commerce] toewijzen aan de overeenkomstige id van Walmart.

Deze stap is vereist om [!DNL Commerce] -producten af te stemmen op bestaande [!DNL Walmart] -aanbiedingen en om de productgegevens te synchroniseren tussen [!DNL Commerce] en [!DNL Walmart] . Het [!DNL Commerce] -product moet ten minste één productkenmerk hebben dat overeenkomt met een van de volgende product-id&#39;s (product-id&#39;s) die door [!DNL Walmart] worden vereist.

**Vereiste [!DNL Walmart] product IDs**

| **Toegelaten Type** | **Naam** | **Doel** | **Acceptabele Cijfers** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaal handelsitem | Algemeen doel, wereldwijd gebruikt | 14 cijfers |
| ISBN | International Standard Book Number | Paperback, hardcover en elektronische boeken | 10 of 13 cijfers |
| ISSN | Internationaal serienummer | Serienummer van 8 cijfers dat wordt gebruikt voor de identificatie van tijdschriften, tijdschriften, dagbladen en tijdschriften van alle soorten die worden geleverd op alle gedrukte en elektronische media | 8 cijfers |
| UPC | Universele productcode | Standaardcode voor bijhouden van detailhandel | 12 cijfers |

Als uw catalogus geen passend attribuut heeft, [ voeg of zet een bestaand catalogusattribuut ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) toe om.

## Unieke id&#39;s toewijzen

1. Selecteer **[!UICONTROL Channel Settings]** op de pagina **[!UICONTROL Listings]** of **[!UICONTROL Orders]** voor de winkel met verkoopkanalen.

1. Selecteer **[!UICONTROL Map Attributes]** bij **[!UICONTROL Channel Settings]** .

   - Zoek het kenmerk [!DNL Walmart Marketplace] dat u wilt toewijzen.

   - Selecteer het bijbehorende kenmerk in de opslagcatalogus van [!DNL Commerce] .

     In het volgende voorbeeld wordt het kenmerk [!UICONTROL Walmart Marketplace UPC] toegewezen aan het kenmerk UPC in de productcatalogus.

     ![ de attributen van de Kaart voor product passen criteria ](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"} aan

   - Selecteer **[!UICONTROL Save]** .
