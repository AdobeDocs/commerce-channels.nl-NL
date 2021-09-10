---
title: Toewijzing Amazon-kenmerk weergeven
description: Verifieer waarden voor uw verbonden attributen van de Handel aan correcte synchronisatie tussen Handel en Amazon.
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Amazon-kenmerktoewijzing weergeven

Als u Amazon-kenmerken toewijst aan [!DNL Commerce]-kenmerken, houdt Amazon het verkoopkanaal bij en biedt het een filterbare lijst met alle Amazon-waarden. Op deze pagina kunt u waarden voor de gekoppelde [!DNL Commerce]-kenmerken controleren door de kenmerken correct te synchroniseren tussen [!DNL Commerce] en Amazon. U kunt gesynchroniseerde waarden controleren voor Amazon-kenmerken die zijn gekoppeld aan een [!DNL Commerce]-kenmerk. Zie [Kenmerken maken en bewerken](./creating-attributes.md) om uw Amazon-kenmerken te maken of te bewerken.

De _Amazon-waarde_ is afhankelijk van het kenmerktype en het Amazon-kenmerk dat u bekijkt. Een vermelde Amazon-waarde voor `Label` zou bijvoorbeeld een tekstwaarde zijn, terwijl `AmazonListPrice` een numerieke waarde zou zijn. De status geeft aan of de Amazon-waarde is geïmporteerd.

## Kenmerkwaarden weergeven

1. Ga op de _[!UICONTROL Admin]_zijbalk naar **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Klik **[!UICONTROL Attributes]** in het linkerzijmenu, bepaal de plaats van een attribuut van Amazon, en klik of **[!UICONTROL Create]** of **[!UICONTROL Edit]** in _[!UICONTROL Action]_kolom.

1. Klik op het tabblad **[!UICONTROL Matching Attribute Values]**.

   Aanbiedingen met een overeenkomend [!DNL Commerce] catalogusproduct geven een gekoppelde waarde aan in de kolom _Magento Product SKU_. Als u op een koppeling klikt, wordt de bijbehorende pagina met productdetails voor de catalogus geopend. Wijzigingen in Amazon-kenmerken op de productdetailpagina worden niet gesynchroniseerd met Amazon-verkoopkanaal.

>[!TIP]
>Zie [Vereiste gegevens bijwerken](./amazon-manually-update-incomplete-listing.md) als u de toewijzing voor een lijst wilt bewerken of toewijzen aan een catalogusproduct.

![Kenmerkwaarden weergeven](assets/amazon-managing-attribute-values.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Region] | Het gebied voor verkoopactiviteit die in **[!DNL Amazon Marketplace]Land** tijdens winkelintegratie wordt bepaald. |
| [!UICONTROL Magento Product SKU] | Geeft de [!DNL Commerce] producten aan die met de Amazon store worden gesynchroniseerd. De waarde is een product-id die is toegewezen door [!DNL Commerce] en is gekoppeld aan een product in de catalogus. Klik op de koppeling om het product te openen in [!DNL Commerce]. |
| [!UICONTROL ASIN] | Hiermee wordt de unieke identificatiecode aangegeven die door Amazon is toegekend aan het product met een standaard Amazon-identificatienummer (ASIN) van 10 tekens dat uit een alfanumeriek identificatienummer bestaat. |
| [!UICONTROL Amazon Value] | Geeft de waarde voor het geselecteerde kenmerk aan. De Amazon-waarde is afhankelijk van het kenmerktype en het Amazon-kenmerk dat u bekijkt. Een vermelde Amazon-waarde voor `Label` zou bijvoorbeeld een tekstwaarde zijn, terwijl `AmazonListPrice` een numerieke waarde zou zijn. De status geeft aan of de Amazon-waarde is geïmporteerd. |
| [!UICONTROL Status] | Geeft aan of de kenmerkwaarden zijn geïmporteerd in [!DNL Commerce] en gekoppeld aan een [!DNL Commerce]-kenmerk. Opties: `Not Imported` / `Imported` |
