---
title: Alias Amazon Seller SKU maken
description: Met de Alias Amazon Seller SKU kunt u multiregionale Amazon-aanbiedingen maken op basis van je catalogusproducten voor Handel.
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Alias Amazon Seller SKU maken

Een [!DNL Alias Amazon Seller SKU] wordt gebruikt om een Amazon-aanbieding te maken van hetzelfde product in uw [!DNL Commerce]-catalogus. Als u een ervaren verkoper van Amazon bent, kunt u met [Amazon Globale SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target=&quot;_blank&quot;} en Marketplace-specifieke SKU voor inventaris en het verschepen vertrouwd zijn. Volgens vergelijkbare beginselen voor Amazon-verkoopkanalen controleert de verkoopeenheid van Amazon productinformatie op multiregionaal niveau en kan de [!DNL Alias Amazon Seller SKU] worden gebruikt om productinformatie op regionaal niveau te controleren.

Deze functie kan worden gebruikt om twee functies uit te voeren:

- Maak een [!DNL Alias Amazon Seller SKU] voor een van uw [!DNL Commerce] catalogusproducten om regiospecifieke aanbiedingsgegevens te beheren.

   **Voorbeeld**: Je bent een verkoper in zowel de VS als Canada. Vergeet niet dat elk van uw Amazon-winkels voor verkoopkanalen tijdens de installatie slechts één Amazon-regio kan worden toegewezen. U hebt dus een Amazon-winkel voor verkoopkanalen met een bepaalde regio in de VS en een andere winkel met een bepaalde regio in Canada. Beide winkels delen uw [!DNL Commerce]-catalogus voor aanbiedingsgegevens in beide regio&#39;s, inclusief de productkenmerken Amazon Seller SKU en ASIN. Aanbiedingen voor het catalogusproduct zouden dus hetzelfde zijn in zowel winkels als winkels, waar prijzen, voorraad/hoeveelheid en andere productkenmerken worden gedeeld. Maar uw voorraad voor uw Canada slaat schepen op vanaf een locatie in Canada, en uw Amerikaanse winkelschepen vanaf een locatie in de VS. Je moet dus voor elke winkel afzonderlijk het aantal aanbiedingen bepalen. Voor dit type regiospecifiek besturingselement kunt u een Alias Amazon Seller SKU maken.

   In feite kunt u een SKU voor Alias Amazon-verkopers maken die is gekoppeld aan hetzelfde catalogusproduct en kan worden gebruikt om dezelfde aanbieding in dat gebied opnieuw te publiceren.

- Maak een [!DNL Alias Amazon Seller SKU] en combineer een van uw [!DNL Commerce] catalogusproducten met twee Amazon-aanbiedingen.

   **Voorbeeld**: Je hebt een catalogusproduct dat overeenkomt met een Amazon-aanbieding. Aangezien Amazon vaak meerdere aanbiedingen voor hetzelfde product bevat, kun je een andere Amazon-aanbieding voor hetzelfde product vinden, maar Amazon heeft een andere ASIN aan de aanbieding toegewezen. Als u uw product beter zichtbaar wilt maken, wilt u het catalogusproduct afstemmen op de verschillende ASIN-waarden en aanbiedingen maken voor beide ASIN-waarden. Hiervoor kunt u een Alias Amazon Seller SKU maken.

   In feite kunt u een [!DNL Alias Amazon Seller SKU] maken die kan worden gebruikt om één catalogusproduct aan een tweede Amazon-aanbieding aan te passen en een lijst maken voor de zojuist overeenkomende ASIN. In dit scenario hebt u twee Amazon-aanbiedingen voor hetzelfde catalogusproduct.

   Nadat je een Alias Amazon Seller SKU hebt gemaakt, kun je je aanbiedingsinstellingen, regels en overschrijvingen gebruiken om de aanbiedingsgegevens voor het gebied te bepalen. Productkenmerken die voor een aanbieding per regio kunnen worden gedefinieerd, zijn hoeveelheid/voorraad, uitvoeringsmethode, voorwaarde, geschiktheid van het product en verwerkingstijd.

## Wordt gebruikt voor een regiospecifiek doel {#region-specific}

