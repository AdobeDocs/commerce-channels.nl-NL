---
title: Amazon-orders beheren
description: U kunt het importeren van bestellingen inschakelen in uw Order Settings om uw Amazon-bestellingen eenvoudiger te beheren vanuit uw Commerce Admin.
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Amazon-orders beheren

U kunt uw de ordeinformatie van Amazon bekijken, zoals die van Amazon, in de _[!UICONTROL Recent Orders]_sectie van het [ opslagdashboard ](./amazon-store-dashboard.md) of op de_[!UICONTROL Amazon orders]_ pagina (ook genoemd de _[!UICONTROL All Orders]_mening) wordt ontvangen.

Hoe u uw orden van Amazon beheert hangt af van of de ordeinvoer of gehandicapt in uw [ Montages van de Orde ](./order-settings.md#configure-order-settings) wordt toegelaten.

## Importeren van volgorde ingeschakeld

Na [ opslagintegratie ](./store-integration.md), is het [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) plaatsen `Enabled` door gebrek. Met dit het plaatsen, wordt de overeenkomstige [!DNL Commerce] orden gecreeerd voor uw orden van Amazon en kan in het [[!DNL Commerce]  Orders ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) werkschema worden beheerd.

>[!NOTE]
>
>Ongeacht uw orde voert montages in, de orden van Amazon die in uw [!DNL Amazon Seller Central] rekening vóór uw [ opslagintegratie ](./store-integration.md) bestonden worden niet ingevoerd.

De ingevoerde orden van Amazon worden beheerd in het [[!DNL Commerce]  bevel ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) werkschema, enkel zoals uw andere [!DNL Commerce] opslag. Klik het de ordeaantal van Amazon in de *[!UICONTROL Order Number]* kolom om de orde in het [[!DNL Commerce]  ordeproces ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions) te openen. Zie {de Orden van Amazon van 0} Mening ](./amazon-orders-all.md).[

### Importproces bestellen

Wanneer een orde op Amazon wordt geplaatst en [ de ordeinvoer ](./order-settings.md) wordt toegelaten, begint het volgende proces.

| Wijzigen | Handelingen |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Er wordt een bestelling geplaatst op Amazon. | <ul><li>Amazon stelt de orderstatus in op `Pending` .</li><li>Bestandsgegevens worden verzonden naar [!DNL Commerce] .</li><li>De orde wordt toegevoegd aan [_Amazon orden_ lijst ](./amazon-orders-all.md) met een `Pending` status.</li></ul> |
| Amazon wijzigt de orderstatus in `Unshipped` . | <ul><li>De statuswijziging wordt verzonden naar [!DNL Commerce] .</li><li>In de [_orden van Amazon_ lijst ](./amazon-orders-all.md), verandert de ordestatus in `Unshipped`.</li><li>In het [[!DNL Commerce]  werkschema van orden ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), wordt een overeenkomstige [!DNL Commerce] orde gecreeerd met een `Processing` status.</li></ul> |
| In [[!DNL Commerce]  het werkschema van orden ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), wordt de [!DNL Commerce] orde verwerkt en de statusveranderingen in `Shipped`. | <ul><li>In de [_orden van Amazon_ lijst ](./amazon-orders-all.md), verandert de ordestatus in `Shipped`.</li><li>Op de volgende gezamenlijke baan, verandert de ordestatus in `Complete` in het [[!DNL Commerce]  werkschema van orden ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).</li></ul> |

### Blokkeringen voor het maken van orders

Er zijn een paar scenario&#39;s die het creëren van de overeenkomstige [!DNL Commerce] orde verhinderen. [!DNL Commerce] orders worden niet gemaakt voor orders die worden ontvangen wanneer een van de volgende problemen optreedt.

| Scenario | Oplossing |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Het item bestaat niet in de catalogus van [!DNL Commerce] . | [ creeer het product ](./creating-assigning-catalog-products.md) in uw [!DNL Commerce] catalogus en [ aanpassen manueel ](./creating-assigning-catalog-products.md) het aan het product. |
| Het item in de catalogus is uitgeschakeld. | Zorg ervoor dat de [ productstatus ](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) wordt toegelaten. |
| Het geordende item is uit voorraad. | Werk of vorm de [ productopties ](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) voor hoeveelheid en bron bij. |

Wanneer orders niet kunnen worden geïmporteerd, verschijnt een systeembericht zoals hieronder boven in het scherm:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Wanneer het probleem is opgelost, wordt de volgorde [!DNL Commerce] gemaakt bij de volgende synchronisatie.

## Importeren met volgorde uitgeschakeld

Als u uw Amazon-orders niet wilt importeren en beheren in [!DNL Commerce] , kunt u de instelling [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) wijzigen in `Disabled` . Deze instelling houdt in dat wanneer nieuwe bestellingen worden ontvangen van Amazon, er geen overeenkomende [!DNL Commerce] -bestellingen worden gemaakt.

Als deze optie is uitgeschakeld, worden de ordergegevens die u van Amazon hebt ontvangen, weergegeven in de sectie _[!UICONTROL Recent Orders]_van het opslagdashboard en in de weergave_[!UICONTROL All Orders]_ . Deze volgordegegevens zijn alleen-weergeven en u moet deze bestellingen beheren in [!DNL Amazon Seller Central] . Als u de ordergegevens in [!DNL Amazon Seller Central] wilt openen, klikt u op het Amazon-ordernummer in de kolom _[!UICONTROL Order Number]_.

Zie ook {de Orden van Amazon van 0} Mening ](./amazon-orders-all.md), [ de Details van de Orde van Amazon van de Mening ](./amazon-order-details.md), en [ Gemeenschappelijke Taken van de Verwerking van de Orde ](./common-order-processing.md).[
