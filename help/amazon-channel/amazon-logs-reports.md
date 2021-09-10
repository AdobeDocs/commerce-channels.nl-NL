---
title: Logboeken en winkelrapporten
description: Gebruik de logboeken en winkelrapporten om te zien wat er gebeurt in je Adobe Commerce- of Magento Open Source-winkel en je Amazon Marketplace-aanbiedingen.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Logboeken en opslagrapporten

De Amazon-extensie voor verkoopkanalen bevat enkele waardevolle logboeken en winkelrapporten waarmee u de wijzigingen kunt bekijken die van invloed zijn op uw Amazon-aanbiedingen en -bestellingen. Met deze rapporten kun je zien wat er in je winkel gebeurt en verschillende statussen van aanbiedingen begrijpen.

Er zijn geen acties beschikbaar voor de logboeken of opslagrapporten, omdat het alleen-revisiefuncties zijn.

De volgende logboeken kunnen van [store dashboard](./amazon-store-dashboard.md) worden betreden.

- In het [Logbestand met wijzigingen in aanbiedingen](./listing-changes-log.md) worden de wijzigingen weergegeven die zijn opgetreden in uw Amazon-verkopersaccount als een weerspiegeling van uw Amazon-instellingen voor verkoopkanalen.

- In het [Communication Errors Log](./communication-errors-log.md) worden alle gerapporteerde communicatiefouten met Amazon weergegeven.

De volgende store-specific rapporten kunnen van [store dashboard](./amazon-store-dashboard.md) worden betreden.

- Het [Concurrentieprijsanalyse](./competitive-price-analysis.md)-rapport laat zien dat uw Amazon _landingsprijs_ (aanbiedingsprijs plus verzendprijs) in verhouding tot de [Buy Box](./buy-box-competitor-pricing.md)-prijs en [laagste concurrent](./lowest-competitor-pricing.md)-prijs.

- In het rapport [Aanbiedingsverbeteringen](./listing-improvements.md) worden alle voorgestelde verbeteringen voor aanbiedingen weergegeven die Amazon voor de geselecteerde winkel biedt.

>[!TIP]
>
>U kunt het logboekdossier voor extra informatie ook controleren wanneer het oplossen van problemen nodig is. Zie [Beheerinstellingen verkoopkanaal](./sales-channel-settings.md). Logboekregistratie voor synchronisatie van Amazon-verkoopkanalen wordt naar het `{Commerce Root}/var/log/channel_amazon.log`-bestand geschreven en kan worden weergegeven in [ontwikkelingsmodus](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}.
