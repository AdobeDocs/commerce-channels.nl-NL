---
title: Bestellingen beheren
description: U kunt het importeren van bestellingen inschakelen in uw Orderinstellingen om uw Amazon-bestellingen eenvoudiger te beheren via uw Commerce Admin.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Bestellingen beheren

U kunt de Amazon-ordergegevens die u van Amazon hebt ontvangen, weergeven in de sectie _[!UICONTROL Recent Orders]_van het [opslagdashboard](./amazon-store-dashboard.md) of op de pagina_[!UICONTROL Amazon orders]_ (ook wel de _[!UICONTROL All Orders]_-weergave genoemd).

Hoe u uw Amazon-bestellingen beheert, hangt af van het feit of het importeren van bestellingen is in- of uitgeschakeld in uw [Order Settings](./order-settings.md#configure-order-settings).

## Importeren van volgorde ingeschakeld

Na [store integration](./store-integration.md), is [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) het plaatsen `Enabled` door gebrek. Met dit plaatsen, worden de overeenkomstige [!DNL Commerce] orden gecreeerd voor uw orden van Amazon en kunnen in [[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html) {target= &quot;_blank&quot;} werkschema worden beheerd.

>[!NOTE]
>
>Ongeacht de instellingen voor het importeren van uw bestelling, worden Amazon-bestellingen die vóór uw [store-integratie](./store-integration.md) in uw [!DNL Amazon Seller Central]-account bestonden, niet geïmporteerd.

Geïmporteerde Amazon-orders worden in de workflow [[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} beheerd, net als in uw andere [!DNL Commerce]-winkels. Klik het de ordeaantal van Amazon in *[!UICONTROL Order Number]* kolom om de orde in [[!DNL Commerce] ordeproces](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;} te openen. Zie [Amazon-bestellingen weergeven](./amazon-orders-all.md).

### Importproces bestellen

Wanneer een orde op Amazon wordt geplaatst en [orde wordt de invoer ](./order-settings.md) toegelaten, begint het volgende proces.

| Wijzigen | Handelingen |
|---|---|
| Er wordt een bestelling geplaatst op Amazon. | <ul><li>Amazon stelt de orderstatus in op `Pending`.</li><li>Ordergegevens worden verzonden naar [!DNL Commerce].</li><li>De orde wordt toegevoegd aan [_Amazon orden_ lijst](./amazon-orders-all.md) met een `Pending` status.</li></ul> |
| Amazon wijzigt de orderstatus in `Unshipped`. | <ul><li>De statuswijziging wordt verzonden naar [!DNL Commerce].</li><li>In [_Amazon orders_ table](./amazon-orders-all.md), verandert de ordestatus in `Unshipped`.</li><li>In [[!DNL Commerce] orders workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} wordt een corresponderende [!DNL Commerce] volgorde gemaakt met een `Processing` status.</li></ul> |
| In [[!DNL Commerce] orders workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} wordt de [!DNL Commerce] volgorde verwerkt en verandert de status in `Shipped`. | <ul><li>In [_Amazon orders_ table](./amazon-orders-all.md), verandert de ordestatus in `Shipped`.</li><li>Bij de volgende uitsnijdtaak verandert de orderstatus in `Complete` in de [[!DNL Commerce] orderworkflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}.</li></ul> |

### Blokkeringen voor het maken van orders

Er zijn een paar scenario&#39;s die de verwezenlijking van de overeenkomstige [!DNL Commerce] orde verhinderen. [!DNL Commerce] orders worden niet gemaakt voor orders die worden ontvangen wanneer zich een van de volgende problemen voordoet.

| Scenario | Oplossing |
|---|---|
| Het item bestaat niet in de catalogus [!DNL Commerce]. | [Maak het ](./creating-assigning-catalog-products.md) product van uw  [!DNL Commerce] catalogus en  [pas het ](./creating-assigning-catalog-products.md) product handmatig aan. |
| Het item in de catalogus is uitgeschakeld. | Zorg ervoor dat de [productstatus](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;} is ingeschakeld. |
| Het geordende item is uit voorraad. | Werk of vorm [productopties ](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;} voor hoeveelheid en bron bij. |

Wanneer orders niet kunnen worden geïmporteerd, verschijnt een systeembericht zoals hieronder boven in het scherm:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Wanneer het probleem is opgelost, wordt de volgorde [!DNL Commerce] bij de volgende synchronisatie gemaakt.

## Importeren met volgorde uitgeschakeld

Als u uw Amazon-orders niet wilt importeren en beheren in [!DNL Commerce], kunt u de instelling [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) wijzigen in `Disabled`. Deze instelling betekent dat wanneer nieuwe orders worden ontvangen van Amazon, er geen corresponderende [!DNL Commerce]-orders worden gemaakt.

Als deze optie is uitgeschakeld, worden de ordergegevens die u van Amazon hebt ontvangen, weergegeven in de sectie _[!UICONTROL Recent Orders]_van het opslagdashboard en in de weergave_[!UICONTROL All Orders]_. Deze ordegegevens zijn alleen-weergeven en u moet deze bestellingen beheren in [!DNL Amazon Seller Central]. Als u de ordergegevens in [!DNL Amazon Seller Central] wilt openen, klikt u op het Amazon-ordernummer in de kolom _[!UICONTROL Order Number]_.

Zie ook [Amazon-bestellingen weergeven](./amazon-orders-all.md), [Amazon-bestellingsgegevens weergeven](./amazon-order-details.md) en [Algemene taken voor het verwerken van bestellingen](./common-order-processing.md).
