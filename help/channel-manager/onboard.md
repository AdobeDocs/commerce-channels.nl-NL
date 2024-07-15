---
title: Aan boord  [!DNL Channel Manager]
description: "Verbind uw instantie met de  [!DNL Channel Manager]  dienst door een paar aan boord komende stappen te voltooien."
level: Intermediate
role: Leader, Admin, Developer
feature: Sales Channels, Install
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---


# Aan boord [!DNL Channel Manager]

Nadat u het proces van de Manager van het Kanaal op het instappen voltooit, kunt u tot de verkoopverrichtingen van het kanaal van de Marketplace van de Markt toegang hebben, vormen en beheren van Adobe Commerce. Kanaalbeheer is beschikbaar via de optie [!UICONTROL Channel Manager] in het menu [!UICONTROL Commerce Admin Marketing] .

![[!DNL Channel Manager] in de beheerweergave ](assets/channel-manager-admin-view.png){width="500"}

## Vereisten

Controleer de vereisten voor het gebruik van Channel Manager en verzamel de vereiste accountgegevens en referenties om de extensie te downloaden, installeren en configureren.

- ](walmart-requirements.md)**- verifieer de vereisten van de Marketplace van het 0} Markeren dat u aan de vereisten voldoet om met de Manager van het Kanaal te integreren met inbegrip van [ vestiging uw rekening van de Verkoper ](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) en het produceren van de API sleutel om de integratie toe te laten.**[

- **de rekeningsinformatie van Commerce** - het downloaden en het installeren [!DNL Channel Manager] vereist de rekening van a [ Commerce ](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-create.html). U hebt een account-id en gebruikersgegevens nodig met de toegang tot de instantie [!DNL Adobe Commerce] of [!DNL Magento Open Source] door Eigenaar of Beheerder.

   - **identiteitskaart van de MAAK** - [ Login ](https://account.magento.com/customer/account/login/) aan de [!DNL Commerce] rekening om identiteitskaart van **[!UICONTROL My Account - Magento settings]** te krijgen.

     ![[!DNL MAGEID] op [!DNL Commerce] accountinstellingen ](assets/mageid-my-commerce-account.png){width="250"}

   - **Toegangstoetsen -** krijgen authentificatietoetsen om [!DNL Commerce] uitbreidingen van de [!DNL Commerce] bewaarplaats Composer `([!DNL repo.magento.com]` te downloaden).

     ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png){width="400"}

     Voor Adobe Commerce en de projecten van de Magento Open Source, kan de eigenaar opstelling [ Gedeelde Toegang ](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) om vertrouwde op werknemers en dienstverleners toe te staan om uitbreidingen te downloaden gebruikend geloofsbrieven van de Eigenaar of de rekening van de vergunninghouder.

     Voor [!DNL Adobe Commerce] in projecten met cloudinfrastructuur moeten softwareinstallatieprogramma&#39;s de volgende toegang hebben tot het [!DNL Commerce] -exemplaar:

      - Toegang van supergebruikers tot het Cloud-project
      - Beheerders krijgen toegang tot een specifieke omgeving
      - een [!DNL Adobe Commerce] -account met toegangsrechten tot de Composer-opslagplaats

     Zie [ gebruikerstoegang beheren ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html) in *Commerce op de Gids van de Infrastructuur van de Wolk*.

- **Ervaring gebruikend Composer en[!DNL Commerce CLI]** - zie [ installeer een uitbreiding ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) in de *Gids van de Installatie* voor informatie over het gebruiken van deze hulpmiddelen om uitbreidingen op [!DNL Adobe Commerce] of [!DNL Magento Open Source] platforms te installeren en te beheren.

- **[[!DNL Amazon Sales Channel] versie 4.4.2 of later ](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)** - als u [!DNL Amazon Sales Channel] voor uw [!DNL Commerce] plaatsen activeerde, verifieer dat uw [!DNL Commerce] platform versie 4.4.2 of later heeft geïnstalleerd alvorens u [!DNL Channel Manager] installeert.

- **[!DNL Inventory Management]extension for Adobe Commerce and Magento Open Source**

  Als u Channel Manager wilt gebruiken voor inventarisatie- en bestelbeheer, moet de Inventory management-extensie zijn geïnstalleerd en ingeschakeld op uw Adobe Commerce- en Magento Open Source-exemplaar. Deze extensie wordt standaard geïnstalleerd en ingeschakeld op Adobe Commerce en [!DNL Magento Open Source] 2.3.x en hoger.

  Als u Commerce hebt geüpgraded vanaf 2.2.x of als u Inventory management hebt uitgeschakeld, moet u de installatie bijwerken en de vereiste modules opnemen. Zie [ Inventory management ](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html) in de *Gids van Inventory management installeren*.

### Systeemvereisten

- [ Adobe Commerce 2.4.x ](https://experienceleague.adobe.com/docs/commerce-operations/release/versions.html)
- [ PHP 7.3 / 7.4 ](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)
- [ Composer 1.x of later ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/overview.html)
- [[!DNL Amazon Sales Channel]  versie 4.4.2 of later ](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) - als u [!DNL Amazon Sales Channel] voor uw [!DNL Commerce] plaatsen hebt geactiveerd, verifieer dat uw [!DNL Commerce] platform versie 4.4.2 geïnstalleerd heeft alvorens u [!DNL Channel Manager] installeert.
- [[!DNL Inventory Management]](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)

### Ondersteunde platforms

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce in bedrijven (EE) : 2.4.x
- Magento Open Source 2.4.x

## Stappen aan boord

1. [ Opstelling uw rekening van de Seller van de Marm ](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [ installeer de  [!DNL Channel Manager]  uitbreiding ](install.md).

1. [ verbind met de Diensten van Commerce ](connect.md) om de Manager van het Kanaal met de instantie van Commerce, en andere ondersteunende diensten te integreren.

1. [ verbind uw  [!DNL Commerce]  opslag met  [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [ Volledige opslagopstelling ](complete-sales-channel-store-setup.md).
