---
title: Klaar voor lijst
description: Het verkoopkanaal van Amazon verstrekt Klaar aan Lijst tabel om u te helpen producten herzien van de Handel die aan geschiktheid maar niet automatisch vermeld zijn.
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

De _[!UICONTROL Ready to List]_tab geeft [!DNL Commerce] catalogusproducten die voldoen aan je aanbiedingsinstellingen en die klaar zijn om als een **new**aanbieding. In tegenstelling tot andere tabbladen wordt dit tabblad niet altijd weergegeven op de [_[!UICONTROL Product Listings]_](./managing-product-listings.md) pagina.

De _[!UICONTROL Ready to List]_wordt alleen weergegeven wanneer [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in je aanbieding zijn de instellingen ingesteld op `Do Not Automatically List Eligible Products`. Deze instelling vertelt Amazon-verkoopkanaal dat nieuwe Amazon-aanbiedingen handmatig moeten worden gepubliceerd.

Wanneer [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) is ingesteld op `Automatically List Eligible Products`verkoopkanaal van Amazon publiceert automatisch nieuwe aanbiedingen voor in aanmerking komende catalogusproducten. Omdat nieuwe aanbiedingen automatisch worden gepubliceerd, worden de _[!UICONTROL Ready to List]_wordt niet weergegeven.

Onder _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: Kies of u de aanbieding opnieuw wilt publiceren naar de [!DNL Amazon Marketplace]. Zie [Een Amazon-aanbieding publiceren](./publish-listings-manually.md)

Onder **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom:

- **[!UICONTROL Publish On Amazon]**: Kies of u de aanbieding opnieuw wilt publiceren naar de [!DNL Amazon Marketplace]. Zie [Een Amazon-aanbieding publiceren](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: Kies ervoor om de details van de aanbieding weer te geven, inclusief de [Logboek met aanbiedingsactiviteiten](./product-listing-details.md#listing-activity-log), [Prijsstelling voor Buy Box-concurrent](./product-listing-details.md#buy-box-competitor-pricing), en [Laagste concurrerende Prijs](./product-listing-details.md#lowest-competitor-pricing). Deze handeling is alleen bedoeld voor weergave. De details van de aanbieding kunnen niet worden gewijzigd. Zie [Details weergeven](./product-listing-details.md).

U hebt enkele opties om handmatig [een nieuwe aanbieding naar Amazon publiceren](./publish-listings-manually.md).

>[!NOTE]
>Als je aanbiedingen in behandeling hebt, wordt het aantal aanbiedingen weergegeven in een bericht boven de tabbladen.

![Klaar voor lijst](assets/amazon-ready-to-list.png)

## Standaardkolommen

| Kolom | Beschrijving |
|---|---|
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br>ASIN staat voor de [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Condition] | De [voorwaarde](./product-listing-condition.md) van het product. |
| [!UICONTROL Landed Price] | De prijs van de aanbieding voor het product plus de verzendprijs. |
| [!UICONTROL Amazon Quantity] | De hoeveelheid die beschikbaar is wanneer het product actief op Amazon wordt aangeboden. |
| [!UICONTROL Status] | De status van de aanbieding, gedefinieerd door Amazon. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom en kies een optie:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Algemene oorzaken van aanbiedingen die je wilt aanbieden

- **[!UICONTROL Ready to List]** - Het product komt overeen met een Amazon ASIN en is gepland voor aanbieding. Indien [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in je aanbieding zijn de instellingen ingesteld op `Do Not Automatically List Eligible Products`Deze status vertegenwoordigt de producten die klaar zijn om handmatig te worden vermeld.

- **[!UICONTROL List in Progress]** - De productaanbieding is naar Amazon verzonden en wacht op acceptatie door Amazon.
