---
title: 'Installeren [!DNL Channel Manager]'
description: 'Installeer de[!DNL Channel Manager] extensie.'
role: Admin, Developer
feature: Sales Channels, Install
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---


# Installeren [!DNL Channel Manager]

Controleer de [vereisten](onboard.md#requirements) en verzamel de vereiste informatie voordat u Channel Manager installeert.

## De extensie installeren

De installatie-instructies voor Channel Manager zijn afhankelijk van het feit of Adobe Commerce of Magento Open Source op locatie of op cloudinfrastructuur wordt geïmplementeerd.

- Installeren op een [Instantie ter plaatse](#install-on-an-on-premises-instance).

- Installeren op een [[!DNL Adobe Commerce] over cloudinframinstructie-instantie](#install-adobe-commerce-on-cloud-infrastructure)

Beide methodes vereisen u om de Interface van de Lijn van het Bevel (CLI) te gebruiken.

>[!NOTE]
>
>Voor hulp bij het installeren [!DNL Commerce] software die CLI gebruikt, zie [Een extensie installeren](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

### Installeren op een exemplaar ter plaatse

Gebruik deze instructies om te installeren [!DNL Channel Manager] op Adobe Commerce en Magento Open Source aan een instantie ter plaatse.

1. Aanmelden bij de [!DNL Commerce] server als een [gebruiker met machtigingen](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html) om te schrijven naar [!DNL Commerce] bestandssysteem.

1. Plaats uw website in [onderhoudsmodus](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html).

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

Voor hulp bij het gebruiken van takken, zie [Aan de slag met vertakkingen](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) in de _Handleiding voor handel in Cloud-infrastructuur_.

Tijdens de installatie wordt de extensienaam (`magento\channel-manager`) wordt automatisch ingevoegd in het dialoogvenster [app/etc/config.php](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html) bestand. U hoeft het bestand niet rechtstreeks te bewerken.

1. Wijzig op uw lokale werkstation de hoofdmap van het Cloud-project.

1. Een ontwikkeling maken of uitchecken [vertakking](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html).

1. Voeg met de naam Composer de extensie toe aan de `require` van de `composer.json` bestand.

   ```bash
   composer require magento/module-sales-channels-extension --no-update
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
   $ git commit -m "Install channel manager extension" 
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

Als de module is uitgeschakeld, [inschakelen in uw lokale omgeving](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html) en implementeer uw wijzigingen.


1. Meld u aan bij de [!UICONTROL Admin] tot [Configureer de Commerce Services Connector](connect.md).

   >[!NOTE]
   >
   >Ga voor instructies voor het bijwerken van Channel Manager naar een nieuwe versie naar [Modules en extensies upgraden](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html).


## Problemen oplossen

Gebruik de volgende informatie om fouten op te lossen die tijdens het installatieproces van de Manager van het Kanaal voorkomen.

### Onjuiste Composer-sleutels

Als de [toegangstoets](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) gebruikt om te verifiëren bij de Composer-gegevensopslagruimte ongeldig is of niet is gekoppeld aan de [!DNL MAGE ID] gebruikt voor aanmelden voor [!DNL Channel Manager] -service, wordt de volgende fout weergegeven.

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Controleer de sleutelconfiguratie:

1. Zoek de locatie van het dialoogvenster `auth.json` bestand:

   ```bash
   $ composer config –global home
   ```

1. De weergave `auth.json` bestand.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Controleren of de gegevens in auth.json overeenkomen [de sleutels verbonden aan MAGE identiteitskaart](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) gebruikt om zich te registreren voor de service Channel Manager.

### Onvoldoende geheugen voor PHP

De volgende fout geeft aan of er onvoldoende geheugen is toegewezen aan PHP.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Gebruik een van de volgende methoden om het geheugenprobleem op te lossen:

- [De geheugenlimiet voor PHP verhogen](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html) in het milieu `php.ini` bestand. Controleer ook of de instantie Commerce de [aanbevolen waarden](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) voor andere PHP-instellingen.

- Geef de geheugenlimiet op vanaf de opdrachtregel.

  ```bash
  $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
  ```

  Bijvoorbeeld:

  ```bash
  $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
  ```

### Ontbrekende weergave

Als er een fout optreedt bij een ontbrekende `process_catalog_exporter_view` tijdens de installatie van Channel Manager probeert u [indexeerprogramma&#39;s vernieuwen](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html).

```bash
php bin/magento indexer:refresh
```

### Implementatiefouten in cloud

Voor problemen met de implementatie van de extensie in de cloud raadpleegt u [implementatiefout extensie](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html).
