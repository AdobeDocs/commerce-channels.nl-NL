---
title: Installeren [!DNL Channel Manager]
description: Installeer de extensie Kanaalbeheer.
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 4242115d178a4e4a21a271f2ea47fcd8ad9250ed
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Installeren [!DNL Channel Manager]

Controleer de [vereisten](onboard.md#requirements) en verzamel de vereiste informatie voordat u Channel Manager installeert.

## Minimale stabiliteit bijwerken

Voordat u de extensie installeert, moet u de `minimum-stability` vereist in uw `composer.json` zodat u eerdere versies van Channel Manager kunt installeren met Composer.

Als u de configuratie wilt bijwerken, voegt u de volgende regels toe aan de `composer.json` bestand.

```json
{
   "minimum-stability": "alpha",
   "prefer-stable": true
}
```

## De extensie installeren

De installatie-instructies voor Channel Manager zijn afhankelijk van het feit of Adobe Commerce of Magento Open Source wordt geïmplementeerd op locatie of op een cloudinfrastructuur.

- Installeren op een [Instantie ter plaatse](#install-on-an-on-premises-instance).

- Installeren op een [[!DNL Adobe Commerce] over cloudinframinstructie-instantie](#install-adobe-commerce-on-cloud-infrastructure)

Beide methodes vereisen u om de Interface van de Lijn van het Bevel (CLI) te gebruiken.

>[!NOTE]
>
>Voor hulp bij het installeren [!DNL Commerce] software die CLI gebruikt, zie [Algemene installatie van CLI](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;}.

### Installeren op een exemplaar ter plaatse

Gebruik deze instructies om te installeren [!DNL Channel Manager] op Adobe Commerce en Magento Open Source naar een instantie ter plaatse.

1. Aanmelden bij de [!DNL Commerce] server als een [gebruiker met machtigingen](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/file-system-perms.html){target=&quot;_blank&quot;} om naar de [!DNL Commerce] bestandssysteem.

1. Plaats uw website in [onderhoudsmodus](https://devdocs.magento.com/guides/v2.4/install-gde/install/cli/install-cli-subcommands-maint.html){target=&quot;_blank&quot;}.

   ```bash
   $ bin/magento maintenance:enable
   ```

1. Van de [!DNL Commerce] projecthoofdmap, Kanaalbeheer toevoegen aan `composer.json`.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. Voer desgevraagd de toegangstoetsen in uit uw [!DNL Commerce] account.

   Uw openbare sleutel is uw gebruikersnaam; uw persoonlijke sleutel is uw wachtwoord.

1. Werk de gebiedsdelen bij en installeer de uitbreiding.

   ```bash
   composer update magento/channel-manager
   ```

   De `composer update` bevel werkt slechts de gebiedsdelen bij die voor worden vereist [!DNL Channel Manager]. Om alle gebiedsdelen bij te werken, gebruik in plaats daarvan dit bevel: `composer update`.

1. Wacht tot Composer de projectafhankelijkheden heeft bijgewerkt en eventuele fouten heeft opgelost.

1. Controleer de installatie van de module:

   - Controleer de modulestatus.

      ```bash
      bin/magento module:status Magento_SalesChannels
      ```

      Monsterrespons:

      ```terminal
      Module is enabled
      ```

   - Als de module niet wordt toegelaten, laat het toe.

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. Registreer de extensie.

   ```bash
   bin/magento setup:upgrade
   ```

1. Indien gevraagd, compileert u uw [!DNL Commerce] project.

   ```bash
   bin/magento setup:di:compile
   ```

1. Maak de cache leeg.

   ```bash
   bin/magento cache:clean
   ```

1. Onderhoudsmodus uitschakelen.

   ```bash
   bin/magento maintenance:disable
   ```

### Installeren in een Adobe Commerce op een Cloud Infrastructure-instantie

Werk in een ontwikkelingsvertakking wanneer u een extensie toevoegt aan uw cloudinstantie.

Voor hulp bij het gebruiken van takken, zie [Aan de slag met het maken van vertakkingen](https://devdocs.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;} in de documentatie voor Adobe Commerce-ontwikkelaars.

Tijdens de installatie wordt de extensienaam (`magento\channel-manager`) wordt automatisch ingevoegd in het dialoogvenster [app/etc/config.php](https://devdocs.magento.com/cloud/live/sens-data-over.html#configuration-data){target=&quot;_blank&quot;} bestand. U hoeft het bestand niet rechtstreeks te bewerken.

1. Wijzig op uw lokale werkstation de hoofdmap van het Cloud-project.

1. Een ontwikkeling maken of uitchecken [vertakking](https://devdocs-beta.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;}.

1. Voeg met de naam Composer de extensie toe aan de `require` van de `composer.json` bestand.

   ```bash
   composer require require magento/module-sales-channels-extension --no-update
   ```

1. Werk de gebiedsdelen bij en installeer de uitbreiding.

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   De `composer update` bevel werkt slechts de gebiedsdelen bij die voor worden vereist [!DNL Channel Manager]. Om alle gebiedsdelen bij te werken, gebruik in plaats daarvan dit bevel: `composer update`.

1. Wijzigingen in code toevoegen, doorvoeren en pushcode doorvoeren, inclusief wijzigingen in het dialoogvenster `composer.lock` en `composer.json` bestand.

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m “Install channel manager extension” 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. Nadat het bouwstijl en plaatsingsproces voltooit, gebruik SSH aan login aan het verre milieu en verifieer dat de uitbreiding correct geïnstalleerd was.

```bash
   bin/magento module:status Magento_SalesChannels
```

Monsterrespons:

```terminal
Module is enabled
```

Als de module is uitgeschakeld, [inschakelen in uw lokale omgeving](https://devdocs.magento.com/cloud/howtos/install-components.html#manage-extensions) en implementeer uw wijzigingen.


1. Nadat u de extensie hebt geïnstalleerd, meldt u zich aan bij de [!UICONTROL Admin] tot [Configureer de Commerce Services Connector](connect.md).

   >[!NOTE]
   >
   >Ga voor instructies voor het bijwerken van Channel Manager naar een nieuwe versie naar [Modules en extensies upgraden](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html){target=&quot;_blank&quot;}.


## Problemen oplossen

Gebruik de volgende informatie om fouten op te lossen die tijdens het installatieproces van de Manager van het Kanaal voorkomen.

### Onjuiste Composer-sleutels

Als de [toegangstoets](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;} gebruikt om te verifiëren bij de Composer-opslagplaats, is ongeldig of is niet gekoppeld aan de [!DNL MAGE ID] gebruikt om u aan te melden voor de [!DNL Channel Manager] -service, wordt de volgende fout weergegeven.

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Controleer de sleutelconfiguratie:

1. Zoek de locatie van het dialoogvenster `auth.json` bestand:

   ```bash
   $ composer config –global home
   ```

1. De weergave van `auth.json` bestand.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Controleren of de gegevens in auth.json overeenkomen [de sleutels verbonden aan MAGE identiteitskaart](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;} gebruikt om te registreren voor de service Channel Manager.

### Onvoldoende geheugen voor PHP

De volgende fout geeft aan of er onvoldoende geheugen is toegewezen aan PHP.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Gebruik een van de volgende methoden om het geheugenprobleem op te lossen:

- [De geheugenlimiet voor PHP verhogen](https://devdocs.magento.com/cloud/project/magento-app-php-ini.html#increase-php-memory-limit){target=&quot;_blank&quot;} in de omgeving `php.ini` bestand. Controleer ook of de instantie Commerce de [aanbevolen waarden](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html){target=&quot;_blank&quot;} voor andere PHP-instellingen.

- Geef de geheugenlimiet op vanaf de opdrachtregel.

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   Bijvoorbeeld:

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### Ontbrekende weergave

Als er een fout optreedt bij een ontbrekende `process_catalog_exporter_view` tijdens de installatie van Channel Manager probeert u [indexeerprogramma&#39;s vernieuwen](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-index.html#config-cli-subcommands-index-reindex){target=&quot;_blank&quot;}.

```bash
php bin/magento indexer:refresh
```

### Implementatiefouten in cloud

Voor problemen met de implementatie van de extensie in de cloud raadpleegt u [implementatiefout extensie](https://devdocs.magento.com/cloud/trouble/trouble_comp-deploy-fail.html){target=&quot;_blank&quot;}.
