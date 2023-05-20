---
title: Aan boord [!DNL Channel Manager]
description: '''Sluit uw instantie aan op de [!DNL Channel Manager] de dienst door een paar onboarding stappen te voltooien."'
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---


# Aan boord [!DNL Channel Manager]

Nadat u het proces van de Manager van het Kanaal op het instappen voltooit, kunt u tot de verkoopverrichtingen van het kanaal van de Marketplace van de Markt toegang hebben, vormen en beheren van Adobe Commerce. Kanaalbeheer is beschikbaar via de [!UICONTROL Channel Manager] de optie [!UICONTROL Commerce Admin Marketing] -menu.

![[!DNL Channel Manager] optie in de beheerweergave](assets/channel-manager-admin-view.png)

## Vereisten

Controleer de vereisten voor het gebruik van Channel Manager en verzamel de vereiste accountgegevens en referenties om de extensie te downloaden, installeren en configureren.

- **[Vereisten voor de Marketplace van Walmart](walmart-requirements.md)**-Verifieer dat u aan vereisten om met de Manager van het Kanaal met inbegrip van te integreren voldoet [Je verkopersaccount instellen](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) en het genereren van de API-sleutel om integratie mogelijk te maken.

- **Informatie over handelsrekeningen**-Downloaden en installeren [!DNL Channel Manager] vereist een [Handelsrekening](https://docs.magento.com/user-guide/magento/magento-account.html){target="_blank"}. U hebt een account-id en gebruikersgegevens nodig met de toegang tot de [!DNL Adobe Commerce] of [!DNL Magento Open Source] -instantie.

   - **ID MAGE**-[Aanmelden](https://account.magento.com/customer/account/login/) aan de [!DNL Commerce] account om de id op te halen van **[!UICONTROL My Account - Magento settings]**.

      ![[!DNL MAGEID] op [!DNL Commerce] accountinstellingen](assets/mageid-my-commerce-account.png)

   - **Toegangstoetsen-** Verificatietoetsen downloaden [!DNL Commerce] uitbreidingen van de [!DNL Commerce] Composer-opslagplaats `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Bij Adobe Commerce- en Magento Open Source-projecten kan de eigenaar [Gedeelde toegang](https://docs.magento.com/user-guide/magento/magento-account-share.html) om vertrouwde werknemers en serviceproviders toe te staan extensies te downloaden met hun aanmeldingsgegevens van de Eigenaar of de account van de Licentiehouder.

      Voor [!DNL Adobe Commerce] in het geval van cloudinfrastructuurprojecten moeten softwareinstallateurs de volgende toegang hebben tot de [!DNL Commerce] instantie:

      - Toegang van supergebruikers tot het Cloud-project
      - Beheerders krijgen toegang tot een specifieke omgeving
      - een [!DNL Adobe Commerce] account met toegangsrechten tot de Composer-opslagplaats

      Zie [Gebruikerstoegang beheren](https://devdocs.magento.com/cloud/project/user-admin.html).


- **Ervaring met Composer en de[!DNL Commerce CLI]**-Zie [Algemene installatie van CLI](https://devdocs.magento.com/extensions/install/){target="_blank"} voor informatie over het gebruik van deze gereedschappen om extensies te installeren en te beheren op [!DNL Adobe Commerce] of [!DNL Magento Open Source] platforms.

- **[[!DNL Amazon Sales Channel] versie 4.4.2 of hoger](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-Als u hebt geactiveerd [!DNL Amazon Sales Channel] voor uw [!DNL Commerce] sites, controleer of uw [!DNL Commerce] platform heeft versie 4.4.2 of hoger geïnstalleerd voordat u de installatie uitvoert [!DNL Channel Manager].

- **[!DNL Inventory Management]extensie voor Adobe Commerce en Magento Open Source**

   Als u Channel Manager wilt gebruiken voor inventarisatie- en bestelbeheer, moet de Inventory management-extensie zijn geïnstalleerd en ingeschakeld op uw Adobe Commerce- en Magento Open Source-exemplaar. Deze extensie wordt standaard geïnstalleerd en ingeschakeld op Adobe Commerce en [!DNL Magento Open Source] 2.3.x en hoger.

   Als u Commerce hebt geüpgraded vanaf 2.2.x, of als u Inventory management hebt uitgeschakeld, werkt u uw installatie bij om de vereiste modules op te nemen. Zie [Inventory management installeren](https://devdocs.magento.com/extensions/inventory-management/) in de documentatie van Adobe Commerce Developer.

### Systeemvereisten

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Composer 1.x of hoger](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] versie 4.4.2 of hoger](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Als u hebt geactiveerd [!DNL Amazon Sales Channel] voor uw [!DNL Commerce] sites, controleer of uw [!DNL Commerce] platform heeft versie 4.4.2 geïnstalleerd voordat u de installatie uitvoert [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://devdocs.magento.com/extensions/inventory-management/)

### Ondersteunde platforms

- Adobe Commerce on Cloud (ECE) : 2,4 x
- Adobe Commerce ter plaatse (EE): 2,4 x
- Magento Open Source 2.4.x

## Stappen aan boord

1. [Je Walmart-verkopersaccount instellen](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [Installeer de [!DNL Channel Manager] extension](install.md).

1. [Verbinden met de Diensten van de Handel](connect.md) om de Manager van het Kanaal met de instantie van de Handel, en andere ondersteunende diensten te integreren.

1. [Verbind uw [!DNL Commerce] opslaan naar [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [Volledige installatie van de winkel](complete-sales-channel-store-setup.md).
