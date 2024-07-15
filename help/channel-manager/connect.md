---
title: "verbind met  [!DNL Commerce]  de Diensten"
description: "Verbind de Manager van het Kanaal aan  [!DNL Commerce]  diensten om gegevenssynchronisatie en communicatie tussen de  [!DNL Commerce]  instantie, de Manager van het Kanaal, en andere ondersteunende diensten toe te laten."
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Verbinding maken met [!DNL Commerce] Services

In [!DNL Commerce Services Connector] wordt de service Channel Manager geïntegreerd met instanties van Adobe Commerce en Magento Open Source. De connector maakt gegevenssynchronisatie en communicatie mogelijk tussen de [!DNL Commerce] -instantie [!DNL Channel Manager] en andere ondersteunende services.

[!DNL Commerce Services Connector] de opstelling is een eenmalig proces dat wordt vereist om [ de diensten van Adobe Commerce SaaS ](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) zoals [!DNL Channel Manager], [!DNL Live Search], en [!DNL Product Recommendations] te gebruiken. Als u reeds de schakelaar voor een andere dienst hebt gevormd, sla deze stap over.

## Vereisten

- **de rekening van Commerce** - om software op [!DNL Commerce] instanties te installeren, moet u een rekening met Eigenaar of toegang Admin tot het [!DNL Commerce] platform hebben.

  Accounteigenaars en Super-gebruikers kunnen Admin-accounts maken vanaf de [!DNL Commerce] -instantie of vanaf de opdrachtregel met de [!DNL Commerce] CLI-opdracht `admin:user:create` .

- **- Deze [ sleutel van de Productie van Adobe Commerce ](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey) laat API toegang tot de diensten toe die door de Manager van het Kanaal worden vereist.** U hebt de openbare en privé geloofsbrieven voor deze sleutel nodig.

>[!TIP]
>
>Om de geloofsbrieven te verstrekken, heeft de a [!DNL Commerce] vergunninghouder of rekeningeigenaar opties om [ toegang ](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) te delen, of geeft de [ API Zeer belangrijke ](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html) geloofsbrieven aan een vertrouwde op ontwikkelaar.

## De [!DNL Commerce Services Connector] configureren

1. Open de Configuratie van de Diensten van de Opslag.

   - Selecteer **[!UICONTROL Stores]** in het menu Beheer.

   - Selecteer onder *[!UICONTROL Settings]* de optie **[!UICONTROL Configuration]** .

   - Vouw **[!UICONTROL Services]** uit en selecteer **[!UICONTROL Commerce Services Connector]** .

1. Voeg de belangrijkste referenties voor de productie-API van uw Adobe Commerce-account toe.

   ![[!DNL Commerce Services Connector] in de [!DNL Admin] view ](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > Als voor uw [!DNL Commerce] -instantie andere [!DNL Adobe Commerce] services zoals [!DNL Live Search] of [!DNL Product Recommendations] zijn geïnstalleerd, worden de referentie-informatie weergegeven in de interface en is er geen verdere configuratie vereist.

1. Vorm het project SaaS en gegevensruimte zodat de Diensten van Commerce gegevens naar de dienst van de Manager van het Kanaal kunnen verzenden.

   ![[!DNL Commerce Services Connector] Configuratie SaaS-id in de [!DNL Admin] view ](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

