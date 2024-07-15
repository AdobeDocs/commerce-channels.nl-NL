---
title: Verkoopkanaal in Amazon - Prijsregelvoorwaarden
description: Gebruik de prijsregelvoorwaarden om te bepalen welke producten in aanmerking komen voor de prijsregel voor aanbiedingen.
feature: Sales Channels, Price Rules
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Prijsregelvoorwaarden

De voorwaarden bepalen welke producten in aanmerking komen voor de prijsregel. Het bepalen van de voorwaarden voor uw Amazon die prijsregels volgen de zelfde logica en het proces zoals het bepalen van de voorwaarden voor [ Regels van de Prijs van de Kar ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) in [!DNL Commerce].

>[!IMPORTANT]
>
>Als de prijsregel van toepassing is op alle producten in de catalogus van [!DNL Commerce] , laat u deze sectie leeg.

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

## Voorbeeld: een prijsregelvoorwaarde maken

Dit proces kan eenvoudig of gedetailleerd zijn, afhankelijk van uw catalogusconfiguratie. U kunt uw voorwaarden zodanig definiëren dat wanneer `ALL` of `ANY` van de voorwaarden `TRUE` of `FALSE` voor een product zijn, het product in aanmerking komt voor de prijsregel die moet worden toegepast.

De voorwaarden zijn gebaseerd op uw [ productattributen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). Als u de regel op alle producten wilt toepassen, laat u de sectie Voorwaarden leeg.

>[!NOTE]
>
>Als u een voorwaarde wilt bepalen die op een specifiek productattribuut wordt gebaseerd, **Gebruik voor de Voorwaarden van de Regel van de Bevordering** voor de attributen moet aan `Yes` in uw [ Eigenschappen van de Storefront ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html) voor de attributen worden geplaatst.

![ de regelvoorwaarde van de Prijs - lijn 1 ](assets/ob-price-rules-condition-1.png){width="600" zoomable="yes"}

In dit voorbeeld wordt een regel gedefinieerd die een korting van 25% toepast op alle producten die in de categorie `Books` zijn gedefinieerd.

De regelinstructie heeft twee vette koppelingen, die, wanneer erop wordt geklikt, de opties voor dat gedeelte van de voorwaardelement weergeven. Als u de voorwaarde opslaat zonder een vette optie te wijzigen, geldt de regel voor al uw producten.

- Klik op **[!UICONTROL ALL]** en kies `ALL` of `ANY` .
- Klik op **[!UICONTROL TRUE]** en kies `TRUE` of `FALSE` .
- Als u de regel op alle producten wilt toepassen, laat u de voorwaarde ongewijzigd.

U kunt verschillende voorwaarden maken door de combinatie van deze waarden te wijzigen. In dit voorbeeld wordt de volgende voorwaarde gebruikt:

`If ALL of these conditions are TRUE:`

1. Om beschikbare attributen te tonen waarvoor de voorwaarde van toepassing is, klik toevoegen (![ pictogram ](assets/btn-add-grn.png)) pictogram aan het begin van de voorwaardenlijn en selecteer een attribuut waarop om de voorwaarde te baseren.

   **[!UICONTROL Conditions Combination]** - Maak een andere set `All/Any` - en `True/False` -voorwaarden binnen de bestaande voorwaarde.

   ![ de combinatie van de de regelvoorwaarden van de Prijs ](assets/ob-conditions-combinations.png){width="500"}

   **[!UICONTROL Product Attribute]** - de beschikbare productattributen hangen van de [ opstelling van de attributen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html) af. Een kenmerk wordt alleen in de lijst weergegeven als *[!UICONTROL Use for Promo Rule Conditions]* voor het kenmerk is ingesteld op `Yes` in de storefront-eigenschappen.

   - Kies bij **[!UICONTROL Product Attribute]** het kenmerk dat u wilt definiëren als basis voor de voorwaarde. In dit voorbeeld is de geselecteerde voorwaarde `Category` .

     ![ de regelvoorwaarde van de Prijs - lijn 2, deel 2 ](assets/ob-price-rule-condition-2.png){width="500"}

     De geselecteerde voorwaarde wordt weergegeven in de instructie, gevolgd door nog twee vette koppelingen. Welke opties beschikbaar zijn, is afhankelijk van het productkenmerk dat u selecteert.

     Nadat u het kenmerk hebt ingesteld, kunt u het niet meer bewerken. Als u het kenmerk wilt wijzigen, moet u de regel verwijderen en het nieuwe kenmerk toevoegen. U kunt een voorwaardenlijn schrappen door de Schrapping (![ te klikken pictogram van de Schrapping ](assets/btn-del-red.png) aan het eind van de lijn.

   - Klik op **[!UICONTROL is]** en kies de vergelijkingsoperator die de voorwaarde beschrijft waaraan producten moeten voldoen.

     In dit voorbeeld is de vergelijkingsoperator `is` . De beschikbare opties zijn afhankelijk van het kenmerk dat u in de vorige stap hebt geselecteerd en kunnen verschillende vergelijkingsopties bevatten. Opties kunnen overeenkomende waarden bevatten, met uitzondering van of met inbegrip van ten minste een van een waarde, en groter dan, gelijk aan en kleiner dan een numeriek bedrag. In dit voorbeeld zijn de opties `is` en `is not` .

   - Klik op **[!UICONTROL ...]** en kies de kenmerkwaarde waarop de voorwaarde is gebaseerd. Welke opties beschikbaar zijn, is afhankelijk van de instelling van het kenmerk.

     Mogelijk wordt u gevraagd een optie te selecteren of een waarde voor de voorwaarde in te voeren. In dit voorbeeld wordt het veld leeg weergegeven. Om uw categorie(ën) voor de regel te selecteren, klik het selecteurspictogram (![ pictogram van de Kiezer ](assets/btn-chooser.png)) om uw selectieopties te tonen. Deze regel is voor _Boeken_, selecteer **[!UICONTROL Books]** checkbox. Het categorienummer wordt gevuld. Om uw categorieselecties goed te keuren, klik het groene pictogram van het vinkje (![ het merkpictogram van de Controle ](assets/btn-check-mark-green.png)).

     ![ de regelvoorwaarde van de Prijs - lijn 2, deel 3 ](assets/ob-price-rule-condition-3.png){width="500"}

     Het geselecteerde item wordt weergegeven in de instructie om de voorwaarde te voltooien.

     ![ de regelvoorwaarde van de Prijs - lijn 2, deel 4 ](assets/ob-price-rule-condition-4.png){width="500"}

     Deze voorbeeldvoorwaarde is voltooid. Zoals vermeld, betekent deze voorwaarde dat om het even welk product in uw [!DNL Commerce] catalogus die een bepaalde categorie Boeken (`4`) heeft voor deze het tarief regel in aanmerking komt. U kunt meer voorwaardenlijnen toevoegen om uw in aanmerking komende producten verder te beperken.

1. Als u nog een voorwaardelijn aan de instructie wilt toevoegen, gaat u terug naar Stap 1 en herhaalt u het proces totdat alle gewenste voorwaarden zijn voltooid.

   U kunt een lijn van de voorwaardenverklaring op elk ogenblik schrappen door de Schrapping (![ pictogram van de Schrapping ](assets/btn-del-red.png)) aan het eind van de lijn te klikken.
