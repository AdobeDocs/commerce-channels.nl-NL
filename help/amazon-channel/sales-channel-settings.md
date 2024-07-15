---
title: Instellingen verkoopkanaal
description: Als u logbestanden, uitsnijdbronnen en synchronisatie voor Amazon-verkoopkanaalfuncties wilt beheren, werkt u de Commerce-configuratie bij.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Instellingen verkoopkanaal

Wanneer de extensie [!DNL Amazon Sales Channel] is geïnstalleerd, worden standaardwaarden ingesteld in het verkoopkanaal Admin for Amazon. Deze instellingen kunnen worden gewijzigd in de configuratie-instellingen voor uw Amazon-winkel. Deze instellingen zijn:

- Intervallen voor het wissen van de geschiedenis van het activiteitenlog
- Bronselectie uitsnijden
- Synchronisatieopties voor logbestanden

## De Commerce-kanaalinstellingen wijzigen

1. Voor _Admin_ sidebar, ga **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Vouw in het linkerdeelvenster **[!UICONTROL Sales Channels]** uit en kies **[!UICONTROL Global Settings]** .

1. Kies bij **[!UICONTROL Clear Log History]** een optie:

   - `Once Daily` - Verkies om de historie van uw winkelactiviteiten één keer per dag te wissen.

   - `Once Weekly` - Maak de historie van je winkelactiviteiten één keer per week leeg.

   - `Once Monthly` - (Standaard) Kies deze optie om de historie van je winkelactiviteiten één keer per maand te wissen.

1. Kies `Magento CRON` bij **[!UICONTROL Background Tasks (CRON) Source]** .

   Deze optie staat het verkoopkanaal van Amazon toe om uw [!DNL Commerce] ](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) montages van 1} Uitsnede {te gebruiken om mededeling en de intervallen van de gegevenssynchronisatie met [!DNL Amazon Seller Central] te bepalen.[

1. Kies `Enabled` voor **[!UICONTROL Enable Debug Logging]** om aanvullende synchronisatiegegevens te verzamelen wanneer problemen moeten worden opgelost.

   Amazon het registreren van het verkoopkanaal wordt geschreven aan het `{Commerce Root}/var/log/channel_amazon.log` dossier en kan op [ ontwikkelaarwijze ](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes) worden bekeken. Logboekregistratie mag alleen `Enabled` zijn tijdens probleemoplossing en moet `Disabled` zijn wanneer het oplossen van problemen is voltooid.

1. Selecteer voor **[!UICONTROL Read-Only Mode]** `Enabled` om alle uitgaande, in de status veranderende API-aanvragen te blokkeren.

   Met deze instelling worden potentiële wijzigingen opgeslagen, maar niet verzonden, totdat [!UICONTROL Read-Only Mode] is uitgeschakeld. De configuratiecache moet worden gewist voor de modus Alleen-lezen om in te schakelen. Selecteer `Disabled` om de gegevensoverdracht opnieuw te starten.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] is ontworpen voor kopieën van de instantie Production, zoals ophaling of QA, en mag niet worden gebruikt voor de instantie Production.
   >
   >Wanneer een database wordt gemigreerd naar een nieuwe kopie van de instantie (wordt gedetecteerd wanneer de URL van een winkel in de configuratie verandert), wordt [!UICONTROL Read-Only Mode] automatisch ingeschakeld.

1. Klik op **[!UICONTROL Save Config]**.

![ de configuratiemontages van de Sales Channel ](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
