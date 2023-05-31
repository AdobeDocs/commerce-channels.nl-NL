---
title: '"Intelligente prijsregel: Voorwaardelijke variaties van concurrent'
description: Bepaal de prijs van je Amazon-aanbieding op basis van de prijs van een concurrent en de conditie van het product door een intelligente prijsregel te maken.
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Intelligente prijsregel: Voorwaardelijke variaties van concurrent

Secties van een intelligente prijsstellingsregel omvatten:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Een intelligente prijsstellingsregel gebruikt de prijs van Amazon-concurrenten om je aanbiedingsprijs te bepalen. Concurrenten zijn andere verkopers die dezelfde producten aanbieden die je op Amazon aanbiedt.

Als een product met dezelfde voorwaarde bestaat, is de basisprijs gelijk aan [laagste concurrent](./lowest-competitor-pricing.md) prijs met dezelfde voorwaarde. Als geen enkel product van een concurrent aan uw voorwaarde voldoet, doorloopt de basisprijs van de prijsovereenkomst vervolgens andere beschikbare concurrentievoorwaarden, te beginnen met New, Refurbished en continue tot de beschikbare voorwaarden. Nadat een voorwaarde wordt gevonden, zal de basisprijs de laagste prijs binnen die voorwaarde zijn.

Als u een product hebt dat met de voorwaarde wordt vermeld `Used; Good` en de basisprijs van de prijsvraag, en een concurrent heeft hetzelfde product in dezelfde staat en tegen een lagere prijs, wordt de prijs van de concurrent gebruikt. Indien een concurrent niet onder dezelfde voorwaarde bestaat, controleert het systeem of een concurrent aan de volgende voorwaarde voldoet, namelijk `New`. Indien een concurrent met deze voorwaarde wordt gevonden, wordt de laagste prijs gebruikt.

## Voorwaardelijke variaties voor concurrenten configureren

Definieer de variaties van uw toestand in het dialoogvenster _[!UICONTROL Competitor Conditional Variances]_sectie.

Voor **[!UICONTROL Conditional Variance]** kiest u een optie:

- `Use all competitor's product conditions` - (Standaard) Kies wanneer je het product wilt vergelijken met een beschikbare voorwaarde (als er geen overeenkomst is voor de voorwaarde die je aanbiedt).

- `Use Only Matching Competitor's Product Condition` - Kies wanneer u uw product alleen wilt vergelijken met de producten van de concurrent in dezelfde staat. Als er geen overeenkomst is, wordt het product geprijsd op _Magento-prijsbron_ gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md).

- `Apply Variance (if competitor's product condition differs)` - Kies ervoor eerst te proberen om te vergelijken met uw overeenkomende productvoorwaarde. Als er geen overeenkomstige voorwaarde bestaat, wordt een variantie (als een percentage) toegepast ten opzichte van uw productsituatie en de toestand van de laagste concurrent.

   Wanneer de _[!UICONTROL Apply Variance]_-functie is gekozen, worden extra variatievelden weergegeven voor elk van uw Amazon-voorwaarden. Met deze functie kunt u intelligente prijsstellingsregels gebruiken wanneer u producten aanbiedt die zich in een andere situatie bevinden dan uw concurrenten. Om de berekening achter voorwaardelijke variantie te begrijpen, moet u eerst begrijpen dat alle variantie wordt bepaald van een basis gelijke prijs.

   Opties voor voorwaardelijke variatie die worden weergegeven, zijn gebaseerd op de instellingen voor je aanbieding voor `Condition` die zijn toegewezen aan voorwaardenwaarden met behulp van een [!DNL Commerce] [productkenmerk](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). Voor alle omgezette voorwaarden kunt u een variatiepercentage van 1-100 opgeven. De uitzondering is &#39;collectibles&#39;, in welk geval een percentage groter dan 100 mag worden toegepast.

![Intelligente prijsregel - voorwaardelijke variaties voor concurrenten](assets/amazon-competitor-cond-variances.png){width="500" zoomable="yes"}

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Competitor Conditional Variances] | Opties: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - Als er geen overeenkomst is voor de voorwaarde waarmee je het product aanbiedt, komt deze optie overeen met elke beschikbare voorwaarde. Het probeert eerst uw voorwaarde aan te passen en dan zijn weg van `New` voorwaarde aan `Used; Acceptable`.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - Deze optie komt overeen met de voorwaarde van uw product. Als er geen overeenkomst bestaat, worden de productprijzen op de _[!UICONTROL Magento Price Source]_.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - Met deze optie wordt eerst geprobeerd een overeenkomst te bereiken met uw productvoorwaarde. Als er geen overeenkomstige voorwaarde bestaat, wordt een variantie (als een percentage) toegepast ten opzichte van de toestand van het product en de toestand van de laagste concurrent.</li></ul><br><br>De opties voor voorwaardelijke variantie die worden weergegeven op basis van de aanbiedingsinstellingen voor Voorwaarde die aan voorwaardenwaarden zijn toegewezen met behulp van een [!DNL Commerce] [productkenmerk](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). Voor alle omgezette voorwaarden kunt u een variatiepercentage tussen 1 en 100 opgeven. De uitzondering is &#39;collectibles&#39;, in welk geval een percentage groter dan 100 mag worden toegepast.<br><br>Met deze functie kunt u intelligente prijsstellingsregels gebruiken wanneer u producten aanbiedt die zich in een andere situatie bevinden dan uw concurrenten. Om de berekening achter voorwaardelijke variantie te begrijpen, moet u eerst begrijpen dat alle variantie wordt bepaald van een basis gelijke prijs. |

## De basis voor voorwaardelijke variantie berekenen

- De Verandering van de Voorwaarde van de Overeenkomst van de Basis (BMC) = de variantie voor de voorwaarde van uw concurrent van de basisgelijke prijs. Met behulp van het eerdere voorbeeld is BMC de variatie voor de `New` voorwaarde.
- Merchant Condition Variance (MCV) = De variantie voor de conditie van uw product. Met behulp van het eerdere voorbeeld, MCV = de variantie voor het `Used; Good` voorwaarde.
- Basis Match Price (BMP) = $7,99 (hierboven toegelicht)

De formule voor de berekening van de voorwaardelijke variantiebasis is als volgt:

![formule voor berekening van de voorwaardelijke variabasis](assets/amazon-cond-variance-calc-1.png){width="300"}

## Voorbeeld

De instellingen voor voorwaardelijke variantie zijn als volgt:

![voorbeeld voorwaardelijke variatie-instellingen](assets/amazon-cond-variances.png){width="500" zoomable="yes"}

- BMC = 100 (Concurrentievoorwaarde = Nieuw)
- MCV = 80 (Merchant condition = gebruikt; Goed)
- BMP = $7,99 (basisprijs = de laagste prijs van de gematchte concurrent)

![voorbeeld van berekening van voorwaardelijke variabasis](assets/amazon-cond-variance-calc-2.png){width="300"}

Met behulp van de voorwaardelijke variabele basisberekening van bovenaf, is uw voorwaardelijke variantiebasis = $6,39. Deze berekening is de bron van de prijs van de concurrent die wordt gebruikt voor uw prijsregelingsacties, zoals nader toegelicht in [Prijsaanpassing](./price-adjustment.md).
