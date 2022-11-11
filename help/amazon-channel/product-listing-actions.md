---
title: Handelingen voor productaanbiedingen
description: Met de instellingen voor acties voor het aanbieden van producten kunt u bepalen hoe de handelscatalogus reageert op Amazon.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Handelingen voor productaanbiedingen

De handelingsinstellingen voor productaanbiedingen maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via de [opslagdashboard](./amazon-store-dashboard.md).

Met deze instellingen wordt gedefinieerd hoe uw catalogus reageert op Amazon. Deze instellingen:

- Geef aan of uw [!DNL Commerce] catalogusproducten die voldoen aan de Amazon-voorwaarden worden automatisch naar je verzonden [!DNL Amazon Seller Central] account om aanbiedingen te maken.

- Stel de standaardverwerkingstijd voor een bestelling in. Deze waarde definieert het aantal dagen dat u nodig hebt om een bestelling te verwerken en te verzenden. Als iemand bijvoorbeeld 2-dagen verzending selecteert, begint de tijd van de verzending niet voordat de verwerking is voltooid en worden de pakketten aan een vervoerder afgegeven. De totale levertijd is (verwerkingstijd + doorvoertijd + feestdagen).

## Instellingen configureren

1. Klikken **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Product Listing Actions]_uit.

1. Voor **[!UICONTROL Automatic List Action]** (vereist) kiest u een optie:

   - `Automatically List Eligible Products` - (Standaard) Kies wanneer u uw [!DNL Commerce] catalogusproducten (die voldoen aan de Amazon-voorwaarden) om automatisch te publiceren naar Amazon en Amazon-aanbiedingen te maken.

   - `Do Not Automatically List Eligible Products` - Kies wanneer u uw in aanmerking komende optie handmatig wilt selecteren [!DNL Commerce] catalogusproducten en Amazon-aanbiedingen maken. Als je kiest, catalogiseer je producten die voldoen aan je aanbiedingscriteria en die alle vereiste informatie bevatten, weergegeven op de [_[!UICONTROL Ready to List]_](./ready-to-list.md) voor handmatig publiceren naar Amazon.

1. Voor **[!UICONTROL Default Handling Time]** (vereist), voert u het aantal dagen in dat nodig is voor de aanlooptijd vóór de verzending.

   De standaardwaarde is `2` dagen.

   >[!NOTE]
   >
   >Deze standaardwaarde voor de afhandelingstijd geldt alleen voor Amazon-aanbiedingen die via Amazon-verkoopkanalen zijn gemaakt. Alle Amazon-aanbiedingen die in je [!DNL Amazon Seller Central] -account de standaardverwerkingstijd gebruiken die in Amazon is ingesteld.

1. Klik op **[!UICONTROL Save listing settings]**.

![Handelingen voor productaanbiedingen](assets/amazon-product-listing-actions.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Automatic List Action] | Opties:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Aanbevolen) Kies wanneer u uw [!DNL Commerce] catalogusproducten (die voldoen aan de Amazon-voorwaarden) om automatisch te publiceren naar Amazon en Amazon-aanbiedingen te maken. Wanneer u kiest, wordt [_[!UICONTROL Ready to List]_](./ready-to-list.md) wordt niet weergegeven. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Kies wanneer u handmatig subsidiabele items wilt selecteren [!DNL Commerce] catalogusproducten en maak Amazon-aanbiedingen. Als je kiest, catalogiseer je producten die voldoen aan je aanbiedingscriteria en die alle vereiste informatie bevatten, weergegeven op de [_[!UICONTROL Ready to List]_](./ready-to-list.md) tabblad voor handmatig publiceren.</li></ul> |
| [!UICONTROL Default Handling Time] | De numerieke waarde die het aantal dagen vertegenwoordigt, in het algemeen, dat het u vergt om uw orden te verwerken en te verzenden. De standaardwaarde is `2`. Deze waarde wordt gebruikt voor Amazon-aanbiedingen die zijn gemaakt in [!DNL Commerce] en gepubliceerd naar Amazon. De standaardverwerkingstijd voor Amazon-aanbiedingen voordat deze worden geïntegreerd met [!DNL Commerce] worden niet beïnvloed door deze instelling.<br><br>De waarde die in het verkoopkanaal van Amazon is gedefinieerd, vervangt de standaardverwerkingstijd die in een bestaande Amazon-aanbieding is gedefinieerd, niet. Wanneer een **[!UICONTROL Handling Time Override]** wordt toegelaten en dan verwijderd, keert de Behandelingstijd voor een orde aan de hier bepaalde waarde terug.<br><br>Als u producten hebt die verschillende behandelingstijden hebben, kunt u een Behandelingstijd met voeten treden op het product-specifieke niveau. U kunt overschreven verwerkingstijd beheren in het dialoogvenster [_[!UICONTROL Overrides]_](./overrides.md) , zodat u over de flexibiliteit beschikt om uw product te laten voldoen. Als er geen verwerkingstijd is die binnen [!DNL Commerce] voor een product is de standaardinstelling van de verwerkingstijd de waarde die is gedefinieerd in de Amazon-aanbieding.<br><br>Verwerkingstijd is een regionaal kenmerk. Wanneer de waarde voor een aanbieding wordt gewijzigd, heeft de wijziging invloed op alle aanbiedingen die de [!DNL Amazon Seller SKU] in alle Amazon-winkels die voor hetzelfde gebied bestaan (gedefinieerd als [winkelintegratie](./store-integration.md)). De waarde voor een gedeelde [!DNL Amazon Seller SKU] in de regio Noord-Amerika niet van invloed is op dezelfde producten die zijn opgenomen in een winkel met een ander afgebakend gebied. De opslagruimte voor het gebied met de oudste aanmaakdatum bepaalt de prioriteit voor de instellingen voor de standaardverwerkingstijd. |

**Snelle toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
