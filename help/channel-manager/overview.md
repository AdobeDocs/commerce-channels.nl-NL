---
title: Info [!DNL Channel Manager]
description: Leer installeren en gebruiken [!DNL Channel Manager] om Adobe Commerce- en Magento Open Source-winkels te integreren met externe markten en een verkoopkanaal te creëren voor het naadloos beheren van aanbiedingen op de markt, prijzen, voorraden en verkopen van uw Commerce Admin.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 7412a3d5b78e206521a048fb56edacd8f11ddb58
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Overzicht

Channel Manager voor Adobe Commerce en Magento Open Source biedt een handige werkruimte in de Admin voor het beheer van kanaalverkoop op markten van derden, zoals Walmart, Amazon en eBay. Verhoog de omzet en vergroot de omzet naar nieuwe markten terwijl u de verkoopkanaalbewerkingen naadloos beheert vanuit uw Commerce Admin.

![[!DNL Channel Manager] extensiebeheerweergave](assets/channel-manager-admin-entry-page.png)

## Overzicht van bètaversie

De bètaversie van Channel Manager ondersteunt verkopers van Adobe Commerce of Magento Open Source die producten willen aanbieden op de Walmart Marketplace.

Deze release biedt ondersteuning voor de volgende mogelijkheden voor het beheer van verkoopkanaalbewerkingen:

* Een API-verbinding tot stand brengen tussen Adobe Commerce of Magento Open Source en Walmart Marketplace

* Producten van Channel Manager naar Walmart publiceren met productmatching

* De status van productaanbiedingen weergeven in Channel Manager, bijvoorbeeld *ontwerp*, *verwerking*, *overeenkomend*, *fout*.

* De inventarisatiehoeveelheden van de synchronisatie van afgedekte producten van de Handel aan Walmart

* Catalogusprijzen synchroniseren voor gematchte producten van de Handel aan Walmart

* Ontvang bestellingen van Walmart Marketplace en bekijk deze in de [!DNL Commerce] ordedashboard

### Verwachte vertraging voor Channel Manager-bewerkingen

De processen van de gegevenssynchronisatie tussen [!DNL Channel Manager] en een gekoppeld [!DNL Walmart Marketplace] opslag moet enige tijd worden voltooid. Bekijk de verwachte verwerkingstijd voor [!DNL Channel Manager] de verrichtingen helpen de verrichtingen van het verkoopkanaal plannen werken.

**Geschatte vertraging voor Channel Manager-bewerkingen**

| **Bewerking** | **Beschrijving** | **Verwachte vertraging** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| Producten toevoegen aan Channel Manager | Selecteer producten uit de productcatalogus van de Handel en voer hen in de Manager van het Kanaal in. | **Tot 5 minuten**- Als u bijvoorbeeld een groot aantal producten selecteert, duurt het importeren langer. |
| Producten afstemmen op Walmart Marketplace | Selecteer productaanbiedingen in Channel Manager en verzend naar Walmart voor matching. | **Tot 30 minuten**-Als u veel producten selecteert, duurt het afstemmen langer afhankelijk van de geselecteerde hoeveelheid. |
| Inventarisupdates | Wanneer de voorraadhoeveelheid in de Handel verandert. Channel Manager synchroniseert update naar Walmart. | **Tot 10 minuten** |
| Prijsupdates | Wanneer een productprijs verandert, synchroniseert de Manager van het Kanaal de update aan Walmart. | **Tot 5 minuten** |
| Synoniemen bestellen van Walmart naar Commerce | De klant bestelt een product van de Handel op de Marketplace van het Martard Walmart. Walmart verzendt de orde naar de Manager van het Kanaal. De vertoningen van de orde in orde dashboard. | **Tot 30 minuten** |
| Orde gemaakt in Commerce Order Management | De Manager van het kanaal leidt tot de orde van de Handel van de orde van de Maramslim en werkt het ordedashboard bij om het de ordeaantal van de Handel te omvatten. | **Tot 5 minuten** |

## Walmart-voorwaarden

U hebt de volgende informatie van Walmart nodig om Handel met de Marketplace van de Markt te integreren:

* Goedkeuring om te verkopen op Walmart en aanmeldingsgegevens voor de geregistreerde verkopersaccount

* Een API-sleutel om Adobe Commerce of Magento Open Source te verbinden met Walmart Marketplace

   De Walmart Marketplace API sleutel laat de integratie tussen de Manager van het Kanaal voor Adobe Commerce of Magento Open Source en de Marketplace van de Markeren toe. Stel de API-sleutel in Seller Central in voordat u Kanaalbeheer aan boord gaat.

### Een verkopersaccount instellen

1. [De toepassing Walmart-verkoper verzenden](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)
2. Na goedkeuring door Walmart, [je Walmart Seller-account instellen](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

### Een Walmart Marketplace API-sleutel genereren

1. Ga naar Walmart Marketplace om een [productie-API-sleutel voor oplossingsprovider voor Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Maak de sleutel en configureer machtigingen:

   * Selecteer Adobe als oplossingsleverancier.

   * Stel de machtigingen in zoals weergegeven in de volgende tabel. Zie voor meer informatie [API-referenties](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) in de *Help bij Marketplace Walmart*.

|    **Adobe API sleutelconfiguratie voor Walmart**
| **Machtiging** | **Instelling** | |—|—| | Inhoud | Volledige toegang | | Feeds ophalen | Alleen weergeven | | Inventaris | Volledige toegang | | Items | Volledige toegang | | Lag Time | Volledige toegang | | Volgorde | Volledige toegang | | Prijs | Volledige toegang | | Rapporten | Alleen weergeven | | Retourzendingen | Volledige toegang | | Regels | Volledige toegang | | Verzending | Volledige toegang |

## Status van Walmart Marketplace Store

Wanneer u producten aan Marketplace publiceert, hangt de beschikbaarheid van lijsten van de status van uw winkels van de Marketplace van de Markt van de Markt van de Markt van de Markt af:

* Voor live winkels worden je productaanbiedingen aangeboden en te koop aangeboden zodra de match voltooid is.

* Voor winkels die niet live zijn, worden uw productaanbiedingen gefaseerd en niet zichtbaar voor klanten. Zodra de winkel live gaat, worden gefaseerde aanbiedingen automatisch naar de live winkel gestuurd.


![[!DNL Walmart Seller Central] gefaseerde producten](assets/walmart-seller-central-staged.png)
