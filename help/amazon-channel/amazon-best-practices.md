---
title: Beste praktijken en Beperkingen voor het verkoopkanaal van Amazon
description: Bekijk de beste praktijken en beperkingen wanneer het gebruiken van het verkoopkanaal van Amazon voor de Handel van Adobe en Magento Open Source.
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Aanbevolen werkwijzen en beperkingen voor Amazon-verkoopkanalen

De beste praktijken omvatten:

- Het verkoopkanaal van Amazon kan je Amazon-aanbiedingen beïnvloeden door de prijzen te verhogen of te verlagen, de productinformatie te synchroniseren (inclusief beschikbare voorraad) en aanbiedingen toe te voegen, bij te werken en te beëindigen (verwijderen). Controleer uw aanbiedingen op status tijdens de installatie en pas uw instellingen aan ([aanbiedingsinstellingen](./listing-settings.md), [aanbiedingsregels](./listing-rules.md), [prijsregels](./pricing-products.md), [overschrijvingen](./overrides.md) enzovoort) voordat u de installatie van uw winkel voltooit. Deze instellingen kunnen desgewenst ook na de installatie worden gewijzigd.

- Verkoopkanaal van Amazon kan je prijsregels zodanig instellen dat je de objectprijs automatisch aanpast. De geautomatiseerde prijswaarborgen omvatten [vloerprijs](./floor-price.md) en [facultatieve plafondprijs](./optional-ceiling-price.md) eigenschappen van [Intelligente repricing rules](./intelligent-repricing-rules.md). Met deze voorzorgsmaatregelen kun je ervoor zorgen dat je aanbiedingsprijzen niet onder je kosten of boven een bepaalde prijs liggen.

- Gegevenssynchronisatie tussen Amazon-verkoopkanaal en Amazon wordt beheerd door uw [[!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;} instellingen. De ingebouwde vertraging tussen [!DNL Commerce] en Amazon draagt bij aan een soepele en efficiënte gegevensoverdracht, maar tijdens de hoge tijden van eCommerce-verkeer (zoals Zwarte Vrijdag) kan het langer duren dan gewoonlijk om de systemen van Amazon bij te werken. Stel uw [!DNL Commerce] uitsnede in zodat deze elke vijf minuten wordt uitgevoerd.

- Amazon-verkoopkanaal importeert uw Amazon-ordergegevens. Als u uw Amazon-orders in Amazon-verkoopkanalen wilt beheren, moet u ervoor zorgen dat uw [orderinstellingen](./order-settings.md) zijn gedefinieerd voor het importeren en maken van een corresponderende [!DNL Commerce]-volgorde voor elke Amazon-order. Als deze niet is gedefinieerd, kunt u alleen de Amazon-ordergegevens bekijken. Alle verkoopkosten via Amazon worden nog steeds beheerd en via uw [!DNL Amazon Seller Central]-account kwijtgescholden. In sommige landen is Amazon verplicht om automatisch belastingen te innen en terug te betalen. In andere staten kunnen verkopers de belastingen handmatig of automatisch berekenen. Zie [Amazon: Belastingsbeleid](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target=&quot;_blank&quot;}. Mogelijk moet u zich aanmelden bij uw [!DNL Amazon Seller Central]-account om de documentatie over het belastingbeleid van Amazon weer te geven.

- Voor Britse regio&#39;s, is het beste praktijken om in [de Dienst van de Berekening van de BTW van Amazon ](https://sell.amazon.co.uk/learn/vat-resources/){target=&quot;_blank&quot;} vóór aan boord het verkoopkanaal van Amazon te inschrijven.


   >[!NOTE]
   >
   >Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

De beperkingen omvatten:

- Bundel, cadeaukaart en gegroepeerde producttypen die deel uitmaken van uw [!DNL Commerce]-catalogus, worden niet ondersteund door Amazon-verkoopkanaal voor aanbieding aan Amazon.

- Verkoopkanaal van Amazon kan geen aanbieding maken voor een product dat geen bestaande of vorige Amazon-aanbieding heeft. Als een product niet in [!DNL Amazon Seller Central] met een ASIN bestaat, moet het in [!DNL Amazon Seller Central] worden toegevoegd zodat Amazon het product een ASIN kan toewijzen. Nadat een product in Amazon is toegevoegd en een aanbieding is gemaakt, kan de aanbieding via Amazon worden aangepast aan uw catalogus en worden gesynchroniseerd.
