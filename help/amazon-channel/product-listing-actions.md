---
title: Verkoopkanaal in Amazon - Handelingen voor productaanbiedingen
description: Met de instellingen voor acties voor aanbiedingen van producten kunt u bepalen hoe uw Commerce-catalogus reageert op Amazon.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Handelingen voor productaanbiedingen

De handelingsinstellingen voor productaanbiedingen maken deel uit van de aanbiedingsinstellingen van je winkel. De lijsten van montages worden betreden van het [ opslagdashboard ](./amazon-store-dashboard.md).

Met deze instellingen wordt gedefinieerd hoe uw catalogus reageert op Amazon. Deze instellingen:

- Geef aan of je catalogusproducten van [!DNL Commerce] die voldoen aan de Amazon-voorwaarden automatisch naar je [!DNL Amazon Seller Central] -account worden verzonden om aanbiedingen te maken.

- Stel de standaardverwerkingstijd voor een bestelling in. Deze waarde definieert het aantal dagen dat u nodig hebt om een bestelling te verwerken en te verzenden. Als iemand bijvoorbeeld 2-dagen verzending selecteert, begint de tijd van de verzending niet voordat de verwerking is voltooid en worden de pakketten aan een vervoerder overhandigd. De totale levertijd is (verwerkingstijd + doorvoertijd + feestdagen).

## Instellingen configureren

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Product Listing Actions]_uit.

1. Kies bij **[!UICONTROL Automatic List Action]** (vereist) een optie:

   - `Automatically List Eligible Products` - (Standaard) Kies wanneer u wilt dat uw catalogusproducten van [!DNL Commerce] (die voldoen aan de Amazon-voorwaarden om in aanmerking te komen) automatisch naar Amazon publiceren en Amazon-aanbiedingen maken.

   - `Do Not Automatically List Eligible Products` - Kies wanneer u handmatig in aanmerking komende catalogusproducten van [!DNL Commerce] wilt selecteren en Amazon-aanbiedingen wilt maken. Als je kiest, worden catalogusproducten die voldoen aan de criteria voor je aanbieding en die alle vereiste informatie bevatten, weergegeven op het tabblad [_[!UICONTROL Ready to List]_](./ready-to-list.md) voor handmatige publicatie naar Amazon.

1. Voer voor **[!UICONTROL Default Handling Time]** (vereist) het aantal dagen in dat nodig is voor de doorlooptijd vóór de verzending.

   De standaardwaarde is `2` dagen.

   >[!NOTE]
   >
   >Deze standaardwaarde voor de afhandelingstijd geldt alleen voor Amazon-aanbiedingen die via Amazon-verkoopkanalen zijn gemaakt. Amazon-aanbiedingen die zijn gemaakt in uw [!DNL Amazon Seller Central] -account, gebruiken de standaard verwerkingstijd die is ingesteld in Amazon.

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ de lijstacties van het Product acties ](assets/amazon-product-listing-actions.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Automatic List Action] | Opties:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Aanbevolen) Kies wanneer u wilt dat uw catalogusproducten van [!DNL Commerce] (die voldoen aan de Amazon-voorwaarden om in aanmerking te komen) automatisch naar Amazon publiceren en Amazon-aanbiedingen maken. Wanneer u deze optie kiest, wordt de tab [_[!UICONTROL Ready to List]_](./ready-to-list.md) niet weergegeven. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Kies wanneer u handmatig in aanmerking komende [!DNL Commerce] catalogusproducten wilt selecteren en Amazon-aanbiedingen wilt maken. Wanneer u een catalogus kiest die voldoet aan de criteria voor je aanbieding en die alle vereiste informatie bevat, worden deze op het tabblad [_[!UICONTROL Ready to List]_](./ready-to-list.md) weergegeven voor handmatig publiceren.</li></ul> |
| [!UICONTROL Default Handling Time] | De numerieke waarde die het aantal dagen vertegenwoordigt, in het algemeen, dat het u vergt om uw orden te verwerken en te verzenden. De standaardwaarde is `2` . Deze waarde wordt gebruikt voor Amazon-aanbiedingen die zijn gemaakt in [!DNL Commerce] en gepubliceerd naar Amazon. Deze instelling heeft geen invloed op de standaardverwerkingstijd voor Amazon-aanbiedingen voordat deze worden geïntegreerd met [!DNL Commerce] .<br><br> de waarde die in het verkoopkanaal van Amazon wordt bepaald vervangt niet de standaardbehandelingstijd die in een bestaande lijst van Amazon wordt bepaald. Wanneer een **[!UICONTROL Handling Time Override]** wordt toegelaten en dan verwijderd, keert de Behandelingstijd voor een orde aan de hier bepaalde waarde terug.<br><br> als u producten hebt die verschillende behandelingstijden hebben, kunt u een Behandelingstijd van de Tijd met voeten treden op het product-specifieke niveau tot stand brengen. U kunt overschrijvingen van de verwerkingstijd beheren op het tabblad [_[!UICONTROL Overrides]_](./overrides.md) , zodat u over voldoende flexibiliteit beschikt om de naleving van uw product te beheren. Als [!DNL Commerce] voor een product geen verwerkingstijd overschrijft, is de standaardinstelling van de verwerkingstijd de waarde die in de Amazon-lijst is gedefinieerd.<br><br> behandelende Tijd is een regionaal attribuut. Wanneer de waarde voor een lijst wordt veranderd, beïnvloedt de verandering alle lijsten die [!DNL Amazon Seller SKU] in alle opslag delen van Amazon die voor het zelfde gebied (die bij [ wordt bepaald opslagintegratie ](./store-integration.md)) bestaan. Het wijzigen van de waarde voor een gedeelde [!DNL Amazon Seller SKU] in de regio Noord-Amerika heeft echter geen invloed op dezelfde producten die zijn opgenomen in een winkel met een ander gedefinieerd gebied. De opslagruimte voor het gebied met de oudste aanmaakdatum bepaalt de prioriteit voor de instellingen voor de standaardverwerkingstijd. |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
