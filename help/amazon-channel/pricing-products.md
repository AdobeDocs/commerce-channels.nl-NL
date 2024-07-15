---
title: Amazon-prijzen beheren
description: Je kunt de prijzen voor Amazon-aanbiedingen zodanig instellen dat ze verschillen van je Commerce-winkel door de prijsregels te gebruiken.
feature: Sales Channels, Price Rules
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# Amazon-prijzen beheren

Het de verkoopkanaal van Amazon staat u toe om het tarief regels te plaatsen, die u toestaan om uw het lijstprijs van Amazon verschillend van bepaalde **[!UICONTROL Magento Price Source]** in uw [ lijstprijs ](./listing-price.md) te plaatsen. U kunt veelvoudige regels ook stapelen en zelfs de intelligente prijs gebruiken om uw Amazon lijstprijs aan te passen die op concurrenten&#39; [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prijs of [ wordt gebaseerd laagste concurrerende prijs ](./lowest-competitor-pricing.md).

Er zijn twee soorten prijsregels:

- [Standaardprijsregel](./standard-price-rules.md)
- [Intelligente regel voor herstelling](./intelligent-repricing-rules.md)

  >[!IMPORTANT]
  >
  >Intelligente prijsstellingsregels werken niet correct als de Amazon-regio is ingesteld op `Inactive` status, zoals tijdens het instappen. Je prijsberekeningen zijn afhankelijk van je verzendkosten en je regio moet de status `Active` hebben om de verzendkosten te synchroniseren vanuit Amazon.
  >
  >Ga naar Instellingen > Accountinformatie > Vakantie-instellingen om de status van uw regio in uw Amazon-account bij te werken. Verwijs naar [ Amazon: De Status van de lijst voor Vakantie ](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620) (vereist login van de Verkoper Centrale).

Deze eigenschap staat u toe om uw prijzen van Amazon op een manier te manipuleren die aan de [!DNL Commerce] [ regels van de catalogusprijs ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html) gelijkaardig is. U kunt complexe regels maken waarmee u de prijzen voor specifieke producten, producten binnen specifieke categorieën of zelfs met specifieke kenmerken kunt wijzigen.

Je kunt prijsregels toevoegen voor je Amazon-aanbiedingen. Met prijsregels kun je je aanbiedingsprijzen automatisch aanpassen op basis van een aantal gedefinieerde voorwaarden. De prijsregels worden geactiveerd en de aangepaste prijs wordt berekend voordat je product op Amazon wordt aangeboden.

>[!NOTE]
>
>De prijsbron voor uw aanbiedingen van Amazon wordt bepaald voor **[!UICONTROL Magento Price Source]** in uw [ aanbiedingsprijsmontages ](./listing-price.md). Bij alle aanpassingsberekeningen die in de prijsregel worden gedefinieerd, wordt de bron van de prijs als startwaarde gebruikt.

De prijsstellingsregels staan u toe om uw Amazon aanbiedingsprijs verschillend van uw **[!UICONTROL Magento Price Source]** in uw [ aanbiedingsprijs ](./listing-price.md) montages te plaatsen. U kunt ook meerdere regels stapelen die samenwerken om de prijs aan te passen.

Voor een prijsstellings-/prijsstellingsregel zijn drie sets gegevens vereist tijdens de installatie:

- [ Algemene montages ](./pricing-rule-general-settings.md): Bepaalt de naam, de beschrijving, de actieve data, de prioriteit voor een regel en plaatst het gedrag van verdere regels, die op zijn prioriteit het plaatsen worden gebaseerd.
- [ Voorwaarden ](./pricing-rule-conditions.md): Bepaal welke producten voor de prijsregel in aanmerking komen.
- [ Acties ](./pricing-rule-actions.md): Bepaal de aanpassingsberekeningen die op de prijsbron worden toegepast om de lijstprijs te bepalen.

