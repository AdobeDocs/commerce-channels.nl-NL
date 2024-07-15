---
title: Amazon-verkoopkanaal - [!UICONTROL Ready to List]
description: Het Amazon-verkoopkanaal biedt het tabblad Ready to List om u te helpen Commerce-producten te bekijken die wel aan de voorwaarden voldoen, maar niet automatisch worden vermeld.
feature: Sales Channels, Products, Merchandising
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

Het _[!UICONTROL Ready to List]_lusje toont uw [!DNL Commerce] catalogusproducten die uw lijstmontages voldoen en aan Amazon als a **nieuwe**lijst bereid zijn te publiceren. In tegenstelling tot andere tabbladen wordt dit tabblad niet altijd weergegeven op de pagina [_[!UICONTROL Product Listings]_](./managing-product-listings.md) .

Het tabblad _[!UICONTROL Ready to List]_wordt alleen weergegeven wanneer [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in de aanbiedingsinstellingen is ingesteld op `Do Not Automatically List Eligible Products` . Deze instelling vertelt Amazon-verkoopkanaal dat nieuwe Amazon-aanbiedingen handmatig moeten worden gepubliceerd.

Wanneer [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) is ingesteld op `Automatically List Eligible Products` , publiceert Amazon Verkoopkanaal automatisch nieuwe aanbiedingen voor in aanmerking komende catalogusproducten. Omdat nieuwe aanbiedingen automatisch worden gepubliceerd, wordt het tabblad _[!UICONTROL Ready to List]_niet weergegeven.

Onder _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: kies ervoor de vermelding opnieuw te publiceren naar de [!DNL Amazon Marketplace] . Zie [ Publish en Amazon die ](./publish-listings-manually.md) van een lijst voorzien

Onder **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_:

- **[!UICONTROL Publish On Amazon]**: kies ervoor de vermelding opnieuw te publiceren naar de [!DNL Amazon Marketplace] . Zie [ Publish en Amazon die ](./publish-listings-manually.md) van een lijst voorzien.

- **[!UICONTROL View Details]**: verkies om lijstdetails, met inbegrip van het [ Lijst Logboek van de Activiteit ](./product-listing-details.md#listing-activity-log) te bekijken, [ het Prijstarief van de Mededinger van de Buy Box ](./product-listing-details.md#buy-box-competitor-pricing), en [ Laagste Prijsverhoging van de Concurrent ](./product-listing-details.md#lowest-competitor-pricing). Deze handeling is alleen bedoeld voor weergave. De details van de aanbieding kunnen niet worden gewijzigd. Zie [ Details van de Mening ](./product-listing-details.md).

U hebt een paar opties om een nieuwe lijst aan Amazon ](./publish-listings-manually.md) manueel te publiceren. [

>[!NOTE]
>Als je aanbiedingen in behandeling hebt, wordt het aantal aanbiedingen weergegeven in een bericht boven de tabbladen.

![ Klaar aan lijst ](assets/amazon-ready-to-list.png){width="600" zoomable="yes"}

## Standaardkolommen

| Kolom | Beschrijving |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br> ASIN staat voor [!DNL Amazon Standard Identification Number]. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Condition] | De [ voorwaarde ](./product-listing-condition.md) van het product. |
| [!UICONTROL Landed Price] | De prijs van de aanbieding voor het product plus de verzendprijs. |
| [!UICONTROL Amazon Quantity] | De hoeveelheid die beschikbaar is wanneer het product actief op Amazon wordt aangeboden. |
| [!UICONTROL Status] | De status van de aanbieding, gedefinieerd door Amazon. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_en kiest u een optie:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Algemene oorzaken van aanbiedingen die je kunt aanbieden

- **[!UICONTROL Ready to List]** - Het product komt overeen met een Amazon ASIN en is gepland voor aanbieding. Als [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in de aanbiedingsinstellingen is ingesteld op `Do Not Automatically List Eligible Products` , vertegenwoordigt deze status de producten die klaar zijn om handmatig te worden vermeld.

- **[!UICONTROL List in Progress]** - De productaanbieding is naar Amazon verzonden en wacht op acceptatie door Amazon.
