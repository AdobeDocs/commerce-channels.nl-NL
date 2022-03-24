---
title: '"Aan boord [!DNL Channel Manager]"'
description: Sluit uw instantie aan [!DNL Channel Manager] door enkele instapstappen te voltooien.
role: User
level: Intermediate
source-git-commit: ff87f31fec7a689385a93b8cab260fd93ff15f90
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Aan boord [!DNL Channel Manager]

De online Manager van het Kanaal door de uitbreiding van de Manager van het Kanaal op uw te installeren [!DNL Commerce] instantie en het vormen API verbindingen om mededeling en gegevenssynchronisatie tussen uw instantie van de Handel en de Marketplace van de Markering van de Markering toe te laten.

Nadat u het aan boord gaan hebt voltooid, kunt u verkoopkanaalbewerkingen configureren en beheren vanuit de [!UICONTROL Channel Manager] de optie [!UICONTROL Commerce Admin Marketing] -menu.

![[!DNL Channel Manager] optie in de beheerweergave](assets/channel-manager-admin-view.png)

## Overzicht van onboarding

1. [Installeer de [!DNL Channel Manager] extension](install.md).

1. [Configureer de [!DNL Commerce Services Connector]](connect.md) om de Manager van het Kanaal met de instantie van de Handel, en andere ondersteunende diensten te integreren.

1. [Verbind uw [!DNL Commerce] opslaan naar [!DNL Walmart Marketplace]](connect.md).

## Vereisten

- Verifieer dat je account bij Walmart MarketplaceMarketplaceMarmart-vereisten hebt voor verkopen op Walmart Marketplace

- **Informatie over handelsrekeningen**-Downloaden en installeren [!DNL Channel Manager] vereist een id en referenties van een [Handelsrekening](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;} met de eigenaar toegang tot de [!DNL Adobe Commerce] of [!DNL Magento Open Source] -instantie.

   - **ID MAGE**-[Aanmelden](https://account.magento.com/customer/account/login/) naar de Commerce-account om de id op te halen van [!UICONTROL My Account - Magento settings]. U hebt deze id nodig om u te registreren voor de [!DNL Channel Manager] service-bètaprogramma.

      ![[!DNL MAGEID] over de accountinstellingen voor de handel](assets/mageid-my-commerce-account.png)

   - **Toegangstoetsen-** Haal verificatietoetsen op om Commerce-extensies te downloaden uit de Composer-opslagplaats voor handel ([!DNL repo.magento.com]).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Bij Adobe Commerce- en Magento Open Source-projecten kan de Eigenaar [Gedeelde toegang](https://docs.magento.com/user-guide/magento/magento-account-share.html) om vertrouwde werknemers en serviceproviders toe te staan extensies te downloaden met hun aanmeldingsgegevens van de Eigenaar of de account van de Licentiehouder.

      Aan [!DNL Adobe Commerce] in het geval van cloud-infrastructuurprojecten moeten gebruikers over de volgende machtigingen beschikken om software te installeren op de [!DNL Commerce] instantie:

      - Toegang van supergebruikers tot het Cloud-project
      - Beheerders krijgen toegang tot een specifieke omgeving
      - een [!DNL Adobe Commerce] of [!DNL Magento Open Source] account met toegangsrechten tot de Composer-opslagplaats. Zie [Gebruikerstoegang beheren](https://devdocs.magento.com/cloud/project/user-admin.html).

- **Autorisatie voor het downloaden van het pakket Channel Manager Composer**- Geef de MAGE-id op van de Commerce-account die wordt gebruikt om de service te beheren, aan de Adobe-vertegenwoordiger die het Beta-programma voor uw organisatie coördineert.
- **Ervaring met Composer en de[!DNL Commerce CLI]** -Zie [Algemene installatie van CLI](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} voor informatie over het gebruik van deze gereedschappen voor het installeren en beheren van extensies op A[!DNL Adobe Commerce] of [!DNL Magento Open Source] platforms.
- Voor instanties van de Handel die de Sales Channel van Amazon hebben geïnstalleerd, verifieer dat [Amazon Sales Channel versie 4.4.2 of hoger](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) wordt geïnstalleerd voordat Channel Manager wordt geïnstalleerd.


### Vereisten

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Composer 1.x of hoger](https://devdocs.magento.com/cloud/reference/cloud-composer.html)


### Ondersteunde platforms

- Adobe Commerce on Cloud (ECE) : 2,4 x
- Adobe Commerce ter plaatse (EE): 2,4 x
- Magento Open Source 2.4.x
