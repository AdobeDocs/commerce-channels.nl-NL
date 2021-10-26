---
title: '"Intelligente prijsregel: Optionele maximumprijs"'
description: Gebruik optionele prijsinstellingen voor plafonds om je hoogste productprijs te beschermen tegen de intelligente prijsregels die je Amazon-aanbiedingen beheren.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Intelligent repricing rule: optional ceiling price

Sections of an intelligent repricing rule include:

- [Select Rule Type](./intelligent-repricing-rules.md)
- [Voorwaardelijke variaties van concurrent](./competitor-conditional-variances.md)
- [Price Adjustment](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- Optional Ceiling Price

De geautomatiseerde prijsmontages van de plafondprijs beschermen automatisch uw hoogste productprijs tegen de intelligente prijsregels, toelatend u om een plafond (hoogste prijs) voor uw intelligente prijsregels te bepalen.

## Optionele maximumprijs configureren

Definieer de optionele hoogste prijsinstellingen in het dialoogvenster _[!UICONTROL Optional Ceiling Price]_sectie.

1. For **[!UICONTROL Ceiling Price Source]**, choose an attribute.

   Selecteer uw [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} waarmee uw relatieve plafondlimiet wordt aangegeven. Als je bijvoorbeeld niet wilt dat de Amazon-aanbiedingsprijs boven de MSRP van je object komt, kies je de `Manufacturer's Suggested Retail Price` kenmerk.

1. For **[!UICONTROL Ceiling Price Action]**, choose an option.

   - `Decrease By` - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een lagere maximumprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.

   - `Increase By` - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een hogere maximumprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.

   - `Match` - Choose when you do not want the listing price to fluctuate above the defined _[!UICONTROL Ceiling Price Source]_value. When set to `Match`, the_[!UICONTROL Apply]_ and _[!UICONTROL Ceiling Adjustment Amount]_fields are disabled.

1. Leave the **[!UICONTROL Apply]** default as `Apply as percentage`.

1. Voor **[!UICONTROL Ceiling Adjustment Price]** Voer de numerieke waarde in voor het percentage dat u wilt gebruiken om uw _[!UICONTROL Ceiling Price Source]_waarde.

In dit voorbeeld, wordt de plafondprijs geplaatst om 2% onder MSRP van het punt te zijn.

![Intelligent repricing rule - optional ceiling price](assets/ob-intelligent-price-rule-ceiling.png)

| Veld | Description |
|---|---|
| [!UICONTROL Ceiling Price Source] | Choose the [!DNL Commerce] [product attribute](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} that indicates your relative ceiling limit. Als je bijvoorbeeld niet wilt dat de prijs van je productaanbieding boven de MSRP van je object komt, kies je de `Manufacturer's Suggested Retail Price` kenmerk. |
| [!UICONTROL Ceiling Price Action] | Kies een handeling voor het aanpassen van de prijzen. Options:<ul><li>**[!UICONTROL Decrease By]** - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een lagere maximumprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.</li><li>**[!UICONTROL Increase By]** - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een hogere maximumprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.</li><li>**[!UICONTROL Match]** - Choose when you do not want the listing price to fluctuate above the defined _[!UICONTROL Ceiling Price Source]_value. Wanneer ingesteld op `Match`de_[!UICONTROL Apply]_ en _[!UICONTROL Ceiling Adjustment Amount]_velden zijn uitgeschakeld.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Een procentuele aanpassing ten opzichte van de _[!UICONTROL Ceiling Price Source]_waarde. |
| [!UICONTROL Ceiling Price Adjustment] | Voer de numerieke waarde voor het percentage in om uw _[!UICONTROL Ceiling Price Source]_waarde. |
