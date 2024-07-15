---
title: 'Install  [!DNL Channel Manager]'
description: 'Installeer de extensie [!DNL Channel Manager].'
role: Admin, Developer
feature: Sales Channels, Install
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---


# Installeren [!DNL Channel Manager]

Herzie de [ vereisten ](onboard.md#requirements) en verzamel vereiste informatie alvorens u de Manager van het Kanaal installeert.

## De extensie installeren

De installatie-instructies voor Channel Manager zijn afhankelijk van het feit of Adobe Commerce of Magento Open Source op locatie of op cloudinfrastructuur wordt geïmplementeerd.

- Installeer op een [ op-gebouw instantie ](#install-on-an-on-premises-instance).

- Installeer op een [[!DNL Adobe Commerce]  op de instantie van de wolkeninfrastructuur ](#install-adobe-commerce-on-cloud-infrastructure)

Beide methodes vereisen u om de Interface van de Lijn van het Bevel (CLI) te gebruiken.

>[!NOTE]
>
>Voor hulp bij het installeren van [!DNL Commerce] software gebruikend CLI, zie [ een uitbreiding ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) installeren.

### Installeren op een exemplaar ter plaatse

Gebruik deze instructies om [!DNL Channel Manager] te installeren op Adobe Commerce en Magento Open Source te maken naar een exemplaar op locatie.

1. Login aan de [!DNL Commerce] server als a [ gebruiker met toestemmingen ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html) om aan het [!DNL Commerce] dossiersysteem te schrijven.

1. Zet uw website in [ onderhoudswijze ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html).

   ```bash
   $ bin/magento maintenance:enable
   ```

1. Voeg Kanaalbeheer toe aan `composer.json` vanuit de hoofdmap van het [!DNL Commerce] project.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. Voer desgevraagd de toegangstoetsen in van uw [!DNL Commerce] -account.

   Uw openbare sleutel is uw gebruikersnaam; uw persoonlijke sleutel is uw wachtwoord.

1. Werk de gebiedsdelen bij en installeer de uitbreiding.

   ```bash
   composer update magento/channel-manager
   ```

   Met de opdracht `composer update` werkt u alleen de afhankelijkheden bij die vereist zijn voor [!DNL Channel Manager] . Als u alle afhankelijkheden wilt bijwerken, gebruikt u in plaats daarvan de volgende opdracht: `composer update` .

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

1. Compileer het [!DNL Commerce] -project opnieuw als daarom wordt gevraagd.

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

Voor hulp met het gebruiken van takken, zie [ begonnen takken ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) tot stand te brengen in _Commerce op de Gids van de Infrastructuur van de Wolk_.

Tijdens installatie, wordt de uitbreidingsnaam (`magento\channel-manager`) automatisch opgenomen in het [ app/etc/config.php ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html) dossier. U hoeft het bestand niet rechtstreeks te bewerken.

1. Wijzig op uw lokale werkstation de hoofdmap van het Cloud-project.

1. Creeer of controleer een ontwikkelings [ tak ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html).

1. Voeg met de naam Composer de extensie toe aan de sectie `require` van het `composer.json` -bestand.

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. Werk de gebiedsdelen bij en installeer de uitbreiding.

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   Met de opdracht `composer update` werkt u alleen de afhankelijkheden bij die vereist zijn voor [!DNL Channel Manager] . Als u alle afhankelijkheden wilt bijwerken, gebruikt u in plaats daarvan de volgende opdracht: `composer update` .

1. Wijzigingen in code toevoegen, doorvoeren en doorvoeren. Voeg wijzigingen in het bestand `composer.lock` en `composer.json` toe.

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

Als de module gehandicapt is, [ laat het in uw lokaal milieu ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html) toe en stelt uw veranderingen op.


1. Nadat u de uitbreiding met succes installeert, login aan [!UICONTROL Admin] om [ de Schakelaar van de Diensten van Commerce ](connect.md) te vormen.

   >[!NOTE]
   >
   >Voor instructies om de Manager van het Kanaal aan een nieuwe versie bij te werken, zie [ modules en uitbreidingen van de Verbetering ](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html).


## Problemen oplossen

Gebruik de volgende informatie om fouten op te lossen die tijdens het installatieproces van de Manager van het Kanaal voorkomen.

### Onjuiste Composer-sleutels

Als de [ toegangssleutels ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) worden gebruikt om aan de bewaarplaats van Composer voor authentiek te verklaren ongeldig zijn, of niet verbonden met [!DNL MAGE ID] die wordt gebruikt om zich voor de [!DNL Channel Manager] dienst aan te melden, de volgende foutenvertoningen.

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Controleer de sleutelconfiguratie:

1. Zoek de locatie van het `auth.json` -bestand:

   ```bash
   $ composer config –global home
   ```

1. Geef het `auth.json` -bestand weer.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Verifieer dat de geloofsbrieven in auth.json [ aanpassen de sleutels verbonden aan identiteitskaart van de MAGE ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) worden gebruikt om voor de dienst van de Manager van het Kanaal te registreren.

### Onvoldoende geheugen voor PHP

De volgende fout geeft aan of er onvoldoende geheugen is toegewezen aan PHP.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Gebruik een van de volgende methoden om het geheugenprobleem op te lossen:

- [ verhoog de geheugengrens voor PHP ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html) in het milieu `php.ini` dossier. Ook, verifieer dat de instantie van Commerce de [ geadviseerde waarden ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) voor andere PHP montages heeft.

- Geef de geheugenlimiet op vanaf de opdrachtregel.

  ```bash
  $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
  ```

  Bijvoorbeeld:

  ```bash
  $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
  ```

### Ontbrekende weergave

Als u een fout over ontbrekende `process_catalog_exporter_view` tijdens de installatie van de Manager van het Kanaal krijgt, probeer [ verfrissend de indexeerders ](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html).

```bash
php bin/magento indexer:refresh
```

### Implementatiefouten in cloud

Voor problemen die de uitbreiding opstellen aan de wolk, zie [ mislukking van de uitbreidingsplaatsing ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html).
