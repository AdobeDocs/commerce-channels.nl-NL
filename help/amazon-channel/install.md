---
title: De extensie installeren
description: Download en installeer de Amazon Sales Channel-extensie om uw  [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] en verkoop via de  [!DNL Amazon Marketplace] te integreren.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# De extensie installeren

>[!IMPORTANT]
>
>Alleen [!DNL Amazon Sales Channel]-extensie 4.0+-versies worden ondersteund voor Adobe Commerce en Magento Open Source 2.4.x-versies. Als u een versie 2.3.x in werking stelt, verwijs naar de documentatie voor [compatibele versie van het verkoopkanaal van Amazon ](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target=&quot;_blank&quot;}. Voor meer informatie over versiecompatibiliteit, zie [Beschikbaarheid](https://devdocs.magento.com/release/availability.html){target=&quot;_blank&quot;} pagina in de ontwikkelaarsdocumentatie.

De extensie [!UICONTROL Amazon Sales Channel] installeert en voegt functies toe om uw handelscatalogus te integreren met [!DNL Amazon Seller Accounts] om te verkopen via [!DNL Amazon Marketplace]. Als u aanvullende informatie wilt bekijken, raadpleegt u de pagina [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) in [!DNL Commerce Marketplace] en de [releaseopmerkingen](https://devdocs.magento.com/extensions/amazon-sales/release-notes/) in de ontwikkelaarsdocumentatie.

## Vereisten

- **Handelsinstantie**: De  [!DNL Amazon Sales Channel] extensie kan worden geïnstalleerd op instanties met Magento Open Source, Adobe Commerce en Adobe Commerce op cloudinfrasinfrastructuurversie 2.3.x of hoger. Deze functie wordt niet meer ondersteund in 2.1-, 2.2- of 1.x-releases.
- **Webaccount** voor handel: U moet een Commerce-webaccount hebben, waarmee een API-sleutel wordt gemaakt en bijgehouden.
- **API-sleutel**: Maak een Amazon-API-sleutel voor verkoopkanalen via uw Commerce-webaccount. De volgende instructies bevatten deze stappen.

## Installeren

Voor meer gedetailleerde informatie over het gebruiken van Composer voor dit proces, zie de [uitbreidingsinstallatie](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} instructies in de ontwikkelaarsdocumentatie.

1. Meld u aan bij [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. Klik op de tab **[!UICONTROL Marketplace]** en klik vervolgens op **[!UICONTROL My Purchases]**.

1. Zoek en selecteer **[!UICONTROL Amazon Sales Channel]**.

1. Selecteer de versie op de extensiepagina.

1. Voor de componentennaam en de versie, klik **[!UICONTROL Technical Details]**.

1. Gebruik de naam en de versieinformatie om de ingang van de de dienstenschakelaar in uw `composer.json` dossier bij te werken.

   - Voeg de naam en de versie van de extensie toe aan het `composer.json`-bestand.

   - Navigeer naar uw [!DNL Commerce] projectfolder en werk uw `composer.json` dossier bij.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Voer uw [verificatietoetsen](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;} in. Uw openbare sleutel is uw gebruikersnaam; uw persoonlijke sleutel is uw wachtwoord.

   - Wacht op Composer om uw projectgebiedsdelen te beëindigen en ervoor te zorgen dat er geen fouten zijn.


1. [Verifieer de extensie](https://devdocs.magento.com/extensions/install/#verify-the-extension){target=&quot;_blank&quot;}.

## De API-sleutel voor het Amazon-verkoopkanaal toevoegen

Na het installeren, ga [API Sleutel](./amazon-verify-api-key.md) in om configuratie te voltooien.

## Amazon-kanaalconfiguratieopties instellen

U hebt de volgende opties om het verkoopkanaal van Amazon te vormen. U hoeft deze instellingen niet aan te passen om aan te vangen en te verkopen op Amazon. Gevorderde beheerders kunnen deze opties het beste in overweging nemen.

1. Meld u aan bij de beheerder.

1. Op _Admin_ sidebar, ga naar **Stores** > _Settings_ > **Configuration**.

1. Klik **Sales Channel**, dan **Globale Montages**.

1. Voor **Loggeschiedenis wissen** definieert u het interval voor het wissen van de verzamelde logbestanden.

   U kunt onder andere `Once Daily`, `Once Weekly` en `Once Monthly` (standaardwaarde) kiezen.

1. (Optioneel) Wijzig voor **Achtergrondtaken (CRON) Source** de instelling in `Command Line (CLI) CRON`.

   Deze instelling wordt aanbevolen voor **_gevorderde gebruikers/beheerders_**.

1. Klik op **[!UICONTROL Save Config]**.

## De extensie bijwerken

1. Meld u aan bij [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. Klik op de tab **[!UICONTROL Marketplace]** en klik vervolgens op **[!UICONTROL My Purchases]**.

1. Zoek en selecteer **[!UICONTROL Amazon Sales Channel]**.

1. Selecteer de versie op de extensiepagina.

1. Voor de componentennaam en de versie, klik **[!UICONTROL Technical Details]**.

1. Voltooi [de instructies van de uitbreidingsverbetering](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target=&quot;_blank&quot;} in de ontwikkelaarsdocumentatie.
