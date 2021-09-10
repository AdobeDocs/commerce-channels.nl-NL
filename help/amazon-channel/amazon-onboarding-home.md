---
title: Amazon-Sales Channel aan boord
description: 'Leer over de pre-opstellingstaken, het aan boord gaan stappen, en hoe Amazon met Amazon Sales Channel in de Handel van Adobe en Magento Open Source werkt.'
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html: 
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 0%

---

# Onboard Amazon-verkoopkanaal

Deze sectie beschrijft de pre-opstellingstaken, de stappen voor aan boord gaan, en sommige zeer belangrijke concepten hoe Amazon met het de verkoopkanaal van Amazon in de Handel van Adobe en Magento Open Source werkt.

De extensie [!DNL Amazon Sales Channel] ondersteunt meerdere Amazon-winkels. Voor één [!DNL Amazon Seller Central]-account die actief is in de regio Amazon U.S./Canada/Mexico, maakt u drie Amazon-winkels (één voor de Amerikaanse verkoop, de Mexicaanse verkoop en de Canadese verkoop). Elk van de drie winkels definieert het land van de markt tijdens zijn oprichting. Als u meer dan één [!DNL Amazon Seller Central] account hebt, kunt u mogelijk maximaal drie Amazon-winkels hebben voor elk van uw [!DNL Amazon Seller Central] accounts. Als je ook in het Verenigd Koninkrijk verkoopt, heb je een vierde Amazon-winkel.

>[!TIP]
>
>Een [Professional-verkopersaccount](https://sell.amazon.com/){target=&quot;_blank&quot;} op [!DNL Amazon Seller Central] in de regio Noord-Amerika of Europees (UK) is vereist. Amazon brengt maandelijks een abonnement en verkoopkosten in rekening. Zie [Amazon: Kies uw het verkopen plan](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.<br><br>
>Onboarding is eenvoudig: maak een winkel en sluit deze aan op uw [!DNL Amazon Seller Central]-account.
>Wanneer uw winkel is verbonden, probeert het Amazon-kanaal uw Amazon-aanbiedingen te importeren en deze aan te passen aan uw catalogus, op basis van uw [kenmerktoewijzing](./attributes-view.md).<br><br>
>De instellingen van het verkoopkanaal van Amazon zijn van invloed op je Amazon-aanbiedingen. Je eerste aanbieding, prijs en productinstellingen worden standaard voor jou gebruikt. U kunt uw [opslagmontages](./ob-store-review.md) (aanbieding, tarifering, orde, en rapportering) wijzigen nadat uw opslag met uw [!DNL Amazon Seller Central] rekening wordt verbonden.

| Stappen | Wat gebeurt er? |
|--- |--- |
| [Taken vooraf instellen](./amazon-pre-setup-tasks.md) | Voordat u aan boord gaat, moet u ervoor zorgen dat u een actieve en goedgekeurde [!DNL Amazon Seller Central]-account hebt. Er zijn ook enkele [!DNL Commerce] vereisten en aanbevelingen om te voltooien alvorens aan boord te gaan. |
| [De Amazon API-sleutel controleren](./amazon-verify-api-key.md) | Als u Amazon-verkoopkanalen opent, controleert en valideert [!DNL Commerce] automatisch de Amazon API-sleutel die u in uw winkelconfiguratie hebt toegevoegd. Als uw API-sleutel niet is toegevoegd of ongeldig is, wordt u gevraagd om de Amazon API-sleutel ](./amazon-verify-api-key.md) toe te voegen of bij te werken.[ |
| [Opslagintegratie](./store-integration.md) | Deze stap omvat het maken van een Amazon-winkel voor verkoopkanalen en het vervolgens verbinden met uw [!DNL Amazon Seller Central]-account. Voor deze stap hebt u de primaire aanmeldingsgegevens voor uw [!DNL Amazon Seller Central]-account nodig (het e-mailadres of telefoonnummer dat wordt gebruikt om de verkopersaccount te maken). |
| [Aanbiedingsregel maken](./ob-create-listing-rule.md) | Nadat je de Amazon-winkel hebt verbonden, wordt je gevraagd een regel voor aanbiedingen te maken. Deze stap wordt aanbevolen, maar je kunt deze ook overslaan om het importproces voor aanbiedingen te starten. U kunt ook toegang krijgen tot uw [opslag- en aanbiedingsinstellingen](./ob-store-review.md) in de winkel [dashboard](./amazon-store-dashboard.md). |
