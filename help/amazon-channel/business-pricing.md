---
title: "[!DNL (B2B) Business Price] voor Amazon-aanbiedingen"
description: U kunt van uw  [!DNL Commerce]  opslagproducten op de Van Bedrijfs Amazon (B2B) plaats een lijst maken door zaken in uw Amazon  [!DNL Seller Central]  rekening toe te laten.
role: Admin
level: Intermediate
feature: Sales Channels, Configuration, B2B, Tools and External Services, Merchandising, Integration
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# [!DNL (B2B) Business Price] voor Amazon-aanbiedingen

(B2B) Zakelijke prijsinstellingen maken deel uit van de aanbiedingsinstellingen van je winkel. De van de lijst montages worden betreden van het [ opslagdashboard van Amazon ](./amazon-store-dashboard.md).

[!DNL Amazon Business] is een markt die exclusief is voor geregistreerde zakelijke accounts van Amazon en alleen beschikbaar is in de Verenigde Staten, Frankrijk, Duitsland en het Verenigd Koninkrijk. Als de markt B2B-prijzen toestaat, is deze binnen je aanbiedingsinstellingen bewerkbaar.

Met [!DNL B2B Business Pricing] kunnen handelaren met een zakelijke account van elkaar aankopen met de verwachte prestaties van de Amazon-winkelervaring. Met B2B-prijzen voor bedrijven kunnen bedrijven gedifferentieerde prijzen aanbieden op basis van de aangeschafte hoeveelheid.

Als u uw producten op de [!DNL Amazon Business (B2B)] -site wilt aanbieden, moet u eerst zaken inschakelen in uw [!DNL Amazon Seller Central] -account. Voor meer informatie over de eigenschap B2B, zie [ Amazon: B2B Centrale ](https://sellercentral.amazon.com/gp/help/G202161480/) {target="_blank"} (vereist Centrale login van de Verkoper).

## [!DNL (B2B) Business Price] -instellingen configureren

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL (B2B) Business Price]_uit.

1. Kies bij **[!UICONTROL Enable Business Pricing]** een optie.

   - `Disabled` - (Standaard) Kies wanneer u geen business-to-business verkoop wilt inschakelen. Alle andere velden in deze sectie worden uitgeschakeld wanneer u deze selecteert.

   - `Enabled` - Kies wanneer u uw zaken-aan-zaken verkoop wilt toelaten. Wanneer toegelaten, wordt de bedrijfsprijs geplaatst gelijk aan de lijstprijs nadat alle prijsregels zijn toegepast. De bedrijfsprijs volgt, indien ingeschakeld, het prijsbereik voor websites. Een zakelijke prijs mag niet lager zijn dan $1.

1. Kies bij **[!UICONTROL Enable Tiered Pricing]** een optie.

   - `Disabled` - (Standaard) Kies wanneer u voor alle bestellingen dezelfde prijs wilt gebruiken. Als u deze optie kiest, worden alle _[!UICONTROL Pricing Level]_-velden in deze sectie uitgeschakeld.

   - `Enabled` - Kies wanneer u prijsaanpassingen wilt inschakelen op basis van het aantal bestellingen. Wanneer u deze optie kiest, worden de velden _[!UICONTROL Pricing Level]_ingeschakeld.

1. Voltooi de instellingen van **[!UICONTROL Pricing Level]** .

   U kunt maximaal vijf instellingen voor aantal/korting definiëren waarmee de prijzen op het niveau van je zakelijke aanbiedingen worden ingesteld. Voer in elke rij de drempelwaarde voor de hoeveelheid en het kortingspercentage in dat u wilt toepassen. Als u bijvoorbeeld `5` invoert in het eerste veld van de eerste rij en `5` in het tweede veld, wordt een korting van 5% toegepast wanneer een ander bedrijf een hoeveelheid van 5 of meer koopt.

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ Van Bedrijfs Amazon Prijsstelling (B2B) ](assets/amazon-business-pricing.png){width="500" zoomable="yes"}

| Veld | Beschrijving |
|----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Business Pricing] | Opties: <ul><li>**[!UICONTROL Disabled]** - (Standaard) Kies wanneer u geen zakelijke verkoop wilt inschakelen. Als u deze optie kiest, worden alle andere velden in deze sectie uitgeschakeld.</li><li>**[!UICONTROL Enabled]** - Kies wanneer u uw bedrijf wilt inschakelen voor zakelijke verkoop. Wanneer gekozen, wordt de bedrijfsprijs gelijk aan de lijstprijs na alle prijsregels toegepast. De bedrijfsprijs volgt, indien ingeschakeld, het prijsbereik voor websites. Een zakelijke prijs mag niet lager zijn dan $1.</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | (Vereist) opties: <ul><li>**[!UICONTROL Disabled]** - (Standaard) Kies wanneer u voor alle bestellingen dezelfde prijs wilt gebruiken. Als u deze optie kiest, worden alle _[!UICONTROL Pricing Level]_-velden in deze sectie uitgeschakeld.</li><li>**[!UICONTROL Enabled]** - Kies wanneer u prijzen wilt inschakelen die worden aangepast op basis van het aantal bestellingen. Wanneer u deze optie kiest, worden de velden _[!UICONTROL Pricing Level]_ingeschakeld.</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | Als Gelaagde prijsstelling is ingeschakeld, kunt u maximaal vijf instellingen voor aantal/korting definiëren waarmee de prijzen op de laag voor je zakelijke aanbiedingen worden ingesteld. Voer in elke rij de drempelwaarde voor de hoeveelheid en het kortingspercentage in dat u wilt toepassen. Als u bijvoorbeeld `5` invoert in het eerste veld van de eerste rij en `5` in het tweede veld, wordt een korting van 5% toegepast wanneer een ander bedrijf een hoeveelheid van vijf of meer koopt. |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
