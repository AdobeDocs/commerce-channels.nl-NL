---
title: Pre-setup taken voor  [!DNL Amazon sales channel]
description: Controleer de vereiste taken die moeten worden voltooid voordat u uw Adobe Commerce- of Magento Open Source-winkel in Amazon-Sales Channel integreert.
role: Admin, Developer
feature: Sales Channels, Install, Configuration
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Pre-setingstaken voor [!DNL Amazon sales channel]

Vóór [ de Integratie van de Opslag ](./store-integration.md), moet u ervoor zorgen dat uw [!DNL Amazon Seller Central] rekening en uw [!DNL Commerce] rekening voor de integratie klaar zijn. Voor een geslaagde integratie zijn er enkele vereiste voorbereidingstaken nodig.

Wanneer u uw eerste Amazon-winkel instelt in Amazon-verkoopkanaal, wordt een lijst met instellingstaken weergegeven. Het wordt geadviseerd dat u deze taken alvorens u [ bekijkt een opslag van Amazon ](./store-integration.md) toevoegt. Na het toevoegen van uw eerste opslag, kunt u deze taken in het Leren en de mening van de Voorbereiding van de het verkoopkanaal van Amazon [ homepage ](./amazon-sales-channel-home.md) herzien.

## 1. Schakel achtergrondtaken in [!DNL Commerce]

Alle producten en gegevens die tussen [!DNL Commerce] en Amazon worden gesynchroniseerd worden beheerd door de baan van de a [ cron ](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html). Wanneer u alle taken hebt voltooid, zoals het toevoegen of bijwerken van aanbiedingen en het ontvangen van bestellingen, verzendt en ontvangt een uitsnijdtaak gegevens tussen uw [!DNL Commerce] backend en uw [!DNL Amazon Seller Central] -account.

- [ laat  [!DNL Commerce]  kroon ](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) toe.

- Voor maximumprestaties, [ plaats  [!DNL Commerce]  kroon ](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html) om eens om de vijf minuten in werking te stellen.

## 2. Maak uw [!DNL Amazon Seller Central] -account

