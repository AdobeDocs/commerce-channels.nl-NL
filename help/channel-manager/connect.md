---
title: Verbinden met [!DNL Commerce] diensten
description: Kanaalbeheer verbinden met [!DNL Commerce] diensten om gegevenssynchronisatie en communicatie tussen de [!DNL Commerce] bijvoorbeeld Kanaalbeheer en andere ondersteunende services.
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: aaab7aa7feb05264c24386e62193564dc5ae8fe3
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---


# Verbinden met [!DNL Commerce] diensten

De schakelaar van de Diensten van de Handel integreert de dienst van de Manager van het Kanaal met instanties Adobe Commerce en Magento Open Source. De schakelaar laat gegevenssynchronisatie en communicatie tussen toe [!DNL Commerce] instantie, [!DNL Channel Manager]en andere ondersteunende diensten.

De de schakelaaropstelling van de Diensten van de handel is een eenmalig proces dat wordt vereist om Adobe te gebruiken [Commerciële SaaS-diensten](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;} als [!DNL Channel Manager], [!DNL Live Search], en [!DNL Product Recommendations]. Als u reeds de schakelaar voor een andere dienst hebt gevormd, sla deze stap over.

## Vereisten

- **Handelsrekening**- Als u software wilt installeren op instanties van Commerce, moet u een account met Eigenaar of Admin toegang hebben tot het platform Commerce.

   Accounteigenaars en Super-gebruikers kunnen Admin-accounts maken via de instantie Commerce of via de opdrachtregel [!DNL Commerce] CLI, opdracht `admin:user:create`.

- **Adobe Commerce Production API Key**-This [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} biedt API-toegang tot services die zijn vereist door Channel Manager. U hebt de openbare en privé geloofsbrieven voor deze sleutel nodig.

>[!TIP]
>
>Om de geloofsbrieven te verstrekken, heeft een de vergunninghouder of rekeninghouder van de Handel opties om [gedeelde toegang](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;} of geef de [API-sleutel](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} referenties naar een vertrouwde ontwikkelaar.

## De Commerce Services Connector configureren

1. Open de Configuratie van de Diensten van de Opslag.

   - Selecteer bij Beheer de optie **[!UICONTROL Stores]**.

   - Selecteer onder *[!UICONTROL Settings]* de optie **[!UICONTROL Configuration]**.

   - Uitbreiden **[!UICONTROL Services]** en selecteert u **[!UICONTROL Commerce Services Connector]**.

1. Voeg de belangrijkste referenties voor de productie-API van uw Adobe Commerce-account toe.

   ![[!DNL Commerce Service Connector] in de [!DNL Admin] weergave](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Als uw [!DNL Commerce] instantie heeft andere [!DNL Adobe Commerce] services zoals [!DNL Live Search] of [!DNL Product Recommendations] geïnstalleerd, wordt de referentie informatie getoond in de interface, en geen verdere configuratie wordt vereist.

1. Vorm het project SaaS en gegevensruimte zodat de Diensten van de Handel gegevens naar de dienst van de Manager van het Kanaal kunnen verzenden.

   ![[!DNL Commerce Service Connector] SaaS-id-configuratie in de [!DNL Admin] weergave](assets/commerce-services-connector-saas-config.png)

