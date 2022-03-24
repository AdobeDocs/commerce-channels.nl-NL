---
title: Aanbiedingen publiceren naar Walmart
description: Publiceer aanbiedingen voor Commerce-producten naar Walmart Marketplace om te beginnen met verkopen.
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Aanbiedingen publiceren naar Walmart

Net als andere markten biedt Walmart verkopers van derden de mogelijkheid om objecten aan te bieden die door anderen worden verkocht.

Het platform gebruikt product-id&#39;s zoals UPC en GTIN om overeen te komen met items die al te koop zijn.
Voor gematchte producten wordt de bestaande Walmart Marketplace-vermelding bijgewerkt en bevat deze de aanbieding voor het product Commerce.
Doorgaans worden producten met de laagste prijzen eerst in de resultaten vermeld. Maar andere factoren zoals recensies beïnvloeden ook plaatsing.

## Werkstroom afstemmen

Wanneer u producten aanpast, stuurt de Manager van het Kanaal de productgegevens naar Marketplace van de Markt van de Markt van de Markt om naar bestaande lijsten met attributenwaarden te zoeken die de in kaart gebrachte het productattribuut van de Handel aanpassen.

Als er een overeenkomst wordt gevonden, wordt de bestaande productaanbieding bijgewerkt en wordt je voorstel toegevoegd.

## Vereisten

Alvorens producten aan te passen, verifieer dat uw de attributenwaarden van de productcatalogus voldoen aan de vereisten van het Martard en attributenmontages vormen. Zie [Productovereenkomst configureren](map-product-attributes-for-matching.md)

## Producten selecteren en afstemmen

1. Open een verbonden verkoopkanaal.

1. Van **[!UICONTROL Listings]**, selecteer de producten die overeenkomen met de producten in *[!UICONTROL Draft]* status.

   ![Producten uit aanbiedingen selecteren en verzenden voor overeenkomst](assets/products-in-marketplace-sales-channel.png)

1. Selecteren **[!UICONTROL Match Products]**.

   Een bericht geeft het aantal producten aan dat voor matching is verzonden.

   ![Producten naar het verbonden verkoopkanaal verzenden](assets/products-submit-for-matching.png)

   Het kan tot 30 minuten voor Walmart Marketplace duren om de gelijke verrichting te voltooien.

   De status van geselecteerde producten verandert in *[!UICONTROL Processing]* totdat de overeenkomende bewerkingen zijn voltooid. Het kan tot 30 minuten voor Walmart Marketplace duren om de gelijke verrichting te voltooien.

## Overeenkomststatus controleren

1. Selecteren **Producten vernieuwen** om de meest recente productstatus bij te werken.

1. Controleer de productstatus.

   Nadat de overeenkomst is voltooid, kan de status *Overeenkomst* of *Fout*.

   * **[!UICONTROL Match]** geeft aan dat het product is gevonden. Je productaanbod is gepubliceerd naar een bestaande Walmart Marketplace-aanbieding.

   * **[!UICONTROL Error]** Hiermee wordt een van de volgende items aangegeven:

      * Er is een fout opgetreden en de overeenkomende bewerking is mislukt.

      * Er is geen overeenkomst gevonden.

      * Overeenkomst gevonden, maar product gepubliceerd als gefaseerd omdat [Marktarchief is niet actief](walmart-prerequisites.md#walmart-marketplace-store-status).

## Problemen met overeenkomende productfouten oplossen

Als de verrichting van de productgelijke ontbreekt, keert de Marketplace van de Markt van de Markeren een foutencode terug en de Manager van het Kanaal toont de foutenstatus in de informatie van de productlijst.

Geef de details van foutberichten weer door de muisaanwijzer op de knop **Fout** statuslabel. Gangbare geretourneerde fouten zijn onjuist opgemaakte product-id-waarden of ontbrekende vereiste kenmerken.

## ID-waarden van product corrigeren

| Type | Beschrijving | Voorbeeld |
|------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, het 12-cijferige getal inclusief controlecijfer.</br></br>Als uw UPC minder dan 12 cijfers, zoals UPC-E heeft die 8 cijfers is, voeg toe</br>nullen met regelafstand om aan deze eis te voldoen. | Wijzigen van `45678912345` tot `045678912345` |
| GTIN | GTIN-14, het 14-cijferige getal inclusief controlecijfer.</br></br>Als de GTIN uit minder dan 14 cijfers bestaat, voegt u voorloopnullen toe </br>om aan deze eis te voldoen. | Wijzigen `456789123456` tot `0045678912345` |
| EAN | GTIN-13, het 13-cijferige getal inclusief controlecijfer.</br></br>Als uw EAN minder dan 13 cijfers heeft, voeg belangrijke</br>nullen om aan de vereiste te voldoen. | Wijzigen van `4567891234` tot `0004567891234` |

Voor meer informatie over de foutcodes van Walmart Marketplace raadpleegt u de [Help bij Walmart Seller](https://sellerhelp.walmart.com/s/guide?article=000005844).
