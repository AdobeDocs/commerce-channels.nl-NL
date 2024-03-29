---
title: Verkoopkanaal in Amazon - Prijsregelvoorwaarden
description: Gebruik de prijsregelvoorwaarden om te bepalen welke producten in aanmerking komen voor de prijsregel voor aanbiedingen.
feature: Sales Channels, Price Rules
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Prijsregelvoorwaarden

De voorwaarden bepalen welke producten in aanmerking komen voor de prijsregel. Als u de voorwaarden voor uw prijsregels voor Amazon definieert, volgt u dezelfde logica en hetzelfde proces als het definiëren van de voorwaarden voor [Lijnen met winkelprijzen](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) in [!DNL Commerce].

>[!IMPORTANT]
>
>Als uw prijsregel van toepassing is op alle producten in uw [!DNL Commerce] en laat deze sectie leeg.

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

## Voorbeeld: een prijsregelvoorwaarde maken

Dit proces kan eenvoudig of gedetailleerd zijn, afhankelijk van uw catalogusconfiguratie. U kunt uw voorwaarden zodanig definiëren dat wanneer `ALL` of `ANY` van de voorwaarden: `TRUE` of `FALSE` voor een product komt het product in aanmerking voor toepassing van de prijsregel.

Voorwaarden zijn gebaseerd op uw [productkenmerken](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). Als u de regel op alle producten wilt toepassen, laat u de sectie Voorwaarden leeg.

>[!NOTE]
>
>Als u een voorwaarde wilt bepalen die op een specifiek productattribuut wordt gebaseerd, **Voorwaarden voor promotieregels gebruiken** for the attribute must be set to `Yes` in uw [Eigenschappen van Storefront](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html) voor het kenmerk.

![Prijsregelvoorwaarde - regel 1](assets/ob-price-rules-condition-1.png){width="600" zoomable="yes"}

In dit voorbeeld wordt een regel gedefinieerd die een korting van 25% toepast op alle producten die in het dialoogvenster `Books` categorie.

De regelinstructie heeft twee vette koppelingen, die, wanneer erop wordt geklikt, de opties voor dat gedeelte van de voorwaardelement weergeven. Als u de voorwaarde opslaat zonder een vette optie te wijzigen, geldt de regel voor al uw producten.

- Klikken **[!UICONTROL ALL]** en kiest u `ALL` of `ANY`.
- Klikken **[!UICONTROL TRUE]** en kiest u `TRUE` of `FALSE`.
- Als u de regel op alle producten wilt toepassen, laat u de voorwaarde ongewijzigd.

U kunt verschillende voorwaarden maken door de combinatie van deze waarden te wijzigen. In dit voorbeeld wordt de volgende voorwaarde gebruikt:

`If ALL of these conditions are TRUE:`

1. Klik op Toevoegen (![Pictogram toevoegen](assets/btn-add-grn.png)) aan het begin van de voorwaardelijn en selecteer een kenmerk waarop u de voorwaarde wilt baseren.

   **[!UICONTROL Conditions Combination]** - Maak een andere set `All/Any` en `True/False` in de bestaande voorwaarde.

   ![Combinatie van prijsregelvoorwaarden](assets/ob-conditions-combinations.png){width="500"}

   **[!UICONTROL Product Attribute]** - De beschikbare productkenmerken zijn afhankelijk van de [opstelling van het attribuut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html). Voor een kenmerk dat in de lijst moet worden weergegeven, *[!UICONTROL Use for Promo Rule Conditions]* for the attribute must be set to `Yes` in uw winkeleigenschappen.

   - Voor **[!UICONTROL Product Attribute]** kiest u het kenmerk dat u wilt definiëren als basis voor de voorwaarde. In dit voorbeeld is de geselecteerde voorwaarde: `Category`.

     ![Prijsregelvoorwaarde - regel 2, deel 2](assets/ob-price-rule-condition-2.png){width="500"}

     De geselecteerde voorwaarde wordt weergegeven in de instructie, gevolgd door nog twee vette koppelingen. Welke opties beschikbaar zijn, is afhankelijk van het productkenmerk dat u selecteert.

     Nadat u het kenmerk hebt ingesteld, kunt u het niet meer bewerken. Als u het kenmerk wilt wijzigen, moet u de regel verwijderen en het nieuwe kenmerk toevoegen. U kunt een voorwaardenlijn schrappen door Schrapping te klikken (![Pictogram Verwijderen](assets/btn-del-red.png) aan het einde van de regel.

   - Klikken **[!UICONTROL is]** en kiest u de vergelijkingsoperator die de voorwaarde beschrijft waaraan producten moeten voldoen.

     In dit voorbeeld is de vergelijkingsoperator `is`. De beschikbare opties zijn afhankelijk van het kenmerk dat u in de vorige stap hebt geselecteerd en kunnen verschillende vergelijkingsopties bevatten. Opties kunnen overeenkomende waarden bevatten, met uitzondering van of met inbegrip van ten minste een van een waarde, en groter dan, gelijk aan en kleiner dan een numeriek bedrag. In dit voorbeeld zijn de opties: `is` en `is not`.

   - Klikken **[!UICONTROL ...]** en kiest u de kenmerkwaarde waarop de voorwaarde is gebaseerd. Welke opties beschikbaar zijn, is afhankelijk van de instelling van het kenmerk.

     Mogelijk wordt u gevraagd een optie te selecteren of een waarde voor de voorwaarde in te voeren. In dit voorbeeld wordt het veld leeg weergegeven. Als u de categorie(ën) voor de regel wilt selecteren, klikt u op het pictogram van de kiezer (![Pictogram Kiezer](assets/btn-chooser.png)) om de selectieopties weer te geven. Deze regel geldt voor _Boeken_, selecteert u de **[!UICONTROL Books]** selectievakje. Het categorienummer wordt gevuld. Als je rubriekselecties wilt accepteren, klik je op het groene vinkje (![Pictogram vinkje](assets/btn-check-mark-green.png)).

     ![Prijsregelvoorwaarde - regel 2, deel 3](assets/ob-price-rule-condition-3.png){width="500"}

     Het geselecteerde item wordt weergegeven in de instructie om de voorwaarde te voltooien.

     ![Prijsregelvoorwaarde - regel 2, deel 4](assets/ob-price-rule-condition-4.png){width="500"}

     Deze voorbeeldvoorwaarde is voltooid. Zoals gezegd betekent deze voorwaarde dat elk product in uw [!DNL Commerce] catalogus met een gedefinieerde categorie Boeken (`4`) komt in aanmerking voor deze prijsregel. U kunt meer voorwaardenlijnen toevoegen om uw in aanmerking komende producten verder te beperken.

1. Als u nog een voorwaardelijn aan de instructie wilt toevoegen, gaat u terug naar Stap 1 en herhaalt u het proces totdat alle gewenste voorwaarden zijn voltooid.

   U kunt op elk gewenst moment een regel van de instructie condition verwijderen door op Verwijderen te klikken (![Pictogram Verwijderen](assets/btn-del-red.png)) aan het einde van de regel.
