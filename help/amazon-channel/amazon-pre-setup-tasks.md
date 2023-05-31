---
title: Taken vooraf instellen voor [!DNL Amazon sales channel]
description: Controleer de vereiste taken die moeten worden voltooid voordat u uw Adobe Commerce- of Magento Open Source-winkel in Amazon Sales Channel integreert.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# Taken vooraf instellen voor [!DNL Amazon sales channel]

Voor [Opslagintegratie](./store-integration.md)moet u ervoor zorgen dat uw [!DNL Amazon Seller Central] account en uw [!DNL Commerce] -account is klaar voor integratie. Voor een geslaagde integratie zijn er enkele vereiste voorbereidingstaken nodig.

Wanneer u uw eerste Amazon-winkel instelt in Amazon-verkoopkanaal, wordt een lijst met instellingstaken weergegeven. U wordt aangeraden deze taken te controleren voordat u [een Amazon-winkel toevoegen](./store-integration.md). Nadat u de eerste winkel hebt toegevoegd, kunt u deze taken bekijken in de weergave Leren en voorbereiden van het Amazon-verkoopkanaal [homepage](./amazon-sales-channel-home.md).

## 1. Achtergrondtaken inschakelen in [!DNL Commerce]

Alle producten en gegevens gesynchroniseerd tussen [!DNL Commerce] en Amazon wordt beheerd door een [snijtaak](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html). Wanneer u alle taken hebt voltooid, zoals het toevoegen of bijwerken van aanbiedingen en het ontvangen van bestellingen, verzendt en ontvangt een uitsnijdtaak gegevens tussen uw [!DNL Commerce] en uw [!DNL Amazon Seller Central] account.

- [Inschakelen [!DNL Commerce] kraan](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html).

- Voor maximale prestaties [set [!DNL Commerce] kraan](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html) om de vijf minuten te draaien.

## 2. Maak uw [!DNL Amazon Seller Central] account

