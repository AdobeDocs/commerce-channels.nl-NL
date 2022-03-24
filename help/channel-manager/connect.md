---
title: Verbinden met de Diensten van de Handel
description: Connect Channel Manager-instantie naar [!DNL Commerce services] om gegevenssynchronisatie en communicatie tussen de instantie van de Handel, Manager van het Kanaal, en andere ondersteunende diensten toe te laten.
role: User
level: Intermediate
source-git-commit: ec950579a9b2220f9ec106b616779fc3503f3add
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Verbinden met de Diensten van de Handel

De schakelaar van de Diensten van de Handel integreert de dienst van de Manager van het Kanaal met instanties Adobe Commerce en Magento Open Source. De schakelaar laat gegevenssynchronisatie en communicatie tussen toe [!DNL Commerce] instantie, [!DNL Channel Manager]en andere ondersteunende diensten.

De opstelling van de Verbinding van de Diensten van de Handel is een eenmalig proces dat wordt vereist om Adobe te gebruiken [Commerciële SaaS-diensten](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;} als [!DNL Channel Manager], [!DNL Live Search], en [!DNL Product Recommendations]. Als u reeds de schakelaar voor een andere dienst hebt gevormd, kunt u deze stap overslaan.

## Vereisten

- **Handelsaccount met [Toegang voor beheerders](https://docs.magento.com/user-guide/stores/admin.html){target=&quot;_blank&quot;}** aan uw instantie van de Handel**-Rekeningeigenaars en Admin-gebruikers kunnen gebruikersrekeningen van de Inschakeling van de Handel of van de bevellijn plaatsen gebruikend [!DNL Commerce] CLI, opdracht `admin:user:create`.

- **Adobe Commerce [API-sleutels voor productie](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;}**-API-toegang inschakelen tot services die worden vereist door Channel Manager

   Om de geloofsbrieven te verstrekken, heeft een de vergunninghouder of rekeninghouder van de Handel opties om
   [gedeelde toegang](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;} of geef de [API-sleutel](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} referenties naar een vertrouwde ontwikkelaar.

## De Commerce Services Connector configureren

1. Open de Configuratie van de Diensten van de Opslag.

   - Selecteer bij Beheer de optie [!UICONTROL Stores].

   - Onder *Instellingen*, selecteert u [!UICONTROL Configuration].

   - Op de [!UICONTROL Configuration] pagina, uitvouwen [!UICONTROL Services] en selecteert u [!UICONTROL Commerce Services Connector].

1. Voeg de API-sleutels voor productie toe van uw Adobe Commerce-account.

   ![[!DNL Commerce Service Connector] in de [!DNL Admin] weergave](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Als uw [!DNL Commerce] instantie heeft andere [!DNL Adobe Commerce] services zoals [!DNL Live Search] of [!DNL Product Recommendations] geïnstalleerd, wordt de referentie informatie getoond in de interface, en geen verdere configuratie wordt vereist.

1. Vorm het project SaaS en gegevensruimte zodat de Diensten van de Handel gegevens naar de dienst van de Manager van het Kanaal kunnen verzenden.

   ![[!DNL Commerce Service Connector] SaaS-id-configuratie in de [!DNL Admin] weergave](assets/commerce-services-connector-saas-config.png)

