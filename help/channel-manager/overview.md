---
title: 'Introduction to  [!DNL Channel Manager]'
description: "Leer hoe te om  [!DNL Channel Manager]  te installeren en te gebruiken om de winkels van Adobe Commerce en van de Magento Open Source met de Marketplace van de Markt te integreren en een verkoopkanaal tot stand te brengen om aanbiedingen van de markt, de tarifering, de inventaris, en de verkoop foutloos van uw Admin van Commerce te beheren."
role: Leader, Admin, User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 850aece134084e108b324a964d7d834042c7ddfd
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---


# Inleiding tot [!DNL Channel Manager]

Met [!DNL Channel Manager] kunnen handelaren hun verkoop verhogen, nieuwe klanten bereiken, verkoopactiviteiten stroomlijnen en tijd besparen door een Adobe Commerce- of Magento Open Source-productcatalogus te integreren met [!DNL Walmart Marketplace] .

![[!DNL Channel Manager] de mening van Admin van de uitbreiding ](assets/channel-manager-home.png){width="700" zoomable="yes"}

[!DNL Channel Manager] biedt ondersteuning voor Adobe Commerce- of Magento Open Source-handelaren die op [!DNL Walmart Marketplace] willen verkopen door de beheerfunctie voor [!DNL Commerce] uit te breiden. Als [!DNL Channel Manager] is geïnstalleerd, kunnen opslagbeheerders en operatiepersoneel de verkoop, voorraad en productprijzen van [!DNL Walmart Marketplace] naadloos beheren vanuit de Commerce-omgeving.

Uitgebreid Admin stroomlijnt verrichtingen omdat de handelaren de zelfde werkschema&#39;s en processen kunnen gebruiken om verkoop van zowel [!DNL Commerce] winkelefronts als de Marketplace van het Markeren van het Markeren te beheren.

Nadat u [!DNL Channel Manager] hebt geïnstalleerd en geconfigureerd, kunt u de volgende mogelijkheden gebruiken om de verkooporders van Walmart Marketplace te beheren:

* **het lijstbeheer** - verbind productlijsten gemakkelijk door producten van uw [!DNL Commerce] catalogus aan bestaande [!DNL Walmart Marketplace] lijsten aan te passen.

* **Inventory management** - De Punten in de verkopersrekening van de handelaar worden automatisch gesynchroniseerd en van [!DNL Commerce] bijgewerkt om nauwkeurige inventarisniveaus te verzekeren.

* **Prijsende updates** - handhaaf nauwkeurige tarifering voor marktplaatslijsten met automatische prijssynchronisatie. Wanneer een prijs in Adobe Commerce verandert, worden de veranderingen weerspiegeld in de markt.

* **het beheer van de Orde** - wanneer de nieuwe orden in de markt worden gecreeerd, [!DNL Channel Manager] synchroniseert bevelen met Adobe Commerce, en verzendt ordererkenning naar de markt. Deze erkenning zorgt ervoor dat de inventaris voor elke orde wordt gereserveerd. De laatste stap bestaat uit het maken van de bijbehorende bestellingen in het Order Management-systeem van [!DNL Commerce] voor verwerking.

* **Verzendbeheer** - wanneer de orden zoals verscheept in Adobe Commerce duidelijk zijn, wordt de ladingsupdate verzonden naar [!DNL Walmart Marketplace]. Deze melding zorgt ervoor dat verkopers voldoen aan hun SLA-vereisten en dat klanten verzendupdatemeldingen ontvangen voor hun huidige bestellingen.

* **Annuleringen** - wanneer de orden in Adobe Commerce worden geannuleerd, [!DNL Channel Manager] verzendt bijgewerkte ordeinformatie naar de markt om de actie voor de overeenkomstige marktplaatsorde te herhalen. Nadat de annulering van de bestelling is voltooid, wordt de voorraad van [!DNL Commerce] bijgewerkt met de geretourneerde items en worden de voorraadupdates automatisch gesynchroniseerd met [!DNL Walmart Marketplace] .

