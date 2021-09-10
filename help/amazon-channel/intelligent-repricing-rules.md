---
title: '"Intelligente prijsregel: Regeltype selecteren'
description: Bepaal de prijs van je Amazon-aanbieding op basis van de prijs van een concurrent door een intelligente prijsregel te maken.
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Intelligente prijsregel: regeltype selecteren

>[!IMPORTANT]
>
>Intelligente prijsstellingsregels werken niet correct als de Amazon-regio is ingesteld op `Inactive`-status, zoals tijdens instapweigering. Uw prijsberekeningen zijn afhankelijk van uw verzendkosten en uw regio moet de status `Active` hebben om de verzendkosten te synchroniseren vanuit Amazon.<br><br>
>
>Ga naar Instellingen > Accountinformatie > Vakantie-instellingen om de status van uw regio in uw Amazon-account bij te werken. Zie [Amazon: Aanbiedingsstatus voor vakanties](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

Een intelligente prijsstellingsregel gebruikt de prijs van Amazon-concurrenten om je aanbiedingsprijs te bepalen. Concurrenten zijn andere verkopers die dezelfde producten aanbieden als die van jou op Amazon.

Secties van een intelligente prijsstellingsregel omvatten:

- Regeltype selecteren
- [Voorwaardelijke variaties van concurrent](./competitor-conditional-variances.md)
- [Prijsaanpassing](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- [Optionele maximumprijs](./optional-ceiling-price.md)

## Vorm het regeltype

Definieer het regeltype in de sectie _[!UICONTROL Select Rule Type]_.

1. Kies **[!UICONTROL Rule Type]** bij `Intelligent repricing rule`.

   Met deze instelling worden het veld _[!UICONTROL Competitor Price Source]_en de secties [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md) en [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) ingeschakeld.

1. Kies voor **[!UICONTROL Competitor Price Source]** een optie:

   - **[!UICONTROL Use "Buy Box" Price]** - Kies wanneer je de Amazon-prijs wilt aanpassen op basis van de Amazon- [[!DNL Buy Box]](./buy-box-competitor-pricing.md) verkoopprijs. Er is een [!DNL Buy Box] prijs wanneer meerdere verkopers op Amazon hetzelfde product aanbieden. Amazon definieert de verkoper [!DNL Buy Box] op basis van prestatievereisten. Handelaren willen de verkopersstatus van [!DNL Buy Box] winnen en hun productaanbiedingen maximaal zichtbaar maken.

   - **[!UICONTROL Use Lowest Competitor Price]** - Kies wanneer je de prijs van je aanbieding wilt vergelijken en aanpassen aan de prijs van een concurrent voor hetzelfde product. Als u deze optie kiest, worden de velden _[!UICONTROL Minimum Positive Feedback]_en_[!UICONTROL Minimum Feedback Count]_ ingeschakeld.

1. Kies indien ingeschakeld een optie voor **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Kies wanneer u uw prijzen wilt vergelijken en aanpassen op basis van alle prijzen van concurrenten voor hetzelfde product.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Kies wanneer u de concurrenten wilt beperken tot wie de prijs voor hetzelfde product wordt vergeleken. Deze instelling beperkt de concurrenten verder door te eisen dat hun aanbieding een minimum van het gekozen percentage positieve feedback heeft voordat de regel voor de laagste prijs wordt toegepast.

1. Indien ingeschakeld, voert u een numerieke waarde in voor **[!UICONTROL Minimum Feedback Count]**.

   Deze optionele numerieke waarde beperkt de concurrerende prijsstelling verder. Als een handelaar bijvoorbeeld een 95% positieve feedbackscore heeft, maar alleen een feedbacktelling van `20` heeft, is het mogelijk geen concurrent waarvoor u de prijs wilt wijzigen. Als u echter de waarde `1000` invoert, is het vereist dat de handelaar 95% positieve feedback heeft en minimaal 1000 bedrijfsherzieningen.

>[!NOTE]
>
>U kunt deze prijsstellings- en feedbackopties van concurrenten gebruiken om te voorkomen dat uw prijzen worden gebaseerd op een concurrent die weinig feedback heeft en een product van lagere kwaliteit verkoopt.

![Intelligente prijsregel - selecteer regeltype](assets/ob-intelligent-price-rule-type.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Rule Type] | Selecteer een regeltype. Opties:<ul><li>**[!UICONTROL Standard price rule]** - Met dit regeltype kun je de Amazon-prijs verhogen of verlagen met een bepaald percentage of een bepaald bedrag in dollar ten opzichte van de  _[!UICONTROL Magento Price Source]_prijs. </li><li>**[!UICONTROL Intelligent repricing rule]** - Met dit soort regels kun je de prijs van je Amazon-aanbieding aanpassen op basis van de prijs van de concurrent. Als u deze optie kiest, worden de velden _[!UICONTROL Minimum Positive Feedback]_en_[!UICONTROL Minimum Feedback Count]_ ingeschakeld.</li></ul> |
| [!UICONTROL Competitor Price Source] | Selecteer de gewenste prijsbron. Opties:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Kies deze optie als je de Amazon-prijs wilt aanpassen op basis van de Amazon- [[!DNL Buy Box]](./buy-box-competitor-pricing.md) verkoopprijs. Er is een [!DNL Buy Box] prijs wanneer meerdere verkopers op Amazon hetzelfde product aanbieden. Amazon definieert de verkoper [!DNL Buy Box] op basis van prestatievereisten. Handelaren willen de verkopersstatus van [!DNL Buy Box] winnen en hun productaanbiedingen maximaal zichtbaar maken.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Kies deze optie als je de aanbiedingsprijs wilt vergelijken en aanpassen aan de  [laagste ](./lowest-competitor-pricing.md) prijs van een concurrent voor hetzelfde product. Als u deze optie kiest, worden de velden _[!UICONTROL Minimum Positive Feedback]_en_[!UICONTROL Minimum Feedback Count]_ ingeschakeld.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | Alleen actief als `Use Lowest Competitor Price` is gekozen. Opties:<ul><li>**[!UICONTROL All Competitor's Prices]** - Kies wanneer u uw prijzen wilt vergelijken en aanpassen op basis van alle prijzen van concurrenten voor hetzelfde product.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Kies wanneer u de concurrenten wilt beperken tot wie u vergelijkt en pas uw prijzen aan. Met deze instelling worden uw concurrenten verder beperkt doordat hun aanbieding een minimum van het gekozen percentage positieve feedback moet hebben en vervolgens de laagste prijs van die subset concurrenten moet gebruiken.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | Alleen actief als `Use Lowest Competitor Price` is gekozen. Door deze optionele numerieke waarde wordt de vergelijking van de concurrerende prijzen verder beperkt. Als een handelaar bijvoorbeeld een 95% positieve feedbackscore heeft maar alleen een feedbacktelling van `20` heeft, is het mogelijk geen concurrent waarvoor u de prijs wilt wijzigen. Als u echter de waarde `1000` invoert, is het vereist dat de handelaar 95% positieve feedback heeft en minimaal 1000 bedrijfsherzieningen. |
