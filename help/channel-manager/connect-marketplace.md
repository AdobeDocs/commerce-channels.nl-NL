---
title: '''Verbinden [!DNL Channel Manager] tot [!DNL Walmart Marketplace]'''
description: '"Verbind een de opslagmening van de Handel met [!DNL Walmart Marketplace] om het verkoopkanaal te creëren voor het beheren van aanbiedingen, voorraad, prijs en bestellingen van producten voor de handel in Walmart Marketplace."'
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 8146be1c94ffb1c8abd0d28e53d3476fd78f2c62
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Verbinden [!DNL Channel Manager] tot [!DNL Walmart Marketplace]

Na installatie van Channel Manager op uw [!DNL Commerce] instantie, een verkoopkanaal in de Manager van het Kanaal creëren en de geloofsbrieven vormen om te verbinden [!DNL Channel Manager] tot [!DNL Walmart Marketplace].

1. [Het verkoopkanaal maken](#create-the-sales-channel) door [!DNL Commerce] winkel voor productaanbiedingen.

1. [Het kanaal verbinden met [!DNL Walmart Marketplace] door toevoegen [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Volledige installatie verkoopkanaal](#complete-store-setup) om aanbiedingen, voorraad, prijzen en bestellingen voor je [!DNL Walmart Marketplace] productassortiment.

>[!NOTE]
>
>De Manager van het kanaal vereist een één-aan-één verbinding tussen een rekening van het Spoor en een [!DNL Commerce] winkelweergave. U kunt niet de zelfde archiefmening met veelvoudige rekeningen verbinden van de Mara.

## Het verkoopkanaal maken

1. Open vanuit de beheerder [!DNL Channel Manager] door **[!UICONTROL Marketing** > _Kanalen _> **Kanaalbeheer]**.

1. In de **[!UICONTROL Marketplaces available to connect]** sectie, selecteert u **[!UICONTROL Get Started]**.

   ![Nieuwe verbinding maken [!DNL Walmart] opslaan naar [!DNL Channel Manager]](assets/channel-manager-home.png)

1. Indien nodig, stelt u uw [!DNL Walmart Marketplace Seller] account.

1. De opslag en verbinding configureren:

   - Selecteren **[!UICONTROL Add Credentials]**.

   - Selecteer [!DNL Commerce] Winkelweergave die de producten aanbiedt die je op de markt wilt verkopen.

      ![Verbinding configureren tussen [!DNL Commerce] en [!DNL Walmart Marketplace] van [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - Voer een unieke waarde in **[!UICONTROL store name]**.

   - Selecteer **[!UICONTROL Adobe [!DNL Commerce] site]** voor productaanbiedingen en orderverwerking.

   - Om meldingen te ontvangen met betrekking tot [!DNL Channel Manager], voegt u een **[!UICONTROL email address]**.

1. Het kanaal verbinden met [!DNL Walmart Marketplace].

   - Voeg de geloofsbrieven voor toe de [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) van uw [!DNL Walmart Marketplace Seller] account.

   - Als u niet de geloofsbrieven hebt, krijg hen van [!DNL Walmart Marketplace Developer Portal] door **[!UICONTROL Get API credentials]**.

      Selecteer in het Developer Portal uw regio (VS en Canada) en meld u vervolgens aan.

      ![[!DNL Walmart Marketplace] accountaanmelding](assets/walmart-marketplace-login-page.png)

   - Kopieer en sla de **[!UICONTROL Client ID]** en **[!UICONTROL Client Secret]** waarden voor de [!UICONTROL Adobe Inc Production API key] naar een beveiligde locatie.

      ![[!DNL Walmart Marketplace API key] configuratiepagina](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >Als de [!DNL Adobe Inc] De sleutel wordt niet vermeld in het Developer Portal. Selecteer **[!UICONTROL Add New Key for a Solution Provider]** om toestemmingen te vormen en de sleutel te produceren. Voor configuratiedetails, zie [Een [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - Terug naar [!DNL Channel Manager] om de geloofsbrieven aan toe te voegen **[!UICONTROL Walmart Connection]** informatie.

      Wanneer u geloofsbrieven toevoegt, verbergt Adobe het cliëntgeheim en slaat de waarde in een veilige kluis op.

1. Selecteren **[!UICONTROL Save Store]** om de configuratie toe te passen en met [!DNL Walmart marketplace].

1. Na verbinding met succes, [volledige installatie van de winkel](complete-store-setup.md) van de **[!UICONTROL Channel Manager]** winkelpagina.

![Eerste winkel instellen](assets/channel-manager-setup-first-store.png)

### Verbindingsproblemen oplossen

Als de verbinding met [!DNL Walmart] ontbreekt, zie [Veelgestelde vragen over Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;} voor tips voor het oplossen van problemen.

- Van de [!DNL Walmart Developer Portal], controleert u of u de juiste gegevens voor de productie-API-sleutel hebt gekopieerd voor [!UICONTROL Adobe Inc.]

- Verifieer dat de toegangsconfiguratie voor [!UICONTROL Walmart Adobe API key] heeft de juiste machtigingen. Zie [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- Bevestig dat de [!DNL Walmart API] de dienst is beschikbaar bij [De statuspagina van de Walmart-API](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.
