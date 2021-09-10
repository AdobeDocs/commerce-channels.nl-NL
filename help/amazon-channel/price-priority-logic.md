---
title: Prijsprioriteitslogica
description: Verkoopkanaal in Amazon past prioriteitstelling toe bij het bepalen van de gepubliceerde prijs voor een Amazon-aanbieding.
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# Logica voor prijsprioriteiten

In het volgende voorbeeld, hoe bepaalt het systeem als u $31.99, $24.99, of $27.99 zou moeten publiceren?

![Omvang van de handelsprijs](assets/amazon-price-scope.png)

Als u wilt bepalen welke prijs wordt gebruikt als een product zich op twee websites bevindt en een variabele prijs per website heeft, gebruikt u de logica voor prijsprioriteit (bepaald door de waarde [Sorteervolgorde](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}).

Als u de sorteervolgorde van uw winkels wilt weergeven, gaat u naar **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** in de zijbalk _Admin_. Klik in de kolom _[!UICONTROL Web Site]_op de naam van de website. Op de pagina_[!UICONTROL Web Site Information]_ wordt de _[!UICONTROL Sort Order]_-instelling voor de website weergegeven, die de prioriteit van de website bepaalt. De waarde `1` geeft de hoogste prioriteit aan.

Als de productprijs is ingesteld op `Use Default`, wordt de standaardwaarde voor de prijs in plaats van de prijs van de website gebruikt.

## Voorbeeld 1

|  | Prioriteit website | Prijs (website) | Standaardinstellingen gebruiken |
|---|---|---|---|
| Standaard | 0 | $ 31,99 | — |
| Winkel 1 | 1 | $ 24,99 | Nee |
| Winkel 2 | 2 | $ 27,99 | Ja |

- **[!UICONTROL Magento Price Source]** (gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) wordt ingesteld op het `Price`-kenmerk.
- Kijk naar de website met de hoogste websiteprioriteit, die Store 1 is (gedefinieerd door de waarde [Sorteervolgorde](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}).
- Aangezien Store 1 is ingesteld op het gebruik van de websiteprijs (Standaardinstelling gebruiken = Nee), is de gepubliceerde prijs $24,99.

## Voorbeeld 2

|  | Prioriteit website | Prijswebsite | Standaardinstellingen gebruiken |
|---|---|---|---|
| Standaard | 0 | $ 31,99 | — |
| Winkel 1 | 3 | $ 24,99 | Ja |
| Winkel 2 | 2 | $ 27,99 | Nee |

- **[!UICONTROL Magento Price Source]** (gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) wordt ingesteld op het `Price`-kenmerk.
- Kijk naar de website met de hoogste websiteprioriteit, die Store 1 is (gedefinieerd door de waarde [sort order](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}).
- Aangezien Store 1 **niet** wordt geplaatst om de websiteprijs te gebruiken (Gebruik Gebrek = ja), bekijk de volgende website in de soortorde.
- Aangezien Store 2 **is** geplaatst om de websiteprijs te gebruiken (Gebrek van het Gebruik = Nr), is de gepubliceerde prijs $27.99.

## Voorbeeld 3

|  | Prioriteit website | Prijswebsite | Standaardinstellingen gebruiken |
|---|---|---|---|
| Standaard | 0 | $ 31,99 | $ 30,00 |
| Winkel 1 | 1 | $ 24,99 | — |
| Winkel 2 | 2 | $ 27,99 | $ 20,00 |

In dit voorbeeld wordt de waarde zonder prijs toegevoegd. Deze waarde wordt gebruikt als u een andere waarde voor de instellingen _[!UICONTROL Magento Price Source_] (gedefinieerd in de instellingen [Aanbiedingsprijs](./listing-price.md)) selecteert. De niet-prijswaarde gebruikt altijd de prijs als terugvalprijs.

- **[!UICONTROL Magento Price Source]** (gedefinieerd in uw [[!UICONTROL Listing Price]](./listing-price.md)-instellingen) wordt ingesteld op `Non-Price`.
- Bekijk de website met de hoogste website-prioriteit, die `Store 1`(gedefinieerd door de waarde [Sorteervolgorde](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}) is.
- Aangezien Store 1 **niet** wordt geplaatst om het `Non-Price` attribuut te gebruiken, kijk de volgende website in de soortorde.
- Aangezien Store 2 **is** wordt geplaatst om het `Non-Price` attribuut (niet-Prijs [Website] = $20.00) te gebruiken, is de gepubliceerde prijs $20.00.