Voordat je een verkoopkanaal voor Amazon instelt, moet je over een actieve [!DNL Amazon Seller Central] account. Als je geen bestaande Amazon-verkopersaccount hebt in het dialoogvenster [Noord-Amerika (VS, CA, MX)](https://sell.amazon.com/){target="_blank"} or [European (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} -regio, kunt u het installatieproces van een Amazon-verkopersaccount voltooien.

Amazon-verkoopkanaal vereist een [!DNL Professional Seller] account op [!DNL Amazon Seller Central]. Amazon brengt maandelijks een abonnement en verkoopkosten in rekening. Zie [Amazon: Kies je verkoopplan](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3. Ervoor zorgen dat je een goedgekeurde Amazon-verkoper bent

Voor integratie moet u beschikken over een goedgekeurd [!DNL Amazon Seller Central] account. Je account mag geen beperkingen hebben voor producten of rubrieken. Voor sommige producten en categorieën is goedkeuring vereist voordat aanbiedingen worden gemaakt. Bekijk het Amazon-beleid voor rubriek en productgoedkeuring om te controleren of je producten zijn goedgekeurd. Zie [Amazon: Categorieën en producten waarvoor goedkeuring vereist is](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} (Aanmelden bij Verkoper is vereist).

Het is ook belangrijk om ervoor te zorgen dat u het volgende in uw hebt gevormd [!DNL Amazon Seller Central] account:

- Zorg ervoor dat je retourbeleid even goed is als of beter is dan het retourbeleid van Amazon. Zie [Amazon: Retourbeleid](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- Zorg ervoor dat de belastinginstellingen zijn geconfigureerd. Zie [Amazon: Belastingbeleid](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} (Aanmelden bij Verkoper is vereist).

- Zorg ervoor dat uw verzendmethoden correct zijn geconfigureerd. De verzendmethoden instellen die [!DNL Commerce] worden aangeboden aan klanten om aan uw Amazon-bestellingen te voldoen, de [Amazon: Verzendinstellingen](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} in uw [!DNL Amazon Seller Central] account.

## 4. Zorg ervoor dat de BTW is geconfigureerd voor uw winkels

(Hoofdzakelijk gebruikt door verkopers in het Verenigd Koninkrijk.) Amazon raadt u aan zich aan te melden voor de [Amazon BTW-berekeningsservice](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}. Als u een andere methode kiest, bent u verantwoordelijk voor de naleving van de BTW.

>[!NOTE]
>
>Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

## 5. Het aantal automatische overeenkomende catalogi verhogen

Tijdens het instappen gebruikt het verkoopkanaal van Amazon productkenmerken om bestaande Amazon-aanbiedingen (indien van toepassing) aan bestaande producten in je [!DNL Commerce] catalogus. Na het instappen, worden deze productattributen gebruikt om uw te publiceren [!DNL Commerce] objecten catalogiseren naar een Amazon-aanbieding en de productgegevens synchroniseren tussen [!DNL Commerce] en Amazon.

Het hoogste aantal [!DNL Commerce] producten komen automatisch overeen met Amazon-aanbiedingen. Maak een set productkenmerken voor je [!DNL Commerce] catalogus. Voordat u de Amazon-winkel voor verkoopkanalen instelt, moet u [!DNL Commerce] productkenmerken die overeenkomen met deze Amazon-kenmerken, bijvoorbeeld: ASIN, EAN, ISBN, UPC of GCID. Zie [Een productkenmerk maken in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Uw valuta en conversie configureren (indien nodig)

Als je Amazon-winkel een andere valuta gebruikt dan voor jouw configuratie [!DNL Commerce] opslaan, [de munt](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) en stelt de [valutakoers](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html).

## 7. Een kenmerk voor de productvoorwaarde maken (indien nodig)

Als je Amazon-aanbiedingen meer dan één productvoorwaarde bevatten, zoals _new_, _gebruikt_, of _zoals nieuw_), een [!DNL Commerce] en wijs voorwaardenwaarden toe. U moet dit kenmerk tijdens het instappen toewijzen aan het Amazon Condition-productkenmerk. Zie [Kenmerken maken voor Amazon](./ob-creating-magento-attributes.md).

## 8. Configureer uw [!DNL Amazon Seller Central] verzendmethode

Als u verzendmethoden wilt instellen om aan uw Amazon-bestellingen te voldoen, raadpleegt u _Instellingen en verzendinstellingen_ in uw [!DNL Amazon Seller Central] account.

## Aanvullende configuraties

Als je Amazon-account is ingesteld en geactiveerd, zijn er verschillende [!DNL Commerce] aanbevelingen die helpen het Amazon verkoopkanaal aan boord nemen te stroomlijnen.

### Bekijk en noteer alle producten die u wilt uitsluiten

Mogelijk wilt u niet dat bepaalde producten op Amazon worden vermeld. Het verkoopkanaal van Amazon heeft een regelengine voor aanbiedingen die wordt gebruikt om te bepalen welke producten in aanmerking komen voor publicatie naar Amazon. [Aanbiedingsregels](./listing-rules.md) u toestaan om ondergroepen van producten te selecteren die (of niet gepubliceerd) aan uw [!DNL Amazon Seller Central] -account, bijvoorbeeld op categorie of door een of meer productkenmerken te definiëren. leuk [!DNL Commerce] [catalogus](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) of [winkelwagentje](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) prijsregels, productkenmerken die worden gebruikt om in aanmerking te komen voor Amazon-aanbiedingen, moeten **[!UICONTROL Use for Promo Rule Conditions]** instellen op `Yes`. Zie de **[!UICONTROL Use for Promo Rule Conditions]** in [Productkenmerken](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

### Stel uw [!DNL Amazon Seller Central] regio naar inactief

Als u de overgang van foutloze gegevens tijdens de integratie wilt vergemakkelijken, kunt u het beste de Amazon-regio instellen op `Inactive` status in Instellingen > Accountinformatie > Vakantie-instellingen. Wanneer de installatie is voltooid, wijzigt u de status weer in `Active` in Amazon.

![Volgende pictogram](assets/btn-next.png) [**Doorgaan met maken [!DNL Commerce] Attributen**](./ob-creating-magento-attributes.md)
