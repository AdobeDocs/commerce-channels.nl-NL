---
title: Attributen
description: Amazon Sales Channel biedt het tabblad [!UICONTROL Attributes] om de lijst met Amazon- en Commerce-kenmerken te controleren en na te gaan hoe deze worden toegewezen voor overeenkomende producten.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Attributen

In de weergave _[!UICONTROL Attributes]_wordt uw lijst met Amazon- en [!DNL Commerce]-kenmerken weergegeven. De lijst geeft ook kenmerken aan die zijn toegewezen voor overeenkomende producten. Zie [Kenmerken beheren](./managing-attributes.md) voor meer informatie.

![Kenmerken, weergave](assets/amazon-attributes-view.png)

In de weergave _[!UICONTROL Attributes]_kunt u de kenmerkinstellingen in de tabel bekijken en [een kenmerk maken of bewerken.](./creating-attributes.md)

## De lijst met kenmerken weergeven

1. Ga op de zijbalk _Admin_ naar **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klik **[!UICONTROL Attributes]** in het linkerzijmenu, bepaal de plaats van een attribuut van Amazon, en herzie uw attributenlijst.

1. Maak of bewerk indien nodig een kenmerk:

   - Als u [create](./creating-attributes.md#create-an-attribute) wilt en Overeenkomende kenmerkwaarden voor het kenmerk wilt definiëren, klikt u op **[!UICONTROL Create]**.

   - Als u de instellingen](./creating-attributes.md#edit-an-attribute) of Overeenkomende kenmerkwaarden voor het kenmerk wilt deactiveren of [bewerken, klikt u op **[!UICONTROL Edit]**.

      Het uitgeven van een attribuut omvat het veranderen van de attributenafbeelding voor product aanpassing.

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Country] | Het land voor verkoopactiviteit die in **[!DNL Amazon Marketplace]Land** tijdens [store integratie](./store-integration.md) wordt bepaald. |
| [!UICONTROL ID] | Algemene kenmerkwaarde die wordt gegenereerd door [!DNL Commerce] wanneer het kenmerk wordt gemaakt. |
| [!UICONTROL Amazon Attribute Name] | De naam van het kenmerk dat uit Amazon is geïmporteerd. |
| [!UICONTROL Product Catalog Attribute Code] | Indien toegewezen, het [!DNL Commerce] attribuut dat aan kaart wordt toegewezen _[!UICONTROL Amazon Attribute Name]_voor passende catalogus en lijstproducten. |
| [!UICONTROL Overwrite Magento Values] | Als het attribuut aan `Overwrite Existing Magento Values` in de Montages van Attributen wordt geplaatst, toont de lijst `Enabled`. Ingeschakeld betekent dat wanneer bijgewerkte productinformatie voor het kenmerk wordt ontvangen van Amazon, de nieuwe informatie de bijbehorende informatie voor het product in uw [!DNL Commerce]-catalogus bijwerkt (overschrijft). Het kan ook van invloed zijn op uw producten die in uw [!DNL Commerce]-winkels worden vermeld. |
| Status | Geeft aan of de kenmerkwaarden zijn geïmporteerd in [!DNL Commerce] en toegewezen aan een [!DNL Commerce]-kenmerk. Opties: `Enabled` / `Disabled` |
| Handeling | Geeft de taakopties aan die beschikbaar zijn voor het kenmerk. Opties: `Create` / `Edit` |
