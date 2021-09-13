---
title: Voorwaarden voor prijsregels
description: Gebruik de prijsregelvoorwaarden om te bepalen welke producten in aanmerking komen voor de prijsregel voor aanbiedingen.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: ac190d88711f07c0b255a8cb50b12b62945f625e
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Prijsregelvoorwaarden

De voorwaarden bepalen welke producten in aanmerking komen voor de prijsregel. Als u de voorwaarden voor uw Amazon-prijsregels definieert, volgt u dezelfde logica en hetzelfde proces als het definiëren van de voorwaarden voor [Cart Price Rules](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){:target=&quot;_blank&quot;} in [!DNL Commerce].

>[!IMPORTANT]
>
>Als uw prijsregel op alle producten in uw [!DNL Commerce] catalogus van toepassing is, dan verlaat deze sectie leeg.

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

## Voorbeeld: een prijsregelvoorwaarde maken

Dit proces kan eenvoudig of gedetailleerd zijn, afhankelijk van uw catalogusconfiguratie. U kunt uw voorwaarden zodanig definiëren dat wanneer `ALL` of `ANY` van de voorwaarden of `TRUE` of `FALSE` voor een product zijn, het product in aanmerking komt voor de toe te passen prijsregel.

De voorwaarden zijn gebaseerd op uw [productkenmerken](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;}. Laat de sectie voor voorwaarden leeg als u de regel op alle producten wilt toepassen.

>[!NOTE]
>
>Als u een voorwaarde wilt bepalen die op een specifiek productattribuut wordt gebaseerd, **Gebruik voor de Voorwaarden van de Regel van de Promo** voor het attribuut moet aan `Yes` in uw [Eigenschappen Storefront ](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target= &quot;_blank&quot;} voor het attribuut worden geplaatst.

![Prijsregelvoorwaarde - regel 1](assets/ob-price-rules-condition-1.png)

In dit voorbeeld wordt een regel gedefinieerd die een korting van 25% toepast op alle producten die in de categorie `Books` zijn gedefinieerd.

De regelinstructie heeft twee vette koppelingen, die, wanneer erop wordt geklikt, de opties voor dat gedeelte van de voorwaardelement weergeven. Als u de voorwaarde opslaat zonder een vette optie te wijzigen, geldt de regel voor al uw producten.

- Klik **[!UICONTROL ALL]** en kies of `ALL` of `ANY`.
- Klik **[!UICONTROL TRUE]**, en kies of `TRUE` of `FALSE`.
- Als u de regel op alle producten wilt toepassen, laat u de voorwaarde ongewijzigd.

U kunt verschillende voorwaarden maken door de combinatie van deze waarden te wijzigen. In dit voorbeeld wordt de volgende voorwaarde gebruikt:

`If ALL of these conditions are TRUE:`

1. Als u beschikbare kenmerken wilt weergeven waarvoor de voorwaarde geldt, klikt u op het pictogram Toevoegen (![Pictogram toevoegen](assets/btn-add-grn.png)) aan het begin van de voorwaardelijn en selecteert u een kenmerk waarop u de voorwaarde wilt baseren.

   **[!UICONTROL Conditions Combination]** - Kies of u een andere set voorwaarden  `All/Any` en  `True/False` voorwaarden binnen de bestaande voorwaarde wilt maken.

   ![Combinatie van prijsregelvoorwaarden](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]** - De beschikbare productkenmerken zijn afhankelijk van de  [instelling van het kenmerk](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}. Een kenmerk wordt alleen in de lijst weergegeven als *[!UICONTROL Use for Promo Rule Conditions]* voor het kenmerk is ingesteld op `Yes` in de [storefront-eigenschappen](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}.

   - Kies voor **[!UICONTROL Product Attribute]** het kenmerk dat u als basis van de voorwaarde wilt definiëren. In dit voorbeeld is de geselecteerde voorwaarde `Category`.

      ![Prijsregelvoorwaarde - regel 2, deel 2](assets/ob-price-rule-condition-2.png)

      De geselecteerde voorwaarde wordt weergegeven in de instructie, gevolgd door nog twee vette koppelingen. Welke opties beschikbaar zijn, is afhankelijk van het productkenmerk dat u selecteert.

      Nadat u het kenmerk hebt ingesteld, kunt u het niet meer bewerken. Als u het kenmerk wilt wijzigen, moet u de regel verwijderen en het nieuwe kenmerk toevoegen. U kunt een voorwaardelijn schrappen door de Schrapping (![pictogram van de Schrapping](assets/btn-del-red.png) aan het eind van de lijn te klikken.

   - Klik op **[!UICONTROL is]** en kies de vergelijkingsoperator die de voorwaarde beschrijft waaraan producten moeten voldoen.

      In dit voorbeeld is de vergelijkingsoperator `is`. De beschikbare opties zijn afhankelijk van het kenmerk dat u in de vorige stap hebt geselecteerd en kunnen verschillende vergelijkingsopties bevatten. Opties kunnen overeenkomende waarden bevatten, met uitzondering van of met inbegrip van ten minste een van een waarde, en groter dan, gelijk aan en kleiner dan een numeriek bedrag. In dit voorbeeld zijn de opties `is` en `is not`.

   - Klik **[!UICONTROL ...]** en kies de kenmerkwaarde waarop de voorwaarde is gebaseerd. Welke opties beschikbaar zijn, is afhankelijk van de instelling van het kenmerk.

      Mogelijk wordt u gevraagd een optie te selecteren of een waarde voor de voorwaarde in te voeren. In dit voorbeeld wordt het veld leeg weergegeven. Als u uw categorie(ën) voor de regel wilt selecteren, klikt u op het pictogram Kiezer (![Kiezerpictogram](assets/btn-chooser.png)) om uw selectieopties weer te geven. Deze regel geldt voor _Boeken_, selecteer **[!UICONTROL Books]** checkbox. Het categorienummer wordt gevuld. Als u de rubriekselecties wilt accepteren, klikt u op het groene vinkje (![Pictogram vinkje](assets/btn-check-mark-green.png)).

      ![Prijsregelvoorwaarde - regel 2, deel 3](assets/ob-price-rule-condition-3.png)

      Het geselecteerde item wordt weergegeven in de instructie om de voorwaarde te voltooien.

      ![Prijsregelvoorwaarde - regel 2, deel 4](assets/ob-price-rule-condition-4.png)

      Deze voorbeeldvoorwaarde is voltooid. Zoals vermeld, betekent deze voorwaarde dat om het even welk product in uw [!DNL Commerce] catalogus die een bepaalde categorie Boeken (`4`) heeft voor deze het tarief regel in aanmerking komt. U kunt meer voorwaardenlijnen toevoegen om uw in aanmerking komende producten verder te verfijnen.

1. Als u nog een voorwaardelijn aan de instructie wilt toevoegen, gaat u terug naar Stap 1 en herhaalt u het proces totdat alle gewenste voorwaarden zijn voltooid.

   U kunt een lijn van de voorwaardenverklaring op elk ogenblik schrappen door de Schrapping (![pictogram van de Schrapping](assets/btn-del-red.png)) aan het eind van de lijn te klikken.
