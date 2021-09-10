---
title: Handelingen voor standaardprijsregels
description: Gebruik de standaardhandelingen voor prijsregels om een Amazon-aanbiedingsprijs te verhogen of te verlagen ten opzichte van de catalogusprijs (of de prijsbron) van de Handel.
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Standaardprijzenregel

Met een standaardhandeling voor prijsregels kunt u een Amazon-aanbiedingsprijs verhogen of verlagen met een bepaald percentage of een bepaald dollarbedrag ten opzichte van de catalogusprijs (of prijsbron) van [!DNL Commerce].

De volgende onderdelen van een standaardprijsregel zijn:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Prijsregelacties configureren

1. Kies **[!UICONTROL Rule Type]** bij `Standard price rule`.

   Met deze optie worden de overige velden in de sectie _[!UICONTROL Select Rule Type]_uitgeschakeld.

1. Vouw indien nodig de sectie _[!UICONTROL Price Adjustment]_uit.

1. Kies voor **[!UICONTROL Price Action]** een optie om te bepalen hoe u de waarde *[!UICONTROL Magento Price Source]* (gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md)) wilt wijzigen.

   - `Decrease By` - Kies wanneer je de waarde wilt verlagen voordat je een aanbieding naar Amazon maakt.

   - `Increase By` - Kies wanneer je de waarde wilt verhogen voordat je een aanbieding naar Amazon maakt.

1. Kies voor **[!UICONTROL Apply]** een optie om te bepalen hoe u de gedefinieerde *[!UICONTROL Magento Price Source]*-waarde in de [Aanbiedingsprijs](./listing-price.md) wilt aanpassen:

   - `Apply as percentage` - Kies wanneer je de gedefinieerde  *[!UICONTROL Magento Price Source]* waarde in je  [ ](./listing-price.md) aanbiedingsprijs wilt aanpassen met een percentage

   - `Apply as fixed amount` - Kies wanneer je de gedefinieerde waarde in je  *[!UICONTROL Magento Price Source]* aanbiedingsprijs  [ ](./listing-price.md) wilt aanpassen met een vaste hoeveelheid.

1. Voer bij **[!UICONTROL Adjustment Amount]** (verplicht) de numerieke waarde voor de prijsaanpassing in.

   - Wanneer *[!UICONTROL Apply]* aan `Apply as percentage` wordt geplaatst, ga de percentagewaarde (voorbeeld: Voer `25` in voor een prijsaanpassing van 25%).

   - Wanneer *[!UICONTROL Apply]* wordt geplaatst aan `Apply as fixed amount`, ga de numerieke waarde voor het vaste bedrag in (voorbeeld: Voer `25` in voor een vaste prijsaanpassing van $ 25).

1. Klik op **[!UICONTROL Save pricing rule]** als u klaar bent.

![Standaardprijsregel](assets/ob-price-rule-action-standard-example.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Rule Type] | Selecteer `Standard price rule`. |
| [!UICONTROL Price Action] | Opties:<ul><li>**[!UICONTROL Decrease By]** - Kies wanneer je de waarde van de gedefinieerde  [!DNL Commerce] prijsbron wilt laten dalen voordat je de aanbieding naar Amazon uitvoert.</li><li>**[!UICONTROL Increase By]** - Kies wanneer je de waarde van de gedefinieerde  [!DNL Commerce] prijsbron wilt verhogen voordat je de aanbieding naar Amazon uitvoert.</li></ul> |
| [!UICONTROL Apply] | Opties:<ul><li>**[!UICONTROL Apply as percentage]** - Kies wanneer u de waarde van de gedefinieerde  [!DNL Commerce] prijsbron wilt aanpassen met een percentage.</li><li>**[!UICONTROL Apply as fixed amount]** - Kies wanneer u de waarde van de gedefinieerde  [!DNL Commerce] prijsbron wilt aanpassen met een vast bedrag.</li></ul> |
| [!UICONTROL Adjustment Amount] | Vereist.<br><br>Als u  `Apply as percentage` voor  *[!UICONTROL Apply]* kiest, ga de percentagewaarde (voorbeeld: Voer een aanpassing  `25` van 25% in).<br><br>Als u  `Apply as fixed amount` voor  *[!UICONTROL Apply]* kiest, voert u de numerieke waarde voor het vaste bedrag in (bijvoorbeeld: Voer  `25` een vaste correctie van € 25 in). |
