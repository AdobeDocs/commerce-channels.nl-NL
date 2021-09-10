---
title: Producten maken en toewijzen
description: Amazon Sales Channel biedt het tabblad [!UICONTROL New Third Party] om te helpen bij het maken en toewijzen van overeenkomstige handelscatalogusproducten met Amazon-aanbiedingen.
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Producten maken en toewijzen

Wanneer u _[!UICONTROL New Third Party]_tabblad weergeeft, kunt u uw [!DNL Commerce] catalogusproducten aanpassen aan een bestaande Amazon-aanbieding. Er zijn twee opties voor deze overeenkomst. U kunt een aanbieding aan een bestaand catalogusproduct toewijzen of u kunt de informatie uit de aanbieding gebruiken om catalogusproducten te maken. Deze opties zijn handig wanneer uw Amazon-aanbiedingen niet automatisch overeenkomen met uw [!DNL Commerce]-catalogus.

Als je de volledige functieset van het verkoopkanaal van Amazon wilt gebruiken, moet je je producten afstemmen op je Amazon-aanbiedingen.

Wanneer u een catalogusproduct maakt op basis van een Amazon-aanbieding:

- De **ASIN** wordt de [!DNL Commerce] SKU
- De **Naam van productlijst** wordt de naam van de cataloguslijst
- De **Prijs** en **Hoeveelheid** worden geïmporteerd uit de Amazon-aanbieding

De overige benodigde instellingen worden bepaald door de [!DNL Commerce] productinstellingen die u selecteert tijdens het maken.

Wanneer deze items zijn gemaakt en overeenkomen, worden ze verwijderd van het tabblad _[!UICONTROL New Third Party]_en weergegeven op het tabblad_[!UICONTROL Active]_.

## Eén catalogusproduct toewijzen aan een Amazon-aanbieding

1. Bekijk je productaanbiedingen op het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md).

1. Zoek de aanbieding die u wilt toewijzen in de lijst, klik op **[!UICONTROL Select]** in de kolom _[!UICONTROL Action]_en klik op **[!UICONTROL Assign Catalog Product]**.

   Met deze handeling wordt de pagina _[!UICONTROL Assign Magento Catalog Product]_geopend.

1. Blader naar of filter de lijst met de [werkruimte-besturingselementen](./workspace-controls.md) en zoek het geschikte catalogusproduct dat u wilt aanpassen aan de lijst.

1. Wanneer het correcte product in de lijst verschijnt, klik **[!UICONTROL Assign Catalog Product]** in _[!UICONTROL Action]_kolom.

Je product en aanbieding komen nu overeen. Verkoopkanaal van Amazon kan nu product- en aanbiedingsgegevens delen met Amazon en je aanbieding en de bijbehorende informatie beheren, zoals de prijs van de aanbieding, de verzendprijs, het aantal voorraad/de hoeveelheid, de ordergegevens en status, enzovoort.

## Eén catalogusproduct maken met de Amazon-aanbiedingsgegevens

1. Bekijk je productaanbiedingen op het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md).

1. Zoek de aanbieding die u in uw [!DNL Commerce] catalogus wilt maken, klik **[!UICONTROL Select]** in _[!UICONTROL Action]_kolom, en klik **[!UICONTROL Create New Catalog Product]**.

   Met deze handeling wordt de pagina _[!UICONTROL Create Magento Catalog Product]_geopend.

1. Voltooi de catalogusinstellingen voor het product.

   - Stel **[!UICONTROL Enable Product(s)]** in op `Yes` of `No` (vereist).

      |Ja|Kies of u het product in aanmerking wilt laten komen voor uw [!DNL Commerce]-winkel.|
|Nee|Kies of u het product niet in aanmerking wilt laten komen voor uw [!DNL Commerce]-winkel.|

   - Wijs voor **[!UICONTROL Categories]** een categorie voor het product toe (optioneel).

      Als u de categorie van het product wilt selecteren, klikt u op de pijl omlaag en schakelt u een selectievakje voor de categorie in. Klik **[!UICONTROL Done]** wanneer gebeëindigd.

   - Kies voor **[!UICONTROL Website Ids]** de website (winkel) waaraan het product moet worden gekoppeld.

      De opties in deze lijst hangen van uw [!DNL Commerce] [opslagconfiguratie](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} montages af.

   - Kies een optie voor **[!UICONTROL Attribute Set Id]** (vereist).

      `Default` is de standaardselectie. De opties in deze lijst hangen van uw [!DNL Commerce] [kenmerkreeksen](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;} af u hebt gevormd.

   - Kies voor **[!UICONTROL Visibility]** een optie voor het nieuwe product.

      |**[!UICONTROL Not Visible Individually]** (standaard)|Het product is niet opgenomen in uw winkelaanbiedingen, hoewel het mogelijk beschikbaar is als een variatie van een ander product.|
|**[!UICONTROL Catalog]**|Het product wordt weergegeven in uw cataloguslijsten.|
|**[!UICONTROL Search]**|Het product is beschikbaar voor zoekopdrachten.|
|**[!UICONTROL Catalog and Search]**|Het product is opgenomen in cataloguslijsten en beschikbaar voor zoekopdrachten.|

   - Kies voor **[!UICONTROL Assign Tax Class]** een optie voor het product.

      De opties die in deze lijst tonen hangen van [fiscale klassen ](https://docs.magento.com/user-guide/tax/tax-class.html){target= &quot;_blank&quot;} af u hebt gevormd.

   - Klik op **[!UICONTROL Create Catalog Products]** als u klaar bent.

Het catalogusproduct wordt gemaakt in uw [!DNL Commerce]-catalogus en toegewezen aan de Amazon-aanbieding waaruit het is gemaakt. Nu de aanbieding overeenkomt met een bestaande Amazon-aanbieding, wordt de vermelding verwijderd van het tabblad _[!UICONTROL New Third Party]_en weergegeven op het tabblad_[!UICONTROL Active]_.

## Meerdere catalogusproducten maken met hun Amazon-aanbiedingsgegevens

1. Bekijk je productaanbiedingen op het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md).

