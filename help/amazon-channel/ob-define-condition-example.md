---
title: 'Voorbeeld: een voorwaarde definiëren voor Amazon-aanbiedingsregels'
description: Wanneer je regels voor aanbiedingen maakt, moet je voorwaarden definiëren voor het identificeren van de catalogusproducten die op de Amazon Marketplace moeten worden aangeboden.
feature: Sales Channels, Products, Configuration
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---

# Voorbeeld: een voorwaarde definiëren

## Voorwaarden

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

**Voeg geen voorwaarden toe als alle producten op de geselecteerde website in aanmerking komen.**

>[!NOTE]
>
>Er is een complexe reeks back-end processen om direct met Amazon-systemen te communiceren. Op basis van het aantal objecten dat je probeert aan te bieden en de manier waarop het druk is met Amazon-systemen (zoals &#39;Zwarte Vrijdag&#39;), kan het enige tijd duren voordat je objecten op Amazon worden aangeboden.

Zie de sectie Voorwaarden van [Een regel voor een startprijs maken](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog-create.html).

## Een voorwaarde definiëren

Dit proces kan eenvoudig of gedetailleerd zijn, afhankelijk van de setup van de catalogus. U kunt de voorwaarden zodanig instellen dat wanneer `ALL` of `ANY` van de vastgestelde voorwaarden: `TRUE` of `FALSE` voor een product in aanmerking komt om op Amazon te worden vermeld.

Voorwaarden zijn gebaseerd op bestaande productkenmerkwaarden. Als u de regel op alle producten wilt toepassen, laat u de sectie Voorwaarden leeg.

>[!NOTE]
>
>Als u een voorwaarde wilt bepalen die op een specifiek productattribuut wordt gebaseerd, plaats **[!UICONTROL Use for Promo Rule Conditions]** instellen voor het kenmerk op `Yes`. U kunt deze instelling openen op het tabblad [Eigenschappen van Storefront](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes-add.html) pagina voor het kenmerk.

![Voorwaarde - regel 1](assets/ob-listing-rule-conditions-start.png){width="500"}

De regel in dit voorbeeld definieert een regel die stelt dat Amazon in aanmerking komt voor alle catalogusproducten die de _Amazon FBA_ kenmerk ingesteld op `Yes`.

De regelinstructie heeft twee vette koppelingen, die, wanneer erop wordt geklikt, de opties voor dat gedeelte van de instructie weergeven. Als u de voorwaarde opslaat zonder een vetgedrukte optie te wijzigen, geldt de regel voor al uw producten.

- Klikken **[!UICONTROL ALL]** en kiest u `ALL` of `ANY`.
- Klikken **[!UICONTROL TRUE]** en kiest u `TRUE` of `FALSE`.
- Als u de regel op alle producten wilt toepassen, laat u de voorwaarde ongewijzigd.

U kunt verschillende voorwaarden maken door de combinatie van deze waarden te wijzigen. In dit voorbeeld wordt de volgende voorwaarde gebruikt:

`If ALL of these conditions are TRUE:`

1. Klik op Toevoegen (![Pictogram toevoegen](assets/btn-add-grn.png)) aan het begin van de voorwaardelijn en selecteer een kenmerk waarop de voorwaarde moet worden gebaseerd, zoals een voorwaardencombinatie of een productkenmerk.

   - **[!UICONTROL Conditions Combination]** - Kies deze optie als u een andere set `All/Any` en `True/False` voorwaarden binnen de bestaande set.

     ![Combinatie van voorwaarden](assets/ob-conditions-combinations.png){width="500"}

   - **[!UICONTROL Product Attribute]** - De productkenmerken zijn afhankelijk van de instelling van het kenmerk. Voor een attribuut om in de lijst te verschijnen, moet het voor gebruik in promotionele regelvoorwaarden worden gevormd. Zie de _Voorwaarden voor promotieregels gebruiken_ in [Productkenmerken](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

     In de lijst onder **[!UICONTROL Product Attribute]** kiest u het kenmerk dat u als basis voor de voorwaarde wilt gebruiken. In dit voorbeeld is de geselecteerde voorwaarde: `Amazon FBA`.

     ![Voorwaardelijke regel 2, deel 2](assets/ob-condition-attribute-dropdown.png){width="350"}

     De geselecteerde voorwaarde wordt weergegeven in de instructie, gevolgd door nog twee vette koppelingen. Welke opties beschikbaar zijn, is afhankelijk van het productkenmerk dat u selecteert.

     Nadat u het kenmerk hebt ingesteld, kunt u het niet meer wijzigen. Als u het kenmerk wilt wijzigen, moet u de regel verwijderen en het nieuwe kenmerk toevoegen. U kunt een voorwaardenlijn schrappen door Schrapping te klikken (![Pictogram Verwijderen](assets/btn-del-red.png)) aan het einde van de regel.

      1. Klikken **[!UICONTROL is]** en kiest u de vergelijkingsoperator die de voorwaarde beschrijft waaraan producten moeten voldoen.

         In dit voorbeeld is de vergelijkingsoperator `is`. Welke opties beschikbaar zijn, is afhankelijk van het kenmerk dat u in de vorige stap hebt geselecteerd. Opties kunnen verschillende vergelijkingsopties bevatten, zoals overeenkomende waarden, met of zonder ten minste een waarde en groter dan, gelijk aan en kleiner dan een numeriek bedrag. In dit voorbeeld zijn de opties: `is` en `is not`.

      1. Klikken **[!UICONTROL ...]** en kiest u de kenmerkwaarde waarop de voorwaarde is gebaseerd.

         Welke opties beschikbaar zijn, is afhankelijk van de instelling van het kenmerk. Mogelijk wordt u gevraagd een optie te selecteren of tekst of numerieke waarden voor de voorwaarde in te voeren. In dit voorbeeld is de selectie `Yes`.

         Het geselecteerde item wordt weergegeven in de instructie om de voorwaarde te voltooien.

         ![Voorwaardelijke regel 2, deel 3](assets/ob-listing-rule-condition-is.png){width="500"}

   Deze voorwaarde is voltooid. Zoals gezegd betekent deze voorwaarde dat elk product in uw [!DNL Commerce] catalogus waarvan het Amazon FBA-kenmerk is ingesteld op een waarde van `Yes` komt in aanmerking voor aanbieding aan Amazon voor de regio en winkel. U kunt meer voorwaardenlijnen toevoegen om uw in aanmerking komende producten verder te beperken.

1. Als u nog een voorwaardelijn aan de instructie wilt toevoegen, gaat u terug naar stap 1 en herhaalt u het proces totdat alle gewenste voorwaarden zijn voltooid.

U kunt op elk gewenst moment een regel van de instructie condition verwijderen door op Verwijderen te klikken (![Pictogram Verwijderen](assets/btn-del-red.png)) aan het einde van de regel.
