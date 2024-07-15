---
title: "Intelligente prijsregel: optionele maximumprijs"
description: Gebruik optionele prijsinstellingen voor plafonds om je hoogste productprijs te beschermen tegen de intelligente prijsregels die je Amazon-aanbiedingen beheren.
feature: Sales Channels, Price Rules
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Intelligente prijsregel: optionele maximumprijs

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

   Selecteer uw [!DNL Commerce] [ productattribuut ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) dat op uw relatieve plafondgrens wijst. Als je bijvoorbeeld niet wilt dat de Amazon-aanbiedingsprijs boven de MSRP van je object komt, kiest u het kenmerk `Manufacturer's Suggested Retail Price` .

1. Kies bij **[!UICONTROL Ceiling Price Action]** een optie.

   - `Decrease By` - Kies wanneer u de gedefinieerde _[!UICONTROL Ceiling Price Source]_-waarde wilt aanpassen, zodat een lagere plafondprijs voor de regel wordt verkregen voordat u de regel aanbiedt aan Amazon.

   - `Increase By` - Kies wanneer u de gedefinieerde _[!UICONTROL Ceiling Price Source]_-waarde wilt aanpassen, zodat een hogere plafondprijs voor de regel wordt verkregen voordat u de regel aanbiedt aan Amazon.

   - `Match` - Kies wanneer u niet wilt dat de prijs van de aanbieding boven de gedefinieerde _[!UICONTROL Ceiling Price Source]_-waarde schommelt. Als u deze instelt op `Match` , worden de velden_[!UICONTROL Apply]_ en _[!UICONTROL Ceiling Adjustment Amount]_uitgeschakeld.

1. Laat de standaardwaarde **[!UICONTROL Apply]** op `Apply as percentage` staan.

1. Voer bij **[!UICONTROL Ceiling Adjustment Price]** de numerieke waarde in voor het percentage waarmee de _[!UICONTROL Ceiling Price Source]_-waarde wordt aangepast.

In dit voorbeeld, wordt de plafondprijs geplaatst om 2% onder MSRP van het punt te zijn.

![ Intelligente repricing regel - facultatieve plafondprijs ](assets/ob-intelligent-price-rule-ceiling.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Ceiling Price Source] | Kies het [!DNL Commerce] [ productattribuut ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) dat op uw relatieve plafondgrens wijst. Als u bijvoorbeeld niet wilt dat de aanbiedingsprijs van het product boven de MSRP van het item komt, kiest u het kenmerk `Manufacturer's Suggested Retail Price` . |
| [!UICONTROL Ceiling Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<ul><li>**[!UICONTROL Decrease By]** - Kies wanneer u de gedefinieerde _[!UICONTROL Ceiling Price Source]_-waarde wilt aanpassen, zodat een lagere plafondprijs voor de regel wordt verkregen voordat u de regel aanbiedt aan Amazon.</li><li>**[!UICONTROL Increase By]** - Kies wanneer u de gedefinieerde _[!UICONTROL Ceiling Price Source]_-waarde wilt aanpassen, zodat een hogere plafondprijs voor de regel wordt verkregen voordat u de regel aanbiedt aan Amazon.</li><li>**[!UICONTROL Match]** - Kies wanneer u niet wilt dat de prijs van de aanbieding boven de gedefinieerde _[!UICONTROL Ceiling Price Source]_-waarde schommelt. Als u deze instelt op `Match` , worden de velden_[!UICONTROL Apply]_ en _[!UICONTROL Ceiling Adjustment Amount]_uitgeschakeld.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Een percentageaanpassing ten opzichte van de _[!UICONTROL Ceiling Price Source]_-waarde. |
| [!UICONTROL Ceiling Price Adjustment] | Voer de numerieke waarde voor het percentage in om de _[!UICONTROL Ceiling Price Source]_-waarde aan te passen. |