U kunt [ standaard het tarief regels ](./standard-price-rules.md) tot stand brengen die automatisch uw Amazon lijstprijs met betrekking tot geselecteerde **[!UICONTROL Magento Price Source]** in uw [ het lijstprijs ](./listing-price.md) montages aanpassen. Deze eigenschap staat u toe om uw prijzen van Amazon op een manier te manipuleren die aan de [!DNL Commerce] [ regels van de catalogusprijs ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) gelijkaardig is. U kunt complexe regels maken die automatisch de prijzen voor specifieke producten, producten binnen specifieke categorieën of producten met specifieke kenmerken wijzigen. U kunt traditionele instellingen voltooien en de prijs van uw producten wijzigen om deze te verhogen of te verlagen op basis van een vaste hoeveelheid of een percentage.

Een ander krachtig hulpmiddel is de [ Intelligente het Verprijzen ](./intelligent-repricing-rules.md) eigenschap die uw Amazon lijstprijs aanpast die op concurrent [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prijs wordt gebaseerd of [ Laagste Prijs van de Concurrent ](./lowest-competitor-pricing.md). Gelijkaardig aan de [!DNL Commerce] [ regels van de catalogusprijs ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html), staat deze geavanceerde eigenschap u toe om uw prijzen van Amazon te manipuleren door complexe regels te creëren. De regels kunnen de ruimte voor een prijsverandering voor specifieke producten, producten binnen specifieke categorieën, of zelfs met specifieke productkenmerken bepalen.

Intelligente prijsstelling gebruiken om je Amazon-aanbiedingsprijzen aan te passen op basis van de prijs van de concurrent. Het verkoopkanaal van Amazon heeft ingebouwde waarborgen voor u gebouwd om marges te beschermen te vormen of te vermijden aanpassing van de prijzen van een handelaar met laag terugkoppelt. Gebruikend [ intelligente het opnieuw bepalen regels ](./intelligent-repricing-rules.md), kunnen de beurskoersen van Amazon automatisch als vast of percentagebedrag (omhoog of neer) worden gemanipuleerd of zelfs aan de [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prijs of [ Laagste Prijs van de Concurrant ](./lowest-competitor-pricing.md) op een per puntbasis worden gesynchroniseerd. Regels kunnen zelfs worden gestapeld om onbeperkte flexibiliteit te bieden.

U kunt belangrijke aspecten van regels beheren, zoals actieve/inactieve status, geschiktheid van websites, optionele datumbereiken en optionele prioriteitsniveaus (gebruikt voor het stapelen van regels).

Je kunt bijvoorbeeld de voorwaarden voor een prijsregel definiëren en instellen die, wanneer aan de voorwaarden wordt voldaan, automatisch je aanbiedingsprijs aanpast voordat deze naar Amazon wordt verzonden.

Een andere het tarief optie is a [ prijsopheffing ](./overrides.md), die op het individuele lijstniveau wordt geplaatst. A [ prijsopheffing ](./overrides.md) kan worden geplaatst, en een opheffing negeert/neemt prioriteit over alle andere gebreken, montages, en regels. Een [ opheffing ](./overrides.md) kan voor prijs, behandelingstijd, voorwaarde, en verkopersnota&#39;s (met een paar uitzonderingen) worden geplaatst.

![ het Tarief regels ](assets/amazon-pricing-rules.png){width="600" zoomable="yes"}

## Standaardkolommen

| Kolom | Beschrijving |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Name] | De naam van de het tarief regel, zoals die in [ wordt geplaatst de Algemene Montages van de Regel Prijsende ](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Het regeltype, zoals die in [ wordt geplaatst die de Acties van de Regel van de Prijsprijs ](./pricing-rule-actions.md) (of de Standaardprijsregel of Intelligente het verrekenen regel) |
| [!UICONTROL Is Active] | Of de regel actief is, zoals die in [ wordt geplaatst het Prijsen Algemene Montages van de Regel ](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | De prioriteit over andere het tarief voorwaarden, zoals die in [ worden geplaatst het Prijsen Algemene Montages van de Regel ](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Wijst erop of om het even welke verdere prijsregels op producten die voor deze regel in aanmerking komen, zoals die in [ worden geplaatst de algemene montages van de prijsregel ](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | Het begin van de periode waarin de regel actief is |
| [!UICONTROL To Date] | Het einde van de periode waarin de regel actief is |
| [!UICONTROL Action] | Hiermee worden alle acties weergegeven die op een specifieke aanbieding kunnen worden toegepast. Klik op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_om een handeling toe te passen. Opties: `Edit Price Rule` / `Delete Price Rule` |
