---
title: Amazon-orders beheren
description: U kunt het importeren van bestellingen inschakelen in uw Orderinstellingen om uw Amazon-bestellingen eenvoudiger te beheren via uw Commerce Admin.
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Amazon-orders beheren

U kunt uw Amazon-ordergegevens bekijken, zoals deze zijn ontvangen van Amazon, in het dialoogvenster _[!UICONTROL Recent Orders]_van de [opslagdashboard](./amazon-store-dashboard.md) of op de_[!UICONTROL Amazon orders]_ pagina (ook wel de _[!UICONTROL All Orders]_weergave).

Hoe u uw Amazon-bestellingen beheert, hangt af van het feit of het importeren van bestellingen in uw [Orderinstellingen](./order-settings.md#configure-order-settings).

## Importeren van volgorde ingeschakeld

Na [winkelintegratie](./store-integration.md)de [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) instellen is `Enabled` standaard. Met deze instelling komt deze overeen [!DNL Commerce] bestellingen worden gemaakt voor uw Amazon-bestellingen en kunnen worden beheerd in de [[!DNL Commerce] Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workflow.

>[!NOTE]
>
>Ongeacht de instellingen voor het importeren van uw bestelling, bestelt Amazon de bestellingen die in uw [!DNL Amazon Seller Central] account voor uw [winkelintegratie](./store-integration.md) niet worden geïmporteerd.

Geïmporteerde Amazon-orders worden beheerd in het dialoogvenster [[!DNL Commerce] Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workflow, net als uw andere [!DNL Commerce] winkels. Klik op het Amazon-ordernummer in het dialoogvenster *[!UICONTROL Order Number]* om de volgorde in de [[!DNL Commerce] orderproces](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions). Zie [Amazon-bestellingen weergeven](./amazon-orders-all.md).

### Importproces bestellen

Wanneer een order op Amazon wordt geplaatst en [orderimport](./order-settings.md) is ingeschakeld, wordt het volgende proces gestart.

| Wijzigen | Handelingen |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Er wordt een bestelling geplaatst op Amazon. | <ul><li>Amazon stelt de orderstatus in op `Pending`.</li><li>Bestelgegevens worden verzonden naar [!DNL Commerce].</li><li>Volgorde wordt toegevoegd aan [_Amazon-orders_ table](./amazon-orders-all.md) met een `Pending` status.</li></ul> |
| Amazon wijzigt de orderstatus in `Unshipped`. | <ul><li>De statuswijziging wordt verzonden naar [!DNL Commerce].</li><li>In de [_Amazon-orders_ table](./amazon-orders-all.md), verandert de orderstatus in `Unshipped`.</li><li>In de [[!DNL Commerce] orderwerkstroom](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), een overeenkomstige [!DNL Commerce] order wordt gemaakt met een `Processing` status.</li></ul> |
| In [[!DNL Commerce] orderwerkstroom](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)de [!DNL Commerce] bestelling wordt verwerkt en de status wordt gewijzigd in `Shipped`. | <ul><li>In de [_Amazon-orders_ table](./amazon-orders-all.md), verandert de orderstatus in `Shipped`.</li><li>Bij de volgende uitsnijdtaak verandert de orderstatus in `Complete` in de [[!DNL Commerce] orderwerkstroom](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).</li></ul> |

### Blokkeringen voor het maken van orders

Er zijn een paar scenario&#39;s die de verwezenlijking van overeenkomstige verhinderen [!DNL Commerce] bestelling. [!DNL Commerce] orders worden niet gemaakt voor orders die worden ontvangen wanneer zich een van de volgende problemen voordoet.

| Scenario | Oplossing |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Het item bestaat niet in het dialoogvenster [!DNL Commerce] catalogus. | [Het product maken](./creating-assigning-catalog-products.md) in uw [!DNL Commerce] catalogus en [handmatig afstemmen](./creating-assigning-catalog-products.md) aan het product. |
| Het item in de catalogus is uitgeschakeld. | Zorg ervoor dat de [productstatus](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) is ingeschakeld. |
| Het geordende item is uit voorraad. | Werk of vorm de [productopties](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) voor hoeveelheid en bron. |

Wanneer orders niet kunnen worden geïmporteerd, verschijnt een systeembericht zoals hieronder boven in het scherm:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Wanneer het probleem is opgelost, wordt [!DNL Commerce] volgorde wordt gemaakt bij de volgende synchronisatie.

## Importeren met volgorde uitgeschakeld

Als u uw Amazon-bestellingen niet wilt importeren en beheren in [!DNL Commerce]kunt u de [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) instellen op `Disabled`. Deze instelling houdt in dat wanneer nieuwe orders van Amazon worden ontvangen, de overeenkomstige [!DNL Commerce] bestellingen worden niet gemaakt.

Als deze optie is uitgeschakeld, worden de van Amazon ontvangen ordergegevens weergegeven in het dialoogvenster _[!UICONTROL Recent Orders]_in het winkeldashboard en in het_[!UICONTROL All Orders]_ weergeven. Deze bestelgegevens zijn alleen-weergeven en u moet deze bestellingen beheren in [!DNL Amazon Seller Central]. De ordergegevens openen in [!DNL Amazon Seller Central]klikt u op het Amazon-ordernummer in het dialoogvenster _[!UICONTROL Order Number]_kolom.

Zie ook [Amazon-bestellingen weergeven](./amazon-orders-all.md), [Bestelgegevens Amazon weergeven](./amazon-order-details.md), en [Algemene taken voor het verwerken van orders](./common-order-processing.md).
