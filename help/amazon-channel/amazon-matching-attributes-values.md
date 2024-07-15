---
title: Amazon-kenmerktoewijzing weergeven
description: Controleer de waarden voor de gekoppelde Commerce-kenmerken zodat deze correct kunnen worden gesynchroniseerd tussen Commerce en Amazon.
feature: Sales Channels, Products, Configuration
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Amazon-kenmerktoewijzing weergeven

Als u Amazon-kenmerken toewijst aan [!DNL Commerce] -kenmerken, houdt Amazon het verkoopkanaal bij en biedt het een filterbare lijst met alle Amazon-waarden. Gebruik deze pagina om de waarden voor de gekoppelde [!DNL Commerce] -kenmerken correct te synchroniseren tussen [!DNL Commerce] en Amazon. U kunt gesynchroniseerde waarden controleren voor Amazon-kenmerken die zijn gekoppeld aan een [!DNL Commerce] -kenmerk. Om uw attributen van Amazon tot stand te brengen of uit te geven, zie [ Creërend en het Uitgeven Attributen ](./creating-attributes.md).

De _Waarde van Amazon_ verschilt afhankelijk van het attribuuttype en de attributen van Amazon die u bekijkt. Een vermelde Amazon-waarde voor `Label` zou bijvoorbeeld een tekstwaarde zijn, terwijl `AmazonListPrice` een numerieke waarde zou zijn. De status geeft aan of de Amazon-waarde is geïmporteerd.

## Kenmerkwaarden weergeven

1. Ga op de zijbalk van _[!UICONTROL Admin]_naar **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]** .

1. Klik op **[!UICONTROL Attributes]** in het linkermenu, zoek een Amazon-kenmerk en klik op **[!UICONTROL Create]** of **[!UICONTROL Edit]** in de kolom _[!UICONTROL Action]_.

1. Klik op de tab **[!UICONTROL Matching Attribute Values]** .

   Aanbiedingen met een bijbehorend catalogusproduct van [!DNL Commerce] geven een gekoppelde waarde weer in de kolom _[!UICONTROL Magento Product SKU]_. Als u op een koppeling klikt, wordt de bijbehorende pagina met productdetails voor de catalogus geopend. Wijzigingen in Amazon-kenmerken op de productdetailpagina worden niet gesynchroniseerd met Amazon-verkoopkanaal.

>[!TIP]
>Om de afbeelding voor een lijst aan een catalogusproduct uit te geven of toe te wijzen, zie [ Update Vereiste Info ](./amazon-manually-update-incomplete-listing.md).

![ de attributenwaarden van de Mening ](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region] | Het gebied voor verkoopactiviteit die in **[!DNL Amazon Marketplace]Land** tijdens opslagintegratie wordt bepaald. |
| [!UICONTROL Magento Product SKU] | Geeft de [!DNL Commerce] -producten aan die worden gesynchroniseerd met de Amazon Store. De waarde is een product-id die door [!DNL Commerce] is toegewezen en die is gekoppeld aan een product in de catalogus. Klik op de koppeling om het product te openen in [!DNL Commerce] . |
| [!UICONTROL ASIN] | Hiermee wordt de unieke identificatiecode aangegeven die door Amazon is toegekend aan het product met een standaard Amazon-identificatienummer (ASIN) van 10 tekens dat uit een alfanumeriek identificatienummer bestaat. |
| [!UICONTROL Amazon Value] | Geeft de waarde voor het geselecteerde kenmerk aan. De Amazon-waarde is afhankelijk van het kenmerktype en het Amazon-kenmerk dat u bekijkt. Een vermelde Amazon-waarde voor `Label` zou bijvoorbeeld een tekstwaarde zijn, terwijl `AmazonListPrice` een numerieke waarde zou zijn. De status geeft aan of de Amazon-waarde is geïmporteerd. |
| [!UICONTROL Status] | Geeft aan of de kenmerkwaarden zijn geïmporteerd in [!DNL Commerce] en gekoppeld aan een [!DNL Commerce] -kenmerk. Opties: `Not Imported` / `Imported` |
