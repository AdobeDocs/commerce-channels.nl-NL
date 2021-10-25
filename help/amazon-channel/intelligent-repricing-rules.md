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
>Intelligente prijsstellingsregels functioneren niet naar behoren als de Amazon-regio is ingesteld op `Inactive` status, zoals tijdens het instappen. Je prijsberekeningen zijn afhankelijk van je verzendkosten en je regio moet binnen zijn `Active` status voor je verzendkosten die je vanaf Amazon wilt synchroniseren.<br><br>
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

Definieer het regeltype in het dialoogvenster _[!UICONTROL Select Rule Type]_sectie.

1. Voor **[!UICONTROL Rule Type]** kiest u `Intelligent repricing rule`.

   Deze instelling schakelt de _[!UICONTROL Competitor Price Source]_en [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md), en [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) secties.

1. Voor **[!UICONTROL Competitor Price Source]** kiest u een optie:

   - **[!UICONTROL Use "Buy Box" Price]** - Kies wanneer u de Amazon-prijs wilt aanpassen op basis van de Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) verkoopprijs. A [!DNL Buy Box] Er is een prijs wanneer meerdere verkopers op Amazon hetzelfde product aanbieden. Amazon definieert de [!DNL Buy Box] verkoper op basis van prestatievereisten. Handelaren willen de [!DNL Buy Box] de status van de verkoper en de maximale zichtbaarheid van hun productaanbiedingen.

   - **[!UICONTROL Use Lowest Competitor Price]** - Kies wanneer je de prijs van je aanbieding wilt vergelijken en aanpassen aan de prijs van een concurrent voor hetzelfde product. Wanneer u kiest, wordt _[!UICONTROL Minimum Positive Feedback]_en_[!UICONTROL Minimum Feedback Count]_ velden zijn ingeschakeld.

1. Indien ingeschakeld, kiest u een optie voor **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Kies wanneer u uw prijzen wilt vergelijken en aanpassen op basis van alle prijzen van concurrenten voor hetzelfde product.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Kies wanneer u de concurrenten wilt beperken tot wie de prijs voor hetzelfde product wordt vergeleken. Deze instelling beperkt de concurrenten verder door te eisen dat hun aanbieding een minimum van het gekozen percentage positieve feedback heeft voordat de regel voor de laagste prijs wordt toegepast.

1. Indien ingeschakeld, voert u een numerieke waarde in voor **[!UICONTROL Minimum Feedback Count]**.

   Deze optionele numerieke waarde beperkt de concurrerende prijsstelling verder. Als een handelaar bijvoorbeeld een 95% positieve feedbackscore heeft, maar alleen een feedbacktelling heeft van `20`, is het mogelijk geen concurrent waarvoor u de prijsstelling wilt wijzigen. Als u echter een waarde opgeeft van `1000`de onderneming zou voor 95 % positieve feedback en voor ten minste 1000 beoordelingen door handelaren moeten krijgen .

>[!NOTE]
>
>U kunt deze prijsstellings- en feedbackopties van concurrenten gebruiken om te voorkomen dat uw prijzen worden gebaseerd op een concurrent die weinig feedback heeft en een product van lagere kwaliteit verkoopt.

![Intelligente prijsregel - selecteer regeltype](assets/ob-intelligent-price-rule-type.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Rule Type] | Selecteer een regeltype. Opties:<ul><li>**[!UICONTROL Standard price rule]** - Met dit soort regels kun je de Amazon-prijs verhogen of verlagen met een bepaald percentage of een bepaald bedrag in dollar ten opzichte van _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - Met dit soort regels kun je de prijs van je Amazon-aanbieding aanpassen op basis van de prijs van de concurrent. Wanneer u kiest, wordt _[!UICONTROL Minimum Positive Feedback]_en_[!UICONTROL Minimum Feedback Count]_ velden zijn ingeschakeld.</li></ul> |
| [!UICONTROL Competitor Price Source] | Selecteer de gewenste prijsbron. Opties:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Kies deze optie als u de Amazon-prijs wilt aanpassen op basis van de Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) verkoopprijs. A [!DNL Buy Box] Er is een prijs wanneer meerdere verkopers op Amazon hetzelfde product aanbieden. Amazon definieert de [!DNL Buy Box] verkoper op basis van prestatievereisten. Handelaren willen de [!DNL Buy Box] de status van de verkoper en de maximale zichtbaarheid van hun productaanbiedingen.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Kies deze optie als je de prijs van je aanbieding wilt vergelijken en aanpassen aan de [laagste prijsstelling voor concurrenten](./lowest-competitor-pricing.md) voor hetzelfde product. Wanneer u kiest, wordt _[!UICONTROL Minimum Positive Feedback]_en_[!UICONTROL Minimum Feedback Count]_ velden zijn ingeschakeld.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | Alleen actief als `Use Lowest Competitor Price` wordt gekozen. Opties:<ul><li>**[!UICONTROL All Competitor's Prices]** - Kies wanneer u uw prijzen wilt vergelijken en aanpassen op basis van alle prijzen van concurrenten voor hetzelfde product.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Kies wanneer u de concurrenten wilt beperken tot wie u vergelijkt en pas uw prijzen aan. Met deze instelling worden uw concurrenten verder beperkt doordat hun aanbieding een minimum van het gekozen percentage positieve feedback moet hebben en vervolgens de laagste prijs van die subset concurrenten moet gebruiken.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | Alleen actief als `Use Lowest Competitor Price` wordt gekozen. Door deze optionele numerieke waarde wordt de vergelijking van de concurrerende prijzen verder beperkt. Als een handelaar bijvoorbeeld een 95% positieve feedbackscore heeft, maar alleen een feedbacktelling heeft van `20`, is het mogelijk geen concurrent waarvoor u de prijsstelling wilt wijzigen. Als u echter een waarde opgeeft van `1000`de onderneming zou voor 95 % positieve feedback en voor ten minste 1000 beoordelingen door handelaren moeten krijgen . |
