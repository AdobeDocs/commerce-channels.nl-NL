---
title: Verkoopkanaal in Amazon - Voorwaarde voor aanbieding van producten
description: Met de instellingen voor de aanbiedingsvoorwaarde voor producten kunt u de producten van de Handel toewijzen aan een Amazon-productvoorwaarde, zoals "Nieuw" of "Gereviseerd".
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Voorwaarde voor aanbieding van producten

De instellingen voor de aanbiedingsvoorwaarden van producten maken deel uit van de aanbiedingsinstellingen van je winkel. U kunt de aanbiedingsinstellingen openen op de knop [opslagdashboard](./amazon-store-dashboard.md).

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
>Als u vernieuwde (gereviseerde) producten verkoopt, dient u zich in te schrijven voor de [!DNL Amazon Renewed Program]. Zie [Vernieuwde producten](./renewed-products.md).

Als uw catalogus echter producten bevat onder verschillende omstandigheden (zoals Nieuw, Gebruikt en Gereviseerd), moet u **[!UICONTROL Assign Condition Using Product Attribute]**. Met deze instelling kunt u uw [!DNL Commerce] voorwaardelabel en waarden volgens de voorwaarden van je Amazon-aanbieding.

Tijdens [Taken vooraf instellen](./amazon-pre-setup-tasks.md), wordt u aangeraden een [!DNL Commerce] productkenmerk voor de voorwaarde van een product. Als u producten onder verschillende omstandigheden aanbiedt en u geen voorwaardelement hebt gemaakt, raadpleegt u [Een productkenmerk maken in [!DNL Commerce]](./ob-creating-magento-attributes.md). Nadat het kenmerk condition is gemaakt, kunt u een voorwaardenwaarde toewijzen aan elk van uw producten in uw [!DNL Commerce] catalogus.

## Instellingen configureren

1. Klikken **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Breid uit **[!UICONTROL Product Listing Condition]** sectie.

1. Voor **[!UICONTROL Listing Product Condition]** kiest u een optie.

   Kies een van de standaard Amazon-voorwaarden voor je globale voorwaardenwaarde voor al je aanbiedingen. Standaardinstelling is `New`.

   Kies `Assign Condition Using Product Attribute` om de instellingen voor de productvoorwaarde te definiëren in de extra velden die worden weergegeven.

1. Voor **Condition-kenmerk**, kiest u de [!DNL Commerce] attribuut to map values for each of the standard Amazon condition attributes.

   Als u producten hebt in de `Used` of `Collectible` voorwaarde maar u maakt geen onderscheid meer, u kunt toewijzen aan één voorwaarde `Used` of `Collectible` Amazon-voorwaarde en laat de overige leeg. Deze methode wijst al uw `Used` of `Collectible` voorwaarden voor de enige gebruikte Amazon of de verzamelbare toestand.

   U hebt bijvoorbeeld één `Used` voorwaarde voor uw producten. Bij het toewijzen kiest u of u wilt toewijzen aan de Amazon-voorwaarde `Used; Like New`, `Used; Very Good`, `Used; Good`, of `Used; Acceptable`. Vul alleen het veld in voor de Amazon-voorwaarde die u wilt, en laat de andere voorwaarde los `Used` opties ingesteld op `--Select Option--`. In de voorbeeldafbeelding: alle [!DNL Commerce] producten in `Used` voorwaarde wordt toegewezen aan de Amazon `Used; Very Good` voorwaarde.

   U kunt ook beschrijvende tekst voor uw voorwaarden invoeren, behalve `New`.

1. Klik op **[!UICONTROL Save listing settings]**.

![Voorwaarde voor aanbieding van producten](assets/amazon-product-listing-condition.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Listing Product Condition] | De conditie van je productaanbiedingen. Opties: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Als je één productvoorwaarde verkoopt, kies je een van de standaard Amazon-voorwaarden. Als uw [!DNL Commerce] de catalogus bevat producten onder verschillende omstandigheden, kies `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | De [!DNL Commerce] -kenmerk dat de voorwaarde voor uw producten definieert. Selecteer het Magneto-kenmerk dat u hebt gemaakt om toe te wijzen aan het Amazon-voorwaardeltribuut. In de [Vooraf ingestelde Taken, voorbeeld](./ob-creating-magento-attributes.md) beveelt aan de naam ervan te wijzigen `Amazon Condition`. Als u deze optie kiest, worden extra velden weergegeven voor het toewijzen van de standaard Amazon-voorwaarden. |
| [!UICONTROL Additional Condition fields] | Kies voor elke standaard Amazon-voorwaarde de bijbehorende voorwaarde. De opties zijn de voorwaardelabels die u hebt toegevoegd toen u [Amazon-voorwaardelement maken](./ob-creating-magento-attributes.md).<br><br>Als u producten hebt in de `Used` of `Collectible` voorwaarde maar u maakt geen onderscheid meer, u kunt toewijzen aan één voorwaarde `Used` of `Collectible` Amazon-voorwaarde en laat de overige leeg. Deze methode wijst alle `Used` of `Collectible` voorwaarden voor de enige gebruikte Amazon of de verzamelbare toestand. |

**Snelle toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
