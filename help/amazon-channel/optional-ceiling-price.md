---
title: "Intelligente prijsregel: Optionele maximumprijs"
description: Gebruik optionele prijsinstellingen voor plafonds om je hoogste productprijs te beschermen tegen de intelligente prijsregels die je Amazon-aanbiedingen beheren.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Intelligente prijsregel: Optionele maximumprijs

Secties van een intelligente prijsstellingsregel omvatten:

- [Regeltype selecteren](./intelligent-repricing-rules.md)
- [Voorwaardelijke variaties van concurrent](./competitor-conditional-variances.md)
- [Prijsaanpassing](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- Optionele maximumprijs

De geautomatiseerde prijsmontages van de plafondprijs beschermen automatisch uw hoogste productprijs tegen de intelligente prijsregels, toelatend u om een plafond (hoogste prijs) voor uw intelligente prijsregels te bepalen.

## Optionele maximumprijs configureren

Definieer de optionele hoogste prijsinstellingen in het dialoogvenster _[!UICONTROL Optional Ceiling Price]_sectie.

1. Voor **[!UICONTROL Ceiling Price Source]**, kiest u een kenmerk.

   Selecteer uw [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} dat uw relatieve plafondlimiet aangeeft. Als je bijvoorbeeld niet wilt dat de Amazon-aanbiedingsprijs boven de MSRP van je object komt, kies je de `Manufacturer's Suggested Retail Price` kenmerk.

1. Voor **[!UICONTROL Ceiling Price Action]** kiest u een optie.

   - `Decrease By` - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een lagere maximumprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.

   - `Increase By` - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een hogere maximumprijs voor de regel wordt gecreëerd, voordat de regel aan Amazon wordt aangeboden.

   - `Match` - Kies wanneer je de prijs van de aanbieding niet boven de gedefinieerde prijs wilt laten schommelen _[!UICONTROL Ceiling Price Source]_waarde. Wanneer ingesteld op `Match`de_[!UICONTROL Apply]_ en _[!UICONTROL Ceiling Adjustment Amount]_velden zijn uitgeschakeld.

1. Laat de **[!UICONTROL Apply]** standaard als `Apply as percentage`.

1. Voor **[!UICONTROL Ceiling Adjustment Price]** Voer de numerieke waarde in voor het percentage dat u wilt gebruiken om uw _[!UICONTROL Ceiling Price Source]_waarde.

In dit voorbeeld, wordt de plafondprijs geplaatst om 2% onder MSRP van het punt te zijn.

![Intelligente prijsregeling - optionele maximumprijs](assets/ob-intelligent-price-rule-ceiling.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Ceiling Price Source] | Kies de optie [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} dat uw relatieve plafondlimiet aangeeft. Als je bijvoorbeeld niet wilt dat de prijs van je productaanbieding boven de MSRP van je object komt, kies je de `Manufacturer's Suggested Retail Price` kenmerk. |
| [!UICONTROL Ceiling Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<ul><li>**[!UICONTROL Decrease By]** - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een lagere maximumprijs voor de regel wordt verkregen, voordat deze aan Amazon wordt aangeboden.</li><li>**[!UICONTROL Increase By]** - Kies wanneer u de definitie wilt _[!UICONTROL Ceiling Price Source]_Waarde die moet worden aangepast, waardoor een hogere maximumprijs voor de regel wordt gecreëerd, voordat de regel aan Amazon wordt aangeboden.</li><li>**[!UICONTROL Match]** - Kies wanneer je de prijs van de aanbieding niet boven de gedefinieerde prijs wilt laten schommelen _[!UICONTROL Ceiling Price Source]_waarde. Wanneer ingesteld op `Match`de_[!UICONTROL Apply]_ en _[!UICONTROL Ceiling Adjustment Amount]_velden zijn uitgeschakeld.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Een procentuele aanpassing ten opzichte van de _[!UICONTROL Ceiling Price Source]_waarde. |
| [!UICONTROL Ceiling Price Adjustment] | Voer de numerieke waarde voor het percentage in om uw _[!UICONTROL Ceiling Price Source]_waarde. |
