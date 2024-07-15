---
title: Kenmerken voor Amazon-aanbiedingen
description: Amazon-Sales Channel biedt het tabblad [!UICONTROL Attributes] om de lijst met Amazon- en Commerce-kenmerken te controleren en na te gaan hoe deze worden toegewezen voor overeenkomende producten.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Kenmerken voor Amazon-aanbiedingen

In de weergave _[!UICONTROL Attributes]_wordt uw lijst met Amazon- en [!DNL Commerce] -kenmerken weergegeven. De lijst geeft ook kenmerken aan die zijn toegewezen voor overeenkomende producten. Voor meer informatie, zie [ Attributen ](./managing-attributes.md) beheren.

![ mening van Attributen ](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

Van de _[!UICONTROL Attributes]_mening, creeert u en herziet uw attributenmontages in de lijst en [ of geeft ](./creating-attributes.md) een attribuut uit.

## De lijst met kenmerken weergeven

1. Voor _Admin_ sidebar, ga **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klik op **[!UICONTROL Attributes]** in het menu aan de linkerkant, zoek een Amazon-kenmerk en bekijk de lijst met kenmerken.

1. Maak of bewerk indien nodig een kenmerk:

   - [ creeer ](./creating-attributes.md#create-an-attribute) en bepaal de Waarden van Attributen van de Vergelijking voor de attributen, klik **[!UICONTROL Create]**.

   - Om de montages ](./creating-attributes.md#edit-an-attribute) of het Aanpassen van de Waarden van Attributen voor de attributen te desactiveren of [ uit te geven, klik **[!UICONTROL Edit]**.

     Het uitgeven van een attribuut omvat het veranderen van de attributenafbeelding voor product aanpassing.

| Veld | Beschrijving |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | Het land voor verkoopactiviteit die in **[!DNL Amazon Marketplace]Land** tijdens [ wordt bepaald opslagintegratie ](./store-integration.md). |
| [!UICONTROL ID] | Algemene kenmerkwaarde die door [!DNL Commerce] wordt gegenereerd wanneer het kenmerk wordt gemaakt. |
| [!UICONTROL Amazon Attribute Name] | The name of the attribute imported from Amazon. |
| [!UICONTROL Product Catalog Attribute Code] | Als dit kenmerk wordt toegewezen, wordt het kenmerk [!DNL Commerce] toegewezen aan de _[!UICONTROL Amazon Attribute Name]_voor overeenkomende catalogi en aanbiedingsproducten. |
| [!UICONTROL Overwrite Magento Values] | Als het kenmerk is ingesteld op `Overwrite Existing Magento Values` in Kenmerkinstellingen, wordt in de tabel `Enabled` weergegeven. Ingeschakeld betekent dat wanneer bijgewerkte productinformatie voor het kenmerk wordt ontvangen van Amazon, de nieuwe informatie de bijbehorende informatie voor het product in de [!DNL Commerce] -catalogus bijwerkt (overschrijft). Dit kan ook van invloed zijn op de producten die in uw [!DNL Commerce] -winkels worden vermeld. |
| Status | Geeft aan of de kenmerkwaarden zijn geïmporteerd in [!DNL Commerce] en toegewezen aan een [!DNL Commerce] -kenmerk. Opties: `Enabled` / `Disabled` |
| Handeling | Geeft de taakopties aan die beschikbaar zijn voor het kenmerk. Opties: `Create` / `Edit` |
