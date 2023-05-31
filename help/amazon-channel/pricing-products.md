---
title: Amazon-prijzen beheren
description: Je kunt de prijzen voor je Amazon-aanbiedingen op basis van de prijsregels instellen zodat ze afwijken van je winkels.
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 077d680da3c98ef9a48958eb548a9d5c1612f74e
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# Amazon-prijzen beheren

Met het verkoopkanaal van Amazon kunt u prijsregels instellen waarmee je de prijs van je Amazon-aanbieding kunt wijzigen van de gedefinieerde **[!UICONTROL Magento Price Source]** in uw [aanbiedingsprijs](./listing-price.md). Je kunt ook meerdere regels stapelen en zelfs de intelligente prijs gebruiken om de prijs van je Amazon-aanbieding aan te passen op basis van de prijs van je concurrenten. [[!DNL Buy Box]](./buy-box-competitor-pricing.md) de [laagste prijs van de concurrent](./lowest-competitor-pricing.md).

Er zijn twee soorten prijsregels:

- [Standaardprijsregel](./standard-price-rules.md)
- [Intelligente regel voor herstelling](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >Intelligente prijsstellingsregels functioneren niet naar behoren als de Amazon-regio is ingesteld op `Inactive` status, zoals tijdens het instappen. Je prijsberekeningen zijn afhankelijk van je verzendkosten en je regio moet binnen zijn `Active` status voor je verzendkosten die je vanaf Amazon wilt synchroniseren.
   >
   >Ga naar Instellingen > Accountinformatie > Vakantie-instellingen om de status van uw regio in uw Amazon-account bij te werken. Zie [Amazon: Aanbiedingsstatus voor vakanties](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620) (Aanmelden bij Verkoper is vereist).

Met deze functie kun je je Amazon-prijzen op een vergelijkbare manier manipuleren als met de [!DNL Commerce] [catalogusprijsregels](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html). U kunt complexe regels maken waarmee u de prijzen voor specifieke producten, producten binnen specifieke categorieën of zelfs met specifieke kenmerken kunt wijzigen.

Je kunt prijsregels toevoegen voor je Amazon-aanbiedingen. Met prijsregels kun je je aanbiedingsprijzen automatisch aanpassen op basis van een aantal gedefinieerde voorwaarden. De prijsregels worden geactiveerd en de aangepaste prijs wordt berekend voordat je product op Amazon wordt aangeboden.

>[!NOTE]
>
>De prijsbron voor je Amazon-aanbiedingen is gedefinieerd voor **[!UICONTROL Magento Price Source]** in uw [aanbiedingsprijs](./listing-price.md) instellingen. Bij alle aanpassingsberekeningen die in de prijsregel worden gedefinieerd, wordt de bron van de prijs als startwaarde gebruikt.

Met prijsregels kun je een andere prijs voor aanbiedingen in Amazon instellen dan je **[!UICONTROL Magento Price Source]** in uw [aanbiedingsprijs](./listing-price.md) instellingen. U kunt ook meerdere regels stapelen die samenwerken om de prijs aan te passen.

Voor een prijsstellings-/prijsstellingsregel zijn drie sets gegevens vereist tijdens de installatie:

- [Algemene instellingen](./pricing-rule-general-settings.md): Bepaalt de naam, de beschrijving, de actieve data, de prioriteit voor een regel en plaatst het gedrag van verdere regels, die op zijn prioritaire plaatsen worden gebaseerd.
- [Voorwaarden](./pricing-rule-conditions.md): Bepalen welke producten in aanmerking komen voor de prijsregel.
- [Handelingen](./pricing-rule-actions.md): Definieer de aanpassingsberekeningen die op de prijsbron worden toegepast om de aanbiedingsprijs te bepalen.

U kunt [standaardprijsregels](./standard-price-rules.md) waarmee je Amazon-aanbiedingsprijs automatisch wordt aangepast ten opzichte van de geselecteerde **[!UICONTROL Magento Price Source]** in uw [aanbiedingsprijs](./listing-price.md) instellingen. Met deze functie kun je je Amazon-prijzen op een vergelijkbare manier manipuleren als met de [!DNL Commerce] [catalogusprijsregels](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html). U kunt complexe regels maken die automatisch de prijzen voor specifieke producten, producten binnen specifieke categorieën of producten met specifieke kenmerken wijzigen. U kunt traditionele instellingen voltooien en de prijs van uw producten wijzigen om deze te verhogen of te verlagen op basis van een vaste hoeveelheid of een percentage.

Een ander krachtig gereedschap is het [Intelligente reparatie](./intelligent-repricing-rules.md) functie waarmee je Amazon-aanbiedingsprijs op basis van een concurrent wordt aangepast [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prijs of [Laagste concurrent](./lowest-competitor-pricing.md). Vergelijkbaar met de [!DNL Commerce] [catalogusprijsregels](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html)Met deze geavanceerde functie kun je je Amazon-prijzen manipuleren door complexe regels te maken. De regels kunnen de ruimte voor een prijsverandering voor specifieke producten, producten binnen specifieke categorieën, of zelfs met specifieke productkenmerken bepalen.

Intelligente prijsstelling gebruiken om je Amazon-aanbiedingsprijzen aan te passen op basis van de prijs van de concurrent. Het verkoopkanaal van Amazon heeft ingebouwde waarborgen voor u gebouwd om marges te beschermen te vormen of te vermijden aanpassing van de prijzen van een handelaar met laag terugkoppelt. Gebruiken [intelligente tariefregels](./intelligent-repricing-rules.md), Amazon-aanbiedingsprijzen kunnen automatisch worden gemanipuleerd als een vast bedrag of als een percentage (omhoog of omlaag) of zelfs worden gesynchroniseerd met de [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prijs of [Laagste concurrent](./lowest-competitor-pricing.md) per post. Regels kunnen zelfs worden gestapeld om onbeperkte flexibiliteit te bieden.

U kunt belangrijke aspecten van regels beheren, zoals actieve/inactieve status, geschiktheid van websites, optionele datumbereiken en optionele prioriteitsniveaus (gebruikt voor het stapelen van regels).

Je kunt bijvoorbeeld de voorwaarden voor een prijsregel definiëren en instellen die, wanneer aan de voorwaarden wordt voldaan, automatisch je aanbiedingsprijs aanpast voordat deze naar Amazon wordt verzonden.

Een andere prijsstellingsoptie is een [prijsoverschrijving](./overrides.md), die wordt ingesteld op het niveau van de afzonderlijke aanbiedingen. A [prijsoverschrijving](./overrides.md) kan worden ingesteld en een overschrijving negeert/neemt prioriteit over alle andere standaardwaarden, instellingen en regels. An [override](./overrides.md) kan worden ingesteld op prijs, verwerkingstijd, voorwaarde en verkopersnotities (met een paar uitzonderingen).

![Prijsregels](assets/amazon-pricing-rules.png){width="600" zoomable="yes"}

## Standaardkolommen

| Kolom | Beschrijving |
|---|---|
| [!UICONTROL Name] | De naam van de prijsregel, zoals ingesteld in [Algemene instellingen prijsregel](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Het regeltype, zoals ingesteld in [Handelingen voor prijsregel](./pricing-rule-actions.md) (Standaardprijsregel of Intelligent repricing rule) |
| [!UICONTROL Is Active] | Of de regel actief is, zoals ingesteld in [Algemene instellingen prijsregel](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | De prioriteit boven andere prijsvoorwaarden, zoals vastgesteld in [Algemene instellingen prijsregel](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Geeft aan of verdere prijsregels worden verwerkt voor producten die in aanmerking komen voor deze regel, zoals vastgesteld in [algemene prijsregel](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | Het begin van de periode waarin de regel actief is |
| [!UICONTROL To Date] | Het einde van de periode waarin de regel actief is |
| [!UICONTROL Action] | Hiermee worden alle acties weergegeven die op een specifieke aanbieding kunnen worden toegepast. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de _[!UICONTROL Action]_kolom. Opties: `Edit Price Rule` / `Delete Price Rule` |
