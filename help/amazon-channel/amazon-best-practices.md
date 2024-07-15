---
title: Aanbevolen werkwijzen en beperkingen voor  [!DNL Amazon sales channel]
description: Bekijk de beste praktijken en beperkingen wanneer het gebruiken van het verkoopkanaal van Amazon voor Adobe Commerce en Magento Open Source.
role: Leader, Admin, User
feature: Sales Channels, Best Practices
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Aanbevolen werkwijzen en beperkingen voor [!DNL Amazon sales channel]

De beste praktijken omvatten:

- Het verkoopkanaal van Amazon kan je Amazon-aanbiedingen beïnvloeden door de prijzen te verhogen of te verlagen, de productinformatie te synchroniseren (inclusief beschikbare voorraad) en aanbiedingen toe te voegen, bij te werken en te beëindigen (verwijderen). Herzie uw lijsten door status tijdens uw opstelling en pas uw montages ([ lijst van montages ](./listing-settings.md) aan, [ lijst regels ](./listing-rules.md), [ het tarief regels ](./pricing-products.md), [ met voeten treedt ](./overrides.md), etc.) alvorens uw opslagopstelling te voltooien. Deze instellingen kunnen desgewenst ook na de installatie worden gewijzigd.

- Verkoopkanaal van Amazon kan je prijsregels zodanig instellen dat je de objectprijs automatisch aanpast. De geautomatiseerde tarifering beschermt omvat de [ vloerprijs ](./floor-price.md) en [ facultatieve plafondprijs ](./optional-ceiling-price.md) eigenschappen van [ Intelligente het opnieuw bepalen regels ](./intelligent-repricing-rules.md). Met deze voorzorgsmaatregelen kun je ervoor zorgen dat je aanbiedingsprijzen niet onder je kosten of boven een bepaalde prijs liggen.

- Het synchroniseren van gegevens tussen het verkoopkanaal van Amazon en Amazon wordt gecontroleerd door uw [[!DNL Commerce]  kron ](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) montages. De ingebouwde vertraging tussen [!DNL Commerce] en Amazon helpt een vloeiende en efficiënte gegevenstransmissie te garanderen, maar tijdens de hoge tijden van eCommerce-verkeer (zoals Zwarte Vrijdag) kan het langer duren dan normaal om Amazon-systemen bij te werken. Stel de [!DNL Commerce] -uitsnede in zodat deze elke vijf minuten wordt uitgevoerd.

- Amazon-verkoopkanaal importeert uw Amazon-ordergegevens. Om uw orden van Amazon in Amazon verkoopkanaal te beheren, moet u ervoor zorgen dat uw [ ordemontages ](./order-settings.md) worden bepaald om een overeenkomstige [!DNL Commerce] orde voor elke orde van Amazon in te voeren en tot stand te brengen. Als deze niet is gedefinieerd, kunt u alleen de Amazon-ordergegevens bekijken. Alle BTW voor verkopen via Amazon worden nog steeds beheerd en kwijtgescholden via je [!DNL Amazon Seller Central] -account. In sommige landen is Amazon verplicht om automatisch belastingen te innen en terug te betalen. In andere staten kunnen verkopers de belastingen handmatig of automatisch berekenen. Zie [ Amazon: Belastingsbeleid ](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/) {target="_blank"}. Mogelijk moet u zich aanmelden bij uw [!DNL Amazon Seller Central] -account om de documentatie over het belastingbeleid van Amazon weer te geven.

- Voor de gebieden van het VK, is het beste praktijken om in de [ Dienst van de Berekening van de BTW Amazon ](https://sell.amazon.co.uk/learn/vat-resources/) {target="_blank"} vóór het aan boord gaan van Amazon verkoopkanaal in te schrijven.

  >[!NOTE]
  >
  >Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

De beperkingen omvatten:

- Pakket-, cadeaukaart- en gegroepeerde producttypen die onderdeel zijn van uw catalogus van [!DNL Commerce] , worden niet ondersteund door Amazon voor aanbiedingen naar Amazon.

- Verkoopkanaal van Amazon kan geen aanbieding maken voor een product dat geen bestaande of vorige Amazon-aanbieding heeft. Als een product niet bestaat in [!DNL Amazon Seller Central] met een ASIN, moet het worden toegevoegd in [!DNL Amazon Seller Central] zodat Amazon het product een ASIN kan toewijzen. Nadat een product in Amazon is toegevoegd en een aanbieding is gemaakt, kan de aanbieding via Amazon worden aangepast aan uw catalogus en worden gesynchroniseerd.
