---
title: Sales Channel-instellingen
description: Om registreren, cron bron, en synchronisatie voor de functies van het verkoopkanaal van Amazon te beheren, werk de configuratie van de Handel bij.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Sales Channel-instellingen

Wanneer de extensie [!DNL Amazon Sales Channel] is geïnstalleerd, worden standaardwaarden ingesteld in Admin for Amazon. Deze instellingen kunnen worden gewijzigd in de configuratie-instellingen voor uw Amazon-winkel. Deze instellingen zijn:

- Intervallen voor het wissen van de geschiedenis van het activiteitenlog
- Bronselectie uitsnijden
- Synchronisatieopties voor logbestanden

## De instellingen voor de kanalen voor handel wijzigen

1. Ga op de zijbalk _Admin_ naar **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Vouw **[!UICONTROL Sales Channels]** in het linkerdeelvenster uit en kies **[!UICONTROL Global Settings]**.

1. Kies voor **[!UICONTROL Clear Log History]** een optie:

   - `Once Daily` - Verkies om uw geschiedenis van de winkelactiviteit één keer per dag te ontruimen.

   - `Once Weekly` - Maak de historie van je winkelactiviteiten één keer per week leeg.

   - `Once Monthly` - (Standaard) Wis de historie van je winkelactiviteiten één keer per maand.

1. Kies **[!UICONTROL Background Tasks (CRON) Source]** bij `Magento CRON`.

   Met deze optie kan het Amazon-verkoopkanaal de [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html)-instellingen gebruiken om de communicatie- en gegevenssync-intervallen met [!DNL Amazon Seller Central] te bepalen.

1. Kies **[!UICONTROL Enable Debug Logging]** om extra synchronisatiegegevens te verzamelen wanneer het probleem moet worden opgelost.`Enabled`

   Logboekregistratie van Amazon-verkoopkanalen wordt naar het `{Commerce Root}/var/log/channel_amazon.log`-bestand geschreven en kan worden weergegeven in [ontwikkelingsmodus](https://docs.magento.com/user-guide/magento/installation-modes.html){:target=&quot;_blank&quot;}. Logboekregistratie mag alleen `Enabled` zijn tijdens het oplossen van problemen en moet `Disabled` zijn wanneer het oplossen van problemen is voltooid.

1. Klik op **[!UICONTROL Save Config]**.

![Sales Channel-configuratie-instellingen](assets/config-sales-channel-global-settings.png)
