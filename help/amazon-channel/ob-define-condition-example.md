---
title: 'Voorbeeld: een voorwaarde definiëren voor Amazon-aanbiedingsregels'
description: Wanneer je je aanbiedingsregels maakt, moet je voorwaarden definiëren voor het identificeren van de Commerce-catalogusproducten die op de Amazon Marketplace moeten worden vermeld.
feature: Sales Channels, Products, Configuration
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Voorbeeld: een voorwaarde definiëren

## Voorwaarden

U kunt op alle gebieden in de voorwaarden die vet zijn, klikken om de verschillende opties weer te geven.

**voeg geen voorwaarden toe als alle producten binnen de geselecteerde website verkiesbaar zijn.**

>[!NOTE]
>
>Er is een complexe reeks back-end processen om direct met Amazon-systemen te communiceren. Op basis van het aantal objecten dat je probeert aan te bieden en de manier waarop het druk is met Amazon-systemen (zoals &#39;Zwarte Vrijdag&#39;), kan het enige tijd duren voordat je objecten op Amazon worden aangeboden.

Zie de sectie van Voorwaarden van [ Creërend een Regel van de Prijs van de Kar ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog-create.html).

## Een voorwaarde definiëren

Dit proces kan eenvoudig of gedetailleerd zijn, afhankelijk van de setup van de catalogus. U kunt de voorwaarden zodanig instellen dat wanneer `ALL` of `ANY` van de gedefinieerde voorwaarden `TRUE` of `FALSE` zijn voor een product, het product in aanmerking komt om op Amazon te worden aangeboden.

Voorwaarden zijn gebaseerd op bestaande productkenmerkwaarden. Als u de regel op alle producten wilt toepassen, laat u de sectie Voorwaarden leeg.

>[!NOTE]
>
>Als u een voorwaarde wilt definiëren die is gebaseerd op een specifiek productkenmerk, stelt u de instelling **[!UICONTROL Use for Promo Rule Conditions]** voor het kenmerk in op `Yes` . U kunt tot dit het plaatsen op de [ pagina van Eigenschappen Storefront ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes-add.html) voor de attributen toegang hebben.

![ Voorwaarde - lijn 1 ](assets/ob-listing-rule-conditions-start.png){width="500"}

De regel in dit voorbeeld bepaalt een regel die Amazon geschiktheid voor alle catalogusproducten plaatst die het _FBA van Amazon_ attribuut hebben dat aan `Yes` wordt geplaatst.

De regelinstructie heeft twee vette koppelingen, die, wanneer erop wordt geklikt, de opties voor dat gedeelte van de instructie weergeven. Als u de voorwaarde opslaat zonder een vetgedrukte optie te wijzigen, geldt de regel voor al uw producten.

- Klik op **[!UICONTROL ALL]** en kies `ALL` of `ANY` .
- Klik op **[!UICONTROL TRUE]** en kies `TRUE` of `FALSE` .
- Als u de regel op alle producten wilt toepassen, laat u de voorwaarde ongewijzigd.

U kunt verschillende voorwaarden maken door de combinatie van deze waarden te wijzigen. In dit voorbeeld wordt de volgende voorwaarde gebruikt:

`If ALL of these conditions are TRUE:`

1. Klik toevoegen (![ pictogram ](assets/btn-add-grn.png)) pictogram aan het begin van de voorwaardenlijn en selecteer een attribuut waarop om de voorwaarde, zoals een voorwaardencombinatie of een productattribuut te baseren.

   - **[!UICONTROL Conditions Combination]** - U kunt desgewenst een andere set `All/Any` - en `True/False` -voorwaarden binnen de bestaande set maken.

     ![ de combinatie van Voorwaarden ](assets/ob-conditions-combinations.png){width="500"}

   - **[!UICONTROL Product Attribute]** - De productkenmerken zijn afhankelijk van de instelling van het kenmerk. Voor een attribuut om in de lijst te verschijnen, moet het voor gebruik in promotionele regelvoorwaarden worden gevormd. Zie het _Gebruik voor de Voorwaarden van de Regel van de Aanbieding_ in [ Attributen van het Product ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

     Kies in de lijst onder **[!UICONTROL Product Attribute]** het kenmerk dat u als basis voor de voorwaarde wilt gebruiken. In dit voorbeeld is de geselecteerde voorwaarde `Amazon FBA` .

     ![ lijn 2 van de Voorwaarde, deel 2 ](assets/ob-condition-attribute-dropdown.png){width="350"}

     De geselecteerde voorwaarde wordt weergegeven in de instructie, gevolgd door nog twee vette koppelingen. Welke opties beschikbaar zijn, is afhankelijk van het productkenmerk dat u selecteert.

     Nadat u het kenmerk hebt ingesteld, kunt u het niet meer wijzigen. Als u het kenmerk wilt wijzigen, moet u de regel verwijderen en het nieuwe kenmerk toevoegen. U kunt een voorwaardenlijn schrappen door de Schrapping (![ te klikken pictogram van de Schrapping ](assets/btn-del-red.png)) aan het eind van de lijn.

      1. Klik op **[!UICONTROL is]** en kies de vergelijkingsoperator die de voorwaarde beschrijft waaraan producten moeten voldoen.

         In dit voorbeeld is de vergelijkingsoperator `is` . Welke opties beschikbaar zijn, is afhankelijk van het kenmerk dat u in de vorige stap hebt geselecteerd. Opties kunnen verschillende vergelijkingsopties bevatten, zoals overeenkomende waarden, met of zonder ten minste een waarde en groter dan, gelijk aan en kleiner dan een numeriek bedrag. In dit voorbeeld zijn de opties `is` en `is not` .

      1. Klik op **[!UICONTROL ...]** en kies de kenmerkwaarde waarop de voorwaarde is gebaseerd.

         Welke opties beschikbaar zijn, is afhankelijk van de instelling van het kenmerk. Mogelijk wordt u gevraagd een optie te selecteren of tekst of numerieke waarden voor de voorwaarde in te voeren. In dit voorbeeld is de selectie `Yes` .

         Het geselecteerde item wordt weergegeven in de instructie om de voorwaarde te voltooien.

         ![ lijn 2 van de Voorwaarde, deel 3 ](assets/ob-listing-rule-condition-is.png){width="500"}

   Deze voorwaarde is voltooid. Zoals vermeld, betekent deze voorwaarde dat elk product in uw [!DNL Commerce] -catalogus waarvoor het Amazon FBA-kenmerk is ingesteld op de waarde `Yes` , in aanmerking komt voor aanbieding aan Amazon voor het gebied en de winkel. U kunt meer voorwaardenlijnen toevoegen om uw in aanmerking komende producten verder te beperken.

1. Als u nog een voorwaardelijn aan de instructie wilt toevoegen, gaat u terug naar stap 1 en herhaalt u het proces totdat alle gewenste voorwaarden zijn voltooid.

U kunt een lijn van de voorwaardenverklaring op elk ogenblik schrappen door de Schrapping (![ pictogram van de Schrapping ](assets/btn-del-red.png)) aan het eind van de lijn te klikken.
