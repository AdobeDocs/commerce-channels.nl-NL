---
title: Amazon-kenmerktoewijzing weergeven
description: Verifieer waarden voor uw verbonden attributen van de Handel aan correcte synchronisatie tussen Handel en Amazon.
feature: Sales Channels, Products, Configuration
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Amazon-kenmerktoewijzing weergeven

Als u Amazon-kenmerken toewijst aan [!DNL Commerce] kenmerken, houdt Amazon het verkoopkanaal bij en biedt een filterbare lijst met alle Amazon-waarden. Op deze pagina kunt u waarden voor de gekoppelde waarden verifiëren [!DNL Commerce] kenmerken correct synchroniseren tussen [!DNL Commerce] en Amazon. U kunt gesynchroniseerde waarden controleren voor Amazon-kenmerken die zijn gekoppeld aan een [!DNL Commerce] kenmerk. Als u uw Amazon-kenmerken wilt maken of bewerken, raadpleegt u [Kenmerken maken en bewerken](./creating-attributes.md).

De _Amazon Value_ verschilt afhankelijk van het kenmerktype en het Amazon-kenmerk dat u bekijkt. Bijvoorbeeld een Amazon-waarde in de lijst voor `Label` zou een tekstwaarde zijn `AmazonListPrice` zou een numeriek bedrag zijn. De status geeft aan of de Amazon-waarde is geïmporteerd.

## Kenmerkwaarden weergeven

1. Op de _[!UICONTROL Admin]_zijbalk, ga naar **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Klikken **[!UICONTROL Attributes]** Zoek in het linkermenu een Amazon-kenmerk en klik op **[!UICONTROL Create]** of **[!UICONTROL Edit]** in de _[!UICONTROL Action]_kolom.

1. Klik op de knop **[!UICONTROL Matching Attribute Values]** tab.

   Aanbiedingen met een overeenkomende [!DNL Commerce] catalogusproduct bevat een gekoppelde waarde in het dialoogvenster _[!UICONTROL Magento Product SKU]_kolom. Als u op een koppeling klikt, wordt de bijbehorende pagina met productdetails voor de catalogus geopend. Wijzigingen in Amazon-kenmerken op de productdetailpagina worden niet gesynchroniseerd met Amazon-verkoopkanaal.

>[!TIP]
>Als u de toewijzing voor een aanbieding wilt bewerken of toewijzen aan een catalogusproduct, raadpleegt u [Vereiste gegevens bijwerken](./amazon-manually-update-incomplete-listing.md).

![Kenmerkwaarden weergeven](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region] | Het gebied voor verkoopactiviteiten zoals gedefinieerd in **[!DNL Amazon Marketplace]Land** tijdens winkelintegratie. |
| [!UICONTROL Magento Product SKU] | Hiermee wordt de [!DNL Commerce] producten die worden gesynchroniseerd met de Amazon Store. De waarde is een product-id die is toegewezen door [!DNL Commerce] en zijn gekoppeld aan een product in de catalogus. Als u het product wilt openen in [!DNL Commerce]klikt u op de koppeling. |
| [!UICONTROL ASIN] | Hiermee wordt de unieke identificatiecode aangegeven die door Amazon is toegekend aan het product met een standaard Amazon-identificatienummer (ASIN) van 10 tekens dat uit een alfanumeriek identificatienummer bestaat. |
| [!UICONTROL Amazon Value] | Geeft de waarde voor het geselecteerde kenmerk aan. De Amazon-waarde is afhankelijk van het kenmerktype en het Amazon-kenmerk dat u bekijkt. Bijvoorbeeld een Amazon-waarde in de lijst voor `Label` zou een tekstwaarde zijn `AmazonListPrice` zou een numeriek bedrag zijn. De status geeft aan of de Amazon-waarde is geïmporteerd. |
| [!UICONTROL Status] | Geeft aan of de kenmerkwaarden zijn geïmporteerd in [!DNL Commerce] en die verband houden met een [!DNL Commerce] kenmerk. Opties: `Not Imported` / `Imported` |
