---
title: Verkoopkanaal in Amazon - Voorwaarde voor aanbieding van producten
description: Met de instellingen voor de aanbiedingsvoorwaarde voor producten kunt u Commerce-producten toewijzen aan een Amazon-productvoorwaarde, zoals "Nieuw" of "Gereviseerd".
feature: Sales Channels, Products, Merchandising
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Voorwaarde voor aanbieding van producten

De instellingen voor de aanbiedingsvoorwaarden van producten maken deel uit van de aanbiedingsinstellingen van je winkel. U kunt tot de lijstmontages op het [ opslagdashboard ](./amazon-store-dashboard.md) toegang hebben.

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
>Als u vernieuwde (gereviseerde) producten verkoopt, moet u zich inschrijven in de [!DNL Amazon Renewed Program] . Zie [ Vernieuwde Producten ](./renewed-products.md).

Als uw catalogus echter producten bevat onder verschillende omstandigheden (zoals Nieuw, Gebruikt en Vernieuwd), moet u **[!UICONTROL Assign Condition Using Product Attribute]** kiezen. Met deze instelling kunt u het kenmerk en de waarden van de voorwaarde [!DNL Commerce] toewijzen aan de voorwaarden van je Amazon-aanbieding.

Tijdens [ pre-opstellingstaken ](./amazon-pre-setup-tasks.md), wordt u aangemoedigd om a [!DNL Commerce] productattribuut voor de voorwaarde van een product tot stand te brengen. Als u producten in diverse voorwaarden aanbiedt en u geen voorwaardeltribuut hebt gecreeerd, zie [ een productattribuut in  [!DNL Commerce]](./ob-creating-magento-attributes.md) creëren. Nadat het kenmerk condition is gemaakt, kunt u een voorwaardenwaarde toewijzen aan elk van uw producten in de catalogus van [!DNL Commerce] .

## Instellingen configureren

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie **[!UICONTROL Product Listing Condition]** uit.

1. Kies bij **[!UICONTROL Listing Product Condition]** een optie.

   Kies een van de standaard Amazon-voorwaarden voor je globale voorwaardenwaarde voor al je aanbiedingen. De standaardinstelling is `New` .

   Als je producten/aanbiedingen hebt die verschillende voorwaarden hebben, kies dan `Assign Condition Using Product Attribute` om de instellingen voor de productvoorwaarde te definiëren in de extra velden die worden weergegeven.

1. Voor **Attribuut van de Voorwaarde**, kies het [!DNL Commerce] attribuut aan kaartwaarden voor elk van de standaard de voorwaardelekenmerken van Amazon.

   Als u producten in de voorwaarde `Used` of `Collectible` hebt maar geen onderscheid meer maakt, kunt u een `Used` of `Collectible` Amazon-voorwaarde toewijzen en de andere leeg laten. Met deze methode worden alle `Used` - of `Collectible` -voorwaarden toegewezen aan de enige Gebruikte of Verzamelbare Amazon-voorwaarde.

   U hebt bijvoorbeeld één `Used` -voorwaarde voor uw producten. Bij het toewijzen kiest u of u wilt toewijzen aan de Amazon-voorwaarde `Used; Like New`, `Used; Very Good` , `Used; Good` of `Used; Acceptable` . Vul alleen het veld in voor de gewenste Amazon-voorwaarde, waarbij de andere `Used` -opties op `--Select Option--` worden ingesteld. In de voorbeeldafbeelding worden alle [!DNL Commerce] producten in `Used` -voorwaarde toegewezen aan de Amazon `Used; Very Good` -voorwaarde.

   U kunt ook beschrijvende tekst voor uw voorwaarden invoeren, behalve `New` .

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ de lijstvoorwaarde van het Product ](assets/amazon-product-listing-condition.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Listing Product Condition] | De conditie van je productaanbiedingen. Opties: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br> Als u één productvoorwaarde verkoopt, kiest u een van de standaard Amazon-voorwaarden. Kies `Assign Condition Using Product Attribute` als de catalogus van [!DNL Commerce] producten onder verschillende omstandigheden bevat. |
| [!UICONTROL Condition Attribute] | Het attribuut [!DNL Commerce] dat de voorwaarde voor uw producten bepaalt. Selecteer het Magneto-kenmerk dat u hebt gemaakt om toe te wijzen aan het Amazon-voorwaardeltribuut. In het [ voorbeeld van Taken pre-Opstelling ](./ob-creating-magento-attributes.md) adviseert noemend het als `Amazon Condition`. Als u deze optie kiest, worden extra velden weergegeven voor het toewijzen van de standaard Amazon-voorwaarden. |
| [!UICONTROL Additional Condition fields] | Kies voor elk van de standaard Amazon-voorwaarden de bijbehorende voorwaarde. De opties zijn de voorwaardelabels u toevoegde toen u [ uw de voorwaardeltributen van Amazon ](./ob-creating-magento-attributes.md) creeerde.<br><br> Als u producten in de `Used` of `Collectible` voorwaarde hebt maar niet verder van elkaar onderscheidt, kunt u aan één enkele `Used` of `Collectible` Amazon voorwaarde in kaart brengen en de anderen leeg verlaten. Met deze methode worden alle `Used` - of `Collectible` -voorwaarden toegewezen aan de enige Gebruikte of Verzamelbare Amazon-voorwaarde. |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
