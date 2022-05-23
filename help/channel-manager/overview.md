---
title: Info [!DNL Channel Manager]
description: Leer installeren en gebruiken [!DNL Channel Manager] om Adobe Commerce- en Magento Open Source-winkels te integreren met externe markten en een verkoopkanaal te creëren voor het naadloos beheren van aanbiedingen, prijzen, voorraden en verkopen op de markt van uw Commerce Admin.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: ef4c1362424285d4969fe173a0790809fccff80b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Info [!DNL Channel Manager]

[!DNL Channel Manager] helpt u uw verkoop te verhogen en nieuwe klanten te bereiken door uw Adobe Commerce of Magento Open Source te integreren productcatalogus met [!DNL Walmart US Marketplace].

![[!DNL Channel Manager] extensiebeheerweergave](assets/channel-manager-home.png)

Channel Manager ondersteunt verkopers van Adobe Commerce of Magento Open Source die willen verkopen op Walmart Marketplace.

Nadat u hebt geïnstalleerd en geconfigureerd [!DNL Channel Manager]de [!DNL Commerce] Admin wordt uitgebreid zodat u kunt beheren [!DNL Walmart Marketplace] verkooptransacties naadloos vanuit uw omgeving van de Handel.

* **Aanbiedingsbeheer**-Publiceer eenvoudig productaanbiedingen door producten uit uw handelscatalogus te koppelen aan bestaande aanbiedingen op de Marketplace in het winkelwagentje.

* **Inventory management**-Objecten op de verkopersaccount van de handelaar worden automatisch gesynchroniseerd en bijgewerkt bij Handel om een nauwkeurig voorraadniveau te garanderen.

* **Prijswijzigingen**- Handhaaf nauwkeurige prijzen voor aanbiedingen op de markt met automatische prijssynchronisatie. Wanneer een prijs in Adobe Commerce verandert, worden de wijzigingen binnen 10 minuten op de markt doorgevoerd.

* **Orderbeheer**- Wanneer de nieuwe orden in een markt worden gecreeerd, synchroniseert de Manager van het Kanaal orden met Adobe Commerce en verzendt ordererkenning naar de markt om ervoor te zorgen dat de inventaris voor elke orde wordt gereserveerd.

* **Verzendbeheer**-Als orders zijn gemarkeerd als verzonden in Adobe Commerce, wordt de update van de verzending verzonden naar de [!DNL Walmart Marketplace]. Deze melding zorgt ervoor dat verkopers voldoen aan hun SLA-vereisten en dat klanten verzendupdatemeldingen ontvangen voor hun huidige bestellingen.

* **Annuleringen**-Als orders in Adobe Commerce worden geannuleerd, stuurt Channel Manager bijgewerkte ordergegevens naar de marketingplaats om de handeling voor de corresponderende marktplaatsorder te repliceren.

## Verwachte vertraging voor Channel Manager-bewerkingen

De processen van de gegevenssynchronisatie tussen [!DNL Channel Manager] en een gekoppeld [!DNL Walmart Marketplace] opslag moet enige tijd worden voltooid. Bekijk de verwachte verwerkingstijd voor [!DNL Channel Manager] de verrichtingen helpen de verrichtingen van het verkoopkanaal plannen werken.

**Geschatte vertraging voor Channel Manager-bewerkingen**

| **Bewerking** | **Beschrijving** | **Verwachte vertraging** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Producten toevoegen aan Channel Manager | Selecteer producten uit de productcatalogus van de Handel en voer hen in de Manager van het Kanaal in. | **Tot vijf minuten**- Als u bijvoorbeeld een groot aantal producten selecteert, duurt het importeren langer. |
| Producten afstemmen op Walmart Marketplace | Selecteer productaanbiedingen in Channel Manager en verzend naar Walmart voor matching. | **Tot 30 minuten**-Als u veel producten selecteert, duurt het afstemmen langer afhankelijk van de geselecteerde hoeveelheid. |
| Inventarisupdates | Wanneer de voorraadhoeveelheid verandert in de handel, [!DNL Channel Manager] synchroniseert de update naar Walmart. | **Tot 10 minuten** |
| Prijsupdates | Wanneer een productprijs verandert, synchroniseert de Manager van het Kanaal de update aan Walmart. | **Tot vijf minuten** |
| Synoniemen bestellen van Walmart naar Commerce | De klant bestelt een product van de Handel op de Marketplace van het Martard Walmart. Walmart verzendt de orde naar de Manager van het Kanaal. De vertoningen van de orde in orde dashboard. | **Tot 30 minuten** |
| Orde gemaakt in Commerce Order Management | De Manager van het kanaal leidt tot de orde van de Handel van de orde van de Maramslim en werkt het ordedashboard bij om het de ordeaantal van de Handel te omvatten. | **Tot vijf minuten** |

## Walmart-voorwaarden

U hebt de volgende informatie van Walmart nodig om Handel met de Marketplace van de Markt te integreren:

* Goedkeuring om te verkopen op Walmart en aanmeldingsgegevens voor de geregistreerde verkopersaccount

* Een API-sleutel om Adobe Commerce of Magento Open Source te verbinden met Walmart Marketplace

   De Walmart Marketplace API sleutel laat de integratie tussen de Manager van het Kanaal voor Adobe Commerce of Magento Open Source en de Marketplace van de Markeren toe. Stel de API-sleutel in Seller Central in voordat u Kanaalbeheer aan boord gaat.

### Een verkopersaccount instellen

1. [De toepassing Walmart-verkoper verzenden](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
2. Na goedkeuring door Walmart, [je Walmart Seller-account instellen](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

### Een Walmart Marketplace API-sleutel genereren

1. Ga naar Walmart Marketplace om een [productie-API-sleutel voor oplossingsprovider voor Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Maak de sleutel en configureer machtigingen:

   * Selecteer Adobe als oplossingsleverancier.

   * Stel de machtigingen in zoals weergegeven in de volgende tabel. Zie voor meer informatie [API-referenties](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) in de *[!DNL Walmart Marketplace]Hulp van verkopers*.

   **Adobe API sleutelconfiguratie voor Walmart**

   | **Machtiging** | **Instelling** |
   |----------------|-------------|
   | Inhoud | Volledige toegang |
   | Feeds ophalen | Alleen weergeven |
   | Inventaris | Volledige toegang |
   | Items | Volledige toegang |
   | Laagtijd | Volledige toegang |
   | Volgorde | Volledige toegang |
   | Prijs | Volledige toegang |
   | Rapporten | Alleen weergeven |
   | Retourneert | Volledige toegang |
   | Regels | Volledige toegang |
   | Verzending | Volledige toegang |

## Status van Walmart Marketplace Store

Wanneer u producten aan Marketplace publiceert, hangt de beschikbaarheid van lijsten van de status van uw winkels van de Marketplace van de Markt van de Markt van de Markt van de Markt af:

* Voor live winkels worden je productaanbiedingen aangeboden en te koop aangeboden wanneer de match voltooid is.

* Voor winkels die niet live zijn, worden uw productaanbiedingen gefaseerd en niet zichtbaar voor klanten. Wanneer de winkel live gaat, worden gefaseerde aanbiedingen automatisch naar de live winkel gestuurd.


![[!DNL Walmart Seller Central] gefaseerde producten](assets/walmart-seller-central-staged.png)
