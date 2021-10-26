---
title: Sales Channel Settings
description: Om registreren, cron bron, en synchronisatie voor de functies van het verkoopkanaal van Amazon te beheren, werk de configuratie van de Handel bij.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Sales Channel settings

Wanneer de [!DNL Amazon Sales Channel] Als de extensie is geïnstalleerd, worden standaardwaarden ingesteld in het verkoopkanaal Admin for Amazon. Deze instellingen kunnen worden gewijzigd in de configuratie-instellingen voor uw Amazon-winkel. These settings include:

- Intervallen voor het wissen van de geschiedenis van het activiteitenlog
- Bronselectie uitsnijden
- Synchronisatieopties voor logbestanden

## De instellingen voor de kanalen voor handel wijzigen

1. On the _Admin_ sidebar, go to **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Vouw in het linkerdeelvenster uit **[!UICONTROL Sales Channels]** en kiest u **[!UICONTROL Global Settings]**.

1. Voor **[!UICONTROL Clear Log History]** kiest u een optie:

   - `Once Daily` - Verkies om uw geschiedenis van de winkelactiviteit één keer per dag te ontruimen.

   - `Once Weekly` - Choose to clear your store activity history once weekly.

   - `Once Monthly` - (Standaard) Wis de historie van je winkelactiviteiten één keer per maand.

1. Voor **[!UICONTROL Background Tasks (CRON) Source]** kiest u `Magento CRON`.

   Met deze optie kan Amazon je verkoopkanaal gebruiken [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) instellingen om de communicatie- en gegevenssynchronisatieintervallen te bepalen met [!DNL Amazon Seller Central].

1. Voor **[!UICONTROL Enable Debug Logging]** kiest u `Enabled` om extra synchronisatiegegevens te verzamelen wanneer het oplossen van problemen nodig is.

   Amazon-logboekregistratie van verkoopkanalen wordt geschreven naar `{Commerce Root}/var/log/channel_amazon.log` en kan worden weergegeven in [ontwikkelmodus](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}. Logging should only be `Enabled` during troubleshooting and should be `Disabled` when troubleshooting is complete.

1. Klikken **[!UICONTROL Save Config]**.

![Sales Channel configuration settings](assets/config-sales-channel-global-settings.png)
