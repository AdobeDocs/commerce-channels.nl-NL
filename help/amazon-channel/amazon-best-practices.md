---
title: Beste werkwijzen en beperkingen voor [!DNL Amazon sales channel]
description: Bekijk de beste praktijken en beperkingen wanneer het gebruiken van het verkoopkanaal van Amazon voor Adobe Commerce en Magento Open Source.
role: Leader, Admin, User
feature: Sales Channels, Best Practices
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Beste werkwijzen en beperkingen voor [!DNL Amazon sales channel]

De beste praktijken omvatten:

- Het verkoopkanaal van Amazon kan je Amazon-aanbiedingen beïnvloeden door de prijzen te verhogen of te verlagen, de productinformatie te synchroniseren (inclusief beschikbare voorraad) en aanbiedingen toe te voegen, bij te werken en te beëindigen (verwijderen). Je aanbiedingen bekijken op status tijdens je installatie en je instellingen aanpassen ([aanbiedingsinstellingen](./listing-settings.md), [aanbiedingsregels](./listing-rules.md), [prijsregels](./pricing-products.md), [overschrijvingen](./overrides.md), enzovoort) voordat u de installatie van de winkel hebt voltooid. Deze instellingen kunnen desgewenst ook na de installatie worden gewijzigd.

- Verkoopkanaal van Amazon kan je prijsregels zodanig instellen dat je de objectprijs automatisch aanpast. De geautomatiseerde prijswaarborgen omvatten [bodemprijs](./floor-price.md) en [facultatieve maximumprijs](./optional-ceiling-price.md) kenmerken van [Intelligente prijsstellingsregels](./intelligent-repricing-rules.md). Met deze voorzorgsmaatregelen kun je ervoor zorgen dat je aanbiedingsprijzen niet onder je kosten of boven een bepaalde prijs liggen.

- Gegevenssynchronisatie tussen Amazon-verkoopkanaal en Amazon wordt beheerd door uw [[!DNL Commerce] kraan](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) instellingen. Ingebouwde vertraging tussen [!DNL Commerce] en Amazon draagt bij aan een soepele en efficiënte gegevensoverdracht, maar bij hoge eCommerce-tijden (zoals de Zwarte Vrijdag) kan het langer duren dan gewoonlijk om Amazon-systemen bij te werken. Stel uw [!DNL Commerce] kroon om de vijf minuten te draaien.

- Amazon-verkoopkanaal importeert uw Amazon-ordergegevens. Als u uw Amazon-bestellingen in Amazon wilt beheren, moet u ervoor zorgen dat uw [orderinstellingen](./order-settings.md) zijn gedefinieerd voor het importeren en maken van een overeenkomende [!DNL Commerce] volgorde voor elke Amazon-bestelling. Als deze niet is gedefinieerd, kunt u alleen de Amazon-ordergegevens bekijken. Alle verkoopbelastingen via Amazon worden nog steeds beheerd en kwijtgescholden via je [!DNL Amazon Seller Central] account. In sommige landen is Amazon verplicht om automatisch belastingen te innen en terug te betalen. In andere staten kunnen verkopers de belastingen handmatig of automatisch berekenen. Zie [Amazon: Belastingbeleid](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}. Mogelijk moet u zich aanmelden bij uw [!DNL Amazon Seller Central] -account om de documentatie over het belastingbeleid van Amazon te bekijken.

- Voor Britse regio&#39;s is het de beste praktijk om zich in te schrijven in de [Amazon BTW-berekeningsservice](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} voordat het verkoopkanaal van Amazon wordt ingeschakeld.

  >[!NOTE]
  >
  >Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

De beperkingen omvatten:

- Bundel, cadeaukaart en gegroepeerde producttypen die deel uitmaken van uw [!DNL Commerce] De catalogus wordt niet ondersteund door het verkoopkanaal van Amazon voor aanbiedingen naar Amazon.

- Verkoopkanaal van Amazon kan geen aanbieding maken voor een product dat geen bestaande of vorige Amazon-aanbieding heeft. Als een product niet bestaat in [!DNL Amazon Seller Central] met een ASIN, moet het worden toegevoegd in [!DNL Amazon Seller Central] zodat Amazon het product een ASIN kan toewijzen. Nadat een product in Amazon is toegevoegd en een aanbieding is gemaakt, kan de aanbieding via Amazon worden aangepast aan uw catalogus en worden gesynchroniseerd.
