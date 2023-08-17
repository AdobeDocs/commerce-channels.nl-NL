---
title: Integratie met een [!DNL Amazon Seller Account]
description: Voordat u het instapproces start, moet u een Amazon Sales Channel Store maken (toevoegen) en deze koppelen aan uw Amazon-verkopersaccount.
role: Admin, Developer
feature: Sales Channels, Configuration, Integration, Tools and External Services
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Integratie met een [!DNL Amazon Seller Account]

Als u aan de slag wilt met Amazon-verkoopkanalen, moet u een Amazon-winkel voor verkoopkanalen maken (toevoegen) en deze koppelen aan uw [!DNL Amazon Seller Account]. Deze twee stappen integreren uw [!DNL Commerce] en Amazon-accounts kunnen gegevens delen, producten synchroniseren en nog veel meer.

_U hebt de primaire aanmeldingsgegevens voor uw [!DNL Amazon Seller Central] -account (het e-mailadres of telefoonnummer waarmee de verkopersaccount wordt aangemaakt) om verbinding te maken met je winkel._

>[!NOTE]
>
>Na de eerste winkelintegratie wordt u jaarlijks gevraagd om de Amazon-verbinding met het verkoopkanaal te vernieuwen door opnieuw toegang te verlenen. U kunt deze machtiging vernieuwen of intrekken in het dialoogvenster _Huidige vergunningen_ in de tabel _Amazon MWS-ontwikkelaarsmachtigingen_ van de **Instellingen** > **Gebruikersmachtigingen** pagina van je verkopersaccount.

## Een Amazon-winkel toevoegen

1. Op de _Beheerder_ zijbalk, ga naar **Marketing** > _Kanalen_ > **Amazon Sales Channel**.

   Als je de eerste Amazon-winkel voor verkoopkanalen toevoegt, _Taken vooraf instellen_ wordt weergegeven. Nadat uw eerste winkel is toegevoegd, kunnen taken die vooraf zijn ingesteld, worden geopend op het tabblad [Amazon-verkoopkanaal naar huis](./amazon-sales-channel-home.md) pagina onder _Leren en voorbereiden_ in het linkerzijmenu.

1. Klik op **[!UICONTROL Add Amazon Store]**.

   De _[!UICONTROL Add Amazon sales channel]_pagina wordt geopend.

   ![De Amazon-winkel voor verkoopkanalen toevoegen](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. Voor **[!UICONTROL Magento Website to use for Amazon Listing]**, kiest u welke [!DNL Commerce] websites om verbinding te maken voor deze Amazon-winkel voor verkoopkanalen.

   Deze instelling definieert ook de standaardinstelling [!DNL Commerce] opslaan voor [Amazon-orders importeren](./order-settings.md).

1. Voor **[!UICONTROL Email Address]**, voer uw gewenste e-mailadres in.

1. Voor **[!UICONTROL New Store Name]**, voert u een beschrijvende naam in voor de nieuwe Amazon-winkel voor verkoopkanalen.

   >[!NOTE]
   >
   >Deze naam wordt gebruikt als een [!DNL Commerce] en identificeert de winkel op de [Amazon-verkoopkanaal naar huis](./amazon-sales-channel-home.md) pagina. U wilt het iets maken uw team gemakkelijk kan identificeren. De naam van je Amazon-winkel die in de Verenigde Staten verkoopt, kan bijvoorbeeld worden vermeld `Amazon Store USA`.

1. Voor **[!UICONTROL Amazon Marketplace Country]** kiest u de regio/het land waarin deze Amazon-winkel producten verkoopt. Opties:

   - Verenigde Staten
   - Canada
   - Mexico
   - Verenigd Koninkrijk

1. In de _[!UICONTROL Map your Magento attributes to Amazon]_Ga als volgt te werk:

   - Voor **[!UICONTROL Product ID on the Amazon market]**, kiest u het Amazon-kenmerk dat u wilt toewijzen aan de [!DNL Commerce] hieronder geselecteerd kenmerk.

     Met deze id kunnen overeenkomende producten in uw [!DNL Commerce] catalogus.

   - Voor **[!UICONTROL Map a Magento attribute]**, kiest u de [!DNL Commerce] productkenmerk dat moet worden toegewezen aan het Amazon-kenmerk dat hierboven is geselecteerd.

     [Toewijzingskenmerken](./ob-creating-magento-attributes.md) helpt ervoor te zorgen dat je Amazon-aanbieding correct overeenkomt met het corresponderende product in je [!DNL Commerce] catalogus.

1. Klik op **[!UICONTROL Connect]**.

   Het dialoogvenster wordt gesloten en de nieuwe winkel wordt weergegeven op het tabblad [Amazon-verkoopkanaal naar huis](./amazon-sales-channel-home.md) pagina met een bevestigingsbericht.

## Een winkel verbinden met [!DNL Amazon Seller Central]

1. Klik op het opslagdashboard op **[!UICONTROL Connect store]** op de winkelkaart die u wilt starten [!DNL Amazon Seller Central] op een nieuw tabblad.

1. Voer uw [!DNL Amazon Seller Central] accountgegevens en klik op **[!UICONTROL Sign in]**.

   U moet zich aanmelden bij uw [!DNL Amazon Seller Central] account met de aanmeldingsgegevens voor de primaire gebruiker (het e-mailadres of telefoonnummer waarmee de verkopersaccount is gemaakt).

1. Voer desgevraagd de code in die u van Amazon ontvangt en klik op **[!UICONTROL Sign in]**.

1. Op de _[!UICONTROL Amazon Marketplace Web Service]_bevestigingspagina, selecteer &quot;[!UICONTROL I understand...]&quot; selectievakje en klik op **[!UICONTROL Next]**.

1. Op de _[!UICONTROL You are almost done]_bericht, klik **[!UICONTROL Continue]**.

   U hebt Amazon-verkoopkanalen toestemming gegeven om gegevens te openen en met uw [!DNL Amazon Seller Central] account. De Amazon-pagina wordt gesloten en er verschijnt een bevestigingsbericht.

   De [Amazon-verkoopkanaal naar huis](./amazon-sales-channel-home.md) wordt weergegeven met je Amazon-winkelkaarten.

   Als u het opslagdashboard wilt weergeven, klikt u op **[!UICONTROL View Store]** op de winkelkaart.

![Amazon verkoopkanaal naar huis met nieuwe winkelkaart](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

Je nieuwe Amazon-winkel voor verkoopkanalen is nu verbonden met je [!DNL Amazon Seller Central] account.

![Volgende pictogram](assets/btn-next.png) [**Doorgaan met het maken van een aanbiedingsregel**](./ob-create-listing-rule.md)
