---
title: Kenmerken voor Amazon-aanbiedingen beheren
description: U kunt de toewijzing van de productkenmerken van de Handel aan de attributen van Amazon beheren om nauwkeurige productinformatie tussen de systemen te verzekeren.
feature: Sales Channels, Products, Configuration
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Kenmerken voor Amazon-aanbiedingen beheren

Amazon en [!DNL Commerce] beide gebruiken een systeem van producteigenschappen, die als attributen worden bekend, die worden gebruikt om een product te bepalen. Met kenmerken worden de beschrijving, inhoud, afbeeldingen, prijzen en verschillende gegevens voor uw producten gedefinieerd.

Een geslaagde communicatie tussen Handel en Amazon vereist dat [!DNL Commerce] attributen correct worden toegewezen (of aangepast) aan het overeenkomstige Amazon-kenmerk. Bij integratie met Amazon wijst u deze kenmerken toe aan Amazon-kenmerken. Wanneer voltooid, [!DNL Commerce] kan je Amazon-aanbiedingen synchroniseren en onderhouden met je [!DNL Commerce] productcatalogus.

Stel dat u hetzelfde item in uw [!DNL Commerce] catalogusobjecten en Amazon-aanbiedingen. Eén kenmerk voor het product kan de prijs van de aanbieding van het object zijn. De naam van de aanbiedingsprijs in [!DNL Commerce] zou kunnen worden genoemd `Price`, terwijl de aanbiedingsprijs voor Amazon een naam kan krijgen `ListingPrice`. U moet opdracht geven [!DNL Commerce] dat bij de communicatie met Amazon [!DNL Commerce] kenmerk benoemd `Price` is hetzelfde als het benoemde Amazon-kenmerk `ListingPrice`. Dit proces wordt _beheren, kenmerken_ en omvat het maken van nieuwe en het bewerken van bestaande kenmerken. Ervoor zorgen dat de kenmerken op de juiste wijze overeenkomen, zorgt voor een correcte communicatie tussen [!DNL Commerce] en Amazon.

Wanneer kenmerktoewijzing is ingesteld, [!DNL Commerce] kan productinformatie op en neer met Amazon communiceren. Als je aanbiedingen voor Amazon-producten hebt, [!DNL Commerce] kunt u Amazon-producten en -gegevens importeren in uw [!DNL Commerce] catalogus, zodat je je Amazon-aanbiedingen kunt beheren vanuit één centrale productcatalogus.

Met Amazon-verkoopkanaal hebt u toegang tot kenmerken in het dialoogvenster [_[!UICONTROL Attributes]_weergave](./attributes-view.md) op de homepage van het verkoopkanaal van Amazon. Als u een kenmerk aan uw [!DNL Commerce] catalogiseren, kan het een update van die waarden over alle producten vereisen.

Meer informatie over [!DNL Commerce] en Amazon-kenmerksets en -waarden, zie:

- [Grondbeginselen van kenmerken beheren](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [Een kenmerk maken](./creating-attributes.md#create-an-attribute)
- [Een bestaand kenmerk bewerken](./creating-attributes.md#edit-an-attribute)
- [Kenmerktoewijzing weergeven](./amazon-matching-attributes-values.md)
- [Kenmerktoewijzing bewerken of maken](./amazon-manually-update-incomplete-listing.md)
