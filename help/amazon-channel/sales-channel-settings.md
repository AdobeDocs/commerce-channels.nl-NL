---
title: Sales Channel-instellingen
description: Om registreren, cron bron, en synchronisatie voor de functies van het verkoopkanaal van Amazon te beheren, werk de configuratie van de Handel bij.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 5508fe6e6b2193eaaebc78f485aae972504554cc
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Sales Channel-instellingen

Wanneer de [!DNL Amazon Sales Channel] Als de extensie is geïnstalleerd, worden standaardwaarden ingesteld in het verkoopkanaal Admin for Amazon. Deze instellingen kunnen worden gewijzigd in de configuratie-instellingen voor uw Amazon-winkel. Deze instellingen zijn:

- Intervallen voor het wissen van de geschiedenis van het activiteitenlog
- Bronselectie uitsnijden
- Synchronisatieopties voor logbestanden

## De instellingen voor de kanalen voor handel wijzigen

1. Op de _Beheer_ zijbalk, ga naar **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Vouw in het linkerdeelvenster uit **[!UICONTROL Sales Channels]** en kiest u **[!UICONTROL Global Settings]**.

1. Voor **[!UICONTROL Clear Log History]** kiest u een optie:

   - `Once Daily` - Verkies om uw geschiedenis van de winkelactiviteit één keer per dag te ontruimen.

   - `Once Weekly` - Maak de historie van je winkelactiviteiten één keer per week leeg.

   - `Once Monthly` - (Standaard) Wis de historie van je winkelactiviteiten één keer per maand.

1. Voor **[!UICONTROL Background Tasks (CRON) Source]** kiest u `Magento CRON`.

   Met deze optie kan Amazon je verkoopkanaal gebruiken [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) instellingen om de communicatie- en gegevenssynchronisatieintervallen te bepalen met [!DNL Amazon Seller Central].

1. Voor **[!UICONTROL Enable Debug Logging]** kiest u `Enabled` om extra synchronisatiegegevens te verzamelen wanneer het oplossen van problemen nodig is.

   Amazon-logboekregistratie van verkoopkanalen wordt geschreven naar `{Commerce Root}/var/log/channel_amazon.log` en kan worden weergegeven in [ontwikkelmodus](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}. Logboekregistratie dient alleen plaats te vinden `Enabled` tijdens het oplossen van problemen en moet `Disabled` wanneer het oplossen van problemen volledig is.

1. Voor **[!UICONTROL Read-Only Mode]**, selecteert u `Enabled` om alle uitgaande status-veranderende API verzoeken te blokkeren.

   Met deze instelling worden potentiële wijzigingen opgeslagen, maar niet verzonden tot [!UICONTROL Read-Only Mode] is uitgeschakeld. De configuratiecache moet worden gewist voor de modus Alleen-lezen om in te schakelen. Selecteer `Disabled`.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] is ontworpen voor kopieën van de instantie Production, zoals ophaling of QA, en mag niet worden gebruikt op het productieexemplaar.
   >
   >Wanneer een database wordt gemigreerd naar een nieuwe kopie van de instantie (wordt gedetecteerd wanneer de URL van een winkel in de configuratie verandert), [!UICONTROL Read-Only Mode] wordt automatisch ingeschakeld.

1. Klik op **[!UICONTROL Save Config]**.

![Sales Channel-configuratie-instellingen](assets/config-sales-channel-global-settings.png)
