---
title: "Installeer de [!DNL Amazon Sales Channel] extension"
description: Om uw [!DNL Commerce] catalogus met [!DNL Amazon Seller Accounts] en verkopen via [!DNL Amazon Marketplace], downloadt en installeert u de extensie Amazon Sales Channel.
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Installeer de [!DNL Amazon Sales Channel] extension

>[!IMPORTANT]
>
>Alleen [!DNL Amazon Sales Channel] extensie 4.0+-versies worden ondersteund voor Adobe Commerce en Magento Open Source 2.4.x-versies. Als u een versie van 2.3.x uitvoert, raadpleegt u de documentatie voor het [compatibele Amazon-verkoopkanaalrelease](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html). Zie voor meer informatie over versiecompatibiliteit de [Beschikbaarheid](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) in de ontwikkelaarsdocumentatie.

De [!UICONTROL Amazon Sales Channel] extensie installeert en voegt functies toe om uw handelscatalogus te integreren met [!DNL Amazon Seller Accounts] om via [!DNL Amazon Marketplace]. Als u aanvullende informatie wilt bekijken, raadpleegt u de [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) pagina in [!DNL Commerce Marketplace] en de [releaseopmerkingen](release-notes.md).

## Vereisten

- **Handelsinstantie**: De [!DNL Amazon Sales Channel] De extensie kan worden geïnstalleerd op instanties met Magento Open Source, Adobe Commerce en Adobe Commerce op cloudinfrasinfrastructuurversie 2.3.x of hoger. Deze functie wordt niet meer ondersteund in 2.1-, 2.2- of 1.x-releases.
- **Commerciële webaccount**: U moet een Commerce-webaccount hebben, waarmee een API-sleutel wordt gemaakt en bijgehouden.
- **API-sleutel**: Maak een Amazon-API-sleutel voor verkoopkanalen via uw Commerce-webaccount. De volgende instructies bevatten deze stappen.

## Installeren

Zie voor meer informatie over het gebruik van Composer voor dit proces de [extensieinstallatie](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) instructies in de ontwikkelaarsdocumentatie.

1. Aanmelden bij de [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. Klik op de knop **[!UICONTROL Marketplace]** en klikt u op **[!UICONTROL My Purchases]**.

1. Zoeken en selecteren **[!UICONTROL Amazon Sales Channel]**.

1. Selecteer de versie op de extensiepagina.

1. Klik voor de naam en versie van de component op **[!UICONTROL Technical Details]**.

1. Gebruik de naam en versieinformatie om de ingang van de de dienstenschakelaar in uw bij te werken `composer.json` bestand.

   - De naam en versie van de extensie toevoegen aan uw `composer.json` bestand.

   - Ga naar uw [!DNL Commerce] projectdirectory en werk uw `composer.json` bestand.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Voer uw [verificatietoetsen](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html). Uw openbare sleutel is uw gebruikersnaam; uw persoonlijke sleutel is uw wachtwoord.

   - Wacht op Composer om uw projectgebiedsdelen te beëindigen en ervoor te zorgen dat er geen fouten zijn.

1. [De extensie verifiëren](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

## De API-sleutel voor het Amazon-verkoopkanaal toevoegen

Voer na de installatie een [API-sleutel](./amazon-verify-api-key.md) om de configuratie te voltooien.

## Amazon-kanaalconfiguratieopties instellen

U hebt de volgende opties om het verkoopkanaal van Amazon te vormen. U hoeft deze instellingen niet aan te passen om aan de instap en verkoop op Amazon te beginnen. Gevorderde beheerders kunnen deze opties het beste overwegen.

1. Meld u aan bij de beheerder.

1. Op de _Beheerder_ zijbalk, ga naar **Winkels** > _Instellingen_ > **Configuratie**.

1. Klikken **Sales Channel** vervolgens **Algemene instellingen**.

1. Voor **Logboekgeschiedenis wissen** definieert u de interval voor het wissen van de verzamelde logbestanden.

   Opties omvatten `Once Daily`, `Once Weekly`, en `Once Monthly` (standaard).

1. (Optioneel) Voor **Bron voor achtergrondtaken (CRON)** wijzigt u de instelling in `Command Line (CLI) CRON`.

   Deze instelling wordt aanbevolen voor **_geavanceerde gebruikers/beheerders_**.

1. Klik op **[!UICONTROL Save Config]**.

## De extensie bijwerken

1. Aanmelden bij de [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. Klik op de knop **[!UICONTROL Marketplace]** en klikt u op **[!UICONTROL My Purchases]**.

1. Zoeken en selecteren **[!UICONTROL Amazon Sales Channel]**.

1. Selecteer de versie op de extensiepagina.

1. Klik voor de naam en versie van de component op **[!UICONTROL Technical Details]**.

1. Voltooi de [extensie, upgrade-instructies](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) in de _Installatiehandleiding_.
