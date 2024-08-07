---
title: Verkoopkanaal voor Amazon - Voorbeelden van prijsregels
description: Bekijk deze voorbeelden op basis van algemene scenario's om je prijsregels voor Amazon-aanbiedingen te helpen ontwerpen.
feature: Sales Channels, Price Rules
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---

# Voorbeelden van prijsregels

## Voorbeelden van standaardprijsregels

### Verdere regels negeren

De capaciteit om verdere regels te verwerpen is een grote eigenschap binnen het tarief regels die veelvoudige het tarief regels verhinderen te stapelen en onbedoelde extra kortingen te verstrekken. Om verdere regels te verwerpen, moet een het tarief regel de prioriteiten gebruiken die in de _[!UICONTROL Priority]_sectie van [ het Prijsen Algemene Montages van de Regel ](./pricing-rule-general-settings.md) worden geplaatst.

Als **[!UICONTROL Discard Subsequent Rules]** is ingesteld op `Yes` , zijn de regels met een lagere prioriteit (hogere waarden) niet van toepassing op de in aanmerking komende producten.

Stel dat er drie prijsregels zijn:

| Voorbeeld | Naam van regel | Prioriteit | Volgende regel negeren |
|---------|-----------------------|----------|-------------------------|
| 1 | 10% van de verkochte producten | 1 | Nee |
| 2 | $2 aan uitverkoop producten | 2 | Ja |
| 3 | 5% van alle producten | 3 | Nee |

In dit scenario zijn de regels 1 en 2 van toepassing op de in aanmerking komende producten. Regel 3 is alleen van toepassing op in aanmerking komende producten die niet onder regel 2 vallen, omdat deze een lagere prioriteit heeft dan voorbeeld 2 en **[!UICONTROL Discard Subsequent Rules]** is ingesteld op `Yes` . De in aanmerking komende producten in de verkoopcategorie krijgen dus een korting van 10% en $2 van de Amazon-aanbiedingsprijs.

### Twee standaardprijsregels toepassen

| Veld | Instelling - Artikel 1 | Instelling - Artikel 2 |
|--------------------------------|---------------------|-----------------------|
| [!UICONTROL Rule Name] | Artikel 1 | Artikel 2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | Standaardprijsregel | Standaardprijsregel |
| [!UICONTROL Price action] | Verkleinen met | Verkleinen met |
| [!UICONTROL Apply] | Toepassen als percentage | Toepassen als vast bedrag |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### Product 1

Prijs: $ 45,49

Regel 1 toegepast: $45.49 x (0.9) = $40.94

Regel 2 toegepast: $40.94 - $10.00 = $30.94

De uiteindelijke prijs na regel 1 en regel 2 wordt toegepast: $ 30,94

#### Product 2

Prijs: $ 47,76

Regel 1 toegepast: $47,76 x (0,9) = $42,98

Regel 2 toegepast: $42.98 - $10.00 = $32.98

De uiteindelijke prijs na regel 1 en regel 2 wordt toegepast: $ 32,98

## Voorbeelden van intelligente prijsregelaars

### Buy Box prijs met prijs op de vloer Source = Prijs

| Veld | Instelling |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | Artikel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente prijsregel |
| [!UICONTROL Competitor Price Source] | Prijs &quot;Buy Box&quot; gebruiken |
| [!UICONTROL Price Action] | Prijs voor concurrent afstemmen |
| [!UICONTROL Floor Price Source] | Prijs |
| [!UICONTROL Floor Price Action] | Overeenkomst |

#### Product 1

Prijs: $15

[ Buy Box ](./buy-box-competitor-pricing.md) prijs van Amazon: $10

Omdat de [ Buy Box ](./buy-box-competitor-pricing.md) prijs minder dan de originele prijs is, is het product vermeld aan de originele prijs.

De uiteindelijke prijs na toepassing van de regel: $15

#### Product 2

Prijs: $5

[ Buy Box ](./buy-box-competitor-pricing.md) prijs van Amazon: $10

