---
title: De Amazon API-sleutel toevoegen of verifiëren
description: Met de gevalideerde Amazon API-sleutel in uw configuratie voor handel kunt u uw winkels integreren met uw Amazon Seller-account.
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# De Amazon API-sleutel toevoegen of verifiëren

Als u Amazon-verkoopkanalen opent, controleert en valideert [!DNL Commerce] automatisch de Amazon API-sleutel die u in uw winkelconfiguratie hebt toegevoegd. Als bevestigd, dan kunt u zich op de volgende stap, [Integratie van de opslag](./store-integration.md) bewegen.

Als de Amazon API-sleutel ontbreekt, ongeldig of verlopen is, moet u de sleutel bijwerken. Er verschijnt een bericht waarin u wordt gevraagd een API-sleutel op te halen en deze toe te voegen aan de configuratie van het Amazon-verkoopkanaal.

## De Amazon API-sleutel ophalen en toevoegen wanneer hierom wordt gevraagd

De API-sleutel wordt telkens gevalideerd wanneer u uw Amazon-verkoopkanaal opent.

1. Meld u aan bij [!DNL Commerce] Admin.

1. Ga op de _[!UICONTROL Admin]_zijbalk naar **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Als u voor het eerst Amazon-verkoopkanaal opent of als uw API-sleutel moet worden bijgewerkt, wordt u door het proces gevraagd.

   ![Vraag over Amazon API-sleutel ophalen en toevoegen](assets/amazon-api-verification-prompt.png)

1. Klik op **[!UICONTROL Sign in]** om uw [!DNL Commerce]-webaccount te openen.

   De pagina Commerce-accounts wordt geopend in een nieuw browsertabblad.

   - Als u bent aangemeld bij uw [!DNL Commerce]-account, wordt de sectie _[!UICONTROL API Portal]_van de pagina_[!UICONTROL My Account]_ automatisch weergegeven.

   - Als u niet bent aangemeld, wordt u gevraagd om uw [!DNL Commerce] gebruikersnaam en wachtwoord voor de account in te voeren voordat het tabblad _[!UICONTROL API Portal]_wordt weergegeven.

   - Als u geen rekening hebt, bezoek [the [!DNL Commerce] account page](https://account.magento.com/customer/account/login/){target=&quot;_blank&quot;} en registreer. Deze account moet onderdeel zijn van uw bedrijf of bedrijf.

1. Indien nodig kunt u API-sleutels weergeven en genereren op het tabblad _[!UICONTROL API Portal]_in uw [!DNL Commerce]-account.

   Als u een API-sleutel wilt maken, voert u een beschrijving in zoals `Amazon Sales Channel` en klikt u op **[!UICONTROL Add New]**. De nieuwe sleutel wordt geproduceerd en getoond met de naam u inging. Klik **[!UICONTROL Copy]** om de nieuwe sleutel te kopiëren.

   ![Een API-sleutel genereren of kopiëren](assets/amazon-add-api-key.png)

1. Wanneer de nieuwe sleutel is gegenereerd en gekopieerd, gaat u terug naar het tabblad _[!UICONTROL Amazon Sales Channel]_in de browser.

1. Klik op _[!UICONTROL Welcome to Amazon Sales Channel]_op de pagina.**[!UICONTROL Add the key]**

   De browser sluit het verkoopkanaal van Amazon af en een pagina van de winkelconfiguratie opent _[!UICONTROL Api Keys]_pagina in [!DNL Commerce] Admin. U kunt deze pagina handmatig openen wanneer u naar **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]** gaat, **[!UICONTROL Services]** in het linkervenster uitvouwt en **[!UICONTROL Magento Services]** kiest.

1. Plak de gekopieerde sleutel voor **[!UICONTROL Production Api key]**.

1. Klik op **[!UICONTROL Save Config]**. Je kunt nu terugkeren naar het verkoopkanaal van Amazon.

   ![API-sleutel toevoegen in de configuratie van uw winkel](assets/config-magento-services-api-screen.png)

1. Ga op de _[!UICONTROL Admin]_zijbalk naar **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Als u de Amazon-verkoopkanaaltriggers opnieuw opent, [!DNL Commerce] controleert en valideert u uw API-sleutel en kunt u doorgaan.

   Als u opnieuw wordt gevraagd om de sleutel te verifiëren, herhaalt u dit _proces toevoegen en verifiëren_.

![Volgende ](assets/btn-next.png) [**pictogramDoorgaan met integratie opslaan**](./store-integration.md)