Voordat u begint met het instellen van het verkoopkanaal van Amazon, moet u een actieve [!DNL Amazon Seller Central] account hebben. Als u geen bestaande Amazon Seller rekening in [ Noord-Amerika (V.S., CA, MX) ](https://sell.amazon.com/) {target="_blank"} of [ Europees (VK) ](https://sell.amazon.co.uk/sell-online/beginners-guide) {target="_blank"} gebied hebt, kunt u het proces van de de rekeningsopstelling van de Amazon-verkopersrekening voltooien.

Voor Amazon-verkoopkanaal is een [!DNL Professional Seller] -account op [!DNL Amazon Seller Central] vereist. Amazon brengt maandelijks een abonnement en verkoopkosten in rekening. Zie [ Amazon: Kies uw het verkopen plan ](https://sell.amazon.com/pricing.html) {target="_blank"}.

## 3. Controleer of je een goedgekeurde Amazon-verkoper bent

U moet een goedgekeurd [!DNL Amazon Seller Central] account hebben om te kunnen integreren. Je account mag geen beperkingen hebben voor producten of rubrieken. Voor sommige producten en categorieën is goedkeuring vereist voordat aanbiedingen worden gemaakt. Bekijk het Amazon-beleid voor rubriek en productgoedkeuring om te controleren of je producten zijn goedgekeurd. Zie [ Amazon: Categorieën en producten die goedkeuring ](https://sellercentral.amazon.com/gp/help/200333160) vereisen {target="_blank"} (vereist de Centrale login van de Verkoper).

Het is ook belangrijk om ervoor te zorgen dat u het volgende hebt geconfigureerd in uw [!DNL Amazon Seller Central] account:

- Zorg ervoor dat je retourbeleid net zo goed is als of beter is dan het retourbeleid van Amazon. Zie [ Amazon: Het Beleid van de terugkeer ](https://www.amazon.com/gp/help/customer/display.html) {target="_blank"}.

- Zorg ervoor dat de belastinginstellingen zijn geconfigureerd. Zie [ Amazon: Belastingsbeleid ](https://sellercentral.amazon.com/gp/help/external/help.html) {target="_blank"} (vereist de Centrale login van de Verkoper).

- Zorg ervoor dat uw verzendmethoden correct zijn geconfigureerd. Aan opstelling worden de verschepende methodes die [!DNL Commerce] aan klanten worden aangeboden om uw orden van Amazon te vervullen, update [ Amazon: het verschepen Montages ](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates) {target="_blank"} in uw [!DNL Amazon Seller Central] rekening.

## 4. Controleer of de BTW is geconfigureerd voor uw winkels

(Hoofdzakelijk gebruikt door Britse verkopers.) Amazon adviseert omhoog het ondertekenen voor de [ Dienst van de Berekening van Amazon BTW ](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon) {target="_blank"}. Als u een andere methode kiest, bent u verantwoordelijk voor de naleving van de BTW.

>[!NOTE]
>
>Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

## 5. Verhoog het aantal automatische overeenkomende catalogi

Tijdens het instappen gebruikt het verkoopkanaal van Amazon productkenmerken om bestaande Amazon-aanbiedingen (indien van toepassing) aan bestaande producten in uw catalogus van [!DNL Commerce] aan te passen. Na het instappen worden deze productkenmerken gebruikt om uw catalogusitems van [!DNL Commerce] te publiceren naar een Amazon-aanbieding en om uw productgegevens te synchroniseren tussen [!DNL Commerce] en Amazon.

Als het hoogste aantal [!DNL Commerce] -producten automatisch overeenkomt met Amazon-aanbiedingen, moet u een set productkenmerken voor uw [!DNL Commerce] -catalogus maken. Voordat u de Amazon-winkel voor verkoopkanalen instelt, moet u [!DNL Commerce] -productkenmerken toevoegen die overeenkomen met deze Amazon-kenmerken, zoals ASIN, EAN, ISBN, UPC of GCID. Zie [ een productattribuut in  [!DNL Commerce]](./ob-creating-magento-attributes.md) creëren.

## 6. Uw valuta en conversie configureren (indien nodig)

Als uw opslag van Amazon een verschillende munt gebruikt dan voor uw [!DNL Commerce] opslag wordt gevormd, [ laat de munt ](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) toe en plaatst de [ wisselkoers omzettingspercentage ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html).

## 7. Maak een kenmerk voor de productvoorwaarde (indien nodig)

Als uw lijsten van Amazon meer dan één productvoorwaarde (zoals _nieuw_ bevatten, _gebruikt_, of _als nieuw_), creeer een [!DNL Commerce] attribuut en wijs voorwaardenwaarden toe. U moet dit kenmerk tijdens het instappen toewijzen aan het Amazon Condition-productkenmerk. Zie [ Creërend Attributen voor Amazon ](./ob-creating-magento-attributes.md).

## 8. Configureer uw verzendmethode [!DNL Amazon Seller Central]

Om opstellings verschepende methodes aan te bieden die u voor het vervullen van uw orden van Amazon wilt aanbieden, verwijs naar _Montages &amp; het verschepen Montages_ in uw [!DNL Amazon Seller Central] rekening.

## Aanvullende configuraties

Wanneer uw Amazon-account is ingesteld en geactiveerd, zijn er verschillende [!DNL Commerce] -aanbevelingen die het instapproces voor Amazon-verkoopkanalen helpen stroomlijnen.

### Bekijk en noteer alle producten die u wilt uitsluiten

Mogelijk wilt u niet dat bepaalde producten op Amazon worden vermeld. Het verkoopkanaal van Amazon heeft een regelengine voor aanbiedingen die wordt gebruikt om te bepalen welke producten in aanmerking komen voor publicatie naar Amazon. [ van de lijst de regels ](./listing-rules.md) staan u toe om ondergroepen van producten te selecteren die (of niet gepubliceerd) aan uw [!DNL Amazon Seller Central] rekening, zoals door categorieselectie moeten worden gepubliceerd of door één of meerdere productattributen te bepalen. Als [!DNL Commerce] [ catalogus ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) of [ het winkelwagentje ](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) prijsregels, moeten de productattributen die voor de lijst van Amazon worden gebruikt **[!UICONTROL Use for Promo Rule Conditions]** hebben aan `Yes` worden geplaatst. Zie **[!UICONTROL Use for Promo Rule Conditions]** in [ Attributen van het Product ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

### Plaats uw [!DNL Amazon Seller Central] gebied aan inactief

Als u de gegevensovergang zonder fouten tijdens de integratie wilt vergemakkelijken, kunt u het beste uw Amazon-regio instellen op `Inactive` status in Instellingen > Accountinformatie > Vakantie-instellingen. Wijzig de status terug naar `Active` in Amazon wanneer de installatie is voltooid.

![ Volgende pictogram ](assets/btn-next.png) [**ga aan het Creëren van [!DNL Commerce] Attributen**](./ob-creating-magento-attributes.md)
