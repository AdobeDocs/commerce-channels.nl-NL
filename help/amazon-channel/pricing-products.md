---
title: Amazon-prijzen beheren
description: Je kunt de prijzen voor je Amazon-aanbiedingen op basis van de prijsregels instellen zodat ze afwijken van je winkels.
redirect_from: /sales-channels/asc/ob-pricing-rules.html: 
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 865
ht-degree: 0%

---

# Amazon-prijzen beheren

Met het verkoopkanaal van Amazon kunt u prijsregels instellen waarmee u de prijs van je Amazon-aanbieding kunt wijzigen in de prijs van je **[!UICONTROL Magento Price Source]** in je [aanbiedingsprijs](./listing-price.md). U kunt ook meerdere regels stapelen en zelfs de intelligente prijs gebruiken om de Amazon-aanbiedingsprijs aan te passen op basis van de [[!DNL Buy Box]](./buy-box-competitor-pricing.md)-prijs van de concurrent of de [laagste prijs van de concurrent](./lowest-competitor-pricing.md).

Er zijn twee soorten prijsregels:

- [Standaardprijsregel](./standard-price-rules.md)
- [Intelligente regel voor herstelling](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >Intelligente prijsstellingsregels werken niet correct als de Amazon-regio is ingesteld op `Inactive`-status, zoals tijdens instapweigering. Uw prijsberekeningen zijn afhankelijk van uw verzendkosten en uw regio moet de status `Active` hebben om de verzendkosten te synchroniseren vanaf Amazon.
   >
   >Ga naar Instellingen > Accountinformatie > Vakantie-instellingen om de status van uw regio in uw Amazon-account bij te werken. Zie [Amazon: Aanbiedingsstatus voor Vakantie](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620){:target=&quot;_blank&quot;} (Aanmelding voor Verkoper Central vereist).

Met deze functie kunt u uw Amazon-prijzen op vergelijkbare wijze manipuleren als de [!DNL Commerce] [catalogusprijsregels](https://docs.magento.com/user-guide/catalog/pricing.html){:target=&quot;_blank&quot;}. U kunt complexe regels maken waarmee u de prijzen voor specifieke producten, producten binnen specifieke categorieën of zelfs met specifieke kenmerken kunt wijzigen.

Je kunt prijsregels toevoegen voor je Amazon-aanbiedingen. Met prijsregels kun je je aanbiedingsprijzen automatisch aanpassen op basis van een aantal gedefinieerde voorwaarden. De prijsregels worden geactiveerd en de aangepaste prijs wordt berekend voordat je product op Amazon wordt aangeboden.

>[!NOTE]
>
>De prijsbron voor je Amazon-aanbiedingen is gedefinieerd voor **[!UICONTROL Magento Price Source]** in je [aanbiedingsprijs](./listing-price.md)-instellingen. Bij alle aanpassingsberekeningen die in de prijsregel worden gedefinieerd, wordt de bron van de prijs als startwaarde gebruikt.

Met prijsregels kunt u de Amazon-aanbiedingsprijs anders instellen dan de **[!UICONTROL Magento Price Source]** in uw [aanbiedingsprijs](./listing-price.md)-instellingen. U kunt ook meerdere regels stapelen die samenwerken om de prijs aan te passen.

Voor een prijsstellings-/prijsstellingsregel zijn drie sets gegevens vereist tijdens de installatie:

- [Algemene instellingen](./pricing-rule-general-settings.md): Bepaalt de naam, de beschrijving, de actieve data, de prioriteit voor een regel en plaatst het gedrag van verdere regels, die op zijn prioritaire plaatsen worden gebaseerd.
- [Voorwaarden](./pricing-rule-conditions.md): Bepalen welke producten in aanmerking komen voor de prijsregel.
- [Handelingen](./pricing-rule-actions.md): Definieer de aanpassingsberekeningen die op de prijsbron worden toegepast om de aanbiedingsprijs te bepalen.

U kunt [standaardprijsregels](./standard-price-rules.md) maken waarmee de Amazon-aanbiedingsprijs automatisch wordt aangepast ten opzichte van de geselecteerde **[!UICONTROL Magento Price Source]** in de [aanbiedingsprijs](./listing-price.md)-instellingen. Met deze functie kunt u uw Amazon-prijzen op vergelijkbare wijze manipuleren als de [!DNL Commerce] [catalogusprijsregels](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){:target=&quot;_blank&quot;}. U kunt complexe regels maken die automatisch de prijzen voor specifieke producten, producten binnen specifieke categorieën of producten met specifieke kenmerken wijzigen. U kunt traditionele instellingen voltooien en de prijs van uw producten wijzigen om deze te verhogen of te verlagen op basis van een vaste hoeveelheid of een percentage.

Een ander krachtig hulpmiddel is de [Intelligente Repricing](./intelligent-repricing-rules.md) eigenschap die uw Amazon aanbiedingsprijs op concurrerende [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prijs of [Laagste Concurrentieprijs](./lowest-competitor-pricing.md) aanpast. Net als de [!DNL Commerce] [catalogusprijsregels](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){:target=&quot;_blank&quot;} kunt u met deze geavanceerde functie uw Amazon-prijzen manipuleren door complexe regels te maken. De regels kunnen de mogelijkheid van een prijswijziging voor specifieke producten, producten binnen specifieke categorieën of zelfs met specifieke productkenmerken bepalen.

Intelligente prijsstelling gebruiken om je Amazon-aanbiedingsprijzen aan te passen op basis van de prijs van de concurrent. Het verkoopkanaal van Amazon heeft ingebouwde waarborgen voor u gebouwd om marges te beschermen te vormen of te vermijden aanpassing van de prijzen van een handelaar met laag terugkoppelt. Met behulp van [intelligente regels voor herprijzing](./intelligent-repricing-rules.md) kunnen beurskoersen in Amazon automatisch worden gemanipuleerd als een vast bedrag of een percentage (omhoog of omlaag) of zelfs worden gesynchroniseerd met de [[!DNL Buy Box]](./buy-box-competitor-pricing.md)-prijs of [Laagste concurrent Price](./lowest-competitor-pricing.md) per item. Regels kunnen zelfs worden gestapeld om onbeperkte flexibiliteit te bieden.

U kunt belangrijke aspecten van regels beheren, zoals actieve/inactieve status, geschiktheid van websites, optionele datumbereiken en optionele prioriteitsniveaus (gebruikt voor het stapelen van regels).

Je kunt bijvoorbeeld de voorwaarden voor een prijsregel definiëren en instellen die, wanneer aan de voorwaarden wordt voldaan, automatisch je aanbiedingsprijs aanpast voordat deze naar Amazon wordt verzonden.

Een andere prijsoptie is een [prijsoverschrijving](./overrides.md), die op het individuele aanbiedingsniveau wordt geplaatst. Een [prijsopheffing](./overrides.md) kan worden geplaatst, en een opheffing negeert/neemt prioriteit over alle andere gebreken, montages, en regels. Een [override](./overrides.md) kan worden ingesteld voor prijs, verwerkingstijd, voorwaarde en verkopersnotities (met een paar uitzonderingen).

![Prijsregels](assets/amazon-pricing-rules.png)

## Standaardkolommen

| Kolom | Beschrijving |
|---|---|
| [!UICONTROL Name] | De naam van de prijsregel, zoals ingesteld in [Algemene instellingen van prijsregel](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Het regeltype, zoals ingesteld in [Pricing Rule Actions](./pricing-rule-actions.md) (Standard price rule of Intelligent repricing rule) |
| [!UICONTROL Is Active] | Of de regel actief is, zoals ingesteld in [Algemene instellingen van prijsregel](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | De prioriteit boven andere prijsvoorwaarden, zoals ingesteld in [Algemene instellingen van prijsregel](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Geeft aan of verdere prijsregels worden verwerkt op producten die in aanmerking komen voor deze regel, zoals vastgesteld in [algemene prijsregels](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | Het begin van de periode waarin de regel actief is |
| [!UICONTROL To Date] | Het einde van de periode waarin de regel actief is |
| [!UICONTROL Action] | Hiermee worden alle acties weergegeven die op een specifieke aanbieding kunnen worden toegepast. Als u een handeling wilt toepassen, klikt u op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_. Opties: `Edit Price Rule` / `Delete Price Rule` |
