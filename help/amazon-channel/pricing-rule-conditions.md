---
title: Price Rule Conditions
description: Use the price rule conditions to determine which products are eligible for the listing price rule.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Prijsregelvoorwaarden

Conditions determine which products are eligible for the price rule. Als u de voorwaarden voor uw prijsregels voor Amazon definieert, volgt u dezelfde logica en hetzelfde proces als het definiëren van de voorwaarden voor [Lijnen met winkelprijzen](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;} in [!DNL Commerce].

>[!IMPORTANT]
>
>Als uw prijsregel van toepassing is op alle producten in uw [!DNL Commerce] en laat deze sectie leeg.

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

## Voorbeeld: een prijsregelvoorwaarde maken

Dit proces kan eenvoudig of gedetailleerd zijn, afhankelijk van uw catalogusconfiguratie. U kunt uw voorwaarden zodanig definiëren dat wanneer `ALL` of `ANY` van de voorwaarden: `TRUE` of `FALSE` voor een product komt het product in aanmerking voor toepassing van de prijsregel.

Voorwaarden zijn gebaseerd op uw [productkenmerken](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}. Laat de sectie voor voorwaarden leeg als u de regel op alle producten wilt toepassen.

>[!NOTE]
>
>Als u een voorwaarde wilt bepalen die op een specifiek productattribuut wordt gebaseerd, **Voorwaarden voor promotieregels gebruiken** for the attribute must be set to `Yes` in uw [Eigenschappen van Storefront](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;} voor het kenmerk.

![Prijsregelvoorwaarde - regel 1](assets/ob-price-rules-condition-1.png)

In dit voorbeeld wordt een regel gedefinieerd die een korting van 25% toepast op alle producten die in het dialoogvenster `Books` categorie.

De regelinstructie heeft twee vette koppelingen, die, wanneer erop wordt geklikt, de opties voor dat gedeelte van de voorwaardelement weergeven. Als u de voorwaarde opslaat zonder een vette optie te wijzigen, geldt de regel voor al uw producten.

- Klikken **[!UICONTROL ALL]** en kiest u `ALL` of `ANY`.
- Klikken **[!UICONTROL TRUE]** en kiest u een van `TRUE` of `FALSE`.
- Als u de regel op alle producten wilt toepassen, laat u de voorwaarde ongewijzigd.

U kunt verschillende voorwaarden maken door de combinatie van deze waarden te wijzigen. For this example, the following condition is used:

`If ALL of these conditions are TRUE:`

1. To show available attributes for which the condition applies, click the Add (![Add icon](assets/btn-add-grn.png)) icon at the beginning of the condition line and select an attribute on which to base the condition.

   **[!UICONTROL Conditions Combination]** -  Choose to create another set of `All/Any` and `True/False` conditions inside the existing condition.

   ![Combinatie van prijsregelvoorwaarden](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]** - The available product attributes depend on the [setup of the attribute](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}. Voor een kenmerk dat in de lijst moet worden weergegeven, *[!UICONTROL Use for Promo Rule Conditions]* for the attribute must be set to `Yes` in uw [storefront, eigenschappen](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}.

   - Voor **[!UICONTROL Product Attribute]** kiest u het kenmerk dat u wilt definiëren als basis voor de voorwaarde. For this example, the selected condition is `Category`.

      ![Prijsregelvoorwaarde - regel 2, deel 2](assets/ob-price-rule-condition-2.png)

      De geselecteerde voorwaarde wordt weergegeven in de instructie, gevolgd door nog twee vette koppelingen. Welke opties beschikbaar zijn, is afhankelijk van het productkenmerk dat u selecteert.

      Nadat u het kenmerk hebt ingesteld, kunt u het niet meer bewerken. Als u het kenmerk wilt wijzigen, moet u de regel verwijderen en het nieuwe kenmerk toevoegen. U kunt een voorwaardenlijn schrappen door Schrapping te klikken (![Pictogram Verwijderen](assets/btn-del-red.png) aan het einde van de regel.

   - Klikken **[!UICONTROL is]** en kiest u de vergelijkingsoperator die de voorwaarde beschrijft waaraan producten moeten voldoen.

      In dit voorbeeld is de vergelijkingsoperator `is`. De beschikbare opties zijn afhankelijk van het kenmerk dat u in de vorige stap hebt geselecteerd en kunnen verschillende vergelijkingsopties bevatten. Opties kunnen overeenkomende waarden bevatten, met uitzondering van of met inbegrip van ten minste een van een waarde, en groter dan, gelijk aan en kleiner dan een numeriek bedrag. In dit voorbeeld zijn de volgende opties beschikbaar: `is` en `is not`.

   - Klikken **[!UICONTROL ...]** en kiest u de kenmerkwaarde waarop de voorwaarde is gebaseerd. Welke opties beschikbaar zijn, is afhankelijk van de instelling van het kenmerk.

      Mogelijk wordt u gevraagd een optie te selecteren of een waarde voor de voorwaarde in te voeren. In dit voorbeeld wordt het veld leeg weergegeven. Als u de categorie(ën) voor de regel wilt selecteren, klikt u op het pictogram van de kiezer (![Pictogram Kiezer](assets/btn-chooser.png)) om de selectieopties weer te geven. Deze regel geldt voor _Boeken_, selecteert u de **[!UICONTROL Books]** selectievakje. Het categorienummer wordt gevuld. Als je rubriekselecties wilt accepteren, klik je op het groene vinkje (![Pictogram vinkje](assets/btn-check-mark-green.png)).

      ![Prijsregelvoorwaarde - regel 2, deel 3](assets/ob-price-rule-condition-3.png)

      Het geselecteerde item wordt weergegeven in de instructie om de voorwaarde te voltooien.

      ![Prijsregelvoorwaarde - regel 2, deel 4](assets/ob-price-rule-condition-4.png)

      Deze voorbeeldvoorwaarde is voltooid. As stated, this condition means that any product in your [!DNL Commerce] catalog that has a defined category of Books (`4`) is eligible for this pricing rule. U kunt meer voorwaardenlijnen toevoegen om uw in aanmerking komende producten verder te verfijnen.

1. To add another condition line to the statement, return to Step 1 and repeat the process until all desired conditions are complete.

   U kunt op elk gewenst moment een regel van de instructie condition verwijderen door op Verwijderen te klikken (![Pictogram Verwijderen](assets/btn-del-red.png)) aan het einde van de regel.
