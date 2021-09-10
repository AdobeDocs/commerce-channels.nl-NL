---
title: '"Intelligente prijsregel: Voorwaardelijke variaties van concurrent'
description: Bepaal de prijs van je Amazon-aanbieding op basis van de prijs van een concurrent en de conditie van het product door een intelligente prijsregel te maken.
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Intelligente prijsregel: voorwaardelijke variaties van concurrent

Secties van een intelligente prijsstellingsregel omvatten:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Een intelligente prijsstellingsregel gebruikt de prijs van Amazon-concurrenten om je aanbiedingsprijs te bepalen. Concurrenten zijn andere verkopers die dezelfde producten aanbieden die je op Amazon aanbiedt.

Als een product met dezelfde voorwaarde bestaat, is de basisprijs van de overeenkomst de [laagste prijs van concurrent](./lowest-competitor-pricing.md) met dezelfde voorwaarde. Als geen enkel product van een concurrent aan uw voorwaarde voldoet, doorloopt de basisprijs van de prijsovereenkomst vervolgens andere beschikbare concurrentievoorwaarden, te beginnen met New, Refurbished en continue tot de beschikbare voorwaarden. Nadat een voorwaarde wordt gevonden, zal de basisprijs de laagste prijs binnen die voorwaarde zijn.

Als u een product met de voorwaarde `Used; Good` en de basisprijs van de gelijke hebt, en een concurrent heeft het zelfde product in de zelfde staat tegen een lagere prijs, wordt de concurrerende prijs gebruikt. Als een concurrent niet met dezelfde voorwaarde bestaat, controleert het systeem op een concurrent met de volgende voorwaarde, namelijk `New`. Indien een concurrent met deze voorwaarde wordt gevonden, wordt de laagste prijs gebruikt.

## Voorwaardelijke variaties voor concurrenten configureren

Definieer de variaties van uw voorwaarde in de sectie _[!UICONTROL Competitor Conditional Variances]_.

Kies voor **[!UICONTROL Conditional Variance]** een optie:

- `Use all competitor's product conditions` - (Standaard) Kies wanneer je het product wilt vergelijken met een beschikbare voorwaarde (als er geen overeenkomst is voor de voorwaarde die je aanbiedt).

- `Use Only Matching Competitor's Product Condition` - Kies wanneer u uw product alleen wilt vergelijken met de producten van de concurrent in dezelfde staat. Als er geen overeenkomst bestaat, wordt het product geprijsd bij de _Magento Prijsbron_ die in uw [Aanbiedingsprijs](./listing-price.md) wordt bepaald.

- `Apply Variance (if competitor's product condition differs)` - Kies ervoor eerst te proberen om te vergelijken met uw overeenkomende productvoorwaarde. Als er geen overeenkomstige voorwaarde bestaat, wordt een variantie (als een percentage) toegepast ten opzichte van uw productsituatie en de toestand van de laagste concurrent.

   Wanneer de functie _[!UICONTROL Apply Variance]_wordt gekozen, worden extra variatievelden weergegeven voor elk van uw Amazon-voorwaarden. Met deze functie kunt u intelligente prijsstellingsregels gebruiken wanneer u producten aanbiedt die zich in een andere situatie bevinden dan uw concurrenten. Om de berekening achter voorwaardelijke variantie te begrijpen, moet u eerst begrijpen dat alle variantie wordt bepaald van een basis gelijke prijs.

   De voorwaardelijke variantieopties die verschijnen zijn gebaseerd op uw lijstmontages voor `Condition` die aan voorwaardenwaarden gebruikend [!DNL Commerce] [productattribuut](https://docs.magento.com/user-guide/catalog/product-attributes.html){target= &quot;_blank&quot;} in kaart worden gebracht. Voor alle omgezette voorwaarden kunt u een variatiepercentage van 1-100 opgeven. De uitzondering is &#39;collectibles&#39;, in welk geval een percentage groter dan 100 mag worden toegepast.

![Intelligente prijsregel - voorwaardelijke variaties voor concurrenten](assets/amazon-competitor-cond-variances.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Competitor Conditional Variances] | Opties: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - Als er geen overeenkomst is voor de voorwaarde waarmee je het product aanbiedt, komt deze optie overeen met elke beschikbare voorwaarde. Het probeert eerst om uw voorwaarde aan te passen, en werkt dan zijn manier van de `New` voorwaarde aan `Used; Acceptable`.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - Deze optie komt overeen met de voorwaarde van uw product. Als er geen overeenkomst bestaat, de productprijzen op _[!UICONTROL Magento Price Source]_.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - Deze optie probeert eerst om tegen uw productvoorwaarde te passen. Als er geen overeenkomstige voorwaarde bestaat, wordt een variantie (als een percentage) toegepast ten opzichte van de toestand van het product en de toestand van de laagste concurrent.</li></ul><br><br>De opties voor voorwaardelijke variantie die worden weergegeven op basis van de aanbiedingsinstellingen voor Voorwaarde die aan voorwaardenwaarden zijn toegewezen met behulp van een  [!DNL Commerce] [productkenmerk](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}. Voor alle omgezette voorwaarden kunt u een variatiepercentage tussen 1 en 100 opgeven. De uitzondering is &#39;collectibles&#39;, in welk geval een percentage groter dan 100 mag worden toegepast.<br><br>Met deze functie kunt u intelligente prijsstellingsregels gebruiken wanneer u producten aanbiedt die zich in een andere situatie bevinden dan uw concurrenten. Om de berekening achter voorwaardelijke variantie te begrijpen, moet u eerst begrijpen dat alle variantie wordt bepaald van een basis gelijke prijs. |

## De voorwaardelijke variantiebasis berekenen

- De Verandering van de Voorwaarde van de Overeenkomst van de Basis (BMC) = de variantie voor de voorwaarde van uw concurrent van de basisgelijke prijs. Gebruikend het vroegere voorbeeld, is BMC de variantie voor `New` voorwaarde.
- Merchant Condition Variance (MCV) = De variantie voor de conditie van uw product. Met behulp van het eerdere voorbeeld, MCV = de variantie voor de voorwaarde `Used; Good`.
- Basis Match Price (BMP) = $7,99 (hierboven toegelicht)

De formule voor de berekening van de voorwaardelijke variantiebasis is als volgt:

![formule voor berekening van de voorwaardelijke variabasis](assets/amazon-cond-variance-calc-1.png)

## Voorbeeld

De instellingen voor voorwaardelijke variantie zijn als volgt:

![voorbeeld voorwaardelijke variatie-instellingen](assets/amazon-cond-variances.png)

- BMC = 100 (Concurrentievoorwaarde = Nieuw)
- MCV = 80 (Merchant condition = gebruikt; Goed)
- BMP = $7,99 (basisprijs = de laagste prijs van de gematchte concurrent)

![voorbeeld van berekening van voorwaardelijke variabasis](assets/amazon-cond-variance-calc-2.png)

Met behulp van de voorwaardelijke variabele basisberekening van bovenaf, is uw voorwaardelijke variantiebasis = $6,39. Deze berekening is de prijsbron van de concurrent die wordt gebruikt voor uw prijsregelingsacties, nader toegelicht in [Prijsaanpassing](./price-adjustment.md).
