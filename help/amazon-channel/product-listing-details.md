---
title: Objectgegevens van Amazon bekijken
description: Bekijk de pagina Productaanbiedingsgegevens voor meer informatie over de maatstaven van je Amazon-aanbiedingen en over afzonderlijke wijzigingen in SKU/product.
feature: Sales Channels, Products, Merchandising
exl-id: faece1b1-b4fb-4506-bf77-576ae445ed28
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Objectgegevens van Amazon bekijken

De _[!UICONTROL Product Listing Details]_Deze pagina bevat aanvullende informatie over actieve productaanbiedingen, waaronder het activiteitenlogboek van de aanbieding waarin de wijzigingen op een afzonderlijke SKU/product worden weergegeven. Deze informatie kan u helpen concurrerende metriek op uw producten en op individuele SKU/productveranderingen begrijpen. Aanvullende informatie op deze pagina is onder meer:

- **[!UICONTROL Listing Details]** - Productgegevens inclusief naam en SKU van Amazon-verkoper
- **[!UICONTROL Listing Activity Log]** - Historisch overzicht van alle wijzigingen die zich voor deze aanbieding hebben voorgedaan, zoals prijswijzigingen en wijzigingen in aantal/voorraad. Er zijn geen verdere acties vereist. Dit logboek wordt verstrekt voor overzicht om de veranderingsgeschiedenis te begrijpen.
- **[!UICONTROL Buy Box Competitor Pricing]** - Gegevens voor Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) status en prijsstelling voor concurrenten
- **[!UICONTROL Lowest Competitor Pricing]** - Informatie over de prijzen en feedback van de laagste Amazon-concurrent

Homepages van Amazon-verkoopkanalen delen [besturingselementen voor werkruimte](./workspace-controls.md) waarmee u de weergegeven gegevens kunt aanpassen.

## Aanbiedingsgegevens

De weergegeven productinformatie bevat:

- _[!UICONTROL Amazon Name]_
- _[!UICONTROL Catalog (Magento) SKU]_
- _[!UICONTROL Amazon Seller SKU]_

![Aanbiedingsgegevens](assets/amazon-product-listing-details.png){width="600" zoomable="yes"}

## Logbestand met aanbiedingsactiviteiten {#listing-activity-log}

Alle recente activiteiten voor de Amazon-aanbieding worden weergegeven. De getoonde informatie omvat:

- Amazon-verkoopSKU: Identificeert de Stock Keeping Unit (SKU) die voor de lijst wordt bepaald.
- ASIN: Identificeert de 10-cijferige Amazon product-id.
- Handeling voor aanbieding: Hiermee wordt het type handeling aangegeven dat is uitgevoerd voor de vermelding.
- Opmerkingen: Verstrekt extra details met betrekking tot het type van lijstactie die voorkwam.
- Uitgevoerd om: Identificeert de datum en de tijd de actie voorkwam.

![Gegevens van productaanbiedingen - logboek van aanbiedingsactiviteiten](assets/amazon-listing-activity-log.png){width="600" zoomable="yes"}
__

## Buy Box concurrent {#buy-box-competitor-pricing}

Op dit tabblad wordt informatie weergegeven over de Amazon-handelaar die de [[!DNL Buy Box]](./buy-box-competitor-pricing.md) positie voor de aanbieding. Deze informatie kan worden gebruikt om de prijsstelling van uw concurrenten op Amazon te begrijpen. De getoonde informatie omvat:

- ASIN: De 10-cijferige Amazon product identifier.
- Is verkoper: Hiermee wordt aangegeven of u de [!DNL Buy Box] verkoper. Opties Ja/Nee.
- Voorwaarde: Hiermee wordt de gedefinieerde voorwaarde voor de aanbieding aangegeven.
- Aanbiedingsprijs: Hiermee wordt de prijs aangegeven waartegen de aanbieding is gepubliceerd.
- Verzendprijs: Hiermee wordt de verzendprijs aangegeven die aan de aanbieding is toegevoegd.
- Aanlandingsprijs: Hiermee wordt de aanbiedingsprijs plus de verzendprijs voor de aanbieding aangegeven.
- Laatst bijgewerkt: Geeft de datum en tijd aan waarop de prijsinformatie van Amazon is bijgewerkt.

![Productaanbiedingsgegevens: Buy Box concurrent](assets/amazon-listing-details-buy-box-2.png){width="600" zoomable="yes"}

## Laagste prijsstelling voor concurrenten {#lowest-competitor-pricing}

Op dit tabblad wordt informatie weergegeven over Amazon-concurrenten voor dezelfde aanbieding. Deze informatie kan worden gebruikt om prijsstelling te begrijpen en [laagste prijsstelling voor concurrenten](./lowest-competitor-pricing.md). De getoonde informatie omvat:

- ASIN: De 10-cijferige Amazon product identifier.
- Voorwaarde: Hiermee wordt de gedefinieerde voorwaarde voor de aanbieding aangegeven.
- Fulfillment Channel: Identificeert de partij die verantwoordelijk is voor naleving. Opties: Merchant/Amazon.
- Aanbiedingsprijs: Hiermee wordt de prijs aangegeven waartegen de aanbieding is gepubliceerd.
- Verzendprijs: Hiermee wordt de verzendprijs aangegeven die aan de aanbieding is toegevoegd.
- Aanlandingsprijs: Hiermee wordt de aanbiedingsprijs plus de verzendprijs voor de aanbieding aangegeven.
- Feedbackscore: Identificeert de Amazon-feedbackscore voor de laagste prijs.
- Aantal feedback: Hiermee wordt de Amazon-feedbacktelling aangegeven voor de laagste prijs.
- Laatst bijgewerkt: Geeft de datum en tijd aan waarop de prijsinformatie van Amazon is bijgewerkt.

![Gegevens over productlijsten - laagste prijsstelling voor concurrenten](assets/amazon-listing-details-lowest-comp.png){width="600" zoomable="yes"}
