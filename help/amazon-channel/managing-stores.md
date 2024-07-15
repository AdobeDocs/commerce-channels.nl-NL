---
title: "[!UICONTROL Amazon Stores] view"
description: Ga naar de weergave Amazon-winkels om snel de basisstatistieken van al uw Amazon-winkels en toegangsbeheeropties te bekijken.
feature: Sales Channels, Storefront
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# [!UICONTROL Amazon Stores] weergave

Wanneer het bekijken van de homepage van het verkoopkanaal van Amazon, opent de _1} mening van de Opslag van Amazon door gebrek._

![ de mening van de Opslag van Amazon ](assets/amazon-sales-channel-home-tabs.png){width="600" zoomable="yes"}

In de weergave _[!UICONTROL Amazon Stores]_ziet u een &quot;winkelkaart&quot; voor elk van uw Amazon-winkels, samen met enkele basisstatistieken en beheeropties. De samenvattingsgegevens die op elke creditcard worden weergegeven, omvatten elke winkelstatus, datum waarop de winkel is gemaakt, datum waarop de winkel voor het laatst is bijgewerkt, aanbiedingen die aandacht behoeven (bijvoorbeeld: Onvolledige aanbiedingen) en de toegewezen [!DNL Commerce] -website.

Wanneer u de weergave van _[!UICONTROL Amazon Store]_bekijkt, kunt u op elke winkelkaart het volgende doen:

- Om een opslag [ dashboard ](./amazon-store-dashboard.md) te openen, klik **[!UICONTROL View Store]**.

- Als u een winkelstatus wilt wijzigen of een winkel wilt verwijderen, klikt u op **[!UICONTROL Action]** en kiest u:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Kies of u de status van de winkel wilt wijzigen in respectievelijk `Active` of `Inactive` .

     Als u de status van een `Inactive` winkel wijzigt in `Active` , worden aanbiedingen en bestellingsactiviteiten voor de winkel geactiveerd met behulp van de opslaginstellingen (zoals aanbiedingsinstellingen, prijsregels en overschrijvingen).

     Als u de status van een winkel wijzigt van `Active` in `Inactive` , worden aanbiedingen en bestellingsactiviteiten voor de winkel opgeschort. Een inactieve winkel behoudt alle winkelinstellingen en aanbiedingen, maar stopt tijdelijk de synchronisatie van prijzen, hoeveelheden en orderbeheer totdat de winkel de status `Active` krijgt. Met deze functie kunt u uw winkelactiviteiten op regionaal niveau beheren zonder dat u uw Amazon-winkel opnieuw hoeft te maken of te integreren of uw bestelling en verkoopgegevens uit het verleden kwijtraakt.

   - **[!UICONTROL Delete]** - Kies of u een winkel wilt verwijderen die u niet meer nodig hebt.

     Kies wanneer u een bestaande Amazon-winkel en de bijbehorende integratie-instellingen met uw [!DNL Amazon Seller Central] -account wilt verwijderen. Als u het account verwijdert, wordt de winkel verwijderd uit het verkoopkanaal van Amazon, samen met alle accountinstellingen, aanbiedingen, logbestanden en andere informatie over deze winkel. De opslag kan niet na schrapping worden teruggewonnen, moet een nieuwe opslag worden gecreeerd.

>[!NOTE]
>Als u de website die tijdens de integratie aan de winkel is toegewezen, wilt wijzigen, moet u de winkel verwijderen en de winkel opnieuw toevoegen met de verschillende websites die tijdens de integratie van de winkel zijn gedefinieerd.

| Winkelkaart | Beschrijving |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bovenste sectie | Omvat: <br> het gebiedspictogram voor de opslag, die tijdens [ wordt bepaald opslagintegratie ](./store-integration.md).<br> De toegewezen _[!UICONTROL Magento Website]_, die tijdens de integratie van de opslagruimte wordt gedefinieerd.<br> De_[!UICONTROL Status]_ van uw opslag. Opties: **[!UICONTROL Active]** - De winkelintegratie is voltooid en geverifieerd met Amazon en is beschikbaar voor verkoopactiviteiten. **[!UICONTROL Inactive]** - De integratie van de winkel is voltooid, maar is niet in gebruik of beschikbaar voor verkoopactiviteiten. Wanneer `Inactive` , worden je Amazon-verkopen gepauzeerd. In `Active` kunnen verkoopopbrengsten en extra instellingen worden opgeslagen om bij te werken voordat ze worden geactiveerd.<br> De *[!UICONTROL Last Updated]* datum van de meest recente verandering in de de opslagopstelling van Amazon.<br> De *[!UICONTROL Created]* datum toen de opslag van Amazon in het verkoopkanaal van Amazon werd gecreeerd. |
| Sectie Midden | Bevat een overzicht van winkelactiviteiten voor de laatste 30 dagen en omvat en waarschuwt voor aanbiedingen die aandacht behoeven. |
| Onderste sectie | Hier vindt u de opties Winkel weergeven en Handeling.<br> om het opslag [ dashboard ](./amazon-store-dashboard.md) te openen, klik **[!UICONTROL View Store]**.<br> om, een opslag te activeren te deactiveren of te schrappen, klik **[!UICONTROL Actions]**. |
