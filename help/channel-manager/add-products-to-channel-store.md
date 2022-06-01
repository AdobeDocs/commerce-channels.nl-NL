---
title: Producten toevoegen aan verkoopkanaalwinkel
description: Productassortiment maken voor [!DNL Walmart Marketplace] verkoop door producten uit de catalogus aan het verkoopkanaal toe te voegen
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: e3b12c9ce1ad4b5be17284e98956a773d7ccca24
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Producten toevoegen aan verkoopkanaalwinkel

Producten synchroniseren met de [!DNL Walmart Marketplace] verkoopkanaal, selecteert u producten van [!DNL Commerce] productcatalogus en deze importeren in Channel Manager. De geselecteerde producten moeten de volgende attributenconfiguratie hebben:

- **[!UICONTROL Publish to Channel Manager]** attribute is enabled

- Ten minste één productkenmerk moet overeenkomen met een van de [vereist [!DNL Walmart Marketplace] attributes](map-catalog-attributes.md)-GTIN, ISBN, ISSN, UPC, EAN

Het proces voor de invoer van producten uit [!DNL Commerce] naar Channel Manager kan maximaal 30 minuten of meer in beslag nemen, afhankelijk van het aantal producten dat u selecteert.

## Producten toevoegen

1. Selecteer in een online verkoopkanaalwinkel de optie **Producten toevoegen** om de productcatalogus te openen.

   ![Producten toevoegen aan verkoopkanaalwinkel](assets/add-initial-products-to-connected-channel.png)

   De catalogus wordt op een nieuw tabblad geopend.

1. Selecteer in het productraster van de catalogus de producten waarop u wilt verkopen [!DNL Walmart Marketplace].

   ![Producten naar de winkel van het verkoopkanaal verzenden](assets/select-products-from-catalog.png)

1. De optie **[!UICONTROL Publish to Channel Manager]** voor de geselecteerde items.

   - Van **[!UICONTROL Actions]**, selecteert u **[!UICONTROL Update attributes]**.

   - Naar de **[!UICONTROL Publish to Channel Manager]** en inschakelen.

   - Controleren of de productkenmerken ten minste een van de vereiste kenmerken bevatten [!DNL Walmart Product IDs].

   - Selecteren **[!UICONTROL Save]**.

      Er wordt een bevestigingsbericht weergegeven.

      ![Bevestigingsbericht voor het importeren van producten uit catalogus naar verkoopkanaal](assets/product-import-from-catalog-confirmation.png)

      Als het bericht aangeeft dat de update is gepland, gebruikt u de [wachtrij:consumers:start](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] gebruiken om de update onmiddellijk te verwerken.

      ```bash
      $ bin/magento queue:consumers:start product_action_attribute.update
      ```

1. Nadat het importeren is voltooid, controleert u de producten die u hebt toegevoegd door terug te keren naar [!DNL Channel Manager] en selecteren **[!UICONTROL Listings]**.

   ![Producten geïmporteerd naar verbonden verkoopkanaal](assets/products-in-marketplace-sales-channel.png)

   In eerste instantie bevinden de producten zich in *Concept* status. Selecteren **[!UICONTROL Refresh products]** om de tabel bij te werken.

