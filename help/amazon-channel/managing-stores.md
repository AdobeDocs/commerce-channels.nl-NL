---
title: Weergave Amazon-winkels
description: Ga naar de weergave Amazon-winkels om snel de basisstatistieken van al uw Amazon-winkels en toegangsbeheeropties te bekijken.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Weergave Amazon-winkels

Wanneer u de Amazon-homepage van het verkoopkanaal weergeeft, kunt u _Amazon-winkels_ wordt standaard geopend.

![Weergave Amazon-winkels](assets/amazon-sales-channel-home-tabs.png)

De _[!UICONTROL Amazon Stores]_in deze weergave ziet u een &quot;winkelkaart&quot; voor elk van uw Amazon-winkels, samen met enkele basisstatistieken en beheeropties. De samenvattingsgegevens die op elke kaart worden weergegeven, omvatten elke winkelstatus, gemaakte datum, laatst bijgewerkte datum, aanbiedingen die aandacht behoeven (voorbeeld: Onvolledige aanbiedingen) en toegewezen [!DNL Commerce] website.

Wanneer u de _[!UICONTROL Amazon Store]_bekijken, staat elke winkelkaart u toe:

- Een winkel openen [dashboard](./amazon-store-dashboard.md), klikt u op **[!UICONTROL View Store]**.

- Als u de status van een winkel wilt wijzigen of een winkel wilt verwijderen, klikt u op **[!UICONTROL Action]** en kies:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Kies of u de status van de winkel wilt wijzigen `Active` of `Inactive`, respectievelijk.

      Een `Inactive` opslaan naar `Active` activeert aanbiedingen en bestellingsactiviteiten voor de winkel met behulp van de opslaginstellingen (zoals aanbiedingsinstellingen, prijsregels en overschrijvingen).

      De status van een winkel wijzigen vanuit `Active` tot `Inactive` status schorst aanbiedingen en bestellingsactiviteiten voor de winkel. Een inactieve winkel bewaart alle winkelinstellingen en aanbiedingen, maar stopt tijdelijk de synchronisatie van prijzen, hoeveelheden en orderbeheer totdat de winkel weer is veranderd in `Active` status. Met deze functie kunt u uw winkelactiviteiten op regionaal niveau beheren zonder dat u uw Amazon-winkel opnieuw hoeft te maken of te integreren of uw bestelling en verkoopgegevens uit het verleden kwijtraakt.

   - **[!UICONTROL Delete]** - Kies of u een winkel wilt verwijderen die u niet meer nodig hebt.

      Kies wanneer u een bestaande Amazon-winkel en de bijbehorende integratie-instellingen wilt verwijderen uit uw [!DNL Amazon Seller Central] account. Als u het account verwijdert, wordt de winkel verwijderd uit het verkoopkanaal van Amazon, samen met alle accountinstellingen, aanbiedingen, logbestanden en andere informatie over deze winkel. De opslag kan niet na schrapping worden teruggewonnen, moet een nieuwe opslag worden gecreeerd.

>[!NOTE]
>Als u de website die tijdens de integratie aan de winkel is toegewezen, wilt wijzigen, moet u de winkel verwijderen en de winkel opnieuw toevoegen met de verschillende websites die tijdens de integratie van de winkel zijn gedefinieerd.

| Winkelkaart | Beschrijving |
|--- |--- |
| Bovenste sectie | Omvat: <br>Het regiopictogram voor de winkel, gedefinieerd tijdens [winkelintegratie](./store-integration.md).<br> De toegewezen _[!UICONTROL Magento Website]_, gedefinieerd tijdens de integratie van de winkel.<br>De_[!UICONTROL Status]_ van uw winkel. Opties: **[!UICONTROL Active]** - De winkelintegratie is voltooid en geverifieerd met Amazon en is beschikbaar voor verkoopactiviteiten. **[!UICONTROL Inactive]** - Winkelintegratie is voltooid, maar is niet in gebruik of beschikbaar voor verkoopactiviteiten. Wanneer `Inactive`, je Amazon-verkoop is gepauzeerd. Wanneer `Active`, verkoopopbrengsten en extra instellingen worden opgeslagen om bij te werken voordat deze worden geactiveerd.<br>De *[!UICONTROL Last Updated]* datum van de meest recente wijziging in de installatie van de Amazon Store.<br>De *[!UICONTROL Created]* datum waarop de Amazon-winkel is gemaakt in Amazon-verkoopkanaal. |
| Sectie Midden | Bevat een overzicht van winkelactiviteiten voor de laatste 30 dagen en omvat en waarschuwt voor aanbiedingen die aandacht behoeven. |
| Onderste sectie | Hier vindt u de opties Winkel weergeven en Handeling.<br>De winkel openen [dashboard](./amazon-store-dashboard.md), klikt u op **[!UICONTROL View Store]**.<br>Als u een winkel wilt activeren, deactiveren of verwijderen, klikt u op **[!UICONTROL Actions]**. |
