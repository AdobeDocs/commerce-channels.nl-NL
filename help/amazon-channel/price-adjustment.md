---
title: Prijsaanpassing
description: Prijsaanpassingen configureren om de prijsberekening te bepalen wanneer u de prijsbron van de Amazon-concurrent hebt geïdentificeerd.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Prijsaanpassing

>[!NOTE]
>
>De sectie Prijsaanpassing wijkt enigszins af voor de regels voor standaardprijzen en intelligente prijsaanpassingen. **[!UICONTROL Match Competitor Price]** is alleen beschikbaar onder  _[!UICONTROL Price Action]_wanneer **[!UICONTROL Rule Type]**deze is ingesteld op  `Intelligent repricing rule`.

Secties van een intelligente prijsstellingsregel omvatten:

- [Regeltype selecteren](./intelligent-repricing-rules.md)
- [Voorwaardelijke variaties van concurrent](./competitor-conditional-variances.md)
- Prijsaanpassing
- [Floor Price](./floor-price.md)
- [Optionele maximumprijs](./optional-ceiling-price.md)

De prijsaanpassing bepaalt de prijsberekening wanneer u de prijsbron van de concurrent hebt vastgesteld.

## Prijsaanpassing configureren

Definieer uw prijsaanpassing in de sectie _[!UICONTROL Price Adjustment]_.

1. Kies voor **[!UICONTROL Price Action]** een optie:

   - `Decrease By` - Kies wanneer u de waarde van de gedefinieerde prijsbron wilt aanpassen, zodat een lagere prijs voor de regel wordt verkregen, voordat u deze aanbiedt aan Amazon.

   - `Increase By` - Kies wanneer u de waarde van de gedefinieerde prijsbron wilt aanpassen, zodat een hogere prijs voor de regel wordt verkregen, voordat u deze aanbiedt aan Amazon.

   - `Match Competitor Price` - (Alleen de regel voor intelligente prijsstelling) Kies wanneer u de prijs van je Amazon-aanbieding wilt aanpassen aan de  [laagste ](./lowest-competitor-pricing.md) prijs van een concurrent, op basis van feedback en variantieparameters. Wanneer ingesteld op `Match Competitor Price`, worden de velden _[!UICONTROL Apply]_en_[!UICONTROL Adjustment Amount]_ verwijderd.

1. Kies voor **[!UICONTROL Apply]** een optie:

   - `Apply as percentage` - Kies wanneer je de gedefinieerde prijs in je  **[!UICONTROL Magento Price Source]** aanbieding met een percentage wilt  [ ](./listing-price.md) aanpassen.

   - `Apply as fixed amount` - Kies wanneer je de gedefinieerde prijs in je  **[!UICONTROL Magento Price Source]** aanbieding wilt aanpassen met een vaste  [ ](./listing-price.md) prijs.

1. Voer bij **[!UICONTROL Adjustment Amount]** (verplicht) de numerieke waarde voor de prijsaanpassing in.

   - Wanneer **[!UICONTROL Apply]** aan `Apply as percentage` wordt geplaatst, ga de percentagewaarde (voorbeeld: Voer `25` in voor een aanpassing van 25% procent).

   - Wanneer **[!UICONTROL Apply]** wordt geplaatst aan `Apply as fixed amount`, ga de numerieke waarde voor het vaste bedrag in (voorbeeld: Voer `25` in voor een vaste aanpassing van $25).

![Intelligente prijsregel - prijsaanpassing](assets/amazon-price-adjustment.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<br>**[!UICONTROL Decrease By]**- Kies wanneer u de gedefinieerde _[!UICONTROL Magento Price Source]_in uw [Aanbiedingsprijs](./listing-price.md) wilt aanpassen, zodat een lagere prijs voor de regel wordt gemaakt, voordat u deze aan Amazon aanbiedt.<br>**[!UICONTROL Increase By]**- Kies wanneer je de gedefinieerde prijs in je_[!UICONTROL Magento Price Source]_   [ ](./listing-price.md) aanbiedingsprijs wilt aanpassen, zodat je een hogere prijs voor de regel krijgt, voordat je een aanbieding naar Amazon doet.<br>**[!UICONTROL Match Competitor Price]**- (Alleen de regel voor intelligente prijsstelling) Kies wanneer u de prijs van je Amazon-aanbieding wilt aanpassen aan de  [laagste ](./lowest-competitor-pricing.md) prijs van een concurrent, op basis van feedback en variantieparameters. Als u deze optie kiest, worden de velden _Toepassen_ en _Aanpassingsbedrag_ verwijderd. |
| [!UICONTROL Apply] | Opties:<br>**[!UICONTROL Apply as percentage]**- Kies wanneer u de gedefinieerde _[!UICONTROL Magento Price Source]_in uw [Aanbiedingsprijs](./listing-price.md) wilt aanpassen met een percentage.<br>**[!UICONTROL Apply as fixed amount]**- Kies wanneer je de gedefinieerde prijs in je_[!UICONTROL Magento Price Source]_ aanbieding wilt aanpassen met een vaste  [ ](./listing-price.md) prijs. |
| [!UICONTROL Adjustment Amount] | Vereist.<br>Als u  `Apply as percentage` voor  **[!UICONTROL Apply]** kiest, voert u de percentagewaarde in (bijvoorbeeld: Voer een aanpassing  `25` van 25% in).<br>Als u  `Apply as fixed amount` voor  **[!UICONTROL Apply]** kiest, voert u de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: Voer  `25` een vaste correctie van € 25 in). |