Geef de vermelding weer op de _[!UICONTROL Product Listings]_-pagina (_[!UICONTROL Inactive]_, _Actief_, _Niet in aanmerking komend_ of _Beëindigd_ tabblad).

1. Klik onder _[!UICONTROL Actions]_op **[!UICONTROL Create Alias Seller SKU]**.

1. Voer bij **[!UICONTROL Assign New Seller SKU]** een unieke alfanumerieke waarde in.

   Deze waarde moet uniek zijn (wordt niet gebruikt voor andere producten of alias in uw catalogus).

1. Wijzig **[!UICONTROL Assign New ASIN]** niet.

   Deze waarde wordt automatisch ingevuld met het product-ASIN dat overeenkomt met het catalogusproduct. Als u deze waarde wijzigt, wordt het catalogusproduct omgezet in twee Amazon-aanbiedingen op basis van de ASIN.

1. Schakel indien nodig de optie **[!UICONTROL Remove Existing Seller SKU]** in.

   - `Yes` - Kies of u de aanbieding wilt verwijderen en een aanbieding wilt maken met de nieuwe gegevens die u opgeeft.

   - `No` - Kies of je een aanbieding wilt maken en de oude aanbieding ongewijzigd wilt laten.

1. Klik op **[!UICONTROL Save Listing Update]**.

## Wordt gebruikt om één catalogusproduct aan twee Amazon-aanbiedingen te koppelen

1. Geef de vermelding weer op de _[!UICONTROL Product Listings]_-pagina (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_ of _[!UICONTROL Ended]_tabs).

1. Klik onder _[!UICONTROL Actions]_op **[!UICONTROL Create Alias Seller SKU]**.

1. Voer bij **[!UICONTROL Assign New Seller SKU]** een unieke alfanumerieke waarde in.

   Deze waarde moet uniek zijn (wordt niet gebruikt voor andere producten of alias in uw catalogus).

1. Voer bij **[!UICONTROL Assign New ASIN]** een unieke alfanumerieke waarde in.

   Deze waarde wordt automatisch ingevuld met het product-ASIN dat overeenkomt met het catalogusproduct. Als u deze waarde wijzigt, wordt het catalogusproduct omgezet in twee Amazon-aanbiedingen op basis van de ASIN.

1. Schakel indien nodig de optie **[!UICONTROL Remove Existing Seller SKU]** in.

   - `Yes` - Kies of u de aanbieding wilt verwijderen en een aanbieding wilt maken met de nieuwe gegevens die u opgeeft.

   - `No` - Kies of je nog een aanbieding wilt maken en de oude aanbieding ongewijzigd wilt laten.

1. Klik op **[!UICONTROL Save Listing Update]**.

![een Alias Amazon Seller SKU maken](assets/amazon-alias-sku-create.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Assign New Seller SKU] | Voer een nieuwe, unieke alfanumerieke waarde in die moet worden gekoppeld aan de oorspronkelijke SKU van de Amazon-verkoper. Dit nummer wordt alleen gebruikt door het verkoopkanaal van Amazon om overeen te komen met het catalogusproduct. U kunt om het even welke waarde van SKU gebruiken, maar de waarde kan slechts eenmaal in uw catalogus worden gebruikt. |
| [!UICONTROL Assign New ASIN] | Voer de ASIN-waarde in voor de aanbieding waaraan u het catalogusproduct wilt aanpassen. Pas dit veld alleen aan als een enkel catalogusproduct overeenkomt met de ASIN voor een andere vermelding voor hetzelfde product. Deze waarde moet overeenkomen met de ASIN die door Amazon is toegewezen, anders wordt de aanbieding niet door Amazon afgewezen. |
| [!UICONTROL Remove Existing Seller SKU] | Opties:<ul><li>**[!UICONTROL Yes]** - Kies of u de aanbieding wilt verwijderen en een aanbieding wilt maken met de nieuwe gegevens die u opgeeft. De nieuwe vermelding wordt weergegeven op het tabblad _[!UICONTROL Active]_en de oude vermelding wordt verplaatst naar het tabblad_ Einde _.</li><li>**[!UICONTROL No]** - Kies of je nog een aanbieding wilt maken en de oude aanbieding ongewijzigd wilt laten. Beide aanbiedingen worden weergegeven op het tabblad Actief nadat de nieuwe aanbieding is gemaakt.</li></ul> |
