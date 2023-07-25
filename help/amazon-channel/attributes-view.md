---
title: Kenmerken voor Amazon-aanbiedingen
description: Amazon Sales Channel biedt de [!UICONTROL Attributes] om de lijst met Amazon- en handelskenmerken te controleren en te bepalen hoe deze worden toegewezen voor productmatching.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Kenmerken voor Amazon-aanbiedingen

De _[!UICONTROL Attributes]_toont je lijst met Amazon en [!DNL Commerce] kenmerken. De lijst geeft ook kenmerken aan die zijn toegewezen voor overeenkomende producten. Zie voor meer informatie [Kenmerken beheren](./managing-attributes.md).

![Kenmerken, weergave](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

Van de _[!UICONTROL Attributes]_bekijk, u en herzie uw attributenmontages in de lijst en [maken of bewerken](./creating-attributes.md) een kenmerk.

## De lijst met kenmerken weergeven

1. Op de _Beheer_ zijbalk, ga naar **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klikken **[!UICONTROL Attributes]** in het linkerzijmenu, bepaal de plaats van een attribuut van Amazon, en herzie uw attributenlijst.

1. Maak of bewerk indien nodig een kenmerk:

   - Naar [maken](./creating-attributes.md#create-an-attribute) en definieert u Overeenkomende kenmerkwaarden voor het kenmerk. Klik op **[!UICONTROL Create]**.

   - Om te deactiveren of [de instellingen bewerken](./creating-attributes.md#edit-an-attribute) of Overeenkomende kenmerkwaarden voor het kenmerk klikt u op **[!UICONTROL Edit]**.

     Het uitgeven van een attribuut omvat het veranderen van de attributenafbeelding voor product aanpassing.

| Veld | Beschrijving |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | Het land van verkoop als omschreven in  **[!DNL Amazon Marketplace]Land** tijdens [winkelintegratie](./store-integration.md). |
| [!UICONTROL ID] | Algemene kenmerkwaarde gegenereerd door [!DNL Commerce] wanneer het kenmerk wordt gemaakt. |
| [!UICONTROL Amazon Attribute Name] | De naam van het kenmerk dat uit Amazon is geïmporteerd. |
| [!UICONTROL Product Catalog Attribute Code] | Indien toegewezen, [!DNL Commerce] kenmerk toegewezen aan toewijzing aan _[!UICONTROL Amazon Attribute Name]_voor overeenkomende catalogi en aanbiedingsproducten. |
| [!UICONTROL Overwrite Magento Values] | Als het kenmerk is ingesteld op `Overwrite Existing Magento Values` in de kenmerkinstellingen wordt in de tabel `Enabled`. Ingeschakeld betekent dat wanneer bijgewerkte productinformatie voor het kenmerk wordt ontvangen van Amazon, de nieuwe informatie de bijbehorende informatie voor het product in uw [!DNL Commerce] catalogus. Het kan ook gevolgen hebben voor uw producten die in uw [!DNL Commerce] winkels. |
| Status | Geeft aan of de kenmerkwaarden zijn geïmporteerd in [!DNL Commerce] en toegewezen aan een [!DNL Commerce] kenmerk. Opties: `Enabled` / `Disabled` |
| Handeling | Geeft de taakopties aan die beschikbaar zijn voor het kenmerk. Opties: `Create` / `Edit` |
