---
title: '''Voorbeeld: Een voorwaarde definiëren'''
description: Wanneer je regels voor aanbiedingen maakt, moet je voorwaarden definiëren voor het identificeren van de catalogusproducten die op de Amazon Marketplace moeten worden aangeboden.
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Voorbeeld: Een voorwaarde definiëren

## Voorwaarden

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

**Voeg geen voorwaarden toe als alle producten op de geselecteerde website in aanmerking komen.**

>[!NOTE]
>
>Er is een complexe reeks back-end processen om direct met Amazon-systemen te communiceren. Op basis van het aantal objecten dat je probeert aan te bieden en de manier waarop het druk is met Amazon-systemen (zoals &#39;Zwarte Vrijdag&#39;), kan het enige tijd duren voordat je objecten op Amazon worden aangeboden.

Zie de sectie Voorwaarden van [Een regel voor een startprijs maken](https://docs.magento.com/user-guide/marketing/price-rules-catalog-create.html){:target=&quot;_blank&quot;}.

## Een voorwaarde definiëren

Dit proces kan eenvoudig of gedetailleerd zijn, afhankelijk van de setup van de catalogus. U kunt uw voorwaarden zodanig instellen dat wanneer `ALL` of `ANY` van de gedefinieerde voorwaarden `TRUE` of `FALSE` voor een product zijn, het product in aanmerking komt om op Amazon te worden vermeld.

Voorwaarden zijn gebaseerd op bestaande productkenmerkwaarden. Laat de sectie voor voorwaarden leeg als u de regel op alle producten wilt toepassen.

>[!NOTE]
>
>Als u een voorwaarde wilt bepalen die op een specifiek productattribuut wordt gebaseerd, plaats **[!UICONTROL Use for Promo Rule Conditions]** plaatsen voor het attribuut aan `Yes`. U kunt tot deze het plaatsen op [pagina van Eigenschappen Storefront](https://docs.magento.com/user-guide/catalog/product-attributes-add.html){:target=&quot;_blank&quot;} voor de attributen toegang hebben.

![Voorwaarde - regel 1](assets/ob-listing-rule-conditions-start.png)

De regel in dit voorbeeld definieert een regel die Amazon geschiktheid instelt voor alle catalogusproducten waarvoor het _Amazon FBA_-kenmerk is ingesteld op `Yes`.

De regelinstructie heeft twee vette koppelingen, die, wanneer erop wordt geklikt, de opties voor dat gedeelte van de instructie weergeven. Als u de voorwaarde opslaat zonder een vetgedrukte optie te wijzigen, geldt de regel voor al uw producten.

- Klik **[!UICONTROL ALL]** en kies of `ALL` of `ANY`.
- Klik **[!UICONTROL TRUE]** en kies of `TRUE` of `FALSE`.
- Als u de regel op alle producten wilt toepassen, laat u de voorwaarde ongewijzigd.

U kunt verschillende voorwaarden maken door de combinatie van deze waarden te wijzigen. In dit voorbeeld wordt de volgende voorwaarde gebruikt:

`If ALL of these conditions are TRUE:`

1. Klik op het pictogram Toevoegen (![Pictogram toevoegen](assets/btn-add-grn.png)) aan het begin van de voorwaardelijn en selecteer een kenmerk waarop de voorwaarde moet worden gebaseerd, zoals een voorwaardencombinatie of een productkenmerk.

   - **[!UICONTROL Conditions Combination]** - Kies deze optie als u een andere set  `All/Any` en  `True/False` voorwaarden in de bestaande set wilt maken.

      ![Combinatie van voorwaarden](assets/ob-conditions-combinations.png)

   - **[!UICONTROL Product Attribute]** - De productkenmerken zijn afhankelijk van de instelling van het kenmerk. Voor een attribuut om in de lijst te verschijnen, moet het voor gebruik in promotionele regelvoorwaarden worden gevormd. Zie _Gebruik voor de Voorwaarden van de Regel van de Bevordering_ in [ProductAttributen](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}.

      Kies in de lijst onder **[!UICONTROL Product Attribute]** het kenmerk dat u als basis voor de voorwaarde wilt gebruiken. In dit voorbeeld is de geselecteerde voorwaarde `Amazon FBA`.

      ![Voorwaardelijke regel 2, deel 2](assets/ob-condition-attribute-dropdown.png)

      De geselecteerde voorwaarde wordt weergegeven in de instructie, gevolgd door nog twee vette koppelingen. Welke opties beschikbaar zijn, is afhankelijk van het productkenmerk dat u selecteert.

      Nadat u het kenmerk hebt ingesteld, kunt u het niet meer wijzigen. Als u het kenmerk wilt wijzigen, moet u de regel verwijderen en het nieuwe kenmerk toevoegen. U kunt een voorwaardelijn schrappen door het Schrappingspictogram (![Schrappingspictogram](assets/btn-del-red.png)) aan het eind van de lijn te klikken.

      1. Klik op **[!UICONTROL is]** en kies de vergelijkingsoperator die de voorwaarde beschrijft waaraan producten moeten voldoen.

         In dit voorbeeld is de vergelijkingsoperator `is`. Welke opties beschikbaar zijn, is afhankelijk van het kenmerk dat u in de vorige stap hebt geselecteerd. Opties kunnen verschillende vergelijkingsopties bevatten, zoals overeenkomende waarden, met of zonder ten minste een waarde en groter dan, gelijk aan en kleiner dan een numeriek bedrag. In dit voorbeeld zijn de opties `is` en `is not`.

      1. Klik **[!UICONTROL ...]** en kies de kenmerkwaarde waarop de voorwaarde is gebaseerd.

         Welke opties beschikbaar zijn, is afhankelijk van de instelling van het kenmerk. Mogelijk wordt u gevraagd een optie te selecteren of tekst of numerieke waarden voor de voorwaarde in te voeren. In dit voorbeeld is de selectie `Yes`.

         Het geselecteerde item wordt weergegeven in de instructie om de voorwaarde te voltooien.

         ![Voorwaardelijke regel 2, deel 3](assets/ob-listing-rule-condition-is.png)
   Deze voorwaarde is voltooid. Zoals aangegeven betekent deze voorwaarde dat elk product in uw [!DNL Commerce]-catalogus waarvoor het Amazon FBA-kenmerk is ingesteld op de waarde `Yes`, in aanmerking komt voor aanbieding aan Amazon voor het gebied en de winkel. U kunt meer voorwaardenlijnen toevoegen om uw in aanmerking komende producten verder te verfijnen.

1. Als u nog een voorwaardelijn aan de instructie wilt toevoegen, gaat u terug naar stap 1 en herhaalt u het proces totdat alle gewenste voorwaarden zijn voltooid.

U kunt een lijn van de voorwaardenverklaring op elk ogenblik schrappen door de Schrapping (![pictogram van de Schrapping](assets/btn-del-red.png)) aan het eind van de lijn te klikken.
