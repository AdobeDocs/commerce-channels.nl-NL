---
user-guide-title: Amazon Sales Channel Handboek
user-guide-description: Verkoop genereren via Amazon door Adobe Commerce of Magento Open Source te integreren met uw [!DNL Amazon Seller Central] account.
breadcrumb-title: Amazon-verkoopkanaal
source-git-commit: 193f7bfc0c2373f9a79f9cdb7d01877971f31083
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---


# Verkoopkanaal van Amazon - [!DNL channel manager] voor Adobe Commerce {#amazon}

- [Overzicht van hulplijnen](guide-overview.md)
- [Inleiding tot Amazon-verkoopkanaal](overview.md)
- [Opmerkingen bij de release](release-notes.md)
- Aan de slag {#getting-started}
   - [Over Amazon-verkoopkanaal](about-amazon-sales-channel.md)
   - [Informatie over Amazon Marketplace](about-amazon-marketplace.md)
   - [Over Amazon en je handelscatalogus](about-listings-and-catalog.md)
   - [Aanbevolen werkwijzen en beperkingen](amazon-best-practices.md)
   - [De extensie installeren](install.md)
- Onboarding {#onboarding}
   - [Onboard Amazon-verkoopkanaal](amazon-onboarding-home.md)
   - [Taken vooraf instellen](amazon-pre-setup-tasks.md)
   - [Maken [!DNL Commerce] kenmerken voor Amazon](ob-creating-magento-attributes.md)
   - [De Amazon API-sleutel controleren](amazon-verify-api-key.md)
   - [Integratie van winkels](store-integration.md)
   - [Aanbiedingsregel maken](ob-create-listing-rule.md)
   - [Standaardopslaginstellingen](default-store-settings.md)
- Het verkoopkanaal beheren {#manage}
   - [Homepage](amazon-sales-channel-home.md)
   - [Amazon-winkels](managing-stores.md)
   - [Besturingselementen werkruimte](workspace-controls.md)
   - [Leren en voorbereiden](learning-preparation.md)
   - Attributen {#attributes}
      - [Kenmerken weergeven](attributes-view.md)
      - [Kenmerken beheren](managing-attributes.md)
      - [Kenmerken maken en bewerken](creating-attributes.md)
      - [Kenmerkentoewijzing weergeven](amazon-matching-attributes-values.md)
   - [Beheerinstellingen verkoopkanaal](sales-channel-settings.md)
   - [Amazon-opslagdashboard](amazon-store-dashboard.md)
   - [Opslaginstellingen](ob-store-review.md)
- Aanbiedingsinstellingen {#listing-settings}
   - [Aanbiedingsinstellingen weergeven](listing-settings.md)
   - [Handelingen voor productaanbiedingen](product-listing-actions.md)
   - [Aanbiedingen van derden](third-party-listing-settings.md)
   - [Aanbiedingsprijs](listing-price.md)
   - [(B2B) business pricing](business-pricing.md)
   - [Voorraad/hoeveelheid](stock-quantity.md)
   - [Betaald door](fulfilled-by.md)
   - [Catalogus zoeken](catalog-search.md)
   - [Voorwaarde voor aanbieding van producten](product-listing-condition.md)
   - [Vernieuwde producten](renewed-products.md)
- [Orderinstellingen](order-settings.md)
- [Integratie-instellingen opslaan](store-integration-settings.md)
- Aanbiedings- en prijsregels {#rules}
   - [Aanbiedingsregels](listing-rules.md)
   - Prijsregels {#pricing-rules}
      - [Prijzen beheren](pricing-products.md)
      - [Nieuwe prijsregel toevoegen](add-pricing-rule.md)
      - [Algemene instellingen prijsregel](pricing-rule-general-settings.md)
      - [Prijsregelvoorwaarden](pricing-rule-conditions.md)
      - [Prijsregelacties](pricing-rule-actions.md)
      - [Standaardprijsregel](standard-price-rules.md)
      - [Intelligente prijsregel](intelligent-repricing-rules.md)
      - [Voorwaardelijke variaties voor concurrent](competitor-conditional-variances.md)
      - [Prijsaanpassing](price-adjustment.md)
      - [Floor Price](floor-price.md)
      - [Facultatieve maximumprijs](optional-ceiling-price.md)
      - [Prijsbereik](price-scope.md)
      - [Logica voor prijsprioriteiten](price-priority-logic.md)
      - [Buy Box concurrent](buy-box-competitor-pricing.md)
      - [Laagste prijsstelling voor concurrenten](lowest-competitor-pricing.md)
   - Voorbeelden {#rules-examples}
      - [Een voorwaarde definiëren](ob-define-condition-example.md)
      - [Voorbeelden van prijsregels](price-rule-examples.md)
- Rapporten en logboeken {#reports-logs}
   - [Logboeken en opslagrapporten](amazon-logs-reports.md)
   - Winkelrapporten {#store-reports}
      - [Concurrentieprijsanalyse](competitive-price-analysis.md)
      - [Aanbiedingsverbeteringen](listing-improvements.md)
   - Logboeken {#logs}
      - [Logbestand voor wijzigingen in aanbieding](listing-changes-log.md)
      - [Logboek met communicatiefouten](communication-errors-log.md)
- Aanbiedingen beheren {#admin-listings}
   - [Amazon-aanbiedingen beheren](managing-product-listings.md)
   - Op status/tabblad {#status-tab}
      - [Beheren op status/tabblad](managing-listings-by-tab.md)
      - [Onvolledige aanbiedingen](incomplete-listings.md)
      - [Nieuwe aanbiedingen van derden](new-third-party-listings.md)
      - [Klaar voor lijst](ready-to-list.md)
      - [Inactieve aanbiedingen](inactive-listings.md)
      - [Actieve aanbiedingen](active-listings.md)
      - [Overschrijvingen](overrides.md)
      - [Niet-subsidiabele aanbiedingen](ineligible-listings.md)
      - [Afgelopen aanbiedingen](ended-listings.md)
   - Op acties {#actions}
      - [Beheer via handelingen](managing-listings-by-action.md)
      - [Catalogusproducten maken en toewijzen](creating-assigning-catalog-products.md)
      - [Overschrijvingen maken en bewerken](creating-editing-overrides.md)
      - [Een SKU voor Alias Seller maken](create-alias-seller-sku.md)
      - [Een toegewezen ASIN bewerken](edit-assigned-asin.md)
      - [Een Amazon-aanbieding beëindigen](end-listings-manually.md)
      - [Een Amazon-aanbieding publiceren](publish-listings-manually.md)
      - [Vereiste gegevens bijwerken](amazon-manually-update-incomplete-listing.md)
      - [Details weergeven](product-listing-details.md)
- Bestellingen beheren {#admin-orders}
   - [Bestellingen beheren](managing-orders.md)
   - [Amazon-bestellingen weergeven](amazon-orders-all.md)
   - [Amazon-ordergegevens weergeven](amazon-order-details.md)
   - [Algemene taken voor het verwerken van orders](common-order-processing.md)
   - [Workflows voor afhandeling](fulfillment-workflows.md)
   - [Niet-verzonden bestellingen annuleren](cancel-unshipped-order.md)
