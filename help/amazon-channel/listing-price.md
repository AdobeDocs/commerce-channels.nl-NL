---
title: Verkoopkanaal van Amazon - [!UICONTROL Listing Price]
description: Gebruik de instellingen voor de aanbiedingsprijs om de prijsbron en de basisprijs (standaardprijs) voor je Amazon-aanbiedingen te bepalen.
feature: Sales Channels, Products, Price Rules
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# [!UICONTROL Listing Price]

[!UICONTROL Listing Price] Deze instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via de [opslagdashboard](./amazon-store-dashboard.md).

Deze instellingen bepalen welke [!DNL Commerce] Het prijskenmerk dat als je prijsbron moet worden gebruikt. Dit is de basisprijs (de standaardprijs) voor je Amazon-aanbiedingen. Deze instellingen worden gebruikt door uw [prijsregels](./pricing-rule-general-settings.md) als je de prijs van je Amazon-aanbieding automatisch wilt aanpassen ten opzichte van de waarde die is ingesteld voor _[!UICONTROL Magento Price Source]_.

U kunt uw [prijsbereik](./price-scope.md) als globaal of website. Als uw prijsbereik is ingesteld op `Global`, is er één prijsbron voor al uw winkels/websites. Als uw prijsbereik is ingesteld op `Website`De prijsbron gebruikt een fallback-logica van de websiteprijs (indien beschikbaar) gevolgd door de standaardprijs (global).

Als een aanbiedingsregel op meer dan één website van toepassing is, wordt de volgorde waarin de websiteprijs wordt gebruikt bepaald door de instelling voor de prioriteit van de website die in het dialoogvenster [aanbiedingsregel](./listing-rules.md). Met deze regels kunt u productprijzen in de hele catalogus definiëren. Ga voor meer informatie over het prijsbereik van websites naar [Bereik catalogusprijs](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html).

De opties in _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_, en _[!UICONTROL Strike Through Price (MSRP)]_omvat uw gevormde het Prijsattributen. Prijskenmerken zijn [!DNL Commerce] productkenmerken met de waarde voor Invoertype catalogus voor Winkeleigenaar ingesteld op `Price`. Zie [Kenmerkinvoertypen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/attributes-input-types.html).

## Instellingen voor aanbiedingsprijs configureren {#configure-listing-price-settings}

1. Klikken **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Breid uit _[!UICONTROL Listing Price]_sectie.

1. Voor **[!UICONTROL Magento Price Source]** (vereist), kiest u een optie.

   De standaardwaarde is `Price`. Deze instelling bepaalt de prijsbron die wordt gebruikt voor je Amazon-aanbiedingen. Als u [prijsregels](./pricing-products.md), worden de regels toegepast op de waarde die is gedefinieerd voor het hier geselecteerde kenmerk. U kunt om het even welk gevormd prijsattribuut selecteren. Als het geselecteerde kenmerk echter niet is ingevuld voor een product, wordt de prijsbron voor het product standaard teruggezet naar `Price` wanneer prijsregels worden toegepast om de gepubliceerde Amazon-aanbiedingsprijs te bepalen.

1. Voor **[!UICONTROL Minimum Advertised Price (MAP)**]kiest u een optie.

   Standaard is er geen selectie. Met deze instelling wordt een minimale geadverteerde prijs (MAP) voor een product ingeschakeld. Wanneer je een prijskenmerk definieert en de prijs van je aanbieding voor een product onder de vastgestelde minimumprijs daalt (op basis van je prijsbron en regels), wordt deze waarde de MAP voor de aanbieding. Met deze instelling kunt u implementeren [prijsregels](./pricing-products.md), terwijl je minimumprijs voor een product blijft bepalen. Als je wilt voorkomen dat een aanbiedingsprijs te laag is, kies je een prijskenmerk dat je als KAART wilt gebruiken. Als het geselecteerde prijsveld echter niet is gedefinieerd voor een product, wordt de MAP niet gebruikt.

1. Voor **[!UICONTROL Strike Through Price (MSRP)]** kiest u een optie.

   Standaard is er geen selectie. Deze instelling bepaalt welke prijskenmerk wordt gebruikt als de door de fabrikant voorgestelde detailhandelsprijs (MSRP) voor een product. Als je aanbiedingsprijs lager is dan de gedefinieerde MSRP, wordt je Amazon-aanbieding weergegeven met een doorhaling van de MSRP-prijs met de lagere aanbiedingsprijs, samen met het berekende bedrag en het berekende percentage voor Opslaan. Nochtans, als het geselecteerde het tarief gebied niet voor een product wordt bepaald, wordt MSRP niet berekend.

   >[!NOTE]
   >
   >Deze instelling geldt alleen voor aanbiedingen waarvoor de [Buy Box](./buy-box-competitor-pricing.md) positie. De Buy Box wordt door Amazon toegekend aan de verkoper die het product gewoonlijk tegen de beste prijs heeft aangeboden, samen met andere factoren zoals de FBA/First Shipping, de beschikbaarheid en de prestaties van de verkoper.