Omdat de [ Buy Box ](./buy-box-competitor-pricing.md) prijs groter is dan de originele prijs, is het product vermeld bij de [ Buy Box ](./buy-box-competitor-pricing.md) prijs.

De uiteindelijke prijs na toepassing van de regel: $10

### Buy Box prijs met prijs op de vloer Source = Prijs en een prijsdaling van 20%

| Veld | Instelling |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | Artikel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente prijsregel |
| [!UICONTROL Competitor Price Source] | Prijs &quot;Buy Box&quot; gebruiken |
| [!UICONTROL Price Action] | Prijs voor concurrent afstemmen |
| [!UICONTROL Floor Price Source] | Prijs |
| [!UICONTROL Floor Price Action] | Verkleinen met |
| [!UICONTROL Apply] | Toepassen als een percentage |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### Product 1

Prijs: $20

Berekende bodemprijs: $16

[ Buy Box ](./buy-box-competitor-pricing.md) prijs van Amazon: $15

Omdat de [ Buy Box ](./buy-box-competitor-pricing.md) prijs minder dan de Berekende [ Vloerprijs ](./floor-price.md) is, is het product vermeld bij de Berekende [ Vloerprijs ](./floor-price.md).

De uiteindelijke prijs na toepassing van de regel: $16

#### Product 2

Prijs: $15

Berekende [ Floor Price ](./floor-price.md): $12

[ Buy Box ](./buy-box-competitor-pricing.md) prijs van Amazon: $15

Omdat de [ Buy Box ](./buy-box-competitor-pricing.md) prijs groter is dan de Berekende [ Vloerprijs ](./floor-price.md), is het product vermeld bij de [ Buy Box ](./buy-box-competitor-pricing.md) prijs.

De uiteindelijke prijs na toepassing van de regel: $15

#### Product 3

Prijs: $17

Berekende bodemprijs: $13,60

[ Buy Box ](./buy-box-competitor-pricing.md) prijs van Amazon: $15

Omdat de [ Buy Box ](./buy-box-competitor-pricing.md) prijs groter is dan de Berekende [ Vloerprijs ](./floor-price.md), is het product vermeld bij de [ Buy Box ](./buy-box-competitor-pricing.md) prijs.

De uiteindelijke prijs na toepassing van de regel: $15

### Laagste prijs met alle prijzen van de concurrent en gebruik alle productvoorwaarden van de concurrent

| Veld | Instelling |
|----------------------------------------|-----------------------------------------|
| [!UICONTROL Rule Name] | Artikel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente prijsregel |
| [!UICONTROL Competitor Price Source] | Laagste concurrent gebruiken |
| [!UICONTROL Minimum Positive Feedback] | Alle concurrerende prijzen |
| [!UICONTROL Conditional Variance] | Alle productvoorwaarden van de concurrent gebruiken |
| [!UICONTROL Price Action] | Prijs voor concurrent afstemmen |
| [!UICONTROL Floor Price Source] | Prijs |
| [!UICONTROL Floor Price Action] | Overeenkomst |

| Prijs | Voorwaarde |
|-------|-----------------|
| $ 17 | Nieuw |
| $ 15 | Nieuw |
| $ 14 | Gebruikt; Zeer goed |
| $ 13 | Gebruikt; Goed |

#### Product 1

Prijs: $10

Voorwaarde: Nieuw

Omdat de laagste concurrerende prijs voor de Nieuwe Voorwaarde $15 is, is het product vermeld bij $15.

De uiteindelijke prijs na toepassing van de regel: $15

#### Product 2

Prijs: $10

Voorwaarde: gebruikt; acceptabel

Omdat de [ laagste concurrerende prijs ](./lowest-competitor-pricing.md) voor de Gebruikte voorwaarde $13 is, is het product vermeld bij $13.

De uiteindelijke prijs na toepassing van de regel: $13

### Intelligente prijsregel die plafondprijs, valutaomrekening en btw combineert

