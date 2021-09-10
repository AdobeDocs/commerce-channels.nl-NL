---
title: '"Intelligente prijsregel: Optionele maximumprijs"'
description: Gebruik optionele prijsinstellingen voor plafonds om je hoogste productprijs te beschermen tegen de intelligente prijsregels die je Amazon-aanbiedingen beheren.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Intelligente prijsregel: facultatieve maximumprijs

Secties van een intelligente prijsstellingsregel omvatten:

- [Regeltype selecteren](./intelligent-repricing-rules.md)
- [Voorwaardelijke variaties van concurrent](./competitor-conditional-variances.md)
- [Prijsaanpassing](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- Optionele maximumprijs

De geautomatiseerde prijsmontages van de plafondprijs beschermen automatisch uw hoogste productprijs tegen de intelligente prijsregels, toelatend u om een plafond (hoogste prijs) voor uw intelligente prijsregels te bepalen.

## Optionele maximumprijs configureren

Definieer de optionele hoogste prijsinstellingen in de sectie _[!UICONTROL Optional Ceiling Price]_.

1. Kies bij **[!UICONTROL Ceiling Price Source]** een kenmerk.

   Selecteer uw [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;} dat uw relatieve plafondlimiet aangeeft. Als je bijvoorbeeld niet wilt dat de Amazon-aanbiedingsprijs boven de MSRP van je object komt, kies je het kenmerk `Manufacturer's Suggested Retail Price`.

1. Kies voor **[!UICONTROL Ceiling Price Action]** een optie.

   - `Decrease By` - Kies wanneer u de gedefinieerde  _[!UICONTROL Ceiling Price Source]_waarde wilt aanpassen, zodat een lagere maximumprijs voor de regel wordt verkregen, voordat u deze aan Amazon aanbiedt.

   - `Increase By` - Kies wanneer u de gedefinieerde  _[!UICONTROL Ceiling Price Source]_waarde wilt aanpassen, zodat een hogere maximumprijs voor de regel wordt verkregen, voordat u deze aan Amazon aanbiedt.

   - `Match` - Kies wanneer je de prijs van de aanbieding niet boven de gedefinieerde  _[!UICONTROL Ceiling Price Source]_waarde wilt laten schommelen. Wanneer ingesteld op `Match`, worden de velden_[!UICONTROL Apply]_ en _[!UICONTROL Ceiling Adjustment Amount]_uitgeschakeld.

1. Laat **[!UICONTROL Apply]** standaard als `Apply as percentage` staan.

1. Voer bij **[!UICONTROL Ceiling Adjustment Price]** de numerieke waarde voor het percentage in om de waarde _[!UICONTROL Ceiling Price Source]_aan te passen.

In dit voorbeeld, wordt de plafondprijs geplaatst om 2% onder MSRP van het punt te zijn.

![Intelligente prijsregeling - optionele maximumprijs](assets/ob-intelligent-price-rule-ceiling.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Ceiling Price Source] | Kies [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;} dat uw relatieve plafondlimiet aangeeft. Als u bijvoorbeeld niet wilt dat de aanbiedingsprijs van het product boven de MSRP van het object komt, kiest u het kenmerk `Manufacturer's Suggested Retail Price`. |
| [!UICONTROL Ceiling Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<ul><li>**[!UICONTROL Decrease By]** - Kies wanneer u de gedefinieerde  _[!UICONTROL Ceiling Price Source]_waarde wilt aanpassen, zodat een lagere maximumprijs voor de regel wordt verkregen, voordat u deze aan Amazon aanbiedt.</li><li>**[!UICONTROL Increase By]** - Kies wanneer u de gedefinieerde  _[!UICONTROL Ceiling Price Source]_waarde wilt aanpassen, zodat een hogere maximumprijs voor de regel wordt verkregen, voordat u deze aan Amazon aanbiedt.</li><li>**[!UICONTROL Match]** - Kies wanneer je de prijs van de aanbieding niet boven de gedefinieerde  _[!UICONTROL Ceiling Price Source]_waarde wilt laten schommelen. Wanneer ingesteld op `Match`, worden de velden_[!UICONTROL Apply]_ en _[!UICONTROL Ceiling Adjustment Amount]_uitgeschakeld.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Een percentageaanpassing ten opzichte van de  _[!UICONTROL Ceiling Price Source]_waarde. |
| [!UICONTROL Ceiling Price Adjustment] | Voer de numerieke waarde voor het percentage in om de waarde _[!UICONTROL Ceiling Price Source]_aan te passen. |
