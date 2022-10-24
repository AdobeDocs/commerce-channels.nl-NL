---
title: '"Inleiding tot [!DNL Channel Manager]'''
description: '''Meer informatie over installeren en gebruiken [!DNL Channel Manager] om Adobe Commerce en Magento Open Source winkels te integreren met de Marketplace van de Markt van het Markeren en een verkoopkanaal tot stand te brengen om aanbiedingen, prijzen, voorraad, en verkoop van de markt foutloos van uw Admin van de Handel te beheren. "'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 2e3f8e51b765cda0559d8624d61e1ae9dc1c9667
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---


# Inleiding tot [!DNL Channel Manager]

[!DNL Channel Manager] helpt handelaren hun verkoop te verhogen, nieuwe klanten te bereiken, verkooptransacties te stroomlijnen en tijd te besparen door een Adobe Commerce- of Magento Open Source-productcatalogus te integreren met de [!DNL Walmart Marketplace].

![[!DNL Channel Manager] extensiebeheerweergave](assets/channel-manager-home.png)

[!DNL Channel Manager] biedt ondersteuning voor Adobe Commerce- of Magento Open Source-handelaren die willen doorverkopen [!DNL Walmart Marketplace] door de [!DNL Commerce] Admin. Met [!DNL Channel Manager] geïnstalleerd, opslagbeheerders en operationele medewerkers kunnen beheren [!DNL Walmart Marketplace] de verkoop, de inventaris, en de productprijzen naadloos van de omgeving van de Handel.

De uitgebreide beheerder stroomlijnt bewerkingen omdat verkopers dezelfde workflows en processen kunnen gebruiken om de verkoop van beide te beheren [!DNL Commerce] storefronts en de Walmart Marketplace.

Nadat u hebt geïnstalleerd en geconfigureerd [!DNL Channel Manager], kunt u de volgende mogelijkheden gebruiken om de verkooporden van de Marketplace van de Markt te beheren:

* **Aanbiedingsbeheer**-Aanbiedingen van producten eenvoudig verbinden door producten van je te koppelen [!DNL Commerce] catalogus naar bestaand [!DNL Walmart Marketplace] aanbiedingen.

* **Inventory management**-Objecten op de verkopersaccount worden automatisch gesynchroniseerd en bijgewerkt vanaf [!DNL Commerce] om te zorgen voor nauwkeurige inventarisniveaus.

* **Prijswijzigingen**—Handhaaf nauwkeurige prijzen voor aanbiedingen op de markt met automatische prijssynchronisatie. Wanneer een prijs in Adobe Commerce verandert, worden de veranderingen weerspiegeld in de markt.

* **Orderbeheer**—Wanneer nieuwe orders op de markt worden gecreëerd, [!DNL Channel Manager] synchroniseert orders met Adobe Commerce en verzendt orderbevestigingen naar de markt. Deze erkenning zorgt ervoor dat de inventaris voor elke orde wordt gereserveerd. De laatste stap bestaat uit het maken van de corresponderende orders in de [!DNL Commerce] Bestelbeheersysteem voor verwerking.

* **Verzendbeheer**—Als orders zijn gemarkeerd als verzonden in Adobe Commerce, wordt de update van de verzending verzonden naar de [!DNL Walmart Marketplace]. Deze melding zorgt ervoor dat verkopers voldoen aan hun SLA-vereisten en dat klanten verzendupdatemeldingen ontvangen voor hun huidige bestellingen.

* **Annuleringen**—Wanneer orders in Adobe Commerce worden geannuleerd, [!DNL Channel Manager] verzendt bijgewerkte orderinformatie naar de markt om de actie voor de overeenkomstige marktplaatsorde te herhalen. Nadat de orderannulering is voltooid, worden de [!DNL Commerce] voorraadkwantiteitsupdates voor geretourneerde objecten en voorraadupdates worden automatisch gesynchroniseerd naar [!DNL Walmart Marketplace].

* **Retourneert en terugbetaalt**—Wanneer Walmart Marketplace om een rendement voor voorwerpen verzoekt die door Adobe Commerce of Magento Open Source verkoopkanaal worden bevolen [!DNL Channel Manager] verzendt de informatie van het terugkeerverzoek naar de de verkoopkanaalopslag van de Handel om het terugkeerverzoek te herhalen. Vervolgens kan de restitutie worden verwerkt met behulp van de [!DNL Commerce] [terugbetalingsworkflow](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow), offlinemethode. Nadat de restitutie is voltooid, [!DNL Channel Manager] synchroniseert de update met Walmart zodat de status van de geretourneerde waarde op de verkopersaccount kan worden bijgewerkt met de terugbetaling.

## Verwachte vertraging voor [!DNL Channel Manager] bewerkingen

De processen van de gegevenssynchronisatie tussen [!DNL Channel Manager] en een gekoppeld [!DNL Walmart Marketplace] opslag moet enige tijd worden voltooid. Bekijk de verwachte verwerkingstijd voor [!DNL Channel Manager] de verrichtingen helpen de verrichtingen van het verkoopkanaal plannen werken.

**Geschatte vertraging voor [!DNL Channel Manager] bewerkingen**

| **Bewerking** | **Beschrijving** | **Verwachte vertraging** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Producten toevoegen aan [!DNL Channel Manager] | Producten selecteren in het menu [!DNL Commerce] productcatalogus en importeren in [!DNL Channel Manager]. | **Tot vijf minuten**- Als u bijvoorbeeld een groot aantal producten selecteert, duurt het importeren langer. |
| Producten afstemmen op [!DNL Walmart Marketplace] | Productaanbiedingen selecteren in [!DNL Channel Manager] en stuur naar Walmart voor matching. | **Tot 30 minuten**-Als u veel producten selecteert, duurt het afstemmen langer afhankelijk van de geselecteerde hoeveelheid. |
| Inventarisupdates | Wanneer de voorraadhoeveelheid verandert in de handel, [!DNL Channel Manager] synchroniseert de update naar Walmart. | **Tot 10 minuten** |
| Prijsupdates | Wanneer een productprijs verandert, [!DNL Channel Manager] synchroniseert de update naar Walmart. | **Tot vijf minuten** |
| Synoniemen bestellen van Walmart naar [!DNL Commerce] | Klanten bestellen een [!DNL Commerce] product op de Walmart Marketplace. Walmart verzendt de orde naar [!DNL Channel Manager]. De vertoningen van de orde in orde dashboard. | **Tot 30 minuten** |
| Orde gemaakt in [!DNL Commerce] Orderbeheer | [!DNL Channel Manager] maakt de [!DNL Commerce] orde van de orde van de Marm en werkt het orde dashboard bij om te omvatten [!DNL Commerce] ordernummer. | **Tot vijf minuten** |
| Verzendstatus bijgewerkt in [!DNL Commerce] Orderbeheer | Wanneer een bestelling van de handel wordt verzonden, [!DNL Channel Manager] werkt de Verzendstatus in het orderdashboard bij en verzendt de update naar Marmart Marketplace zodat de klant op de hoogte kan worden gesteld. | **Tot vijf minuten** |
| Update voor orderannulering in Commerce Order Management | Wanneer een order wordt geannuleerd bij de handel, [!DNL Channel Manager] werkt de ordestatus in het orderdashboard bij en verzendt de update naar Marmart Marketplace zodat de klant op de hoogte kan worden gesteld. Nadat de orderannulering is voltooid, worden de [!DNL Commerce] voorraadhoeveelheid wordt bijgewerkt om geretourneerde objecten weer te geven. Vervolgens [!DNL Channel Manager] synchroniseert de update naar de [!DNL Walmart Marketplace]. | **Tot vijf minuten** |


