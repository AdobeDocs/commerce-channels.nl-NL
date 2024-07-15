---
title: Integratie met een  [!DNL Amazon Seller Account] opslaan
description: Voordat u het instapproces start, moet u een Amazon Sales Channel Store maken (toevoegen) en deze koppelen aan uw Amazon-verkopersaccount.
role: Admin, Developer
feature: Sales Channels, Configuration, Integration, Tools and External Services
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Integratie met een [!DNL Amazon Seller Account] opslaan

Als u aan de slag wilt met Amazon-verkoopkanalen, moet u een Amazon-winkel voor verkoopkanalen maken (toevoegen) en deze koppelen aan uw [!DNL Amazon Seller Account] . Deze twee stappen integreren uw [!DNL Commerce] - en Amazon-accounts om gegevens te delen, producten te synchroniseren en meer.

_u hebt de primaire login geloofsbrieven voor uw [!DNL Amazon Seller Central] rekening (e-mail of telefoon die wordt gebruikt om de verkopersrekening tot stand te brengen) nodig om uw opslag te verbinden._

>[!NOTE]
>
>Na de eerste winkelintegratie wordt u jaarlijks gevraagd om de Amazon-verbinding met het verkoopkanaal te vernieuwen door opnieuw toegang te verlenen. U kunt deze vergunning in de _Huidige Vergunningen_ lijst van Vergunningen in de _3} sectie van de Toestemmingen van de Ontwikkelaar van Amazon MWS {van de **Montages**>**pagina van de Toestemmingen van de Gebruiker**van uw Verkoper Centrale rekening vernieuwen of intrekken._

## Een Amazon-winkel toevoegen

1. Op _Admin_ sidebar, ga **Marketing** > _Kanalen_ > **Sales Channel van Amazon**.

   Wanneer het toevoegen van uw eerste opslag van het verkoopkanaal van Amazon, verschijnt de _Modaal van Taken van de Opstelling_ pre-Opstelling. Nadat uw eerste opslag wordt toegevoegd, kunnen de pre-opstellingstaken op het [ huis van het verkoopkanaal van Amazon ](./amazon-sales-channel-home.md) pagina onder _Leren en Voorbereiding_ in het linkerzijmenu worden betreden.

1. Klik op **[!UICONTROL Add Amazon Store]**.

   De pagina _[!UICONTROL Add Amazon sales channel]_wordt geopend.

   ![ voeg de opslag van het verkoopkanaal van Amazon toe ](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. Kies bij **[!UICONTROL Magento Website to use for Amazon Listing]** welke [!DNL Commerce] -websites u wilt verbinden voor deze Amazon-winkel met verkoopkanalen.

   Dit het plaatsen bepaalt ook de standaard [!DNL Commerce] opslag voor [ het invoeren van de orden van Amazon ](./order-settings.md).

1. Voer voor **[!UICONTROL Email Address]** uw e-mailadres van uw voorkeur in.

1. Voer bij **[!UICONTROL New Store Name]** een beschrijvende naam in voor de nieuwe Amazon-winkel voor verkoopkanalen.

   >[!NOTE]
   >
   >Deze naam wordt gebruikt als [!DNL Commerce] verwijzing slechts en identificeert de opslag op de [ 2} pagina van het het verkoopkanaal van Amazon homepage {. ](./amazon-sales-channel-home.md) U wilt het iets maken uw team gemakkelijk kan identificeren. De naam van je Amazon-winkel die in de Verenigde Staten verkoopt, kan bijvoorbeeld `Amazon Store USA` zijn.

1. Kies bij **[!UICONTROL Amazon Marketplace Country]** het gebied/land waarin deze Amazon-winkel producten verkoopt. Opties:

   - Verenigde Staten
   - Canada
   - Mexico
   - Verenigd Koninkrijk

1. Ga als volgt te werk in de sectie _[!UICONTROL Map your Magento attributes to Amazon]_:

   - Kies bij **[!UICONTROL Product ID on the Amazon market]** het Amazon-kenmerk dat u wilt toewijzen aan het hieronder geselecteerde [!DNL Commerce] -kenmerk.

     Deze id zorgt ervoor dat de overeenkomende producten in de catalogus van [!DNL Commerce] correct overeenkomen.

   - Kies bij **[!UICONTROL Map a Magento attribute]** het productkenmerk [!DNL Commerce] dat u wilt toewijzen aan het hierboven geselecteerde Amazon-kenmerk.

     [ de attributen van de Toewijzing ](./ob-creating-magento-attributes.md) helpen ervoor zorgen dat uw lijst van Amazon correct met het overeenkomstige product in uw [!DNL Commerce] catalogus aanpast.

1. Klik op **[!UICONTROL Connect]**.

   De dialoog sluit en de nieuwe opslag verschijnt op het [ huis van het verkoopkanaal van Amazon ](./amazon-sales-channel-home.md) pagina met een bevestigingsbericht.

## Een winkel verbinden met [!DNL Amazon Seller Central]

1. Klik op het winkeldashboard op **[!UICONTROL Connect store]** op de winkelkaart om [!DNL Amazon Seller Central] te starten op een nieuw tabblad.

1. Voer uw [!DNL Amazon Seller Central] -accountgegevens in en klik op **[!UICONTROL Sign in]** .

   Om deze verbinding te voltooien, moet u zich aanmelden bij uw [!DNL Amazon Seller Central] -account met de aanmeldingsgegevens voor de primaire gebruiker (het e-mailadres of de telefoon waarmee de verkopersaccount is gemaakt).

1. Voer desgevraagd de code in die u van Amazon ontvangt en klik op **[!UICONTROL Sign in]** om de Amazon Two-Factor Authorization (2FA) te voltooien.

1. Selecteer op de bevestigingspagina van _[!UICONTROL Amazon Marketplace Web Service]_het selectievakje [!UICONTROL I understand...] en klik op **[!UICONTROL Next]**.

1. Klik in het _[!UICONTROL You are almost done]_-bericht op **[!UICONTROL Continue]**.

   U hebt Amazon-verkoopkanalen toestemming gegeven om gegevens te openen en te delen met uw [!DNL Amazon Seller Central] -account. De Amazon-pagina wordt gesloten en er verschijnt een bevestigingsbericht.

   De ](./amazon-sales-channel-home.md) pagina van het 0} de verkoopkanaalhuis van Amazon opent het tonen van uw de opslagkaarten van Amazon.[

   Als u het winkeldashboard wilt weergeven, klikt u op **[!UICONTROL View Store]** op de winkelkaart.

![ het huis van het verkoopkanaal van Amazon met nieuwe opslagkaart ](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

De nieuwe Amazon-winkel voor verkoopkanalen is nu verbonden met uw [!DNL Amazon Seller Central] -account.

![ Volgende pictogram ](assets/btn-next.png) [**gaat om een het Lijst van de Regel**](./ob-create-listing-rule.md) te creëren
