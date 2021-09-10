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

Als u de startpagina van het Amazon-verkoopkanaal weergeeft, wordt standaard de weergave _Amazon Stores_ geopend.

![Weergave Amazon-winkels](assets/amazon-sales-channel-home-tabs.png)

In de weergave _[!UICONTROL Amazon Stores]_ziet u een &quot;opslagkaart&quot; voor elk van uw Amazon-winkels, samen met enkele basisstatistieken en beheeropties. De samenvattingsgegevens die op elke kaart worden weergegeven, omvatten elke winkelstatus, gemaakte datum, laatst bijgewerkte datum, aanbiedingen die aandacht behoeven (voorbeeld: Onvolledige aanbiedingen) en de toegewezen [!DNL Commerce]-website.

Wanneer het bekijken van de _[!UICONTROL Amazon Store]_mening, staat elke archiefkaart u toe:

- Als u een opslagmap [dashboard](./amazon-store-dashboard.md) wilt openen, klikt u op **[!UICONTROL View Store]**.

- Als u de status van een winkel wilt wijzigen of een winkel wilt verwijderen, klikt u op **[!UICONTROL Action]** en kiest u:

   - **[!UICONTROL Activate]** /  **[!UICONTROL Deactivate]** - Kies of u de status van de winkel wilt wijzigen in respectievelijk  `Active` of  `Inactive`.

      Als u een `Inactive`-winkel wijzigt in `Active`-status, worden aanbiedingen en bestellingsactiviteiten voor de winkel geactiveerd met behulp van de opslaginstellingen (zoals aanbiedingsinstellingen, prijsregels en overschrijvingen).

      Als u de status van een winkel wijzigt van `Active` in `Inactive`, worden aanbiedingen en bestellingsactiviteiten voor de winkel opgeschort. In een inactieve winkel blijven alle winkelinstellingen en aanbiedingen behouden, maar wordt de synchronisatie van prijzen, hoeveelheden en orderbeheer tijdelijk stopgezet totdat de winkel de status `Active` krijgt. Met deze functie kunt u uw winkelactiviteiten op regionaal niveau beheren zonder dat u uw Amazon-winkel opnieuw hoeft te maken of te integreren of uw bestelling en verkoopgegevens uit het verleden kwijtraakt.

   - **[!UICONTROL Delete]** - Kies of u een winkel wilt verwijderen die u niet meer nodig hebt.

      Kies wanneer u een bestaande Amazon-winkel en de bijbehorende integratie-instellingen met uw [!DNL Amazon Seller Central]-account wilt verwijderen. Als u het account verwijdert, wordt de winkel verwijderd uit het verkoopkanaal van Amazon, samen met alle accountinstellingen, aanbiedingen, logbestanden en andere informatie over deze winkel. De opslag kan niet na schrapping worden teruggewonnen, moet een nieuwe opslag worden gecreeerd.

>[!NOTE]
>Als u de website die tijdens de integratie aan de winkel is toegewezen, wilt wijzigen, moet u de winkel verwijderen en de winkel opnieuw toevoegen met de verschillende websites die tijdens de integratie van de winkel zijn gedefinieerd.

| Winkelkaart | Beschrijving |
|--- |--- |
| Bovenste sectie | Omvat: <br>Het regiopictogram voor de opslag, gedefinieerd tijdens [store integration](./store-integration.md).<br> De toegewezen  _[!UICONTROL Magento Website]_, die tijdens archiefintegratie wordt bepaald.<br>De_[!UICONTROL Status]_ van je winkel. Opties: **[!UICONTROL Active]** - De winkelintegratie is voltooid en geverifieerd met Amazon en is beschikbaar voor verkoopactiviteiten. **[!UICONTROL Inactive]** - Winkelintegratie is voltooid, maar is niet in gebruik of beschikbaar voor verkoopactiviteiten. Wanneer `Inactive`, wordt uw verkoop van Amazon gepauzeerd. Wanneer `Active`, verkoopopbrengst en extra montages sparen om bij te werken alvorens te activeren.<br>De  *[!UICONTROL Last Updated]* datum van de meest recente wijziging in de installatie van de Amazon Store.<br>De  *[!UICONTROL Created]* datum waarop de Amazon-winkel is gemaakt in Amazon-verkoopkanaal. |
| Sectie Midden | Bevat een overzicht van winkelactiviteiten voor de laatste 30 dagen en omvat en waarschuwt voor aanbiedingen die aandacht behoeven. |
| Onderste sectie | Hier vindt u de opties Winkel weergeven en Handeling.<br>Klik op het  [dashboard](./amazon-store-dashboard.md) van de winkel om dit te openen  **[!UICONTROL View Store]**.<br>Klik op een winkel om deze te activeren, te deactiveren of te verwijderen.  **[!UICONTROL Actions]** |
