---
title: Aan boord [!DNL Channel Manager]
description: Sluit uw instantie aan [!DNL Channel Manager] door enkele instapstappen te voltooien.
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: f57c6db4c0314272d10bb5483d2c8a0ae396a9fc
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Aan boord [!DNL Channel Manager]

De online Manager van het Kanaal door de uitbreiding van de Manager van het Kanaal op uw te installeren [!DNL Commerce] -instantie en API-verbindingen configureren. Deze verbindingen laten communicatie en gegevenssynchronisatie tussen uw instantie van de Handel en de Marketplace van de Markt van de Markeren toe.

Nadat u aan boord gaat, vorm en beheer de verrichtingen van het verkoopkanaal van [!UICONTROL Channel Manager] de optie [!UICONTROL Commerce Admin Marketing] -menu.

![[!DNL Channel Manager] optie in de beheerweergave](assets/channel-manager-admin-view.png)

## Overzicht van onboarding

1. [Installeer de [!DNL Channel Manager] extension](install.md).

1. [Configureer de [!DNL Commerce Services Connector]](connect.md) om de Manager van het Kanaal met de instantie van de Handel, en andere ondersteunende diensten te integreren.

1. [Verbind uw [!DNL Commerce] opslaan naar [!DNL Walmart Marketplace]](connect.md).

1. [Volledige installatie van de winkel](complete-store-setup.md).

## Vereisten

- Controleer of u de vereiste [Voorwaarden voor Walmart Marketplace](walmart-prerequisites.md) om te integreren met Kanaalbeheer.

- **Informatie over handelsrekeningen**-Downloaden en installeren [!DNL Channel Manager] vereist een [Handelsrekening](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}. U hebt een account-id en gebruikersgegevens nodig met de toegang tot de [!DNL Adobe Commerce] of [!DNL Magento Open Source] -instantie.

   - **ID MAGE**-[Aanmelden](https://account.magento.com/customer/account/login/) naar de Commerce-account om de id op te halen van **[!UICONTROL My Account - Magento settings]**. U hebt deze id nodig om u te registreren voor de [!DNL Channel Manager] service-bètaprogramma.

      ![[!DNL MAGEID] over de accountinstellingen voor de handel](assets/mageid-my-commerce-account.png)

   - **Toegangstoetsen-** Vraag verificatietoetsen aan om Commerce-extensies te downloaden van de Composer-opslagplaats voor handel `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Bij Adobe Commerce- en Magento Open Source-projecten kan de eigenaar [Gedeelde toegang](https://docs.magento.com/user-guide/magento/magento-account-share.html) om vertrouwde werknemers en serviceproviders toe te staan extensies te downloaden met hun aanmeldingsgegevens van de Eigenaar of de account van de Licentiehouder.

      Aan [!DNL Adobe Commerce] bij cloudinfrastructuurprojecten moeten softwareinstallateurs de volgende toegang hebben tot [!DNL Commerce] instantie:

      - Toegang van supergebruikers tot het Cloud-project
      - Beheerders krijgen toegang tot een specifieke omgeving
      - een [!DNL Adobe Commerce] of [!DNL Magento Open Source] account met toegangsrechten tot de Composer-opslagplaats.

      Zie [Gebruikerstoegang beheren](https://devdocs.magento.com/cloud/project/user-admin.html).


- **Autorisatie voor het downloaden van het pakket Channel Manager Composer**- Geef de MAGE-id op van de Commerce-account die wordt gebruikt om de service te beheren, aan de Adobe-vertegenwoordiger die het Beta-programma voor uw organisatie coördineert.
- **Ervaring met Composer en de[!DNL Commerce CLI]** -Zie [Algemene installatie van CLI](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} voor informatie over het gebruik van deze gereedschappen voor het installeren en beheren van extensies op [!DNL Adobe Commerce] of [!DNL Magento Open Source] platforms.
- **[Amazon Sales Channel versie 4.4.2 of hoger](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)- Als u Amazon Sales Channel voor uw plaatsen van de Handel hebt geactiveerd, verifieer dat uw platform van de Handel versie 4.42 heeft geïnstalleerd alvorens u de Manager van het Kanaal installeert.


### Vereisten

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Composer 1.x of hoger](https://devdocs.magento.com/cloud/reference/cloud-composer.html)


### Ondersteunde platforms

- Adobe Commerce on Cloud (ECE) : 2,4 x
- Adobe Commerce ter plaatse (EE): 2,4 x
- Magento Open Source 2.4.x
