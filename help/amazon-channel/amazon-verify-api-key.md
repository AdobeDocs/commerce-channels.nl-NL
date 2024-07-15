---
title: De Amazon API-sleutel toevoegen of verifiëren
description: In uw Commerce-configuratie kunt u met de gevalideerde Amazon API-sleutel uw winkels integreren met uw Amazon Seller-account.
role: Admin, Developer
feature: Sales Channels, Integration, Tools and External Services
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# De Amazon API-sleutel toevoegen of verifiëren

Wanneer u Amazon-verkoopkanalen opent, controleert en valideert [!DNL Commerce] automatisch de Amazon API-sleutel die u in uw winkelconfiguratie hebt toegevoegd. Als bevestigd, dan kunt u zich op de volgende stap, [ Integratie van de Opslag ](./store-integration.md) bewegen.

Als de Amazon API-sleutel ontbreekt, ongeldig of verlopen is, moet u de sleutel bijwerken. Er verschijnt een bericht waarin u wordt gevraagd een API-sleutel op te halen en deze toe te voegen aan de configuratie van het Amazon-verkoopkanaal.

## De Amazon API-sleutel ophalen en toevoegen wanneer hierom wordt gevraagd

De API-sleutel wordt telkens gevalideerd wanneer u uw Amazon-verkoopkanaal opent.

1. Meld u aan bij de [!DNL Commerce] Admin.

1. Ga op de zijbalk van _[!UICONTROL Admin]_naar **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]** .

   Als het uw eerste keer is dat u Amazon-verkoopkanaal opent of als uw API-sleutel moet worden bijgewerkt, vraagt het systeem u om het proces.

   ![ krijg en voeg de Zeer belangrijke Vraag van Amazon API toe ](assets/amazon-api-verification-prompt.png){width="500"}

1. Klik op **[!UICONTROL Sign in]** om uw [!DNL Commerce] -webaccount te openen.

   De pagina Commerce-accounts wordt geopend in een nieuw browsertabblad.

   - Als u bent aangemeld bij uw [!DNL Commerce] -account, wordt de _[!UICONTROL API Portal]_-sectie van de_[!UICONTROL My Account]_ -pagina automatisch weergegeven.

   - Als u niet bent aangemeld, wordt u gevraagd uw gebruikersnaam en wachtwoord voor de [!DNL Commerce] -account in te voeren voordat het tabblad _[!UICONTROL API Portal]_wordt weergegeven.

   - Als u geen rekening hebt, bezoek [ de  [!DNL Commerce]  rekeningspagina ](https://account.magento.com/customer/account/login/) {target="_blank"} en registreer. Deze account moet onderdeel zijn van uw bedrijf of bedrijf.

1. Indien nodig kunt u API-sleutels weergeven en genereren op het tabblad _[!UICONTROL API Portal]_in uw [!DNL Commerce] -account.

   Als u een API-sleutel wilt maken, voert u een beschrijving in zoals `Amazon Sales Channel` en klikt u op **[!UICONTROL Add New]** . De nieuwe sleutel wordt geproduceerd en getoond met de naam die u inging. Klik op **[!UICONTROL Copy]** om de nieuwe toets te kopiëren.

   ![ produceer of kopieer een API sleutel ](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. Wanneer de nieuwe sleutel is gegenereerd en gekopieerd, gaat u terug naar de tab _[!UICONTROL Amazon Sales Channel]_in de browser.

1. Klik op de pagina _[!UICONTROL Welcome to Amazon Sales Channel]_op **[!UICONTROL Add the key]**.

   De browser sluit het Amazon-verkoopkanaal af en een winkelconfiguratiepagina opent de pagina _[!UICONTROL Api Keys]_in [!DNL Commerce] Admin. U kunt deze pagina handmatig openen wanneer u naar **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]** gaat, **[!UICONTROL Services]** in het linkerdeelvenster uitvouwt en **[!UICONTROL Magento Services]** kiest.

1. Plak de gekopieerde sleutel voor **[!UICONTROL Production Api key]** .

1. Klik op **[!UICONTROL Save Config]**. Je kunt nu terugkeren naar het verkoopkanaal van Amazon.

   ![ Toevoegend uw API Sleutel in uw archiefconfiguratie ](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. Ga op de zijbalk van _[!UICONTROL Admin]_naar **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]** .

   Als u de Amazon-verkoopkanaaltriggers opnieuw opent, controleert en valideert [!DNL Commerce] de API-sleutel en kunt u doorgaan.

   Als u wordt ertoe aangezet om de sleutel opnieuw te verifiëren, herhaal dit _toevoegt en_ proces verifieert.

![ Volgende pictogram ](assets/btn-next.png) [**ga Integratie**](./store-integration.md) opslaan