* **Keert terug en terugkeert** - wanneer de Marketplace van de Markeren van de Markt van de Markt om een terugkeer voor punten verzoekt die door Adobe Commerce of het de verkoopkanaal van de Magento Open Source worden bevolen, [!DNL Channel Manager] verzendt de informatie van het terugkeerverzoek naar de opslag van het het verkoopkanaal van Commerce om het terugkeerverzoek te herhalen. Dan, kan de terugbetaling worden verwerkt gebruikend het [!DNL Commerce] [ terugbetalingswerkschema ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html#refund-workflow), off-line methode. Nadat de terugbetaling is voltooid, synchroniseert [!DNL Channel Manager] de update naar Walmart, zodat de status van de geretourneerde waarde op de verkopersaccount kan worden bijgewerkt met de terugbetaling.

## Verwachte vertraging voor [!DNL Channel Manager] bewerkingen

De gegevenssynchronisatieprocessen tussen [!DNL Channel Manager] en een gekoppelde [!DNL Walmart Marketplace] -opslag vereisen enige tijd om te voltooien. Bekijk de verwachte verwerkingstijd voor [!DNL Channel Manager] -bewerkingen om verkoopkanaalbewerkingen beter te plannen.

**Geschatte latentie voor [!DNL Channel Manager] verrichtingen**

| **Verrichting** | **Beschrijving** | **Verwachte vertraging** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Producten toevoegen aan [!DNL Channel Manager] | Selecteer producten in de productcatalogus van [!DNL Commerce] en importeer ze in [!DNL Channel Manager] . | **tot vijf minuten** - als u vele producten, bijvoorbeeld, een volledige productcatalogus selecteert, duurt het de invoerproces langer. |
| Producten afstemmen op [!DNL Walmart Marketplace] | Selecteer productaanbiedingen in [!DNL Channel Manager] en stuur deze naar Walmart voor overeenkomende objecten. | **tot 30 minuten** - als u vele producten selecteert, duurt het passende proces langer afhankelijk van de geselecteerde hoeveelheid. |
| Inventarisupdates | Wanneer de inventarishoeveelheid in Commerce verandert, synchroniseert [!DNL Channel Manager] de update naar Walmart. | **tot 10 minuten** |
| Prijsupdates | Wanneer de prijs van een product verandert, synchroniseert [!DNL Channel Manager] de update naar Walmart. | **tot vijf minuten** |
| Syncs bestellen van Walmart naar [!DNL Commerce] | De klant bestelt een [!DNL Commerce] -product op de Walmart Marketplace. Walmart verzendt de orde naar [!DNL Channel Manager]. De vertoningen van de orde in orde dashboard. | **tot 30 minuten** |
| Order gemaakt in [!DNL Commerce] Order Management | [!DNL Channel Manager] maakt de [!DNL Commerce] -volgorde in de Walmart-volgorde en werkt het orderdashboard bij en voegt het [!DNL Commerce] -ordernummer toe. | **tot vijf minuten** |
| Verzendstatus bijgewerkt in [!DNL Commerce] Order Management | Wanneer een bestelling vanuit Commerce wordt verzonden, werkt [!DNL Channel Manager] de verzendstatus in het orderdashboard bij en verzendt het de update naar Walmart Marketplace zodat de klant op de hoogte kan worden gesteld. | **tot vijf minuten** |
| Update voor annulering van bestellingen in Commerce Order Management | Wanneer een bestelling van Commerce wordt geannuleerd, werkt [!DNL Channel Manager] de orderstatus in het orderdashboard bij en wordt de update naar de Marmart-markt verzonden, zodat de klant op de hoogte kan worden gesteld. Nadat de orderannulering is voltooid, wordt de voorraad van [!DNL Commerce] bijgewerkt om de geretourneerde items weer te geven. Vervolgens synchroniseert [!DNL Channel Manager] de update naar de map [!DNL Walmart Marketplace] . | **tot vijf minuten** |