1. Voor **BTW toepassen** kiest u een optie:

   - `Disabled` - (Standaard) Kies wanneer je geen BTW op je aanbiedingsprijs wilt toepassen.

   - `Enabled` - Kies wanneer je BTW op je aanbiedingsprijs wilt toepassen. BTW wordt in Europese landen doorgaans als BTW gebruikt en wordt toegevoegd aan de uiteindelijke verkoopprijs in Amazon. BTW is niet van toepassing op de uiteindelijke prijs voor aanbiedingen die binnen een intelligente prijsregel worden gebruikt, tenzij de [bodemprijs](./floor-price.md) is geraakt.

   >[!NOTE]
   >
   >Bedrijven in de Europese Unie (EU) zijn verplicht facturen naar zakelijke kopers te sturen, zodat de klant belasting kan terugbetalen. U kunt deze facturen genereren en de belastingen zelf berekenen of een service voor belastingberekening gebruiken, zoals Amazon Btw Berekening Service. Amazon raadt u aan zich aan te melden voor de [Amazon BTW-berekeningsservice](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;). Als u een andere methode kiest, bent u verantwoordelijk voor de naleving van de BTW.>
   >
   >Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

1. Voor **[!UICONTROL VAT Percentage]**, voer de waarde voor je BTW-tarief in.

   De standaardwaarde is `0.00`. Deze waarde wordt gebruikt om het BTW-bedrag te berekenen dat aan de aanbiedingsprijs moet worden toegevoegd. Indien `10.2` wordt opgegeven. Er wordt een BTW van 10,20% toegepast op de aanbiedingsprijs. Dit veld is uitgeschakeld wanneer het veld BTW toepassen is ingesteld op `Disabled`.

1. **(Alleen Britse winkels)** Voor **[!UICONTROL Amazon Product Tax Code (PTC)]** kiest u een optie:

   - `Do Not Manage PTC` - (Standaardinstelling) Kies of u een service voor de berekening van BTW van derden gebruikt of dat al uw belastingberekeningen al in uw [!DNL Amazon Seller Central] account. Wanneer gekozen, stuurt het verkoopkanaal van Amazon geen gegevens over de productbelastingcode naar je [!DNL Amazon Seller Central] account.

   - `Set Default PTC` - Kies of je een PTC (Universal Product Tax Code) hebt die je voor al je producten wilt gebruiken. Wanneer u kiest, moet u voltooien _[!UICONTROL Default PTC]_.

      - Voor **[!UICONTROL Default PTC]**, voert u de standaard PTC in die moet worden gebruikt voor alle in aanmerking komende Amazon-aanbiedingen. Als uw standaard-PTC is ingesteld in uw [!DNL Amazon Seller Central] account, laat dit veld leeg. Wijzigingen in dit veld hebben geen invloed op bestaande Amazon-aanbiedingen. Als u de standaard-PTC voor een bestaande aanbieding wilt wijzigen, moet de aanbieding [beëindigd](./end-listings-manually.md) en een nieuwe aanbieding gemaakt.

   >[!NOTE]
   >
   >Als je gebruik maakt van de Amazon Btw-berekeningsservice, moet je weten wat de belastingcategorie voor je producten is. Een PTC is de identificatiecode van de belastingcategorie Amazon voor B2B-aankopen in de EU. Zie [Amazon - Productbelastingcodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}.

1. Voor **[!UICONTROL Currency Conversion]** kiest u een optie.

   De standaardwaarde is `Disabled`. Deze opties zijn afhankelijk van uw [!DNL Commerce] [valuta](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) instellingen. Als er geen opties beschikbaar zijn, stelt u de valuta-instellingen in.

1. Klik op **[!UICONTROL Save listing settings]**.

![Aanbiedingsprijs](assets/amazon-listing-price.png){width="500" zoomable="yes"}