1. Selecteer de aanbiedingen waarvoor u catalogusproducten wilt maken.

   U kunt afzonderlijke selectievakjes in de linkerkolom selecteren of u kunt op de pijl omlaag in de linkerkolom klikken en **[!UICONTROL Select All]** of **[!UICONTROL Select All on this Page]** kiezen.

1. Klik onder _[!UICONTROL Actions]_op **[!UICONTROL Create New Catalog Product(s)]**.

1. Als u het bevestigingsbericht wilt accepteren en de pagina _[!UICONTROL Create Magento Catalog Product]_wilt openen, klikt u op **[!UICONTROL OK]**.

1. Voltooi de catalogusinstellingen voor de producten.

   >[!NOTE]
   >Wanneer u catalogusproducten maakt voor meerdere geselecteerde aanbiedingen, worden de ingevoerde productinstellingen toegepast op alle aanbiedingen.

   - Stel **[!UICONTROL Enable Product(s)]** in op `Yes` of `No` (vereist).

      |Ja|Kies of u het product in aanmerking wilt laten komen voor uw [!DNL Commerce]-winkel.|
|Nee|Kies of u het product niet in aanmerking wilt laten komen voor uw [!DNL Commerce]-winkel.|

   - Wijs voor **[!UICONTROL Categories]** een categorie voor het product toe (optioneel).

      Als u de categorie van het product wilt selecteren, klikt u op de pijl omlaag en schakelt u een selectievakje voor de categorie in. Klik **Done** wanneer gebeëindigd.

   - Kies voor **[!UICONTROL Website Ids]** de website (winkel) waaraan het product moet worden gekoppeld.

      De opties in deze lijst hangen van uw [!DNL Commerce] [opslagconfiguratie](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} montages af.

   - Kies een optie voor **[!UICONTROL Attribute Set Id]** (vereist).

      `Default` is de standaardselectie. De opties in deze lijst hangen van uw [!DNL Commerce] [kenmerkreeksen](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;} af u hebt gevormd.

   - Kies voor **[!UICONTROL Visibility]** een optie voor het nieuwe product.

      |**[!UICONTROL Not Visible Individually]** (standaard)|Het product is niet opgenomen in uw winkelaanbiedingen, hoewel het mogelijk beschikbaar is als een variatie van een ander product.|
|**[!UICONTROL Catalog]**|Het product wordt weergegeven in uw cataloguslijsten.|
|**[!UICONTROL Search]**|Het product is beschikbaar voor zoekopdrachten.|
|**[!UICONTROL Catalog and Search]**|Het product is opgenomen in cataloguslijsten en beschikbaar voor zoekopdrachten.|

   - Kies voor **[!UICONTROL Assign Tax Class]** een optie voor het product.

      De opties die in deze lijst tonen hangen van [fiscale klassen ](https://docs.magento.com/user-guide/tax/tax-class.html){target= &quot;_blank&quot;} af u hebt gevormd.

   - Klik op **[!UICONTROL Create Catalog Products]** als u klaar bent.

De catalogusproducten worden gemaakt in uw [!DNL Commerce]-catalogus en toegewezen aan de Amazon-aanbieding waaruit deze is gemaakt. Nu de aanbiedingen overeenkomen met hun respectievelijke Amazon-aanbieding, worden de aanbiedingen verwijderd van het tabblad [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) en weergegeven op het tabblad [_[!UICONTROL Active]_](./active-listings.md).

![Catalogusproduct voor handel maken](assets/amazon-magento-catalog-product.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Enable Product(s)] | (Vereist) Indien ingeschakeld, is het product zichtbaar in uw [!DNL Commerce] winkel. Indien uitgeschakeld, wordt het product niet weergegeven in de winkelomgeving [!DNL Commerce]. |
| [!UICONTROL Categories] | U kunt de naam van de categorie voor het nieuwe product invoeren of een categorie selecteren door op de pijl-omlaag te klikken om de opties weer te geven. De opties hangen van uw [categorieën](https://docs.magento.com/user-guide/catalog/category-create.html){target= &quot;_blank&quot;} configuratie af. |
| [!UICONTROL Website Ids] | (Vereist) Kies de website (winkel) waaraan het product moet worden gekoppeld. De opties hangen van uw [!DNL Commerce] [opslagconfiguratie](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} montages af |
| Kenmerkset-id | Kies een kenmerkset. De opties hangen van uw gevormde [!DNL Commerce] [kenmerkreeksen](https://docs.magento.com/user-guide/stores/attribute-sets.html){target= &quot;_blank&quot;} af. |
| [!UICONTROL Visibility] | Opties:<ul><li>**[!UICONTROL Not Visible Individually]** - Het product is niet zichtbaar in uw  [!DNL Commerce] winkel (meest voorkomende voor variantproducten).</li><li>**[!UICONTROL Catalog]** - Hiermee krijgt u toegang tot het product via de categorie waaraan het is gekoppeld op de website.</li><li>**Zoeken**  - Hiermee kan het product alleen worden gevonden met de zoekfunctie.</li><li>**[!UICONTROL Catalog and Search]** - Hiermee kunt u de producten openen via de categoriestructuur en met het zoekgereedschap.</li></ul> |
| [!UICONTROL Assign Tax Class] | Wijs een belastingklasse aan het nieuwe product toe. De opties hangen van uw gevormde [fiscale klassen ](https://docs.magento.com/user-guide/tax/tax-class.html){target= &quot;_blank&quot;} af. |
