---
title: Verkoopkanaal van Amazon - [!UICONTROL Price Adjustment]
description: Prijsaanpassingen configureren om de prijsberekening te bepalen wanneer u de prijsbron van de Amazon-concurrent hebt geïdentificeerd.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>De sectie Prijsaanpassing wijkt enigszins af voor de regels voor standaardprijzen en intelligente prijsaanpassingen. **[!UICONTROL Match Competitor Price]** is alleen beschikbaar onder _[!UICONTROL Price Action]_wanneer **[!UICONTROL Rule Type]**is ingesteld op `Intelligent repricing rule`.

Secties van een intelligente prijsstellingsregel omvatten:

- [Regeltype selecteren](./intelligent-repricing-rules.md)
- [Voorwaardelijke variaties van concurrent](./competitor-conditional-variances.md)
- Prijsaanpassing
- [Floor Price](./floor-price.md)
- [Optionele maximumprijs](./optional-ceiling-price.md)

De prijsaanpassing bepaalt de prijsberekening wanneer u de prijsbron van de concurrent hebt vastgesteld.

## Prijsaanpassing configureren

Bepaal uw prijsaanpassing in _[!UICONTROL Price Adjustment]_sectie.

1. Voor **[!UICONTROL Price Action]** kiest u een optie:

   - `Decrease By` - Kies wanneer u de waarde van de gedefinieerde prijsbron wilt aanpassen, zodat de prijs voor de regel lager wordt, voordat u de aanbieding aan Amazon uitvoert.

   - `Increase By` - Kies wanneer u de waarde van de gedefinieerde prijsbron wilt aanpassen, zodat een hogere prijs voor de regel wordt verkregen, voordat u deze aanbiedt aan Amazon.

   - `Match Competitor Price` - (Alleen de regel voor intelligente prijsstelling) Kies wanneer je de prijs van je Amazon-aanbieding wilt aanpassen aan de [laagste concurrent](./lowest-competitor-pricing.md) prijs, op basis van feedback van uw concurrent en variantieparameters. Wanneer ingesteld op `Match Competitor Price`de _[!UICONTROL Apply]_en_[!UICONTROL Adjustment Amount]_ velden worden verwijderd.

1. Voor **[!UICONTROL Apply]** kiest u een optie:

   - `Apply as percentage` - Kies wanneer u de definitie wilt **[!UICONTROL Magento Price Source]** gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) aangepast met een percentage.

   - `Apply as fixed amount` - Kies wanneer u de definitie wilt **[!UICONTROL Magento Price Source]** gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) aangepast met een vast bedrag.

1. Voor **[!UICONTROL Adjustment Amount]** (vereist), de numerieke waarde voor de prijsaanpassing invullen.

   - Wanneer **[!UICONTROL Apply]** is ingesteld op `Apply as percentage`Voer de percentagewaarde in (voorbeeld: enter `25` voor een aanpassing van 25%).

   - Wanneer **[!UICONTROL Apply]** is ingesteld op `Apply as fixed amount`Voer de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: enter `25` voor een vaste correctie van $ 25).

![Intelligente prijsregel - prijsaanpassing](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<br>**[!UICONTROL Decrease By]**- Kies wanneer u de definitie wilt _[!UICONTROL Magento Price Source]_gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) om te worden aangepast, waardoor een lagere prijs voor de regel wordt gemaakt, voordat je de aanbieding aan Amazon aanbiedt.<br>**[!UICONTROL Increase By]**- Kies wanneer u de definitie wilt_[!UICONTROL Magento Price Source]_ gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) worden aangepast, waardoor een hogere prijs voor de regel wordt gecreëerd, voordat wordt aangeboden aan Amazon.<br>**[!UICONTROL Match Competitor Price]**- (Alleen de regel voor intelligente prijsstelling) Kies wanneer je de prijs van je Amazon-aanbieding wilt aanpassen aan de [laagste concurrent](./lowest-competitor-pricing.md) prijs, op basis van feedback van uw concurrent en variantieparameters. Wanneer u kiest, wordt _Toepassen_ en _Aanpassingsbedrag_ velden worden verwijderd. |
| [!UICONTROL Apply] | Opties:<br>**[!UICONTROL Apply as percentage]**- Kies wanneer u de definitie wilt _[!UICONTROL Magento Price Source]_gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) aangepast met een percentage.<br>**[!UICONTROL Apply as fixed amount]**- Kies wanneer u de definitie wilt_[!UICONTROL Magento Price Source]_ gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) aangepast met een vast bedrag. |
| [!UICONTROL Adjustment Amount] | Vereist.<br>Als u `Apply as percentage` for **[!UICONTROL Apply]** Voer de percentagewaarde in (voorbeeld: enter `25` voor een aanpassing van 25%).<br>Als u `Apply as fixed amount` for **[!UICONTROL Apply]** Voer de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: enter `25` voor een vaste correctie van $ 25). |
