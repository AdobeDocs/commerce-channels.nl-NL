---
title: Objectgegevens van Amazon bekijken
description: Bekijk de pagina Productaanbiedingsgegevens voor meer informatie over de maatstaven van je Amazon-aanbiedingen en over afzonderlijke wijzigingen in SKU/product.
feature: Sales Channels, Products, Merchandising
exl-id: faece1b1-b4fb-4506-bf77-576ae445ed28
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Objectgegevens van Amazon bekijken

Op de pagina _[!UICONTROL Product Listing Details]_vindt u aanvullende informatie over actieve productaanbiedingen, waaronder het activiteitenlogboek van de aanbieding, waarin de wijzigingen voor een afzonderlijke SKU/product worden weergegeven. Deze informatie kan u helpen concurrerende metriek op uw producten en op individuele SKU/productveranderingen begrijpen. Aanvullende informatie op deze pagina is onder meer:

- **[!UICONTROL Listing Details]** - Productgegevens inclusief naam en SKU van Amazon-verkoper
- **[!UICONTROL Listing Activity Log]** - Historisch overzicht van alle wijzigingen die zich voor deze aanbieding hebben voorgedaan, zoals prijswijzigingen en wijzigingen in aantal/voorraad. Er zijn geen verdere acties vereist. Dit logboek wordt verstrekt voor overzicht om de veranderingsgeschiedenis te begrijpen.
- **[!UICONTROL Buy Box Competitor Pricing]** - Gegevens voor Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) -status en prijzen voor concurrenten
- **[!UICONTROL Lowest Competitor Pricing]** - Informatie over de prijzen en feedback-informatie van de laagste Amazon-concurrent

Amazon delen de homepages van het verkoopkanaal wat gemeenschappelijke [ werkruimtesecontroles ](./workspace-controls.md) die u toestaan om de gegevens aan te passen die worden getoond.

## Aanbiedingsgegevens

De weergegeven productinformatie bevat:

- _[!UICONTROL Amazon Name]_
- _[!UICONTROL Catalog (Magento) SKU]_
- _[!UICONTROL Amazon Seller SKU]_

![ het Lijst details ](assets/amazon-product-listing-details.png){width="600" zoomable="yes"}

## Logbestand met aanbiedingsactiviteiten {#listing-activity-log}

Alle recente activiteiten voor de Amazon-aanbieding worden weergegeven. De getoonde informatie omvat:

- Amazon Verkoper SKU: identificeert de Stock Keeping Unit (SKU) die voor de aanbieding wordt bepaald.
- ASIN: Identificeert de 10-cijferige Amazon product-id.
- Handeling voor aanbieding: identificeert het type handeling dat is opgetreden voor de aanbieding.
- Opmerkingen: bevat aanvullende details met betrekking tot het type handeling dat is opgenomen in de lijst.
- Uitgevoerd om: Identificeert de datum en het tijdstip waarop de handeling heeft plaatsgevonden.

![ de lijstdetails van het Product - het logboek van de lijstactiviteit ](assets/amazon-listing-activity-log.png){width="600" zoomable="yes"}
__

## Buy Box concurrent, prijsstelling {#buy-box-competitor-pricing}

Op dit tabblad wordt informatie weergegeven over de Amazon-handelaar die de [[!DNL Buy Box]](./buy-box-competitor-pricing.md) -positie voor de vermelding bevat. Deze informatie kan worden gebruikt om de prijsstelling van uw concurrenten op Amazon te begrijpen. De getoonde informatie omvat:

- ASIN: De 10-cijferige Amazon product identifier.
- Is verkoper: geeft aan of je de [!DNL Buy Box] verkoper bent. Opties Ja/Nee.
- Voorwaarde: hiermee wordt aangegeven welke voorwaarde voor de aanbieding is gedefinieerd.
- Aanbiedingsprijs: geeft de prijs aan waartegen de aanbieding is gepubliceerd.
- Verzendprijs: geeft de verzendprijs aan die aan de aanbieding is toegevoegd.
- Landed Price: geeft de prijs van de aanbieding plus de verzendprijs voor de aanbieding aan.
- Laatst bijgewerkt: identificeert de datum en tijd waarop de prijsinformatie van Amazon is bijgewerkt.

![ de lijstdetails van het product: Buy Box concurrent tarifering ](assets/amazon-listing-details-buy-box-2.png){width="600" zoomable="yes"}

## Laagste prijsstelling voor concurrenten {#lowest-competitor-pricing}

Op dit tabblad wordt informatie weergegeven over Amazon-concurrenten voor dezelfde aanbieding. Deze informatie kan worden gebruikt om prijspositionering en [ laagste concurrerende tarifering ](./lowest-competitor-pricing.md) te begrijpen. De getoonde informatie omvat:

- ASIN: De 10-cijferige Amazon product identifier.
- Voorwaarde: hiermee wordt aangegeven welke voorwaarde voor de aanbieding is gedefinieerd.
- Fulfillment Channel: identificeert de partij die verantwoordelijk is voor de uitvoering. Opties: Merchant/Amazon.
- Aanbiedingsprijs: geeft de prijs aan waartegen de aanbieding is gepubliceerd.
- Verzendprijs: geeft de verzendprijs aan die aan de aanbieding is toegevoegd.
- Landed Price: geeft de prijs van de aanbieding plus de verzendprijs voor de aanbieding aan.
- Feedbackscore: geeft de Amazon-feedbackscore aan voor de laagste prijs.
- Aantal feedback: hiermee wordt het aantal feedback van Amazon voor de laagste prijs aangegeven.
- Laatst bijgewerkt: identificeert de datum en tijd waarop de prijsinformatie van Amazon is bijgewerkt.

![ de lijstdetails van het Product - laagste concurrerende tarifering ](assets/amazon-listing-details-lowest-comp.png){width="600" zoomable="yes"}
