---
title: Opslagintegratie
description: Voordat u het instapproces start, moet u een Amazon Sales Channel-winkel maken (toevoegen) en deze koppelen aan uw Amazon-verkopersaccount.
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Integratie van winkels

Als je aan de slag wilt met Amazon-verkoopkanalen, moet je een Amazon-winkel voor verkoopkanalen maken (toevoegen) en deze koppelen aan je Amazon-verkopersaccount. Deze twee stappen integreren uw [!DNL Commerce] en Amazon rekeningen om gegevens te delen, producten te synchroniseren, en meer.

_Je hebt de primaire aanmeldingsgegevens voor je  [!DNL Amazon Seller Central] account nodig (het e-mailadres of telefoonnummer waarmee je een verkopersaccount aanmaakt) om verbinding te maken met je winkel._

>[!NOTE]
>
>Na de eerste winkelintegratie wordt u jaarlijks gevraagd om de Amazon-verbinding met het verkoopkanaal te vernieuwen door opnieuw toegang te verlenen. U kunt deze autorisatie verlengen of intrekken in de tabel _Huidige autorisaties_ in de sectie _Amazon MWS-ontwikkelaarmachtigingen_ van de pagina **Instellingen** > **Gebruikersmachtigingen** van uw Verkopersaccount.

## Een Amazon-winkel toevoegen

1. Op _Admin_ zijbalk gaat u naar **Marketing** > _Kanalen_ > **Amazon Sales Channel**.

   Wanneer u de eerste Amazon-winkel voor verkoopkanalen toevoegt, wordt de modus _Taken vóór installatie_ weergegeven. Nadat de eerste winkel is toegevoegd, zijn de vooraf ingestelde taken toegankelijk op de pagina [Amazon-verkoopkanaal home](./amazon-sales-channel-home.md) onder _Leren en voorbereiden_ in het menu aan de linkerkant.

1. Klik op **[!UICONTROL Add Amazon Store]**.

   De pagina _[!UICONTROL Add Amazon sales channel]_wordt geopend.

   ![De Amazon-winkel voor verkoopkanalen toevoegen](assets/amazon-store-integration.png)

1. Kies voor **[!UICONTROL Magento Website to use for Amazon Listing]** welke van uw [!DNL Commerce] websites u wilt verbinden voor deze Amazon-winkel met verkoopkanalen.

   Deze instelling definieert ook de standaard [!DNL Commerce]-opslag voor [het importeren van Amazon-orders](./order-settings.md).

1. Voer voor **[!UICONTROL Email Address]** uw e-mailadres van uw voorkeur in.

1. Voer bij **[!UICONTROL New Store Name]** een beschrijvende naam in voor de nieuwe Amazon-winkel voor verkoopkanalen.

   >[!NOTE]
   >
   >Deze naam wordt alleen gebruikt als een [!DNL Commerce]-verwijzing en geeft de winkel aan op de pagina [Amazon-verkoopkanaal home](./amazon-sales-channel-home.md). U wilt het iets maken uw team gemakkelijk kan identificeren. Zo krijgt uw Amazon-winkel die in de Verenigde Staten verkoopt bijvoorbeeld de naam `Amazon Store USA`.

1. Kies voor **[!UICONTROL Amazon Marketplace Country]** het gebied/land waarin deze Amazon-winkel producten verkoopt. Opties:

   - Verenigde Staten
   - Canada
   - Mexico
   - Verenigd Koninkrijk

1. Voer in de sectie _[!UICONTROL Map your Magento attributes to Amazon]_de volgende handelingen uit:

   - Kies bij **[!UICONTROL Product ID on the Amazon market]** het Amazon-kenmerk dat u wilt toewijzen aan het [!DNL Commerce]-kenmerk dat u hieronder hebt geselecteerd.

      Met deze id kunnen overeenkomende producten in uw [!DNL Commerce]-catalogus op de juiste wijze met elkaar overeenkomen.

   - Kies bij **[!UICONTROL Map a Magento attribute]** het productkenmerk [!DNL Commerce] om het kenmerk Amazon dat hierboven is geselecteerd toe te wijzen.

      [Toewijzingskenmerken ](./ob-creating-magento-attributes.md) zorgen ervoor dat je Amazon-aanbieding correct overeenkomt met het overeenkomende product in je  [!DNL Commerce] catalogus.

1. Klik op **[!UICONTROL Connect]**.

   Het dialoogvenster wordt gesloten en de nieuwe winkel wordt weergegeven op de pagina [Amazon-verkoopkanaal home](./amazon-sales-channel-home.md) met een bevestigingsbericht.

## Een winkel verbinden met [!DNL Amazon Seller Central]

1. Klik op **[!UICONTROL Connect store]** op het winkeldashboard om [!DNL Amazon Seller Central] op een nieuw tabblad te starten.

1. Voer uw [!DNL Amazon Seller Central] accountgegevens in en klik op **[!UICONTROL Sign in]**.

   Om deze verbinding te voltooien, moet u zich aanmelden bij uw [!DNL Amazon Seller Central]-account met de aanmeldingsgegevens voor de primaire gebruiker (het e-mailadres of telefoonnummer dat wordt gebruikt om de verkopersaccount te maken).

1. Voer desgevraagd de code in die u van Amazon ontvangt en klik op **[!UICONTROL Sign in]** om de Amazon Two-Factor Authorization (2FA) in te vullen.

1. Selecteer op de bevestigingspagina _[!UICONTROL Amazon Marketplace Web Service]_het selectievakje &quot;[!UICONTROL I understand...]&quot; en klik op **[!UICONTROL Next]**.

1. Klik in het _[!UICONTROL You are almost done]_-bericht op **[!UICONTROL Continue]**.

   U hebt Amazon Sales Channel toestemming verleend om gegevens te openen en te delen met uw [!DNL Amazon Seller Central]-account. De Amazon-pagina wordt gesloten en er verschijnt een bevestigingsbericht.

   De pagina [Amazon Verkoopkanaal home](./amazon-sales-channel-home.md) wordt geopend en toont uw Amazon-winkelkaarten.

   Als u het opslagdashboard wilt weergeven, klikt u op **[!UICONTROL View Store]** op de opslagkaart.

![Amazon verkoopkanaal naar huis met nieuwe winkelkaart](assets/asc-dashboard-after-2fa.png)

Uw nieuwe Amazon-winkel voor verkoopkanalen is nu verbonden met uw [!DNL Amazon Seller Central]-account.

![Volgende ](assets/btn-next.png) [**pictogramDoorgaan met het maken van een aanbiedingsregel**](./ob-create-listing-rule.md)