| Veld | Instelling |
|-----------------------------------|---------------|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | $ 10 |
| [!UICONTROL Currency conversion] | 1,25 EUR:1 USD |

[ Plafondprijs ](./optional-ceiling-price.md) in de Europese (BTW) markt: $10 x 1.25 = $12.50

Wanneer de [ maximumprijs ](./optional-ceiling-price.md) op de Europese (BTW) markt wordt geraakt, wordt de BTW berekend en toegevoegd.

Uiteindelijke prijs na BTW: $12,50 x (1,1) = $13,75

### Meerdere prijsregels, plafondprijs, valutaomrekening en btw combineren

#### Intelligente prijsregel (uit vorige voorbeeld)

| Veld | Instelling |
|----------------------|---------------|
| Prioriteit | 1 |
| BTW | 10% |
| Maximumprijsbron | $ 10 |
| Omrekening in valuta | 1,25 EUR:1 USD |

[ Plafondprijs ](./optional-ceiling-price.md) in de Europese (BTW) markt: $10 x 1.25 = $12.50

Uiteindelijke prijs na BTW: $12,50 x (1,1) = $13,75

#### Standaardprijsregel

| Veld | Instelling |
|--------------------------------|-----------------------|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | Vergroten met |
| [!UICONTROL Apply] | Toepassen als vast bedrag |
| [!UICONTROL Adjustment Amount] | $ 5,00 |

Wanneer de [ plafondprijs ](./optional-ceiling-price.md) wordt geraakt, wordt de standaardprijsregel toegepast bovenop de intelligente prijsstellingsregel.

Uiteindelijke prijs na toepassing van de standaardprijsregel: $13,75 + $5,00 = $18,75

### Prijsaanpassing

In dit voorbeeld, wordt de meest concurrerende prijs bepaald door de laagste prijs van de Amazon [ concurrent ](./lowest-competitor-pricing.md) met een 95% positieve terugkoppel en een minimum terugkoppelt telling van 1.000 koopvaardijoverzichten te bekijken.

![ de aanpassingsvoorbeeld van de Prijs ](assets/amazon-price-adjustment-example.png){width="600" zoomable="yes"}

Nadat deze zoekopdracht op basis van deze parameters is uitgevoerd, komt de concurrerende prijs terug op $25.

Van hier, zijn er drie verschillende ](./pricing-rule-actions.md) keuzen van de prijsregel 0} die op deze laagste prijs worden gebaseerd.[

| Veld | Beschrijving |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | Opties:<ul><li>**[!UICONTROL Decrease By]** - deze optie vermindert uw lijstprijs met betrekking tot de [ laagste concurrerende prijs ](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Increase By]** - deze optie verhoogt uw lijstprijs met betrekking tot de [ laagste concurrerende prijs ](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** - Met deze optie wordt de prijs van je Amazon-aanbieding aangepast aan de laagste prijs op basis van de parameters. In het voorbeeld is de Amazon-prijs $25.</li></ul> |
| [!UICONTROL Apply] | Opties: Toepassen als percentage / Toepassen als vaste hoeveelheid |
| [!UICONTROL Adjustment Amount] | Numerieke waarde om het percentage of vaste bedrag voor de toe te passen korting te bepalen. <br> deze selecties resulteren in het nemen van de laagste prijs en het plaatsen van het bij $0.01 minder. |

### Floor Price

| Veld | Instelling |
|--------------------------------------|---------------------|
| [!UICONTROL Floor Price Source] | Kosten = $5 |
| [!UICONTROL Floor Price Action] | Vergroten met |
| [!UICONTROL Apply] | Toepassen als percentage |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[ Floor Price ](./floor-price.md) berekening = Floor Price Source `$5` x Floor Adjustment Amount `5%` = $5.25

Wanneer de intelligente prijsregel wordt toegepast, staat het de aanbiedingsprijs toe om lager te zijn dan $5.25 voor dit specifieke product wanneer de kosten $5 zijn.
