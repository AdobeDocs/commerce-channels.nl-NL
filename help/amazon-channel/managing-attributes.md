---
title: Kenmerken beheren
description: U kunt de toewijzing van de productkenmerken van de Handel aan de attributen van Amazon beheren om nauwkeurige productinformatie tussen de systemen te verzekeren.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Kenmerken beheren

Amazon en [!DNL Commerce] gebruiken allebei een systeem van producteigenschappen, die als attributen worden bekend, die worden gebruikt om een product te bepalen. Met kenmerken worden de beschrijving, inhoud, afbeeldingen, prijzen en verschillende gegevens voor uw producten gedefinieerd.

Voor geslaagde communicatie tussen Handel en Amazon moeten [!DNL Commerce]-kenmerken correct worden toegewezen (of aangepast) aan het overeenkomstige Amazon-kenmerk. Bij integratie met Amazon wijst u deze kenmerken toe aan Amazon-kenmerken. Als [!DNL Commerce] klaar is, kunt u uw Amazon-aanbiedingen synchroniseren en onderhouden met uw [!DNL Commerce]-productcatalogus.

Stel dat u hetzelfde item in uw [!DNL Commerce]-catalogus en in Amazon-aanbiedingen hebt. Eén kenmerk voor het product kan de prijs van de aanbieding van het object zijn. De naam voor de aanbiedingsprijs in [!DNL Commerce] kan `Price` worden genoemd, terwijl de aanbiedingsprijs voor Amazon `ListingPrice` kan worden genoemd. U moet [!DNL Commerce] instrueren dat wanneer het communiceren met Amazon, [!DNL Commerce] attribuut genoemd `Price` het zelfde als het attribuut van Amazon genoemd `ListingPrice` is. Dit proces wordt _het beheren van attributen_ genoemd, en omvat het creëren van nieuwe en het uitgeven van bestaande attributen. Als u ervoor zorgt dat de kenmerken op de juiste wijze overeenkomen, zorgt u voor de juiste communicatie tussen [!DNL Commerce] en Amazon.

Wanneer kenmerktoewijzing is ingesteld, kan [!DNL Commerce] productinformatie op en neer met Amazon communiceren. Als u Amazon-productaanbiedingen hebt, kunt [!DNL Commerce] uw Amazon-producten en -gegevens importeren in uw [!DNL Commerce]-catalogus, zodat u uw Amazon-aanbiedingen kunt beheren vanuit één centrale productcatalogus.

Met het Amazon-verkoopkanaal hebt u toegang tot kenmerken in de [_[!UICONTROL Attributes]_-weergave](./attributes-view.md) op de startpagina van het Amazon-verkoopkanaal en kunt u deze kenmerken naar wens bekijken, bekijken, maken en beheren. Als u een attribuut aan uw [!DNL Commerce] catalogus toevoegt, zou het een update van die waarden over alle producten kunnen vereisen.

Zie voor meer informatie over [!DNL Commerce] en Amazon-kenmerksets en -waarden:

- [De grondbeginselen](https://docs.magento.com/user-guide/catalog/product-attributes.html) van kenmerken beheren{target=&quot;_blank&quot;}
- [Een kenmerk maken](./creating-attributes.md#create-an-attribute)
- [Een bestaand kenmerk bewerken](./creating-attributes.md#edit-an-attribute)
- [Kenmerktoewijzing weergeven](./amazon-matching-attributes-values.md)
- [Kenmerktoewijzing bewerken of maken](./amazon-manually-update-incomplete-listing.md)
