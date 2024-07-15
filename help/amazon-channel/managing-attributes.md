---
title: Kenmerken voor Amazon-aanbiedingen beheren
description: U kunt de toewijzing van Commerce-productkenmerken aan de Amazon-kenmerken beheren om te zorgen voor nauwkeurige productinformatie tussen de systemen.
feature: Sales Channels, Products, Configuration
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Kenmerken voor Amazon-aanbiedingen beheren

Amazon en [!DNL Commerce] gebruiken allebei een systeem van producteigenschappen, die als attributen worden bekend, die worden gebruikt om een product te bepalen. Met kenmerken worden de beschrijving, inhoud, afbeeldingen, prijzen en verschillende gegevens voor uw producten gedefinieerd.

Voor een geslaagde communicatie tussen Commerce en Amazon moeten [!DNL Commerce] -kenmerken correct worden toegewezen (of overeenkomen) aan het overeenkomstige Amazon-kenmerk. Bij integratie met Amazon wijst u deze kenmerken toe aan Amazon-kenmerken. Wanneer deze bewerking is voltooid, kan [!DNL Commerce] uw Amazon-aanbiedingen synchroniseren en onderhouden met uw productcatalogus van [!DNL Commerce] .

Stel dat je hetzelfde object in je catalogus van [!DNL Commerce] en in Amazon-aanbiedingen hebt. Eén kenmerk voor het product kan de prijs van de aanbieding van het object zijn. De naam van de aanbiedingsprijs in [!DNL Commerce] kan `Price` worden genoemd, terwijl de aanbiedingsprijs voor Amazon een naam kan hebben `ListingPrice` . U moet [!DNL Commerce] de instructie geven dat wanneer u communiceert met Amazon, het kenmerk [!DNL Commerce] named `Price` hetzelfde is als het kenmerk Amazon met de naam `ListingPrice` . Dit proces wordt genoemd _het leiden attributen_, en omvat het creëren van nieuwe en het uitgeven van bestaande attributen. Als u ervoor zorgt dat de kenmerken juist overeenkomen, zorgt u voor een juiste communicatie tussen [!DNL Commerce] en Amazon.

Wanneer kenmerktoewijzing is ingesteld, kan [!DNL Commerce] productinformatie op en neer met Amazon communiceren. Als u Amazon-productaanbiedingen hebt, kunt u in [!DNL Commerce] uw Amazon-producten en -gegevens importeren in uw [!DNL Commerce] -catalogus, zodat u uw Amazon-aanbiedingen kunt beheren vanuit één centrale productcatalogus.

Met Amazon-verkoopkanalen hebt u toegang tot kenmerken in de [_[!UICONTROL Attributes]_weergave ](./attributes-view.md) op de homepage van het Amazon-verkoopkanaal en kunt u deze zo nodig bekijken, maken en beheren. Als u een attribuut aan uw [!DNL Commerce] catalogus toevoegt, zou het een update van die waarden over alle producten kunnen vereisen.

Zie voor meer informatie over [!DNL Commerce] - en Amazon-kenmerksets en -waarden:

- [ beheert attributengrondbeginselen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [Een kenmerk maken](./creating-attributes.md#create-an-attribute)
- [Een bestaand kenmerk bewerken](./creating-attributes.md#edit-an-attribute)
- [Kenmerktoewijzing weergeven](./amazon-matching-attributes-values.md)
- [Kenmerktoewijzing bewerken of maken](./amazon-manually-update-incomplete-listing.md)
