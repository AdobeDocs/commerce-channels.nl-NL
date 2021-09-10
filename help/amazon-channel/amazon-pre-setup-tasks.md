---
title: Taken vooraf instellen
description: Controleer de vereiste taken die moeten worden voltooid voordat u uw Adobe Commerce- of Magento Open Source-winkel in Amazon Sales Channel integreert.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Taken vooraf instellen

Voordat u [Integratie van uw winkel](./store-integration.md) hebt, moet u ervoor zorgen dat uw [!DNL Amazon Seller Central]-account en uw [!DNL Commerce]-account gereed zijn voor integratie. Voor een geslaagde integratie zijn er enkele vereiste voorbereidingstaken nodig.

Wanneer u uw eerste Amazon-winkel instelt in Amazon-verkoopkanaal, wordt een lijst met instellingstaken weergegeven. U wordt aangeraden deze taken te controleren voordat u een Amazon store](./store-integration.md) toevoegt. [ Nadat u de eerste winkel hebt toegevoegd, kunt u deze taken bekijken in de weergave Leren en voorbereiden van het Amazon-verkoopkanaal [startpagina](./amazon-sales-channel-home.md).

## 1. Achtergrondtaken inschakelen in [!DNL Commerce]

Alle producten en gegevens die tussen [!DNL Commerce] en Amazon worden gesynchroniseerd worden beheerd door [cron job](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}. Wanneer u taken hebt voltooid zoals het toevoegen of bijwerken van aanbiedingen en het ontvangen van bestellingen, verzendt en ontvangt een uitsnijdtaak gegevens tussen uw [!DNL Commerce]-back-end en uw [!DNL Amazon Seller Central]-account.

- [ [!DNL Commerce] Enablecron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}.

- Voor maximale prestaties, [set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target=&quot;_blank&quot;} om één keer per vijf minuten te worden uitgevoerd.

## 2. Uw [!DNL Amazon Seller Central]-account maken

Voordat u uw Amazon-verkoopkanaal kunt instellen, moet u een actieve [!DNL Amazon Seller Central]-account hebben. Als u geen bestaande Amazon Seller- rekening in [Noord-Amerika (V.S., CA, MX)](https://sell.amazon.com/){target=&quot;_blank&quot;} of [Europees (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target=&quot;_blank&quot;} gebied hebt, kunt u het installatieproces van de Amazon verkopersrekening voltooien.

Amazon-verkoopkanaal vereist een [!DNL Professional Seller]-account op [!DNL Amazon Seller Central]. Amazon brengt maandelijks een abonnement en verkoopkosten in rekening. Zie [Amazon: Kies uw het verkopen plan](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.

## 3. Ervoor zorgen dat je een goedgekeurde Amazon-verkoper bent

Voor integratie hebt u een goedgekeurd [!DNL Amazon Seller Central] account nodig. Je account mag geen beperkingen hebben voor producten of rubrieken. Voor sommige producten en categorieën is goedkeuring vereist voordat aanbiedingen worden gemaakt. Bekijk het Amazon-beleid voor rubriek en productgoedkeuring om te controleren of je producten zijn goedgekeurd. Zie [Amazon: Categorieën en producten waarvoor goedkeuring](https://sellercentral.amazon.com/gp/help/200333160){target=&quot;_blank&quot;} vereist is (Aanmelding bij Verkoper Central vereist).

Het is ook belangrijk om ervoor te zorgen dat u het volgende in uw [!DNL Amazon Seller Central] rekening hebt gevormd:

- Zorg ervoor dat je retourbeleid even goed is als of beter is dan het retourbeleid van Amazon. Zie [Amazon: Het Beleid van de terugkeer](https://www.amazon.com/gp/help/customer/display.html){target=&quot;_blank&quot;}.

- Zorg ervoor dat de belastinginstellingen zijn geconfigureerd. Zie [Amazon: Belastingsbeleid](https://sellercentral.amazon.com/gp/help/external/help.html){target=&quot;_blank&quot;} (Aanmelden bij verkoper vereist).

- Zorg ervoor dat uw verzendmethoden correct zijn geconfigureerd. Als u de verzendmethoden wilt instellen die [!DNL Commerce] aan klanten wordt aangeboden om uw Amazon-bestellingen te vervullen, werkt u [Amazon bij: Verzendinstellingen](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target=&quot;_blank&quot;} in uw [!DNL Amazon Seller Central]-account.

## 4. Zorg ervoor dat de BTW is geconfigureerd voor uw winkels

(Hoofdzakelijk gebruikt door verkopers in het Verenigd Koninkrijk.) Amazon raadt u aan zich aan te melden voor de [Amazon VAT-berekeningsservice](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target=&quot;_blank&quot;}. Als u een andere methode kiest, bent u verantwoordelijk voor de naleving van de BTW.

>[!NOTE]
>
>Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

## 5. Het aantal automatische overeenkomende catalogi verhogen

Tijdens het instappen gebruikt het verkoopkanaal van Amazon productkenmerken om uw bestaande aanbiedingen van Amazon (indien van toepassing) aan bestaande producten in uw [!DNL Commerce] catalogus aan te passen. Na het instappen, worden deze productattributen gebruikt om uw [!DNL Commerce] cataloguspunten aan een aanbieding van Amazon te publiceren en uw productgegevens tussen [!DNL Commerce] en Amazon te synchroniseren.

Als het hoogste aantal [!DNL Commerce] producten automatisch overeenkomt met Amazon-aanbiedingen, moet u een set productkenmerken voor uw [!DNL Commerce]-catalogus maken. Voordat u de Amazon-winkel voor verkoopkanalen instelt, moet u [!DNL Commerce] productkenmerken toevoegen die overeenkomen met deze Amazon-kenmerken, bijvoorbeeld: ASIN, EAN, ISBN, UPC of GCID. Zie [Een productkenmerk maken in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Uw valuta en conversie configureren (indien nodig)

Als uw opslag van Amazon een verschillende valuta gebruikt dan voor uw [!DNL Commerce] opslag wordt gevormd, [laat de munt ](https://docs.magento.com/user-guide/configuration/general/currency-setup.html) {target=&quot;_blank&quot;} toe en plaatst [muntomzettingspercentage](https://docs.magento.com/user-guide/stores/currency-update.html){target=&quot;_blank&quot;}.

## 7. Een productvoorwaardelement maken (indien nodig)

Als uw Amazon-aanbiedingen meer dan één productvoorwaarde bevatten (zoals _new_, _used_ of _like new_), maakt u een [!DNL Commerce]-kenmerk en wijst u voorwaardenwaarden toe. U moet dit kenmerk tijdens het instappen toewijzen aan het Amazon Condition-productkenmerk. Zie [Kenmerken maken voor Amazon](./ob-creating-magento-attributes.md).

## 8. Uw verzendmethode [!DNL Amazon Seller Central] configureren

Raadpleeg [Instellingen en verzendinstellingen][10] in uw [!DNL Amazon Seller Central]-account voor informatie over het instellen van verzendmethoden die u wilt aanbieden om aan uw Amazon-bestellingen te voldoen.

## Aanvullende configuraties

Wanneer uw Amazon-account is ingesteld en actief is, zijn er verschillende [!DNL Commerce] aanbevelingen die het Amazon-proces voor het instappen van verkoopkanalen helpen stroomlijnen.

### Bekijk en noteer alle producten die u wilt uitsluiten

Mogelijk wilt u niet dat bepaalde producten op Amazon worden vermeld. Het verkoopkanaal van Amazon heeft een regelengine voor aanbiedingen die wordt gebruikt om te bepalen welke producten in aanmerking komen voor publicatie naar Amazon. [Met ](./listing-rules.md) aanbiedingsregels kunt u subsets selecteren van producten die naar uw  [!DNL Amazon Seller Central] account moeten worden gepubliceerd (of niet worden gepubliceerd), bijvoorbeeld op basis van categorieselectie of door een of meer productkenmerken te definiëren. Als [!DNL Commerce] [catalog](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;} of [winkelwagentje](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;} prijsregels, moeten de productkenmerken die worden gebruikt om in aanmerking te komen voor een Amazon-aanbieding **[!UICONTROL Use for Promo Rule Conditions]** zijn ingesteld op `Yes`. Zie **[!UICONTROL Use for Promo Rule Conditions]** in [Productkenmerken](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}.

### Uw [!DNL Amazon Seller Central]-gebied instellen op inactief

Als u de gegevensovergang zonder fouten tijdens de integratie wilt vergemakkelijken, kunt u het beste uw Amazon-regio instellen op `Inactive` status in Instellingen > Accountinformatie > Vakantie-instellingen. Zie [Amazon: Aanbiedingsstatus voor vakanties][11]. Wanneer de installatie is voltooid, wijzigt u de status terug naar `Active` in Amazon.

![Volgende ](assets/btn-next.png) [**pictogramGa door met het maken van  [!DNL Commerce] kenmerken**](./ob-creating-magento-attributes.md)
