---
title: '"Info [!DNL Channel Manager]"'
description: '"Meer informatie over installeren en gebruiken [!DNL Channel Manager] om Adobe Commerce- en Magento Open Source-winkels te integreren met externe markten en een verkoopkanaal te creëren voor het naadloos beheren van aanbiedingen, prijzen, voorraden en verkopen op de markt van uw Commerce Admin."'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 690eeb5d03b23cac11f3c14b04601c514c76e0bd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Info [!DNL Channel Manager]

[!DNL Channel Manager] helpt handelaren hun verkoop te verhogen, nieuwe klanten te bereiken, verkooptransacties te stroomlijnen en tijd te besparen door een Adobe Commerce- of Magento Open Source-productcatalogus te integreren met de [!DNL Walmart Marketplace].

![[!DNL Channel Manager] extensiebeheerweergave](assets/channel-manager-home.png)

[!DNL Channel Manager] biedt ondersteuning voor Adobe Commerce- of Magento Open Source-handelaren die willen doorverkopen [!DNL Walmart Marketplace] door de [!DNL Commerce] Beheerder met beheermogelijkheden [!DNL Walmart Marketplace] de verkoop, de inventaris, en de productprijzen naadloos van de omgeving van de Handel.

Uitgebreid Admin stroomlijnt verrichtingen omdat de handelaren de zelfde werkschema&#39;s en processen kunnen gebruiken om verkoop van zowel de winkelcentra van de Handel als de Marketplace van de Markt van de Markt van de Markt van de Markt te beheren.

Nadat u hebt geïnstalleerd en geconfigureerd [!DNL Channel Manager], kunt u de volgende mogelijkheden gebruiken om de verkooporden van de Marketplace van de Markt te beheren:

* **Aanbiedingsbeheer**-Aanbiedingen van producten eenvoudig verbinden door producten van je te koppelen [!DNL Commerce] catalogus naar bestaand [!DNL Walmart Marketplace] aanbiedingen.

* **Inventory management**-Objecten op de verkopersaccount van de handelaar worden automatisch gesynchroniseerd en bijgewerkt bij Handel om een nauwkeurig voorraadniveau te garanderen.

* **Prijswijzigingen**- Handhaaf nauwkeurige prijzen voor aanbiedingen op de markt met automatische prijssynchronisatie. Wanneer een prijs in Adobe Commerce verandert, worden de veranderingen weerspiegeld in de markt.

* **Orderbeheer**- Wanneer nieuwe orders op een markt worden gecreëerd, [!DNL Channel Manager] Hiermee synchroniseert u orders met Adobe Commerce, stuurt u orderbevestigingen naar de markt om ervoor te zorgen dat de voorraad voor elke bestelling is gereserveerd en maakt u een bijbehorende bestelling in het systeem voor het beheer van handelsorders voor verwerking.

* **Verzendbeheer**-Als orders zijn gemarkeerd als verzonden in Adobe Commerce, wordt de update van de verzending verzonden naar de [!DNL Walmart Marketplace]. Deze melding zorgt ervoor dat verkopers voldoen aan hun SLA-vereisten en dat klanten verzendupdatemeldingen ontvangen voor hun huidige bestellingen.

* **Annuleringen**-Als orders in Adobe Commerce worden geannuleerd, [!DNL Channel Manager] verzendt bijgewerkte orderinformatie naar de markt om de actie voor de overeenkomstige marktplaatsorde te herhalen.  Nadat de orderannulering is voltooid, worden de [!DNL Commerce] voorraadkwantiteitsupdates voor geretourneerde objecten en voorraadupdates worden automatisch gesynchroniseerd naar [!DNL Walmart Marketplace].

## Verwachte vertraging voor [!DNL Channel Manager] bewerkingen

De processen van de gegevenssynchronisatie tussen [!DNL Channel Manager] en een gekoppeld [!DNL Walmart Marketplace] opslag moet enige tijd worden voltooid. Bekijk de verwachte verwerkingstijd voor [!DNL Channel Manager] de verrichtingen helpen de verrichtingen van het verkoopkanaal plannen werken.

**Geschatte vertraging voor [!DNL Channel Manager] bewerkingen**

| **Bewerking** | **Beschrijving** | **Verwachte vertraging** |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Producten toevoegen aan [!DNL Channel Manager] | Producten selecteren uit de productcatalogus van de Handel en importeren in [!DNL Channel Manager]. | **Tot vijf minuten**- Als u bijvoorbeeld een groot aantal producten selecteert, duurt het importeren langer. |
| Producten afstemmen op [!DNL Walmart Marketplace] | Productaanbiedingen selecteren in [!DNL Channel Manager] en stuur naar Walmart voor matching. | **Tot 30 minuten**-Als u veel producten selecteert, duurt het afstemmen langer afhankelijk van de geselecteerde hoeveelheid. |
| Inventarisupdates | Wanneer de voorraadhoeveelheid verandert in de handel, [!DNL Channel Manager] synchroniseert de update naar Walmart. | **Tot 10 minuten** |
| Prijsupdates | Wanneer een productprijs verandert, [!DNL Channel Manager] synchroniseert de update naar Walmart. | **Tot vijf minuten** |
| Synoniemen bestellen van Walmart naar Commerce | De klant bestelt een product van de Handel op de Marketplace van het Martard Walmart. Walmart verzendt de orde naar [!DNL Channel Manager]. De vertoningen van de orde in orde dashboard. | **Tot 30 minuten** |
| Orde gemaakt in Commerce Order Management | [!DNL Channel Manager] leidt tot de orde van de Handel van de orde van de Mara en werkt het ordedashboard bij om het de ordeaantal van de Handel te omvatten. | **Tot vijf minuten** |
| Verzendstatus bijwerken in Commerce Order Management | Wanneer een bestelling van de handel wordt verzonden, [!DNL Channel Manager] werkt de Verzendstatus in het orderdashboard bij en verzendt de update naar Marmart Marketplace zodat de klant op de hoogte kan worden gesteld. | **Tot vijf minuten** |
| Update voor orderannulering in Commerce Order Management | Wanneer een order wordt geannuleerd bij de handel, [!DNL Channel Manager] werkt de ordestatus in het orderdashboard bij en verzendt de update naar Marmart Marketplace zodat de klant op de hoogte kan worden gesteld. Nadat de orderannulering is voltooid, worden de [!DNL Commerce] voorraadhoeveelheid wordt bijgewerkt om geretourneerde objecten weer te geven. Vervolgens [!DNL Channel Manager] synchroniseert de update naar de [!DNL Walmart Marketplace]. | **Tot vijf minuten** |


