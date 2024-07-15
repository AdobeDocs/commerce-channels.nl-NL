---
title: Walmart Marketplace-verbinding beheren
description: 'Werk de API-referenties bij om de verbinding tussen een [DNL!] te autoriseren Commerce] opslagmening en de  [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce]  productlijsten en synchroniseer inventaris, prijs, orde, en het verschepen gegevens tussen  [!DNL Commerce]  en de Maroom van het Las.'
role: Admin, Developer
feature: Sales Channels, Configuration, Shipping/Delivery, Integration
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Verzenddragers toewijzen

Alvorens u [ de ladingen van de procesorde ](process-orders.md#ship-an-order) voor [!DNL Walmart Marketplace] orden, kaarteer de voorkeur van Walmart het verschepen dragers aan de overeenkomstige drager in [!DNL Commerce] zodat de het verschepen gegevens tussen [!DNL Walmart] en [!DNL Commerce] kunnen worden gesynchroniseerd.

Commerce-carriers die niet aan een voorkeurscarrier zijn toegewezen, krijgen het label *[!UICONTROL Other Carrier]* on [!DNL Walmart] .

**Eerste vereisten**

De Vereisten van het overzicht [ Walmart ](walmart-requirements.md) voor [!DNL Marketplace Seller account].

## Verbindingsgegevens bijwerken

1. Selecteer **[!UICONTROL Channel Settings]** op de pagina [!UICONTROL Listings] voor de winkel met verkoopkanalen.

1. Selecteer **[!UICONTROL Walmart Connection]** bij **[!UICONTROL Channel Settings]** .

1. Selecteer **[!UICONTROL Change Credentials]** als u de referenties wilt wijzigen

   ![ Update de Marm API geloofsbrieven om verbinding ](assets/update-connection-credentials.png){width="700" zoomable="yes"} toe te staan

1. Voer de **[!UICONTROL Walmart Client ID]** en **[!UICONTROL Walmart Client Secret]** in.

1. Selecteer **[!UICONTROL Save]** om de configuratie toe te passen.
