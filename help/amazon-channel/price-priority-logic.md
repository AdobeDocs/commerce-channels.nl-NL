---
title: Amazon-verkoopkanaal - Prijsprioriteitslogica
description: Verkoopkanaal in Amazon past prioriteitstelling toe bij het bepalen van de gepubliceerde prijs voor een Amazon-aanbieding.
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 4%

---

# Logica voor prijsprioriteiten

Hoe bepaalt het systeem in het volgende voorbeeld of u $31,99, $24,99 of $27,99 moet publiceren?

![Omvang van de handelsprijs](assets/amazon-price-scope.png){width="400"}

Om te bepalen welke prijs wordt gebruikt als een product op twee websites staat en een variabele prijs per website heeft, gebruikt u de logica voor prijsprioriteit (bepaald door de [Sorteervolgorde](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) waarde).

Ga naar **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** in de _Beheerder_ zijbalk. In de _[!UICONTROL Web Site]_klikt u op de naam van de website. De_[!UICONTROL Web Site Information]_ pagina toont de _[!UICONTROL Sort Order]_Hiermee stelt u de website in, die de prioriteit van de website bepaalt. Een waarde van `1` geeft de hoogste prioriteit aan.

Als de productprijs is ingesteld op `Use Default`, wordt de standaardprijs in plaats van de prijs van de website teruggebracht.

## Voorbeeld 1

|         | Prioriteit website | Prijs (website) | Standaardinstellingen gebruiken |
|---------|------------------|-----------------|-------------|
| Standaard | 0 | $31.99 | — |
| Winkel 1 | 1 | $24.99 | Nee |
| Winkel 2 | 2 | $27.99 | Ja |

- De **[!UICONTROL Magento Price Source]** (gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) is ingesteld op `Price` kenmerk.
- Kijk naar de website met de hoogste prioriteit voor de website, Store 1 (gedefinieerd door de [Sorteervolgorde](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) waarde).
- Aangezien Store 1 is ingesteld op het gebruik van de websiteprijs (Standaardinstelling gebruiken = Nee), is de gepubliceerde prijs $24,99.

## Voorbeeld 2

|         | Prioriteit website | Prijs website | Standaardinstellingen gebruiken |
|---------|------------------|---------------|-------------|
| Standaard | 0 | $31.99 | -- |
| Winkel 1 | 1 | $24.99 | Ja |
| Winkel 2 | 2 | $27.99 | Nee |

- De **[!UICONTROL Magento Price Source]** (gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) is ingesteld op `Price` kenmerk.
- Kijk naar de website met de hoogste prioriteit voor de website, Store 1 (gedefinieerd door de [sorteervolgorde](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) waarde).
- Sinds winkel 1 **is niet** ingesteld op het gebruik van de websiteprijs (Standaard gebruiken = Ja), bekijkt u de volgende website in de sorteervolgorde.
- Sinds winkel 2 **is** De gepubliceerde prijs is $27,99 en is ingesteld op gebruik van de websiteprijs (Standaard gebruiken = Nee).

## Voorbeeld 3

|         | Prioriteit website | Prijs website | Standaardinstellingen gebruiken |
|---------|------------------|---------------|-------------|
| Standaard | 0 | $31.99 | $30.00 |
| Winkel 1 | 1 | $24.99 | -- |
| Winkel 2 | 2 | $27.99 | $20.00 |

In dit voorbeeld wordt de niet-prijswaarde toegevoegd. Deze waarde wordt gebruikt wanneer u een andere waarde voor de _ selecteert[!UICONTROL Magento Price Source_] (gedefinieerd in uw [Aanbiedingsprijs](./listing-price.md) instellingen). De niet-prijswaarde gebruikt altijd de prijs als terugvalprijs.

- De **[!UICONTROL Magento Price Source]** (gedefinieerd in [[!UICONTROL Listing Price]](./listing-price.md) (instellingen) is ingesteld op `Non-Price`.
- Kijk naar de website met de hoogste prioriteit voor de website, namelijk `Store 1`(gedefinieerd door de [Sorteervolgorde](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) waarde).
- Sinds winkel 1 **is niet** ingesteld op `Non-Price` -kenmerk, bekijkt u de volgende website in de sorteervolgorde.
- Sinds winkel 2 **is** ingesteld op `Non-Price` attribute (Non-Price) [Website] = $ 20,00) is de gepubliceerde prijs $ 20,00.
