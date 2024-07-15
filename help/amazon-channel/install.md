---
title: Installeer de  [!DNL Amazon Sales Channel]  uitbreiding
description: Om uw  [!DNL Commerce]  catalogus met  [!DNL Amazon Seller Accounts]  te integreren en door  [!DNL Amazon Marketplace] te verkopen, download en installeer de uitbreiding van de Sales Channel van Amazon.
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 010a95d7be29354515cf4dcbf5d557eebaa40ed6
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# De extensie [!DNL Amazon Sales Channel] installeren

>[!IMPORTANT]
>
>Alleen [!DNL Amazon Sales Channel] extension 4.0+-versies worden ondersteund voor Adobe Commerce en Magento Open Source 2.4.x-versies. Als u een versie 2.3.x in werking stelt, verwijs naar de documentatie voor de [ compatibele versie van het verkoopkanaal van Amazon ](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html). Voor meer informatie over versiecompatibiliteit, zie de [ 1} pagina van de Beschikbaarheid {in de ontwikkelaardocumentatie.](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html)

De extensie [!UICONTROL Amazon Sales Channel] installeert en voegt functies toe om uw Commerce-catalogus te integreren met [!DNL Amazon Seller Accounts] om via [!DNL Amazon Marketplace] te kunnen verkopen. Om extra informatie te herzien, zie de ](https://marketplace.magento.com/magento-module-amazon.html) pagina van de Sales Channel van 0} Amazon {in [!DNL Commerce Marketplace] en de [ versienota&#39;s ](release-notes.md).[

## Vereisten

- **instantie van Commerce**: De [!DNL Amazon Sales Channel] uitbreiding kan op instanties met Magento Open Source, Adobe Commerce, en Adobe Commerce op de versies van de wolkeninfrastructuur 2.3.x of later worden geïnstalleerd. Deze functie wordt niet meer ondersteund in 2.1-, 2.2- of 1.x-releases.
- **het Webrekening van Commerce**: U zou een het Webrekening van Commerce moeten hebben, die wordt gebruikt om een API sleutel tot stand te brengen en te volgen.
- **API sleutel**: Creeer een sleutel van Amazon verkoopkanaal API door uw het Webrekening van Commerce. De volgende instructies bevatten deze stappen.

## Installeren

Voor meer gedetailleerde informatie over het gebruiken van Composer voor dit proces, zie de [ instructies van de uitbreidingsinstallatie ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) in de ontwikkelaarsdocumentatie.

1. Login aan de [ Commerce Marketplace ](https://marketplace.magento.com/customer/account/).

1. Klik op de tab **[!UICONTROL Marketplace]** en klik vervolgens op **[!UICONTROL My Purchases]** .

1. Zoek en selecteer **[!UICONTROL Amazon Sales Channel]** .

1. Selecteer de versie op de extensiepagina.

1. Klik op **[!UICONTROL Technical Details]** voor de naam en versie van de component.

1. Gebruik de naam en versiegegevens om de ingang van de de dienstenschakelaar in uw `composer.json` dossier bij te werken.

   - Voeg de extensienaam en -versie toe aan het `composer.json` -bestand.

   - Navigeer naar de [!DNL Commerce] -projectmap en werk het `composer.json` -bestand bij.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Ga uw [ authentificatietoetsen ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) in. Uw openbare sleutel is uw gebruikersnaam; uw persoonlijke sleutel is uw wachtwoord.

   - Wacht op Composer om uw projectgebiedsdelen te beëindigen en ervoor te zorgen dat er geen fouten zijn.

1. [ verifieer de uitbreiding ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

## De API-sleutel voor het Amazon-verkoopkanaal toevoegen

Na het installeren, ga een [ Sleutel API ](./amazon-verify-api-key.md) in om configuratie te voltooien.

## Amazon-kanaalconfiguratieopties instellen

U hebt de volgende opties om het verkoopkanaal van Amazon te vormen. U hoeft deze instellingen niet aan te passen om aan de instap en verkoop op Amazon te beginnen. Gevorderde beheerders kunnen deze opties het beste overwegen.

1. Meld u aan bij de beheerder.

1. Op _Admin_ sidebar, ga **Opslag** > _Montages_ > **Configuratie**.

1. Klik **Sales Channel**, toen **Globale Montages**.

1. Voor **Duidelijke Geschiedenis van het Logboek**, bepaal het interval voor het ontruimen van de verzamelde logboeken.

   De opties zijn `Once Daily` , `Once Weekly` en `Once Monthly` (standaardwaarde).

1. (Facultatief) voor **AchtergrondTaken (CRON) Source**, verander het plaatsen in `Command Line (CLI) CRON`.

   Dit het plaatsen wordt geadviseerd voor **_geavanceerde gebruikers/beheerders_**.

1. Klik op **[!UICONTROL Save Config]**.

## De extensie bijwerken

1. Login aan de [ Commerce Marketplace ](https://marketplace.magento.com/customer/account/).

1. Klik op de tab **[!UICONTROL Marketplace]** en klik vervolgens op **[!UICONTROL My Purchases]** .

1. Zoek en selecteer **[!UICONTROL Amazon Sales Channel]** .

1. Selecteer de versie op de extensiepagina.

1. Klik op **[!UICONTROL Technical Details]** voor de naam en versie van de component.

1. Voltooi de [ instructies van de uitbreidingsverbetering ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) in de _Gids van de Installatie_.
