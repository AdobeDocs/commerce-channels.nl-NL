---
title: "Aan boord [!DNL Amazon Sales Channel]"
description: Leer meer over de vooraf ingestelde taken, de instapprocedure en de manier waarop Amazon werkt met de Amazon-Sales Channel in Adobe Commerce en Magento Open Source.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 6321f17c0e6f9e86bb3f5755dc7710fa68d68b0d
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Aan boord [!DNL Amazon Sales Channel]

In deze sectie worden de vooraf ingestelde taken, de stappen voor instapweigering en enkele belangrijke concepten beschreven van hoe Amazon werkt met het Amazon-verkoopkanaal in Adobe Commerce en Magento Open Source.

De [!DNL Amazon Sales Channel] -extensie ondersteunt meerdere Amazon-winkels. Voor één [!DNL Amazon Seller Central] -account die actief is in de regio Amazon U.S./Canada/Mexico, maakt drie Amazon-winkels (één voor de verkoop in de VS, de verkoop in Mexico en de verkoop in Canada). Elk van de drie winkels definieert het land van de markt tijdens zijn oprichting. Als u meer dan één [!DNL Amazon Seller Central] account, hebt u mogelijk maximaal drie Amazon-winkels voor elk van uw [!DNL Amazon Seller Central] rekeningen. Als je ook in het Verenigd Koninkrijk verkoopt, heb je een vierde Amazon-winkel.

>[!TIP]
>
>A [Professional-verkopersaccount](https://sell.amazon.com/){target="_blank"} on [!DNL Amazon Seller Central] in the North America or European (UK) region is required. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>Onboarding is eenvoudig: maak uw winkel en sluit deze aan op uw [!DNL Amazon Seller Central] account.
>Wanneer je winkel is verbonden, probeert het Amazon-kanaal je Amazon-aanbiedingen te importeren en deze aan te passen aan je catalogus, op basis van je [kenmerktoewijzing](./attributes-view.md).<br><br>
>De instellingen van het verkoopkanaal van Amazon zijn van invloed op je Amazon-aanbiedingen. Je eerste aanbieding, prijs en productinstellingen worden standaard voor jou gebruikt. U kunt uw [opslaginstellingen](./ob-store-review.md) (aanbieding, prijs, bestelling en rapportage) nadat je winkel is verbonden met je [!DNL Amazon Seller Central] account.

| Stappen | Wat gebeurt er? |
|---------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Taken vooraf instellen](./amazon-pre-setup-tasks.md) | Voordat u aan boord gaat, moet u ervoor zorgen dat u een actieve en goedgekeurde [!DNL Amazon Seller Central] account. Er zijn ook enkele [!DNL Commerce] eisen en aanbevelingen die vóór de instapprocedure moeten worden voltooid. |
| [De Amazon API-sleutel controleren](./amazon-verify-api-key.md) | Bij toegang tot Amazon-verkoopkanaal [!DNL Commerce] controleert en valideert automatisch de Amazon API-sleutel die u in uw winkelconfiguratie hebt toegevoegd. Als de API-sleutel niet is toegevoegd of ongeldig is, wordt u gevraagd [Amazon API-sleutel toevoegen of bijwerken](./amazon-verify-api-key.md). |
| [Opslagintegratie](./store-integration.md) | Deze stap omvat het maken van een Amazon-winkel voor verkoopkanalen en het vervolgens verbinden met uw [!DNL Amazon Seller Central] account. U hebt de primaire aanmeldingsgegevens voor uw [!DNL Amazon Seller Central] -account (het e-mailadres of telefoonnummer waarmee de verkopersaccount is gemaakt) voor deze stap. |
| [Aanbiedingsregel maken](./ob-create-listing-rule.md) | Nadat je de Amazon-winkel hebt verbonden, wordt je gevraagd een regel voor aanbiedingen te maken. Deze stap wordt aanbevolen, maar je kunt deze ook overslaan om het importproces voor aanbiedingen te starten. U hebt ook toegang tot uw [winkelinstellingen en aanbiedingsinstellingen](./ob-store-review.md) in de winkel [dashboard](./amazon-store-dashboard.md). |
