---
title: Amazon-verkoopkanaal - [!UICONTROL Price Adjustment]
description: Prijsaanpassingen configureren om de prijsberekening te bepalen wanneer u de prijsbron van de Amazon-concurrent hebt geïdentificeerd.
feature: Sales Channels, Price Rules
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>De sectie Prijsaanpassing wijkt enigszins af voor de regels voor standaardprijzen en intelligente prijsaanpassingen. **[!UICONTROL Match Competitor Price]** is alleen beschikbaar onder _[!UICONTROL Price Action]_wanneer **[!UICONTROL Rule Type]**is ingesteld op `Intelligent repricing rule` .

Secties van een intelligente prijsstellingsregel omvatten:

- [Regeltype selecteren](./intelligent-repricing-rules.md)
- [Voorwaardelijke variaties van concurrent](./competitor-conditional-variances.md)
- Prijsaanpassing
- [Floor Price](./floor-price.md)
- [Optionele maximumprijs](./optional-ceiling-price.md)

De prijsaanpassing bepaalt de prijsberekening wanneer u de prijsbron van de concurrent hebt vastgesteld.

## Prijsaanpassing configureren

Definieer de prijsaanpassing in de sectie _[!UICONTROL Price Adjustment]_.

1. Kies bij **[!UICONTROL Price Action]** een optie:

   - `Decrease By` - Kies wanneer u de waarde van de gedefinieerde prijsbron wilt verlagen, zodat een lagere prijs voor de regel wordt verkregen, voordat u deze aanbiedt aan Amazon.

   - `Increase By` - Kies wanneer u de waarde van de gedefinieerde prijsbron wilt aanpassen, zodat de regel een hogere prijs krijgt, voordat u de regel aanbiedt aan Amazon.

   - `Match Competitor Price` - (Intelligente het verprijsen regel slechts) verkies wanneer u uw Amazon lijstprijs wilt veranderen om de [ laagste concurrent ](./lowest-competitor-pricing.md) prijs aan te passen, die op uw concurrent wordt gebaseerd terugkoppelt en variantieparameters. Als u deze instelt op `Match Competitor Price` , worden de velden _[!UICONTROL Apply]_en_[!UICONTROL Adjustment Amount]_ verwijderd.

1. Kies bij **[!UICONTROL Apply]** een optie:

   - `Apply as percentage` - kies wanneer u de bepaalde **[!UICONTROL Magento Price Source]** die in uw [ wordt bepaald Prijs van de Lijst ](./listing-price.md) door een percentage wordt aangepast wilt.

   - `Apply as fixed amount` - kies wanneer u de bepaalde **[!UICONTROL Magento Price Source]** die in uw [ wordt bepaald Prijs van de Lijst ](./listing-price.md) door een vast bedrag wordt aangepast wilt.

1. Voer bij **[!UICONTROL Adjustment Amount]** (vereist) de numerieke waarde voor de prijsaanpassing in.

   - Wanneer **[!UICONTROL Apply]** is ingesteld op `Apply as percentage` , voert u de percentagewaarde in (bijvoorbeeld: voer `25` in voor een aanpassing van 25% procent).

   - Wanneer **[!UICONTROL Apply]** is ingesteld op `Apply as fixed amount` , voert u de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: voer `25` in voor een vaste aanpassing van € 25).

![ Intelligente het opnieuw bepalen regel - prijsaanpassing ](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<br>**[!UICONTROL Decrease By]**- kies wanneer u de bepaalde _[!UICONTROL Magento Price Source]_die in uw [ wordt bepaald Prijs van de Lijst ](./listing-price.md) wilt worden aangepast, creërend een lagere prijs voor de regel, alvorens aan Amazon aan te bieden.<br>**[!UICONTROL Increase By]**- kies wanneer u de bepaalde_[!UICONTROL Magento Price Source]_ die in uw [ wordt bepaald Prijs van de Lijst ](./listing-price.md) omhoog wilt worden aangepast, creërend een hogere prijs voor de regel, alvorens aan Amazon aan te bieden.<br>**[!UICONTROL Match Competitor Price]**- (Intelligente het verprijsen regel slechts) verkies wanneer u uw Amazon lijstprijs wilt veranderen om de [ laagste concurrent ](./lowest-competitor-pricing.md) prijs aan te passen, die op uw concurrent wordt gebaseerd terugkoppelt en variantieparameters. Wanneer gekozen, pas __ toe en _de gebieden van het Bedrag van de Aanpassing_ worden verwijderd. |
| [!UICONTROL Apply] | Opties:<br>**[!UICONTROL Apply as percentage]**- kies wanneer u de bepaalde _[!UICONTROL Magento Price Source]_die in uw [ wordt bepaald Prijs van de Lijst ](./listing-price.md) door een percentage wordt aangepast wilt.<br>**[!UICONTROL Apply as fixed amount]**- kies wanneer u de bepaalde_[!UICONTROL Magento Price Source]_ die in uw [ wordt bepaald Prijs van de Lijst ](./listing-price.md) door een vast bedrag wordt aangepast wilt. |
| [!UICONTROL Adjustment Amount] | Vereist.<br> Als u `Apply as percentage` for **[!UICONTROL Apply]** kiest, voert u de percentagewaarde in (bijvoorbeeld: voer `25` in voor een aanpassing van 25%).<br> Als u `Apply as fixed amount` for **[!UICONTROL Apply]** kiest, voert u de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: voer `25` in voor een vaste aanpassing van € 25). |
