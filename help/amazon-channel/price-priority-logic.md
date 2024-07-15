---
title: Amazon-verkoopkanaal - Prijsprioriteitslogica
description: Verkoopkanaal in Amazon past prioriteitstelling toe bij het bepalen van de gepubliceerde prijs voor een Amazon-aanbieding.
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 2%

---

# Logica voor prijsprioriteiten

Hoe bepaalt het systeem in het volgende voorbeeld of u $31,99, $24,99 of $27,99 moet publiceren?

![ Commerce prijswerkingsgebied ](assets/amazon-price-scope.png){width="400"}

Om te bepalen welke prijs wordt gebruikt als een product op twee websites is en een variërende prijs per website heeft, de logica van de gebruiksprioriteit van de gebruiksprijs (die door de [ waarde van de Orde van de Sortering ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) wordt bepaald).

Om de de soortorde van uw opslag te bekijken, ga **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** in _Admin_ sidebar. Klik in de kolom _[!UICONTROL Web Site]_op de naam van de website. Op de pagina_[!UICONTROL Web Site Information]_ ziet u de instelling _[!UICONTROL Sort Order]_voor de website, die de prioriteit van de website bepaalt. De waarde `1` geeft de hoogste prioriteit aan.

Als de productprijs is ingesteld op `Use Default` , wordt de standaardwaarde voor de prijs in plaats van de prijs van de website gebruikt.

## Voorbeeld 1

|         | Prioriteit website | Prijs (website) | Standaardinstellingen gebruiken |
|---------|------------------|-----------------|-------------|
| Standaard | 0 | $ 31,99 | — |
| Winkel 1 | 1 | $ 24,99 | Nee |
| Winkel 2 | 2 | $ 27,99 | Ja |

- **[!UICONTROL Magento Price Source]** (die in uw [ wordt bepaald die Prijs van de Lijst ](./listing-price.md) wordt geplaatst aan het `Price` attribuut.
- Kijk naar de website met de hoogste website prioriteit, die Opslag 1 is (die door de [ wordt bepaald van de Orde van de Soort ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) waarde).
- Aangezien Store 1 is ingesteld op het gebruik van de websiteprijs (Standaardinstelling gebruiken = Nee), is de gepubliceerde prijs $24,99.

## Voorbeeld 2

|         | Prioriteit website | Prijs website | Standaardinstellingen gebruiken |
|---------|------------------|---------------|-------------|
| Standaard | 0 | $ 31,99 | — |
| Winkel 1 | 1 | $ 24,99 | Ja |
| Winkel 2 | 2 | $ 27,99 | Nee |

- **[!UICONTROL Magento Price Source]** (die in uw [ wordt bepaald die Prijs van de Lijst ](./listing-price.md) wordt geplaatst aan het `Price` attribuut.
- Bekijk de website met de hoogste website prioriteit, die Winkel 1 is (die door de [ wordt bepaald orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) waarde).
- Aangezien Opslag 1 **niet** wordt geplaatst om de websiteprijs te gebruiken (Gebrek van het Gebruik = ja), kijk de volgende website in de soortorde.
- Aangezien Opslag 2 **** wordt geplaatst om de websiteprijs te gebruiken (Gebrek van het Gebruik = Nr), is de gepubliceerde prijs $27.99.

## Voorbeeld 3

|         | Prioriteit website | Prijs website | Standaardinstellingen gebruiken |
|---------|------------------|---------------|-------------|
| Standaard | 0 | $ 31,99 | $ 30,00 |
| Winkel 1 | 1 | $ 24,99 | — |
| Winkel 2 | 2 | $ 27,99 | $ 20,00 |

Dit voorbeeld voegt de niet-prijswaarde toe, die wordt gebruikt als u een andere waarde voor _ [!UICONTROL Magento Price Source_] selecteert (die in uw [ wordt bepaald van de Prijs van de Lijst ](./listing-price.md) montages). De niet-prijswaarde gebruikt altijd de prijs als terugvalprijs.

- **[!UICONTROL Magento Price Source]** (gedefinieerd in [[!UICONTROL Listing Price]](./listing-price.md) settings) wordt ingesteld op `Non-Price` .
- Bekijk de website met de hoogste website prioriteit, die `Store 1` (die door de [ wordt bepaald van de Sorteervolgorde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) waarde) is.
- Aangezien Opslag 1 **niet** wordt geplaatst om het `Non-Price` attribuut te gebruiken, kijk de volgende website in de soortorde.
- Aangezien Opslag 2 **** wordt geplaatst om het `Non-Price` attribuut (niet-Prijs [ Website ] = $20.00) te gebruiken, is de gepubliceerde prijs $20.00.
