---
title: "verbind  [!DNL Channel Manager]  met  [!DNL Walmart Marketplace]"
description: "Verbind een de archiefmening van Commerce met  [!DNL Walmart Marketplace]  om het verkoopkanaal tot stand te brengen om de het productlijsten van Commerce, voorraad, prijs, en orden voor de verkoop van de Marketplace van het Markeren van het Markeren te beheren."
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
role: Admin, Developer
feature: Sales Channels, Install, Integration
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Verbinden [!DNL Channel Manager] met [!DNL Walmart Marketplace]

Nadat u Kanaalbeheer op uw [!DNL Commerce] -instantie hebt geïnstalleerd, maakt u een verkoopkanaal in Kanaalbeheer en configureert u de referenties om [!DNL Channel Manager] met [!DNL Walmart Marketplace] te verbinden.

1. [ creeer het verkoopkanaal ](#create-the-sales-channel) door de [!DNL Commerce] opslag voor productlijsten te selecteren.

1. [ verbind het kanaal met  [!DNL Walmart Marketplace]  door [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace) toe te voegen.

1. [ Volledige opstelling van het verkoopkanaal ](#complete-sales-channel-store-setup) om lijsten, inventaris, tarifering, en orden voor uw [!DNL Walmart Marketplace] productassortiment te beheren.

>[!NOTE]
>
>De Manager van het kanaal vereist een één-aan-één verbinding tussen een account van het Spoor en een [!DNL Commerce] opslagmening. U kunt niet de zelfde archiefmening met veelvoudige rekeningen verbinden van de Mara.

## Het verkoopkanaal maken

1. Van Admin, open [!DNL Channel Manager] door **[!UICONTROL Marketing** > _Kanalen _te selecteren > **de Manager van het Kanaal]**.

1. Selecteer **[!UICONTROL Get Started]** in de sectie **[!UICONTROL Marketplaces available to connect]** .

   ![ Nieuwe [!DNL Walmart] winkel verbinden met [!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}

1. Stel zo nodig uw [!DNL Walmart Marketplace Seller] -account in.

1. De opslag en verbinding configureren:

   - Selecteer **[!UICONTROL Add Credentials]** .

   - Selecteer de winkelweergave van [!DNL Commerce] waarin de producten staan die u op de markt wilt verkopen.

     ![ Vorm verbinding tussen [!DNL Commerce] en [!DNL Walmart Marketplace] van [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png){width="500" zoomable="yes"}

   - Voer een uniek **[!UICONTROL store name]** in.

   - Selecteer **[!UICONTROL Adobe [!DNL Commerce] site]** voor productaanbiedingen en orderverwerking.

   - Voeg een **[!UICONTROL email address]** toe om meldingen te ontvangen die betrekking hebben op [!DNL Channel Manager] .

1. Sluit het kanaal aan op [!DNL Walmart Marketplace] .

   - Voeg de referenties voor de [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) toe vanuit uw [!DNL Walmart Marketplace Seller] -account.

   - Als u niet over de referenties beschikt, kunt u deze ophalen uit de [!DNL Walmart Marketplace Developer Portal] door **[!UICONTROL Get API credentials]** te selecteren.

     Selecteer in het Developer Portal uw regio (VS en Canada) en meld u vervolgens aan.

     ![[!DNL Walmart Marketplace] accountaanmelding ](assets/walmart-marketplace-login-page.png){width="600"}

   - Kopieer op het API-sleutelformulier de waarden **[!UICONTROL Client ID]** en **[!UICONTROL Client Secret]** voor de [!UICONTROL Adobe Inc Production API key] naar een beveiligde locatie en sla deze op.

     ![[!DNL Walmart Marketplace API key] configuratiepagina ](assets/walmart-api-key-management-form.png){width="600" zoomable="yes"}

     >[!NOTE]
     >
     >Als de sleutel [!DNL Adobe Inc] niet in het portaal voor ontwikkelaars wordt vermeld, selecteert u **[!UICONTROL Add New Key for a Solution Provider]** om machtigingen te configureren en de sleutel te genereren. Voor configuratiedetails, zie [ a  [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key) produceren.

   - Ga terug naar [!DNL Channel Manager] om de referenties aan de **[!UICONTROL Walmart Connection]** -gegevens toe te voegen.

     Wanneer u geloofsbrieven toevoegt, verbergt de Adobe het cliëntgeheim en slaat de waarde in een veilige kluis op.

1. Selecteer **[!UICONTROL Save Store]** om de configuratie toe te passen en verbinding te maken met [!DNL Walmart marketplace] .

1. Na met succes het verbinden, [ volledige opslagopstelling ](complete-sales-channel-store-setup.md) van de **[!UICONTROL Channel Manager]** opslagpagina.

![ de eerste opslag van de Opstelling ](assets/channel-manager-setup-first-store.png){width="500" zoomable="yes"}

### Verbindingsproblemen oplossen

Als de verbinding aan [!DNL Walmart] ontbreekt, zie [ Veelgestelde Veelgestelde Veelgestelde vragen van de Markt van de Markt 1} ](https://developer.walmart.com/faq/us/faq-auth/) {target="_blank"} voor het oplossen van problemenuiteinden.

- Controleer in het [!DNL Walmart Developer Portal] of u de juiste gegevens voor de productie-API-sleutel voor [!UICONTROL Adobe Inc.] hebt gekopieerd.

- Controleer of de toegangsconfiguratie voor de [!UICONTROL Walmart Adobe API key] de juiste machtigingen heeft. Zie [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key) .

- Bevestig dat de [!DNL Walmart API] dienst van de [ Slimme API statuspagina ](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/) {target="_blank"} beschikbaar is.
