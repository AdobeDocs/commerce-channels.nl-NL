---
title: Verzenddragers toewijzen
description: 'Map attributes for matching [DNL! Commerce] producten aan bestaande  [!DNL Walmart Marketplace]  lijsten en het synchroniseren van gegevens tussen  [!DNL Channel Manager]  en  [!DNL Walmart].'
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Verzenddragers toewijzen

Alvorens u [ de ladingen van de procesorde ](process-orders.md#ship-an-order) voor [!DNL Walmart Marketplace] orden, kaarteer de voorkeur van Walmart het verschepen dragers aan de overeenkomstige drager in [!DNL Commerce] zodat de het verschepen gegevens tussen [!DNL Walmart] en [!DNL Commerce] kunnen worden gesynchroniseerd.

Commerce-carriers die niet aan een voorkeurscarrier zijn toegewezen, krijgen het label *[!UICONTROL Other Carrier]* on [!DNL Walmart] .

**Eerste vereisten**

Voer de volgende taken uit voordat u verzenddragers toewijst:

1. Herzie de [ Methoden van de Drager en het Verzenden Beste praktijken voor levering op tijd ](https://sellerhelp.walmart.com/s/guide?article=000009473) voor [!DNL Walmart Marketplace].

1. Controleer de [[!UICONTROL Shipping Carrier] ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) en [[!UICONTROL Shipping Settings] ](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) configuratie in uw [!DNL Commerce] opslag om ervoor te zorgen dat u de configuratie voor [!DNL Walmart Marketplace sales] hebt geoptimaliseerd.

## Kaart met verzendende maatschappijen

1. Selecteer **[!UICONTROL Channel Settings]** op de pagina **[!UICONTROL Listings]** of **[!UICONTROL Orders]** .

1. Selecteer **[!UICONTROL Shipping Carriers]** bij **[!UICONTROL Channel Settings]** .

   ![ Kaart verzendende dragers ](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. Voor elke [!DNL Walmart] voorkeurscarrier die wordt vermeld, selecteert u de [!DNL Commerce] -naam in het vervolgkeuzemenu als de carrier beschikbaar is.

1. Selecteer **[!UICONTROL Save]** om de configuratie toe te passen.

