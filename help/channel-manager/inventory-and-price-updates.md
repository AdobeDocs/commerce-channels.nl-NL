---
title: Update van voorraad en prijs
description: '"[!DNL Channel Manager] synchrone inventarisatie en prijsupdates tussen de Commerce Store en [!DNL Walmart Marketplace] zodat kunt u uw verkoopkanaalverrichtingen van uw Admin van de Handel beheren"'
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Update van voorraad en prijs

Channel Manager volgt de inventarisatie en prijzen voor gepubliceerde producten en synchroniseert de wijzigingen in Channel Manager en de Walmart Marketplace om de huidige hoeveelheid en prijs van de voorraad in productaanbiedingen weer te geven.**

## Inventarisupdates

Wanneer de inventarisniveaus veranderen, synchroniseert de Manager van het Kanaal updates tussen de het productcatalogus van de Handel en de Marketplace van de Markt van de Markt van de Markt van de Markt zodat zowel de Manager van het Kanaal als de Marketplace van de Markt van de Markt de huidige voorraadhoeveelheid tonen.

Het kan tot 5 minuten voor inventarisveranderingen aan vertoning in de Manager van het Kanaal en de Marketplace van het Walmart duren.

* **Updates van de voorraadhoeveelheid in de productcatalogus**- Als de voorraadhoeveelheid van de Handel verandert voor een product dat op Walmart wegens [handmatig wijzigen van voorraadhoeveelheid](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html) of bij terugbetaling of annulering van een bestelling synchroniseert Channel Manager de wijziging met het verbonden verkoopkanaal en de [!DNL Walmart Marketplace].

* **De voorraad verminderen om de orders van de Marketplace van Walmart weer te geven**- Nadat de de ordesync van de Marketplace van het Spoor aan de Manager van het Kanaal, verzendt de Manager van het Kanaal de update naar het de ordesysteem van de Handel. De handel past de voorraadhoeveelheden op de orde aan. Vervolgens wordt de bijgewerkte hoeveelheid gesynchroniseerd met Walmart Marketplace. Dit kunnen enkele verschillen zijn in de voorraadhoeveelheid die wordt weergegeven in Channel Manager en de Marketplace tot de synchronisatiebewerkingen zijn voltooid.

>[!IMPORTANT]
>
> Nadat een Walmart Marktorder synchroon aan de Manager van het Kanaal, wordt de inventarishoeveelheden en andere informatie van de ordeverwerking bijgewerkt slechts voor terugbetalingen en annuleringen die van Handel in werking worden gesteld. Als een bestelling wordt terugbetaald of geannuleerd van de Walmart Marketplace, verwerkt de verandering van Handel om ervoor te zorgen dat de de inventarishoeveelheden van de Handel en de ordeinformatie nauwkeurig zijn.

## Prijsupdates

Wanneer de productprijs in de Handel verandert, synchroniseert de Manager van het Kanaal de update van de het productcatalogus van de Handel aan de Marketplace van de Markering. Het kan tot 5 minuten duren voor inventariswijzigingen worden weergegeven.

### Prijzen voor een gepubliceerd product beheren

1. Van de [!UICONTROL Admin], selecteert u **[!UICONTROL Catalog > Products]**.
1. Zoek in het productraster het product dat u wilt bijwerken en selecteer **[!UICONTROL Edit]**.
1. Controleer en werk de prijs zo nodig bij.
1. **[!UICONTROL Save]** de wijziging.

Channel Manager synchroniseert eventuele prijsupdates naar de kanaalwinkel en [!DNL Walmart Marketplace]. Deze bewerking kan maximaal 5 minuten duren.

Voor details over het beheren van de configuratie van de productprijs in de Handel, zie [Prijsbeheer](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
