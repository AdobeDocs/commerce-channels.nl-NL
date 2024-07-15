---
title: Producten maken en toewijzen voor Amazon-verkoopkanaal
description: Amazon-Sales Channel biedt het tabblad [!UICONTROL New Third Party] om te helpen bij het maken en toewijzen van overeenkomende Commerce-catalogusproducten aan Amazon-aanbiedingen.
feature: Sales Channels, Products, Configuration
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# Producten maken en toewijzen

Wanneer u het tabblad _[!UICONTROL New Third Party]_weergeeft, kunt u uw catalogusproducten van [!DNL Commerce] aanpassen aan een bestaande Amazon-lijst. Er zijn twee opties voor deze overeenkomst. U kunt een aanbieding aan een bestaand catalogusproduct toewijzen of u kunt de informatie uit de aanbieding gebruiken om catalogusproducten te maken. Deze opties zijn handig als je Amazon-aanbiedingen niet automatisch overeenkomen met je catalogus van [!DNL Commerce] .

Als je de volledige functieset van het verkoopkanaal van Amazon wilt gebruiken, moet je je producten afstemmen op je Amazon-aanbiedingen.

Wanneer u een catalogusproduct maakt op basis van een Amazon-aanbieding:

- **ASIN** wordt [!DNL Commerce] SKU
- De **Naam van de Lijst van het Product** wordt de Catalogus van de Lijst Naam
- De **Prijs** en **Hoeveelheid** worden ingevoerd van Amazon die

De overige benodigde instellingen worden bepaald door de productinstellingen die u selecteert tijdens het maken van het bestand. [!DNL Commerce]

Wanneer deze items zijn gemaakt en overeenkomen, worden ze verwijderd van het tabblad _[!UICONTROL New Third Party]_en weergegeven op het tabblad_[!UICONTROL Active]_ .

## Eén catalogusproduct toewijzen aan een Amazon-aanbieding

1. Bekijk je productaanbiedingen op het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) .

1. Zoek de vermelding die u wilt toewijzen in de lijst, klik op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_en klik op **[!UICONTROL Assign Catalog Product]**.

   Met deze handeling wordt de pagina _[!UICONTROL Assign Magento Catalog Product]_geopend.

1. Blader naar of filter de lijst gebruikend de [ werkruimtecontroles ](./workspace-controls.md) en bepaal de plaats van het aangewezen catalogusproduct om aan de lijst aan te passen.

1. Klik op **[!UICONTROL Assign Catalog Product]** in de kolom _[!UICONTROL Action]_wanneer het juiste product in de lijst wordt weergegeven.

Je product en aanbieding komen nu overeen. Verkoopkanaal van Amazon kan nu product- en aanbiedingsgegevens delen met Amazon en je aanbieding en de bijbehorende informatie beheren, zoals de prijs van de aanbieding, de verzendprijs, het aantal voorraad/de hoeveelheid, de ordergegevens en status, enzovoort.

## Eén catalogusproduct maken met de Amazon-aanbiedingsgegevens

1. Bekijk je productaanbiedingen op het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) .

1. Zoek de vermelding die u wilt maken in de catalogus van [!DNL Commerce] , klik op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_en klik op **[!UICONTROL Create New Catalog Product]**.

   Met deze handeling wordt de pagina _[!UICONTROL Create Magento Catalog Product]_geopend.

1. Voltooi de catalogusinstellingen voor het product.

   - Stel **[!UICONTROL Enable Product(s)]** in op `Yes` of `No` (vereist).

     |Ja|Kies of u het product in aanmerking wilt laten komen voor uw [!DNL Commerce] winkel-omzet.|
|Nee|Kies of u het product niet in aanmerking wilt laten komen voor uw [!DNL Commerce] winkel.|

   - Wijs voor **[!UICONTROL Categories]** een categorie voor het product toe (optioneel).

     Als u de categorie van het product wilt selecteren, klikt u op de pijl omlaag en schakelt u een selectievakje voor de categorie in. Klik op **[!UICONTROL Done]** als u klaar bent.

   - Kies bij **[!UICONTROL Website Ids]** de website (winkel) waaraan het product moet worden gekoppeld.

     De opties in deze lijst hangen van uw [!DNL Commerce] [ montages van de opslagconfiguratie ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) af.

   - Kies een optie bij **[!UICONTROL Attribute Set Id]** (vereist).

     `Default` is de standaardselectie. De opties in deze lijst hangen van uw [!DNL Commerce] [ kenmerkreeksen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) af u hebt gevormd.

   - Kies bij **[!UICONTROL Visibility]** een optie voor het nieuwe product.

     |**[!UICONTROL Not Visible Individually]** (standaard)|Het product is niet in je winkelaanbiedingen opgenomen, hoewel het mogelijk beschikbaar is als een variatie van een ander product.|
|**[!UICONTROL Catalog]**|Het product wordt weergegeven in uw cataloguslijsten.|
|**[!UICONTROL Search]**|Het product is beschikbaar voor zoekacties.|
|**[!UICONTROL Catalog and Search]**|Het product is opgenomen in cataloguslijsten en beschikbaar voor zoekbewerkingen.|

   - Kies bij **[!UICONTROL Assign Tax Class]** een optie voor het product.

     De opties die in deze lijst tonen hangen van de [ belastingklassen ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) af u hebt gevormd.

   - Klik op **[!UICONTROL Create Catalog Products]** als de bewerking is voltooid.