| Veld | Beschrijving |
|---------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Magento Price Source] | Hiermee bepaalt u de prijsbron die wordt gebruikt bij het maken van je Amazon-aanbiedingen. De standaardwaarde is `Price`. Als u een ander kenmerk kiest, bijvoorbeeld `Amazon Price` of `Special Price`, wordt de gedefinieerde waarde voor het kenmerk gebruikt voor je Amazon-aanbieding. Als het geselecteerde kenmerk echter niet is gedefinieerd, `Price` wordt gebruikt. |
| [!UICONTROL Minimum Advertised Price (MAP)] | De [!DNL Commerce] kenmerk voor MAP-prijzen. Als je de optie Winkelbasis kiest, wordt je Amazon-aanbieding automatisch ingesteld op de MAP-prijs als de prijs van de aanbieding lager is dan de MAP-prijs. |
| [!UICONTROL Strike Through Price (MSRP)] | De [!DNL Commerce] attribuut dat het tarief MSRP vertegenwoordigt. Als de Amazon-aanbiedingsprijs lager is dan het MSRP, wordt een doorhaling van de MSRP-prijs en de aanbiedingsprijs weergegeven. Deze instelling wordt ook gebruikt om het bedrag en het percentage voor Opslaan te berekenen, maar deze functie is alleen van toepassing op aanbiedingen waarvoor de [Buy Box](./buy-box-competitor-pricing.md) positie. |
| [!UICONTROL Apply Value Added Tax (VAT)] | BTW wordt gebruikt door verkopers in de Europese Unie.<br><br>Kies `Disabled` als je geen BTW wilt toevoegen aan de aanbiedingsprijzen.<br><br>Kies `Enabled` en voer vervolgens het BTW-percentage in voor de toepassing van BTW op je aanbiedingsprijzen. |
| [!UICONTROL VAT Percentage] | Geef het percentage op dat moet worden gebruikt om het BTW-bedrag te berekenen dat aan de aanbiedingsprijs voor je Amazon-aanbiedingen moet worden toegevoegd. <br><br>Als u `5`Vervolgens wordt een BTW van 5% toegepast op de uiteindelijke prijs van de aanbieding nadat alle prijsregels zijn toegepast. BTW is niet van toepassing op de uiteindelijke prijs voor aanbiedingen die binnen een intelligente prijsregel worden gebruikt, tenzij de [verdieping](./floor-price.md) of [maximum](./optional-ceiling-price.md) is geraakt. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Wordt alleen weergegeven voor Britse winkels) Hiermee wordt bepaald of de gegevens van de productbelastingcode door het verkoopkanaal van Amazon naar je worden verzonden [!DNL Amazon Seller Central] account. <br><br>Selecteren **PTC niet beheren** als u een service voor de berekening van BTW van derden gebruikt of al uw belastingberekeningen hebt ingesteld in uw [!DNL Amazon Seller Central] account. Wanneer deze optie is ingeschakeld, stuurt het verkoopkanaal van Amazon geen gegevens over de productbelastingcode naar je [!DNL Amazon Seller Central] account.<br><br>Selecteren **Standaard PTC instellen** als je een universele productbelastingcode hebt, wil je deze gebruiken voor al je producten.<br><br>Zie [Amazon - Productbelastingcodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}. |
| [!UICONTROL Default PTC] | Wordt alleen weergegeven als **Amazon-productbelastingcode (PTC)** is ingesteld op `Set Default PTC`. Voer de standaard PTC in die moet worden gebruikt voor alle in aanmerking komende Amazon-aanbiedingen. Als uw standaard-PTC is ingesteld in uw [!DNL Amazon Seller Central] account, laat dit veld leeg. <br><br>Wijzigingen in dit veld hebben geen invloed op bestaande aanbiedingen. De aanbieding moet [beëindigd](./end-listings-manually.md) en een nieuwe aanbieding die is gemaakt om de wijziging van kracht te laten worden. |
| [!UICONTROL Currency Conversion] | Staat uw [!DNL Commerce] de standaardvaluta van je winkel wijzigen om de standaard Amazon-valuta correct om te zetten om je aanbiedingsprijzen in de juiste valuta te publiceren. De valutaomrekening is altijd gebaseerd op uw [!DNL Commerce] standaardvaluta.<br><br>U kunt de standaardinstelling nog steeds bekijken [!DNL Commerce] en Amazon-valuta&#39;s wanneer andere valuta&#39;s beschikbaar zijn. Als uw standaard [!DNL Commerce] valuta komt overeen met uw standaard Amazon-valuta, valutaconversie uitgeschakeld laten.<br><br>Als uw [!DNL Commerce] De standaardvaluta is CAD (Canadese dollars) en de standaardvaluta van Amazon is USD, moet u Valutaconversie inschakelen en de CAD Conversion Rate CAD naar USD kiezen. De voorgestelde opties zijn gebaseerd op de ingebouwde [!DNL Commerce] valutaomrekeningen. Als u de gewenste optie niet ziet, [de munteenheid in [!DNL Commerce]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html). |

**Snelle toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
