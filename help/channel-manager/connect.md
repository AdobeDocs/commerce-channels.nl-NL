---
title: '''Verbinden met [!DNL Commerce] Diensten'
description: 'Kanaalbeheer verbinden met [!DNL Commerce] diensten om gegevenssynchronisatie en communicatie tussen de [!DNL Commerce] bijvoorbeeld Channel Manager en andere ondersteunende services.'
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Verbinden met [!DNL Commerce] Services

De [!DNL Commerce Services Connector] De Channel Manager-service wordt geïntegreerd met Adobe Commerce- en Magento Open Source-instanties. De schakelaar laat gegevenssynchronisatie en communicatie tussen toe [!DNL Commerce] instantie, [!DNL Channel Manager]en andere ondersteunende diensten.

[!DNL Commerce Services Connector] Setup is een eenmalig proces dat vereist is voor gebruik [Adobe Commerce SaaS-services](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) zoals [!DNL Channel Manager], [!DNL Live Search], en [!DNL Product Recommendations]. Als u reeds de schakelaar voor een andere dienst hebt gevormd, sla deze stap over.

## Vereisten

- **Handelsrekening**-Om software te installeren op [!DNL Commerce] exemplaren, moet u een rekening met Eigenaar of Admin toegang tot hebben [!DNL Commerce] platform.

  Accounteigenaars en Super-gebruikers kunnen beheerdersaccounts maken via de [!DNL Commerce] instantie of vanaf de opdrachtregel met behulp van de [!DNL Commerce] CLI, opdracht `admin:user:create`.

- **Adobe Commerce Production API Key**-This [key](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey) biedt API-toegang tot services die zijn vereist door Channel Manager. U hebt de openbare en privé geloofsbrieven voor deze sleutel nodig.

>[!TIP]
>
>Om de geloofsbrieven te verstrekken, a [!DNL Commerce] vergunninghouder of rekeninghouder beschikt over opties om [gedeelde toegang](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)of geeft de [API-sleutel](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html) referenties voor een vertrouwde ontwikkelaar.

## Configureer de [!DNL Commerce Services Connector]

1. Open de Configuratie van de Diensten van de Opslag.

   - Selecteer bij Beheer de optie **[!UICONTROL Stores]**.

   - Onder *[!UICONTROL Settings]*, selecteert u **[!UICONTROL Configuration]**.

   - Uitbreiden **[!UICONTROL Services]** en selecteert u **[!UICONTROL Commerce Services Connector]**.

1. Voeg de belangrijkste referenties voor de productie-API van uw Adobe Commerce-account toe.

   ![[!DNL Commerce Services Connector] in de [!DNL Admin] weergave](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > Als uw [!DNL Commerce] instantie heeft andere [!DNL Adobe Commerce] services zoals [!DNL Live Search] of [!DNL Product Recommendations] geïnstalleerd, wordt de referentie informatie getoond in de interface, en geen verdere configuratie wordt vereist.

1. Vorm het project SaaS en gegevensruimte zodat de Diensten van de Handel gegevens naar de dienst van de Manager van het Kanaal kunnen verzenden.

   ![[!DNL Commerce Services Connector] SaaS-id-configuratie in de [!DNL Admin] weergave](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

