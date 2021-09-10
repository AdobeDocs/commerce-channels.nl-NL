---
title: Aanbiedingsvoorwaarde product
description: 'Met de instellingen voor de aanbiedingsvoorwaarde voor producten kunt u de producten van de Handel toewijzen aan een Amazon-productvoorwaarde, zoals "Nieuw" of "Gereviseerd".'
redirect_from: /sales-channels/asc/ob-product-listing-condition.html: 
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 526
ht-degree: 0%

---

# Voorwaarde voor aanbieding van producten

De instellingen voor de aanbiedingsvoorwaarden van producten maken deel uit van de aanbiedingsinstellingen van je winkel. U kunt tot de lijstmontages op [opslagdashboard](./amazon-store-dashboard.md) toegang hebben.

Amazon vereist een productaanbieding om een gedefinieerde voorwaarde te hebben. Als al uw producten dezelfde voorwaarde zijn, kunt u een van de Amazon-voorwaardenopties selecteren om al uw producten weer te geven als uw globale voorwaardenwaarde. Tot de standaard Amazon-voorwaarden behoren:

- `New`
- `Refurbished`
- `Used; Like New`
- `Used; Very Good`
- `Used; Good`
- `Used; Acceptable`
- `Collectible; Like New`
- `Collectible; Very Good`
- `Collectible; Good`
- `Collectible; Acceptable`

>[!IMPORTANT]
>
>Als u vernieuwde (gereviseerde) producten verkoopt, moet u zich inschrijven in [!DNL Amazon Renewed Program]. Zie [Vernieuwde producten](./renewed-products.md).

Als uw catalogus echter producten in verschillende omstandigheden bevat (zoals Nieuw, Gebruikt en Vernieuwd), moet u **[!UICONTROL Assign Condition Using Product Attribute]** kiezen. Met deze instelling kunt u het kenmerk en de waarden van uw voorwaarde [!DNL Commerce] toewijzen aan de voorwaarden van uw Amazon-aanbieding.

Tijdens [Pre-setup taken](./amazon-pre-setup-tasks.md), wordt u aangemoedigd om een [!DNL Commerce] productattribuut voor de voorwaarde van een product tot stand te brengen. Als u producten in diverse voorwaarden aanbiedt en u geen voorwaardeltribuut hebt gecreeerd, zie [een productattribuut in [!DNL Commerce]](./ob-creating-magento-attributes.md) creëren. Nadat het voorwaardeltribuut wordt gecreeerd, kunt u een voorwaardenwaarde aan elk van uw producten in uw [!DNL Commerce] catalogus toewijzen.

## Instellingen configureren

1. Klik **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie **[!UICONTROL Product Listing Condition]** uit.

1. Kies voor **[!UICONTROL Listing Product Condition]** een optie.

   Kies een van de standaard Amazon-voorwaarden voor je globale voorwaardenwaarde voor al je aanbiedingen. De standaardinstelling is `New`.

   Als u producten/aanbiedingen hebt die verschillende voorwaarden hebben, kiest u `Assign Condition Using Product Attribute` om de instellingen voor de productvoorwaarde te definiëren in de extra velden die worden weergegeven.

1. Voor **Condition Attribute**, kies [!DNL Commerce] attributen om waarden voor elk van de standaard Amazon voorwaardelekenmerken in kaart te brengen.

   Als u producten in `Used` of `Collectible` voorwaarde maar u niet verder onderscheidt, kunt u aan één enkele `Used` of `Collectible` Amazon voorwaarde in kaart brengen en de anderen leeg verlaten. Met deze methode worden alle `Used`- of `Collectible`-voorwaarden toegewezen aan de enige gebruikte Amazon- of Collectibele voorwaarde.

   U hebt bijvoorbeeld één `Used` voorwaarde voor uw producten. Bij het toewijzen kiest u of u wilt toewijzen aan de Amazon-voorwaarde `Used; Like New`, `Used; Very Good`, `Used; Good` of `Used; Acceptable`. Vul alleen het veld in voor de Amazon-voorwaarde die u wilt, waarbij de andere `Used`-opties op `--Select Option--` worden ingesteld. In de voorbeeldafbeelding worden alle [!DNL Commerce]-producten in `Used`-voorwaarde toegewezen aan de Amazon `Used; Very Good`-voorwaarde.

   U kunt ook beschrijvende tekst voor uw voorwaarden invoeren, behalve `New`.

1. Klik op **[!UICONTROL Save listing settings]** als u klaar bent.

![Voorwaarde voor aanbieding van producten](assets/amazon-product-listing-condition.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Listing Product Condition] | De conditie van je productaanbiedingen. Opties: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Kies een van de standaard Amazon-voorwaarden als u één productvoorwaarde verkoopt. Als uw [!DNL Commerce] catalogus producten in diverse voorwaarden bevat, kies `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | Het [!DNL Commerce] attribuut dat de voorwaarde voor uw producten bepaalt. Selecteer het Magneto-kenmerk dat u hebt gemaakt om toe te wijzen aan het Amazon-voorwaardeltribuut. In [Vooraf-de voorbeeld van Taken ](./ob-creating-magento-attributes.md) adviseert noemend het als `Amazon Condition`. Als u deze optie kiest, worden extra velden weergegeven voor het toewijzen van de standaard Amazon-voorwaarden. |
| [!UICONTROL Additional Condition fields] | Kies voor elke standaard Amazon-voorwaarde de bijbehorende voorwaarde. De opties zijn de voorwaardelabels u toevoegde toen u [uw Amazon voorwaardeltribuut ](./ob-creating-magento-attributes.md) creeerde.<br><br>Als u producten in de  `Used` of de  `Collectible` voorwaarde hebt maar u maakt geen onderscheid, kunt u aan één enkele  `Used` of  `Collectible` Amazon voorwaarde in kaart brengen en de anderen leeg verlaten. Met deze methode worden alle `Used`- of `Collectible`-voorwaarden toegewezen aan de enige gebruikte Amazon- of Collectibele voorwaarde. |

**Snelle toegang**  -  [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
