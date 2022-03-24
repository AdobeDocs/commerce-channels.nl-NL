---
title: Sales Channel verbinden met [!DNL Walmart Marketplace]
description: Vorm het verkoopkanaal en verbind met de Marketplace van de Markeren van de Markeren.
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 8f07b215c20cc28aa9a6862bcb2b00da30a1ed84
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---


# Verbinden met [!DNL Walmart Marketplace]

Na installatie van Channel Manager op uw [!DNL Commerce] bijvoorbeeld, verbind een opslag van de Handel met Walmart Marketplace.

1. Het verkoopkanaal maken op [het selecteren van de Commerce Store voor productaanbiedingen](#select-the-commerce-store-for-the-sales-channel).

1. [Het kanaal verbinden met [!DNL Walmart Marketplace] door Walmart API-referenties toe te voegen](#connect-the-channel-to-walmart-marketplace).

1. [Volledige installatie verkoopkanaal](#complete-store-setup) zodat je aanbiedingen, voorraad, prijs en verkoop kunt beheren vanuit Channel Manager.

## Het verkoopkanaal maken

1. Kanaalbeheer openen.

   - Selecteer in Beheer de optie **[!UICONTROL Marketing** > _Kanalen _> **Kanaalbeheer]**.

   - Selecteren **[!UICONTROL Connect New Store]**.

      ![Connect Commerce-winkel naar [!DNL Walmart Marketplace] van [!DNL Channel Manager]](assets/connect-commerce-store-to-marketplace.png)


1. De opslag en verbinding configureren:

   - Voer een unieke waarde in **[!UICONTROL store name]**.

   - Selecteer **[!UICONTROL Adobe Commerce site]** voor productaanbiedingen.

   - Een **[!UICONTROL email address]** om dienstberichten te ontvangen met betrekking tot [!DNL Channel Manager].

      ![Verbinding tussen Handel en vormen [!DNL Walmart Marketplace] van [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)


## Verbind het kanaal met de Marketplace van het Slim

1. Voeg de geloofsbrieven voor toe de [!DNL Walmart Marketplace Adobe Production API key] van uw [!DNL Walmart Marketplace Seller] account.

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

1. [!UICONTROL Save] de configuratie om de verbinding tot stand te brengen.

   Nadat de verbinding is gelukt, beheert u het kanaal vanuit **[!UICONTROL Channel Manager > Marketplace Stores]**.

   ![[!DNL Walmart Marketplace API key] configuratiepagina](assets/manage-connected-stores.png)


### Verbindingsproblemen oplossen

Als de verbinding met Walmart ontbreekt, zie [Veelgestelde vragen over Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;} voor tips voor het oplossen van problemen.

- Van de [!DNL Walmart Developer Portal], controleert u of u de juiste gegevens voor de productie-API-sleutel hebt gekopieerd voor [!UICONTROL Adobe Inc.]

- Verifieer dat de toegangsconfiguratie voor de sleutel van de Adobe API van het Smarm de correcte toestemmingen heeft. Zie [Walmart-vereisten](walmart-prerequisites.md##generate-a-walmart-marketplace-api-key).

- Bevestig dat de dienst van de Marm API beschikbaar is bij [De statuspagina van de Walmart-API](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.
