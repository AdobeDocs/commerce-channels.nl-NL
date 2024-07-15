---
title: Producten toevoegen aan Channel Manager
description: "Creeer productassorment voor  [!DNL Walmart Marketplace]  verkoop door producten van de catalogus aan het verkoopkanaal toe te voegen dat in de Manager van het Kanaal wordt gevormd."
feature: Sales Channels, Merchandising, Products
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: 0087d60791cf00e4ed2bffe992447ee8e592fd9b
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Producten toevoegen aan [!DNL Channel Manager]

Als u producten wilt toevoegen aan het verkoopkanaal van [!DNL Walmart Marketplace] , selecteert u de producten in de [!DNL Commerce] productcatalogus en importeert u deze naar [!DNL Channel Manager] .
Het importeren kan maximaal 30 minuten duren, afhankelijk van het aantal producten dat u selecteert.

## Vereiste

**[de catalogusattributen van de Kaart](map-catalog-attributes.md)** - in de [!DNL Channel Settings] configuratie, kaart minstens één attribuut van de [!DNL Commerce] productcatalogus aan één van de vereiste Slimme Herkenningstekens van het Product—-GTIN, ISBN, ISSN, UPC, EAN.

## Aanbiedingsvereisten

[!DNL Commerce] productlijsten moeten de volgende vereiste kenmerkconfiguratie hebben:

- **[!UICONTROL Connect to Channel Manager]** -kenmerk is ingeschakeld

- Verstrek geldige waarden voor de vereiste attributen van de Mara.

   - Ten minste één productkenmerk dat overeenkomt met een van de vereiste [!DNL Walmart Marketplace] product-id&#39;s-GTIN, ISBN, ISSN, UPC, EAN.

   - Productprijs opgegeven tot maximaal twee decimalen, bijvoorbeeld `9.99`

   - Productgewicht opgegeven tot maximaal twee decimalen, bijvoorbeeld `1.25`

>[!TIP]
>
>Voor extra informatie over het optimaliseren van lijsten voor uw verkoopkanaal, zie de [ Gids van de Optimalisering van de Kwaliteit van de Marketplaats van de Markt van de Markt van de Markt ](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## Producten toevoegen

1. Van een verbonden opslag van het verkoopkanaal, uitgezochte **voegt producten** toe om de productcatalogus te openen.

   ![ voeg producten aan de opslag van het verkoopkanaal toe ](assets/add-initial-products-to-connected-channel.png){width="600" zoomable="yes"}

   De catalogus wordt op een nieuw tabblad geopend.

1. Selecteer in het raster van het catalogusproduct de producten die u wilt verkopen op [!DNL Walmart Marketplace] .

   ![ verzendt producten naar de opslag van het verkoopkanaal ](assets/select-products-from-catalog.png){width="600" zoomable="yes"}

1. Schakel het kenmerk **[!UICONTROL Connect to Channel Manager]** voor de geselecteerde items in.

   - Selecteer **[!UICONTROL Update attributes]** in **[!UICONTROL Actions]** .

   - Blader naar het kenmerk **[!UICONTROL Connect to Channel Manager]** en schakel dit in.

   - Controleer of de productkenmerken ten minste een van de vereiste [!DNL Walmart Product IDs] bevatten.

   - Selecteer **[!UICONTROL Save]** .

     Er wordt een bevestigingsbericht weergegeven.

     ![ de invoer van het Product van catalogus aan het bevestigingsbericht van het verkoopkanaal ](assets/product-import-from-catalog-confirmation.png){width="400"}

     Als het bericht aangeeft dat de update is gepland, gebruikt u de opdracht [`queue:consumers:start` ](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/start-message-queues.html) [!DNL CLI] om de update direct te verwerken.

     ```bash
     $ bin/magento queue:consumers:start product_action_attribute.update
     ```

1. Nadat het importeren is voltooid, controleert u de producten die u hebt toegevoegd door terug te keren naar [!DNL Channel Manager] en **[!UICONTROL Listings]** te selecteren.

   Aanvankelijk, zijn de producten in *Laag* status. Selecteer **[!UICONTROL Refresh products]** om de tabel bij te werken.

1. Werk de weergave bij om de nieuwe producten weer te geven die aan Kanaalbeheer zijn toegevoegd door de **[!UICONTROL Draft]** -statuskaart te selecteren.

   ![ Producten die aan verbonden verkoopkanaal worden ingevoerd ](assets/products-in-marketplace-sales-channel.png){width="400" zoomable="yes"}


