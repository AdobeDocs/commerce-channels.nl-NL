---
title: Verkoopkanaal verbinden met [!DNL Walmart Marketplace]
description: Vorm het verkoopkanaal en verbind met de Marketplace van de Markeren van de Markeren.
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 7a400bf0b09e65d5375dc15c6a1e004d0fef0592
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Verkoopkanaal verbinden met [!DNL Walmart Marketplace]

Na installatie van Channel Manager op uw [!DNL Commerce] bijvoorbeeld, verbind een opslag van de Handel met Walmart Marketplace.

1. [Het verkoopkanaal maken](#create-the-sales-channel) door de winkel Commerce te selecteren voor productaanbiedingen.

1. [Het kanaal verbinden met [!DNL Walmart Marketplace] door Walmart API-referenties toe te voegen](#connect-the-channel-to-walmart-marketplace).

1. [Volledige installatie verkoopkanaal](#complete-store-setup) om aanbiedingen, voorraad, prijzen en bestellingen voor je productassortiment van de Marketplace te beheren.

## Het verkoopkanaal maken

1. Open [!DNL Channel Manager].

   - Selecteer in Beheer de optie **[!UICONTROL Marketing** > _Kanalen _> **Kanaalbeheer]**.

1. In de **[!UICONTROL Marketplaces available to connect]** sectie, selecteert u **[!UICONTROL Get Started]**.

   ![Nieuwe Walmart-winkel verbinden met [!DNL Channel Manager]](assets/channel-manager-home.png)

1. Stel zo nodig je account bij Marketplace van Walmart in.

1. De opslag en verbinding configureren:

   - Selecteren **[!UICONTROL Add Credentials]**.

   - Op de [!UICONTROL Connect New Walmart Store] Selecteer de Winkelweergave Commerce om verbinding te maken met de Marketplace.

      ![Verbinding tussen Handel en vormen [!DNL Walmart Marketplace] van [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - Voer een unieke waarde in **[!UICONTROL store name]**.

   - Selecteer **[!UICONTROL Adobe Commerce site]** voor productaanbiedingen.

   - Een **[!UICONTROL email address]** om dienstberichten te ontvangen met betrekking tot [!DNL Channel Manager].

1. Het kanaal verbinden met [!DNL Walmart Marketplace].

   - Voeg de geloofsbrieven voor toe de [[!DNL Walmart Marketplace Adobe Production API key]](walmart-prerequisites.md#generate-a-walmart-marketplace-production-api-key) van uw [!DNL Walmart Marketplace Seller] account.

   - Als u niet over de referenties beschikt, selecteert u **[!UICONTROL Get API credentials]** om ze van de [!DNL Walmart Marketplace Developer Portal].

      Selecteer desgevraagd uw regio (VS en Canada) en meld u vervolgens aan.

      ![[!DNL Walmart Marketplace] accountaanmelding](assets/walmart-marketplace-login-page.png)

   - Kopieer en sla de **[!UICONTROL Client ID]** en **[!UICONTROL Client Secret]** waarden voor de [!UICONTROL Adobe Inc Production API key] naar een beveiligde locatie.

      ![[!DNL Walmart Marketplace API key] configuratiepagina](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >Als de [!DNL Adobe Inc] De sleutel wordt niet vermeld in het Developer Portal. Selecteer **[!UICONTROL Add New Key for a Solution Provider]** om toestemmingen te vormen en de sleutel te produceren. Voor configuratiedetails, zie [Een [!DNL Walmart Marketplace API Key]](walmart-prerequisites.md#generate-a-walmart-marketplace-api-key).

   - Terug naar [!DNL Channel Manager] om de geloofsbrieven aan toe te voegen **[!UICONTROL Walmart Connection]** informatie.

      Wanneer u referenties toevoegt aan [!DNL Channel Manager], verbergt Adobe het clientgeheim en slaat de waarde op in een beveiligde kluis.

1. Selecteren **[!UICONTROL Save Store]** om de configuratie toe te passen en met [!DNL Walmart marketplace].

1. Na verbinding met succes, [volledige installatie van de winkel](complete-store-setup.md) van de **[!UICONTROL Channel Manager]** winkellijstpagina.

![Eerste winkel instellen](assets/channel-manager-setup-first-store.png)

### Verbindingsproblemen oplossen

Als de verbinding met Walmart ontbreekt, zie [Veelgestelde vragen over Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;} voor tips voor het oplossen van problemen.

- Van de [!DNL Walmart Developer Portal], controleert u of u de juiste gegevens voor de productie-API-sleutel hebt gekopieerd voor [!UICONTROL Adobe Inc.]

- Verifieer dat de toegangsconfiguratie voor de sleutel van de Adobe API van het Smarm de correcte toestemmingen heeft. Zie [Walmart-vereisten](walmart-prerequisites.md##generate-a-walmart-marketplace-api-key).

- Bevestig dat de [!DNL Walmart API] de dienst is beschikbaar bij [De statuspagina van de Walmart-API](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.