Het catalogusproduct wordt gemaakt in uw catalogus van [!DNL Commerce] en toegewezen aan de Amazon-aanbieding waaruit het is gemaakt. Nu de vermelding overeenkomt met een bestaande Amazon-vermelding, wordt de vermelding verwijderd van het tabblad _[!UICONTROL New Third Party]_en weergegeven op het tabblad_[!UICONTROL Active]_ .

## Meerdere catalogusproducten maken met hun Amazon-aanbiedingsgegevens

1. Bekijk je productaanbiedingen op het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) .

1. Selecteer de aanbiedingen waarvoor u catalogusproducten wilt maken.

   U kunt afzonderlijke selectievakjes selecteren in de linkerkolom of u kunt op de pijl-omlaag in de linkerkolom klikken en **[!UICONTROL Select All]** of **[!UICONTROL Select All on this Page]** kiezen.

1. Klik onder _[!UICONTROL Actions]_op **[!UICONTROL Create New Catalog Product(s)]**.

1. Klik op **[!UICONTROL OK]** om het bevestigingsbericht te accepteren en de pagina _[!UICONTROL Create Magento Catalog Product]_te openen.

1. Voltooi de catalogusinstellingen voor de producten.

   >[!NOTE]
   >Wanneer u catalogusproducten maakt voor meerdere geselecteerde aanbiedingen, worden de ingevoerde productinstellingen toegepast op alle aanbiedingen.

   - Stel **[!UICONTROL Enable Product(s)]** in op `Yes` of `No` (vereist).

     |Ja|Kies of u het product in aanmerking wilt laten komen voor uw [!DNL Commerce] winkel-omzet.|
|Nee|Kies of u het product niet in aanmerking wilt laten komen voor uw [!DNL Commerce] winkel.|

   - Wijs voor **[!UICONTROL Categories]** een categorie voor het product toe (optioneel).

     Als u de categorie van het product wilt selecteren, klikt u op de pijl omlaag en schakelt u een selectievakje voor de categorie in. Klik **Gedaan** wanneer gebeëindigd.

   - Kies bij **[!UICONTROL Website Ids]** de website (winkel) waaraan het product moet worden gekoppeld.

     De opties in deze lijst hangen van uw [!DNL Commerce] [ montages van de opslagconfiguratie ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) af.

   - Kies een optie bij **[!UICONTROL Attribute Set Id]** (vereist).

     `Default` is de standaardselectie. De opties in deze lijst hangen van uw [!DNL Commerce] [ kenmerkreeksen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) af u hebt gevormd.

   - Kies bij **[!UICONTROL Visibility]** een optie voor het nieuwe product.

     |**[!UICONTROL Not Visible Individually]** (standaard)|Het product is niet in je winkelaanbiedingen opgenomen, hoewel het mogelijk beschikbaar is als een variatie van een ander product.|
|**[!UICONTROL Catalog]**|Het product wordt weergegeven in uw cataloguslijsten.|
|**[!UICONTROL Search]**|Het product is beschikbaar voor zoekacties.|
|**[!UICONTROL Catalog and Search]**|Het product is opgenomen in cataloguslijsten en beschikbaar voor zoekbewerkingen.|

   - Kies bij **[!UICONTROL Assign Tax Class]** een optie voor het product.

     De opties die in deze lijst tonen hangen van de [ belastingklassen ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) af u hebt gevormd.

   - Klik op **[!UICONTROL Create Catalog Products]** als de bewerking is voltooid.

De catalogusproducten worden gemaakt in uw catalogus van [!DNL Commerce] en toegewezen aan de Amazon-aanbieding waaruit deze is gemaakt. Nu de aanbiedingen overeenkomen met hun respectievelijke Amazon-aanbieding, worden de aanbiedingen verwijderd van het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) en weergegeven op het tabblad [_[!UICONTROL Active]_](./active-listings.md) .

![ creeer Commerce catalogusproduct ](assets/amazon-magento-catalog-product.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Product(s)] | (Vereist) Indien ingeschakeld, is het product zichtbaar in uw [!DNL Commerce] winkel. Als deze optie is uitgeschakeld, wordt het product niet weergegeven in uw [!DNL Commerce] winkel. |
| [!UICONTROL Categories] | U kunt de naam van de categorie voor het nieuwe product invoeren of een categorie selecteren door op de pijl-omlaag te klikken om de opties weer te geven. De opties hangen van uw [ categorieën ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/categories/create/category-create.html) configuratie af. |
| [!UICONTROL Website Ids] | (Vereist) Kies de website (winkel) waaraan het product moet worden gekoppeld. De opties hangen van uw [!DNL Commerce] ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) montages van de 1} opslagconfiguratie af[ |
| Kenmerkset-id | Kies een kenmerkset. De opties hangen van uw gevormde [!DNL Commerce] [ kenmerkreeksen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) af. |
| [!UICONTROL Visibility] | Opties:<ul><li>**[!UICONTROL Not Visible Individually]** - Het product is niet zichtbaar in uw [!DNL Commerce] winkel (meest gangbaar voor variantproducten).</li><li>**[!UICONTROL Catalog]** - Hiermee kunt u het product openen via de categorie waaraan het is gekoppeld in de website.</li><li>**Onderzoek** - staat het product toe om slechts door het onderzoekshulpmiddel worden gevonden.</li><li>**[!UICONTROL Catalog and Search]** - Hiermee kunt u de producten openen via de categoriestructuur en met het zoekgereedschap.</li></ul> |
| [!UICONTROL Assign Tax Class] | Wijs een belastingklasse aan het nieuwe product toe. De opties hangen van uw gevormde [ belastingklassen ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) af. |
