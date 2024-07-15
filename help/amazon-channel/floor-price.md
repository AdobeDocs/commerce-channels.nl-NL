---
title: "Intelligente prijsregel voor herstelling: prijs op de vloer"
description: Gebruik instellingen voor de laagste prijs om de laagste prijs te bepalen voor een intelligente prijsregel voor het beheren van je Amazon-aanbiedingen.
feature: Sales Channels, Price Rules
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Intelligente prijsregel: Floor Price

Secties van een intelligente prijsstellingsregel omvatten:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

De [ montages van de vloerprijs ](./floor-price.md) beschermen automatisch uw laagste productprijs tegen de intelligente prijsstellingsregels. Gebruik deze instellingen om een ondergrens (laagste prijs) in te stellen voor uw intelligente prijsregels, zodat uw producten niet onder een gewenste prijs worden weergegeven.

Vloerprijskenmerken zijn gebaseerd op het bereik van de website als uw [!DNL Commerce] -winkel een prijsbereik voor websites gebruikt. Zie [ het Toepassingsgebied van de Prijs ](./price-scope.md).

De prijs onder de grond wordt alleen gebruikt wanneer **[!UICONTROL Rule Type]** is ingesteld op `Intelligent repricing rule` .

## Minimumprijs configureren

Definieer de laagste prijsinstelling in de sectie _[!UICONTROL Floor Price]_.

1. Kies bij **[!UICONTROL Floor Price Source]** een kenmerk van een prijsbron.

   Kies het [!DNL Commerce] [ productattribuut ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) dat op uw relatieve vloergrens wijst. Bijvoorbeeld, als u uw Amazon aanbiedingsprijs niet onder de kosten van uw punt wilt gaan, zou u het *1} attribuut van Kosten {kiezen.*

1. Kies bij **[!UICONTROL Floor Price Action]** een optie.

   - `Decrease By` - Bepaal wanneer u de gedefinieerde _[!UICONTROL Floor Price Source]_-waarde wilt aanpassen, zodat de regel een lagere bodemprijs krijgt, voordat u de regel aanbiedt aan Amazon.

   - `Increase By` - Kies wanneer u de gedefinieerde _[!UICONTROL Floor Price Source]_-waarde wilt aanpassen, zodat een hogere bodemprijs voor de regel wordt verkregen, voordat u de regel aanbiedt aan Amazon.

   - `Match` - Kies wanneer u niet wilt dat de prijs van de aanbieding onder de gedefinieerde _[!UICONTROL Floor Price Source]_-waarde schommelt. Als u deze instelt op `Match` , worden de velden_[!UICONTROL Apply]_ en _[!UICONTROL Floor Adjustment Amount]_uitgeschakeld.

1. Laat de standaardwaarde **[!UICONTROL Apply]** op `Apply as percentage` staan.

1. Voer bij **[!UICONTROL Floor Adjustment Price]** de numerieke waarde in voor het percentage waarmee de _[!UICONTROL Floor Price Source]_-waarde wordt aangepast.

In dit voorbeeld is de laagste prijs ingesteld op 3% boven de prijs van het object.

![ Intelligente het repricing regelvoorbeeld - vloerprijs ](assets/ob-intelligent-pricde-rule-floor-price.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Floor Price Source] | Kies het kenmerk [!DNL Commerce] dat uw relatieve ondergrens (laagste prijs) aangeeft. Als je bijvoorbeeld niet wilt dat de prijs van je Amazon-aanbieding onder de kosten van je object daalt, kies je het kenmerk `Cost` . |
| [!UICONTROL Floor Price Action] | Kies een handeling voor het aanpassen van de prijzen. Opties:<ul><li>**[!UICONTROL Decrease By]** - Bepaal wanneer u de gedefinieerde _[!UICONTROL Floor Price Source]_-waarde wilt aanpassen, zodat de regel een lagere bodemprijs krijgt, voordat u de regel aanbiedt aan Amazon.</li><li>**[!UICONTROL Increase By]** - Kies wanneer u de gedefinieerde _[!UICONTROL Floor Price Source]_-waarde wilt aanpassen, zodat een hogere bodemprijs voor de regel wordt verkregen, voordat u de regel aanbiedt aan Amazon.</li><li>**[!UICONTROL Match]** - Kies wanneer u niet wilt dat de prijs van de aanbieding onder de gedefinieerde _[!UICONTROL Floor Price Source]_-waarde schommelt. Als u deze optie kiest, worden de velden_[!UICONTROL Apply]_ en _[!UICONTROL Floor Adjustment Amount]_uitgeschakeld.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Een percentageaanpassing ten opzichte van de _[!UICONTROL Floor Price Source]_-waarde. |
| [!UICONTROL Floor Adjustment Amount] | Voer de numerieke waarde voor het percentage in om de _[!UICONTROL Floor Price Source]_-waarde aan te passen. |
