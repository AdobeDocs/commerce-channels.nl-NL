---
title: "Intelligent Repricing Rule: concurrent Conditional Variances"
description: Bepaal de prijs van je Amazon-aanbieding op basis van de prijs van een concurrent en de conditie van het product door een intelligente prijsregel te maken.
feature: Sales Channels, Configuration
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Intelligente prijsregel: Voorwaardelijke variaties van concurrenten

Secties van een intelligente prijsstellingsregel omvatten:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Een intelligente prijsstellingsregel gebruikt de prijs van Amazon-concurrenten om je aanbiedingsprijs te bepalen. Concurrenten zijn andere verkopers die dezelfde producten aanbieden die je op Amazon aanbiedt.

Als een product met de zelfde voorwaarde bestaat, is de prijs van de basisgelijke de [ laagste concurrent ](./lowest-competitor-pricing.md) prijs met de zelfde voorwaarde. Als geen enkel product van een concurrent aan uw voorwaarde voldoet, doorloopt de basisprijs van de prijsovereenkomst vervolgens andere beschikbare concurrentievoorwaarden, te beginnen met New, Refurbished en continue tot de beschikbare voorwaarden. Nadat een voorwaarde wordt gevonden, zal de basisprijs de laagste prijs binnen die voorwaarde zijn.

Als u een product met de voorwaarde `Used; Good` en de basisprijs van de gelijke hebt, en een concurrent heeft het zelfde product in de zelfde staat tegen een lagere prijs, wordt de concurrerende prijs gebruikt. Als een concurrent niet met dezelfde voorwaarde bestaat, controleert het systeem op een concurrent met de volgende voorwaarde, namelijk `New`. Indien een concurrent met deze voorwaarde wordt gevonden, wordt de laagste prijs gebruikt.

## Voorwaardelijke variaties voor concurrenten configureren

Definieer de voorwaardelijke variaties in de sectie _[!UICONTROL Competitor Conditional Variances]_.

Kies bij **[!UICONTROL Conditional Variance]** een optie:

- `Use all competitor's product conditions` - (Standaard) Kies wanneer u het product wilt vergelijken met een beschikbare voorwaarde (als er geen overeenkomst bestaat voor de voorwaarde die u aanbiedt).

- `Use Only Matching Competitor's Product Condition` - Kies wanneer u uw product alleen wilt vergelijken met de producten van de concurrent in dezelfde staat. Als geen gelijke bestaat, wordt het product geprijst bij de _Source van de Prijs van het Magento_ die in uw [ wordt bepaald die Prijs van de Lijst ](./listing-price.md).

- `Apply Variance (if competitor's product condition differs)` - Kies om eerst te proberen te vergelijken met uw overeenkomende productvoorwaarde. Als er geen overeenkomstige voorwaarde bestaat, wordt een variantie (als een percentage) toegepast ten opzichte van uw productsituatie en de toestand van de laagste concurrent.

  Wanneer u de functie _[!UICONTROL Apply Variance]_kiest, worden extra variatievelden weergegeven voor elk van uw Amazon-voorwaarden. Met deze functie kunt u intelligente prijsstellingsregels gebruiken wanneer u producten aanbiedt die zich in een andere situatie bevinden dan uw concurrenten. Om de berekening achter voorwaardelijke variantie te begrijpen, moet u eerst begrijpen dat alle variantie wordt bepaald van een basis gelijke prijs.

  De voorwaardelijke variantieopties die verschijnen zijn gebaseerd op uw lijstmontages voor `Condition` die aan voorwaardenwaarden gebruikend a [!DNL Commerce] [ productattribuut ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) in kaart worden gebracht. Voor alle omgezette voorwaarden kunt u een variatiepercentage van 1-100 opgeven. De uitzondering is &#39;collectibles&#39;, in welk geval een percentage groter dan 100 mag worden toegepast.

![ Intelligente repricing regel - de concurrent voorwaardelijke varianties ](assets/amazon-competitor-cond-variances.png){width="500" zoomable="yes"}

| Veld | Beschrijving |
|-----------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Competitor Conditional Variances] | Opties: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - Als er geen overeenkomst bestaat voor de voorwaarde waarmee je het product aanbiedt, komt deze optie overeen met elke beschikbare voorwaarde. De code probeert eerst aan uw voorwaarde te voldoen en werkt vervolgens van de voorwaarde `New` naar `Used; Acceptable` .</li><li>**[!UICONTROL Use only matching competitor's product condition]** - Deze optie komt overeen met de voorwaarde van uw product. Als er geen overeenkomst is, worden de productprijzen op de _[!UICONTROL Magento Price Source]_weergegeven.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - Deze optie probeert eerst met uw productvoorwaarde te in overeenstemming te brengen. Als er geen overeenkomstige voorwaarde bestaat, wordt een variantie (als een percentage) toegepast ten opzichte van de toestand van het product en de toestand van de laagste concurrent.</li></ul><br><br> de voorwaardelijke variatieopties die verschijnen gebaseerd op uw lijstmontages voor Voorwaarde die aan voorwaardenwaarden gebruikend a [!DNL Commerce] [ productattributen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) in kaart worden gebracht. Voor alle omgezette voorwaarden kunt u een variatiepercentage tussen 1 en 100 opgeven. De uitzondering is &#39;collectibles&#39;, in welk geval een percentage groter dan 100 mag worden toegepast.<br><br> Deze eigenschap staat u toe om intelligente het verprijzen regels te gebruiken wanneer u producten aanbiedt die in een verschillende voorwaarde dan uw concurrenten zijn. Om de berekening achter voorwaardelijke variantie te begrijpen, moet u eerst begrijpen dat alle variantie wordt bepaald van een basis gelijke prijs. |

## De basis voor voorwaardelijke variantie berekenen

- De Verandering van de Voorwaarde van de Overeenkomst van de Basis (BMC) = de variantie voor de voorwaarde van uw concurrent van de basisgelijke prijs. In het vorige voorbeeld is BMC de variantie voor de voorwaarde `New` .
- Merchant Condition Variance (MCV) = De variantie voor de conditie van uw product. In het eerdere voorbeeld is MCV = de variantie voor de voorwaarde `Used; Good` .
- Basis Match Price (BMP) = $7,99 (hierboven toegelicht)

De formule voor de berekening van de voorwaardelijke variantiebasis is als volgt:

{de formule van de 0} voorwaardelijke berekening van de variaberekening ](assets/amazon-cond-variance-calc-1.png){width="300"}![

## Voorbeeld

De instellingen voor voorwaardelijke variantie zijn als volgt:

![ de montages van de voorbeeldvoorwaardelijke variantie ](assets/amazon-cond-variances.png){width="500" zoomable="yes"}

- BMC = 100 (Concurrentievoorwaarde = Nieuw)
- MCV = 80 (Merchant condition = Used; Good)
- BMP = $7,99 (basisprijs = de laagste prijs van de gematchte concurrent)

![ voorwaardelijk de berekeningsvoorbeeld van de variaberekening van de variatiebasis ](assets/amazon-cond-variance-calc-2.png){width="300"}

Met behulp van de voorwaardelijke variabele basisberekening van bovenaf, is uw voorwaardelijke variantiebasis = $6,39. Deze berekening is de bron van de concurrerende prijs die voor uw acties van de prijsregel wordt gebruikt, die verder in [ de Aanpassing van de Prijs ](./price-adjustment.md) wordt verklaard.
