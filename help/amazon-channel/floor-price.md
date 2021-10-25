---
title: '"Intelligente prijsregel: Floor Price'''
description: Gebruik instellingen voor de laagste prijs om de laagste prijs te bepalen voor een intelligente prijsregel voor het beheren van je Amazon-aanbiedingen.
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Intelligente prijsregel: bodemprijs

Secties van een intelligente prijsstellingsregel omvatten:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

De [bodemprijs](./floor-price.md) de instellingen beschermen automatisch uw laagste productprijs tegen de intelligente prijsregels. Gebruik deze instellingen om een ondergrens (laagste prijs) in te stellen voor uw intelligente prijsregels, zodat uw producten niet onder een gewenste prijs worden weergegeven.

Vloerprijskenmerken zijn gebaseerd op het bereik van de website als uw [!DNL Commerce] store gebruikt prijsbereik voor websites. Zie [Prijsbereik](./price-scope.md).

Floor Price wordt alleen gebruikt wanneer **[!UICONTROL Rule Type]** is ingesteld op `Intelligent repricing rule`.

## Minimumprijs configureren

Geef de laagste prijsinstelling op in het dialoogvenster _[!UICONTROL Floor Price]_sectie.

1. Voor **[!UICONTROL Floor Price Source]**, kiest u een kenmerk van een prijsbron.

   Kies de optie [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} waarmee de relatieve ondergrens wordt aangegeven. Als je bijvoorbeeld niet wilt dat de prijs van je Amazon-aanbieding onder de kosten van je object ligt, kies je de *Kosten* kenmerk.

1. Voor **[!UICONTROL Floor Price Action]** kiest u een optie.

   - `Decrease By` - Kies wanneer u de definitie wilt _[!UICONTROL Floor Price Source]_Waarde die moet worden aangepast, waardoor een lagere bodemprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.

   - `Increase By` - Kies wanneer u de definitie wilt _[!UICONTROL Floor Price Source]_Waarde die moet worden aangepast, waardoor een hogere bodemprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.

   - `Match` - Kies wanneer je de prijs van de aanbieding niet onder de gedefinieerde prijs wilt laten schommelen _[!UICONTROL Floor Price Source]_waarde. Wanneer ingesteld op `Match`de_[!UICONTROL Apply]_ en _[!UICONTROL Floor Adjustment Amount]_velden zijn uitgeschakeld.

1. Laat de **[!UICONTROL Apply]** standaard als `Apply as percentage`.

1. Voor **[!UICONTROL Floor Adjustment Price]** Voer de numerieke waarde in voor het percentage dat u wilt gebruiken om uw _[!UICONTROL Floor Price Source]_waarde.

In dit voorbeeld is de laagste prijs ingesteld op 3% boven de prijs van het object.

![Voorbeeld van een intelligente prijsregel - minimumprijs](assets/ob-intelligent-pricde-rule-floor-price.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Floor Price Source] | Kies de optie [!DNL Commerce] kenmerk dat uw relatieve ondergrens (laagste prijs) aangeeft. Als je bijvoorbeeld niet wilt dat de prijs van je Amazon-aanbieding onder de kosten van je object ligt, kies je de `Cost` kenmerk. |
| [!UICONTROL Floor Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<ul><li>**[!UICONTROL Decrease By]** - Kies wanneer u de definitie wilt _[!UICONTROL Floor Price Source]_Waarde die moet worden aangepast, waardoor een lagere bodemprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.</li><li>**[!UICONTROL Increase By]** - Kies wanneer u de definitie wilt _[!UICONTROL Floor Price Source]_Waarde die moet worden aangepast, waardoor een hogere bodemprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.</li><li>**[!UICONTROL Match]** - Kies wanneer je de prijs van de aanbieding niet onder de gedefinieerde prijs wilt laten schommelen _[!UICONTROL Floor Price Source]_waarde. Wanneer u kiest, wordt_[!UICONTROL Apply]_ en _[!UICONTROL Floor Adjustment Amount]_velden zijn uitgeschakeld.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Een procentuele aanpassing ten opzichte van de _[!UICONTROL Floor Price Source]_waarde. |
| [!UICONTROL Floor Adjustment Amount] | Voer de numerieke waarde voor het percentage in om uw _[!UICONTROL Floor Price Source]_waarde. |
