---
title: Logboeken en winkelrapporten
description: Gebruik de logboeken en winkelrapporten om te zien wat er gebeurt in je Adobe Commerce- of Magento Open Source-winkel en in je Amazon Marketplace-aanbiedingen.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Logboeken en opslagrapporten

De Amazon-extensie voor verkoopkanalen bevat enkele waardevolle logboeken en winkelrapporten waarmee u de wijzigingen kunt bekijken die van invloed zijn op uw Amazon-aanbiedingen en -bestellingen. Met deze rapporten kun je zien wat er in je winkel gebeurt en verschillende statussen van aanbiedingen begrijpen.

Er zijn geen acties beschikbaar voor de logboeken of opslagrapporten, omdat het alleen-revisiefuncties zijn.

De volgende logbestanden zijn toegankelijk via de [opslagdashboard](./amazon-store-dashboard.md).

- De [Logbestand met wijzigingen in aanbieding](./listing-changes-log.md) geeft de wijzigingen weer die zijn opgetreden in je Amazon-verkopersaccount als weergave van je Amazon-verkoopkanaalinstellingen.

- De [Logboek met communicatiefouten](./communication-errors-log.md) geeft eventuele gemelde communicatiefouten met Amazon weer.

De volgende store-specific rapporten kunnen van worden betreden [opslagdashboard](./amazon-store-dashboard.md).

- De [Concurrentieprijsanalyse](./competitive-price-analysis.md) toont aan dat je Amazon _aanlandingsprijs_ (aanbiedingsprijs plus verzendprijs) in verhouding tot de [Buy Box](./buy-box-competitor-pricing.md) prijs en [laagste concurrent](./lowest-competitor-pricing.md) prijs.

- De [Aanbiedingsverbeteringen](./listing-improvements.md) In dit rapport worden alle voorstellen weergegeven die Amazon voor de geselecteerde winkel heeft gedaan.

>[!TIP]
>
>U kunt het logboekdossier voor extra informatie ook controleren wanneer het oplossen van problemen nodig is. Zie [Beheerinstellingen verkoopkanaal](./sales-channel-settings.md). Amazon-logboekregistratie van verkoopkanalen wordt geschreven naar `{Commerce Root}/var/log/channel_amazon.log` en kan worden weergegeven in [ontwikkelmodus](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}.
