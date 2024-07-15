---
title: Verkoopkanaal in Amazon - Handelingen met standaardprijsregels
description: Gebruik de standaardhandelingen voor prijsregels om een Amazon-aanbiedingsprijs te verhogen of te verlagen ten opzichte van de catalogusprijs van de Commerce (of de prijsbron).
feature: Sales Channels, Price Rules
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Standaardprijzenregel

Met een standaardhandeling voor prijsregels kunt u een Amazon-aanbiedingsprijs verhogen of verlagen met een bepaald percentage of een bepaald bedrag in dollar ten opzichte van de catalogusprijs (of prijsbron) van [!DNL Commerce] .

De volgende onderdelen van een standaardprijsregel zijn:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Prijsregelacties configureren

1. Kies `Standard price rule` bij **[!UICONTROL Rule Type]** .

   Met deze optie worden de andere velden in de sectie _[!UICONTROL Select Rule Type]_uitgeschakeld.

1. Vouw indien nodig de sectie _[!UICONTROL Price Adjustment]_uit.

1. Voor **[!UICONTROL Price Action]**, kies een optie om te bepalen hoe u de *[!UICONTROL Magento Price Source]* (die in uw [ wordt bepaald Prijs van de Lijst ](./listing-price.md)) waarde wilt veranderen.

   - `Decrease By` - Kies wanneer je de waarde wilt verlagen voordat je een aanbieding naar Amazon maakt.

   - `Increase By` - Kies wanneer u de waarde wilt verhogen voordat u een aanbieding naar Amazon maakt.

1. Voor **[!UICONTROL Apply]**, kies een optie om te bepalen hoe u de bepaalde *[!UICONTROL Magento Price Source]* bepaald in uw [ ](./listing-price.md) waarde van de Lijstprijs wilt worden aangepast:

   - `Apply as percentage` - kies wanneer u de bepaalde *[!UICONTROL Magento Price Source]* die in uw [ wordt bepaald Prijs ](./listing-price.md) waarde van de Lijst door een percentage wordt aangepast

   - `Apply as fixed amount` - kies wanneer u de bepaalde *[!UICONTROL Magento Price Source]* die in uw [ wordt bepaald Prijs ](./listing-price.md) waarde van de Lijst door een vast bedrag wordt aangepast.

1. Voer bij **[!UICONTROL Adjustment Amount]** (vereist) de numerieke waarde voor de prijsaanpassing in.

   - Wanneer *[!UICONTROL Apply]* is ingesteld op `Apply as percentage` , voert u de percentagewaarde in (bijvoorbeeld: voer `25` in voor een prijsaanpassing van 25%).

   - Wanneer *[!UICONTROL Apply]* is ingesteld op `Apply as fixed amount` , voert u de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: voer `25` in voor een vaste prijsaanpassing van € 25).

1. Klik op **[!UICONTROL Save pricing rule]** als de bewerking is voltooid.

![ Standaard prijsregel ](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | Selecteer `Standard price rule` . |
| [!UICONTROL Price Action] | Opties:<ul><li>**[!UICONTROL Decrease By]** - Kies wanneer u de gedefinieerde waarde voor de prijsbron van [!DNL Commerce] wilt laten dalen voordat u de aanbieding naar Amazon uitvoert.</li><li>**[!UICONTROL Increase By]** - Kies wanneer u de gedefinieerde waarde voor de prijsbron van [!DNL Commerce] wilt verhogen voordat u de aanbieding naar Amazon uitvoert.</li></ul> |
| [!UICONTROL Apply] | Opties:<ul><li>**[!UICONTROL Apply as percentage]** - Kies wanneer u de gedefinieerde waarde voor de [!DNL Commerce] prijsbron wilt aanpassen met een percentage.</li><li>**[!UICONTROL Apply as fixed amount]** - Kies wanneer u de gedefinieerde waarde voor de [!DNL Commerce] -prijsbron wilt aanpassen met een vaste hoeveelheid.</li></ul> |
| [!UICONTROL Adjustment Amount] | Vereist.<br><br> Als u `Apply as percentage` for *[!UICONTROL Apply]* kiest, voert u de percentagewaarde in (bijvoorbeeld: voer `25` in voor een aanpassing van 25%).<br><br> Als u `Apply as fixed amount` for *[!UICONTROL Apply]* kiest, voert u de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: voer `25` in voor een vaste aanpassing van € 25). |
