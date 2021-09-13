---
title: Aanbiedingsprijs
description: Gebruik de instellingen voor de aanbiedingsprijs om de prijsbron en de basisprijs (standaardprijs) voor je Amazon-aanbiedingen te bepalen.
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Aanbiedingsprijs

[!UICONTROL Listing Price] Deze instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. Lijstinstellingen zijn toegankelijk via het [opslagdashboard](./amazon-store-dashboard.md).

Met deze instellingen wordt gedefinieerd welk prijskenmerk [!DNL Commerce] moet worden gebruikt als prijsbron. Dit is de basiswaarde (standaardprijs) voor je Amazon-aanbiedingen. Deze instellingen worden door uw [prijsregels](./pricing-rule-general-settings.md) gebruikt om de Amazon-aanbiedingsprijs automatisch aan te passen ten opzichte van de waarde die voor _[!UICONTROL Magento Price Source]_is ingesteld.

U kunt uw [prijsbereik](./price-scope.md) als globaal of website configureren. Als uw prijsbereik is ingesteld op `Global`, is er één prijsbron voor al uw winkels/websites. Als uw prijsbereik is ingesteld op `Website`, gebruikt de prijsbron een fallback-logica voor de websiteprijs (indien beschikbaar), gevolgd door de standaardprijs (global).

Als een aanbiedingsregel is ingesteld om op meer dan één website van toepassing te zijn, wordt de volgorde waarin de websiteprijs wordt gebruikt bepaald door de instelling voor de prioriteit van de website die is gedefinieerd in de [aanbiedingsregel](./listing-rules.md). Met deze regels kunt u productprijzen in de hele catalogus definiëren. Zie [Catalog Price Scope](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){target=&quot;_blank&quot;} om te zien of u het prijsbereik van de website gebruikt.

De opties in _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_, en _[!UICONTROL Strike Through Price (MSRP)]_omvatten uw gevormde het Tarief attributen. Prijskenmerken zijn [!DNL Commerce] productkenmerken met de waarde `Price` voor Invoertype catalogus voor eigenaar van winkel. Zie [Typen kenmerkinvoer](https://docs.magento.com/user-guide/stores/attributes-input-types.html){target=&quot;_blank&quot;}.

## Instellingen voor aanbiedingsprijs configureren {#configure-listing-price-settings}

1. Klik **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Listing Price]_uit.

1. Kies een optie voor **[!UICONTROL Magento Price Source]** (vereist).

   De standaardwaarde is `Price`. Deze instelling bepaalt de prijsbron die wordt gebruikt voor je Amazon-aanbiedingen. Als u [tariferingsregels](./pricing-products.md) creeert, worden de regels toegepast op de waarde die voor de hier geselecteerde attributen wordt bepaald. U kunt om het even welk gevormd prijsattribuut selecteren. Als het geselecteerde kenmerk echter niet is ingevuld voor een product, wordt de prijsbron voor het product standaard teruggezet naar `Price` wanneer prijsregels worden toegepast om de gepubliceerde Amazon-aanbiedingsprijs te bepalen.

1. Kies voor **[!UICONTROL Minimum Advertised Price (MAP)**] een optie.

   Standaard is er geen selectie. Met deze instelling wordt een minimale geadverteerde prijs (MAP) voor een product ingeschakeld. Wanneer je een prijskenmerk definieert en de prijs van je aanbieding voor een product onder de vastgestelde minimumprijs daalt (op basis van je prijsbron en regels), wordt deze waarde de MAP voor de aanbieding. Met deze instelling kunt u [prijsregels](./pricing-products.md) implementeren en tegelijk de minimumprijs voor een product bepalen. Als je wilt voorkomen dat een aanbiedingsprijs te laag is, kies je een prijskenmerk dat je als KAART wilt gebruiken. Als het geselecteerde prijsveld echter niet is gedefinieerd voor een product, wordt de MAP niet gebruikt.

1. Kies voor **[!UICONTROL Strike Through Price (MSRP)]** een optie.

   Standaard is er geen selectie. Deze instelling bepaalt welke prijskenmerk wordt gebruikt als de door de fabrikant voorgestelde detailhandelsprijs (MSRP) voor een product. Als je aanbiedingsprijs lager is dan de gedefinieerde MSRP, wordt je Amazon-aanbieding weergegeven met een doorhaling van de MSRP-prijs met de lagere aanbiedingsprijs, samen met het berekende bedrag en het berekende percentage voor Opslaan. Nochtans, als het geselecteerde het tarief gebied niet voor een product wordt bepaald, wordt MSRP niet berekend.

   >[!NOTE]
   >
   >Deze instelling is alleen van toepassing op aanbiedingen die de positie [Buy Box](./buy-box-competitor-pricing.md) hebben gewonnen. De Buy Box wordt door Amazon toegekend aan de verkoper die het product gewoonlijk tegen de beste prijs heeft aangeboden, samen met andere factoren zoals de FBA/First Shipping, de beschikbaarheid en de prestaties van de verkoper.

1. Kies een optie voor **BTW toepassen**:

   - `Disabled` - (Standaard) Kies wanneer je geen BTW op je aanbiedingsprijs wilt toepassen.

   - `Enabled` - Kies wanneer je BTW op je aanbiedingsprijs wilt toepassen. BTW wordt in Europese landen doorgaans als BTW gebruikt en wordt toegevoegd aan de uiteindelijke verkoopprijs in Amazon. De BTW is niet van toepassing op de uiteindelijke prijs voor aanbiedingen die binnen een intelligente prijsregel worden gebruikt, tenzij de [bodemprijs](./floor-price.md) wordt bereikt.
   >[!NOTE]
   >
   >Bedrijven in de Europese Unie (EU) zijn verplicht facturen naar zakelijke kopers te sturen, zodat de klant belasting kan terugbetalen. U kunt deze facturen genereren en de belastingen zelf berekenen of een service voor belastingberekening gebruiken, zoals Amazon Btw Berekening Service. Amazon raadt u aan zich aan te melden voor de [Amazon VAT-berekeningsservice](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){target=&quot;_blank&quot;}. Als u een andere methode kiest, bent u verantwoordelijk voor de naleving van de BTW.>
   >
   >Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

1. Voer bij **[!UICONTROL VAT Percentage]** de waarde voor uw BTW-tarief in.

   De standaardwaarde is `0.00`. Deze waarde wordt gebruikt om het BTW-bedrag te berekenen dat aan de aanbiedingsprijs moet worden toegevoegd. Als `10.2` wordt ingevoerd, wordt een BTW van 10,20% toegepast op de prijs van je aanbieding. Dit veld is uitgeschakeld wanneer het veld BTW toepassen is ingesteld op `Disabled`.

1. **(Alleen Britse winkels)** Kies voor  **[!UICONTROL Amazon Product Tax Code (PTC)]** een optie:

   - `Do Not Manage PTC` - (Standaardinstelling) Kies of u een service voor de berekening van BTW van derden gebruikt of dat al uw belastingberekeningen al in uw  [!DNL Amazon Seller Central] account zijn ingesteld. Wanneer gekozen, verzendt het verkoopkanaal van Amazon geen informatie van de productbelastingcode naar uw [!DNL Amazon Seller Central] rekening.

   - `Set Default PTC` - Kies of je een PTC (Universal Product Tax Code) hebt die je voor al je producten wilt gebruiken. Wanneer u kiest, moet u _[!UICONTROL Default PTC]_voltooien.

      - Voer bij **[!UICONTROL Default PTC]** de standaard-PTC in die moet worden gebruikt voor alle Amazon-aanbiedingen die hiervoor in aanmerking komen. Laat dit veld leeg als uw standaard-PTC is ingesteld in uw [!DNL Amazon Seller Central]-account. Wijzigingen in dit veld hebben geen invloed op bestaande Amazon-aanbiedingen. Als u de standaard-PTC voor een bestaande aanbieding wilt wijzigen, moet de vermelding [beëindigd](./end-listings-manually.md) zijn en moet een nieuwe aanbieding worden gemaakt.
   >[!NOTE]
   >
   >Als je gebruik maakt van de Amazon Btw-berekeningsservice, moet je weten wat de belastingcategorie voor je producten is. Een PTC is de ID-code van de Amazon-belastingcategorie voor B2B-aankopen in de EU. Zie [Amazon Product Tax Codes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}.

1. Kies voor **[!UICONTROL Currency Conversion]** een optie.

   De standaardwaarde is `Disabled`. Deze opties hangen van uw [!DNL Commerce] [currency](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;} montages af. Als er geen opties beschikbaar zijn, stelt u de valuta-instellingen in.

1. Klik op **[!UICONTROL Save listing settings]** als u klaar bent.

![Aanbiedingsprijs](assets/amazon-listing-price.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Magento Price Source] | Hiermee bepaalt u de prijsbron die wordt gebruikt bij het maken van je Amazon-aanbiedingen. De standaardwaarde is `Price`. Als u een ander kenmerk kiest, zoals `Amazon Price` of `Special Price`, wordt de gedefinieerde waarde voor het kenmerk gebruikt voor de Amazon-aanbieding. Als het geselecteerde kenmerk echter niet is gedefinieerd, wordt `Price` gebruikt. |
| [!UICONTROL Minimum Advertised Price (MAP)] | Het kenmerk [!DNL Commerce] voor MAP-prijzen. Als je de optie Winkelbasis kiest, wordt je Amazon-aanbieding automatisch ingesteld op de MAP-prijs als de prijs van de aanbieding lager is dan de MAP-prijs. |
| [!UICONTROL Strike Through Price (MSRP)] | Het [!DNL Commerce] attribuut dat de prijs MSRP vertegenwoordigt. Als de Amazon-aanbiedingsprijs lager is dan het MSRP, wordt een doorhaling van de MSRP-prijs en de aanbiedingsprijs weergegeven. Deze instelling wordt ook gebruikt om het bedrag en het percentage voor Opslaan in te stellen, maar deze functie is alleen van toepassing op aanbiedingen die de positie [Buy Box](./buy-box-competitor-pricing.md) hebben gewonnen. |
| [!UICONTROL Apply Value Added Tax (VAT)] | BTW wordt gebruikt door verkopers in de Europese Unie.<br><br>Kies  `Disabled` als je geen BTW wilt toevoegen aan de aanbiedingsprijzen.<br><br>Kies  `Enabled` en voer vervolgens het BTW-percentage in voor de toepassing van BTW op je aanbiedingsprijzen. |
| [!UICONTROL VAT Percentage] | Geef het percentage op dat moet worden gebruikt om het BTW-bedrag te berekenen dat aan de aanbiedingsprijs voor je Amazon-aanbiedingen moet worden toegevoegd. <br><br>Als je een object invoert, wordt een BTW van 5% toegepast op de uiteindelijke prijs van de aanbieding nadat alle prijsregels zijn toegepast.  `5` BTW is niet van toepassing op de uiteindelijke prijs voor aanbiedingen die binnen een intelligente prijsregel worden gebruikt, tenzij [floor](./floor-price.md) of [plafonds](./optional-ceiling-price.md) wordt geraakt. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Wordt alleen weergegeven voor winkels in het Verenigd Koninkrijk) Hiermee wordt bepaald of gegevens over de productbelastingcode door Amazon naar uw [!DNL Amazon Seller Central]-account worden verzonden. <br><br>Selecteer  **PTC niet beheren** als u een service voor de berekening van BTW van derden gebruikt of al uw belastingberekeningen al in uw  [!DNL Amazon Seller Central] account hebt ingesteld. Wanneer deze optie is ingeschakeld, stuurt Amazon Sales Channel geen gegevens over de productbelastingcode naar uw [!DNL Amazon Seller Central]-account.<br><br>Selecteer  **Standaard-** PTC instellen als u een universele productbelastingcode hebt die u voor al uw producten wilt gebruiken.<br><br>Zie  [Amazon Product Tax Codes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}. |
| [!UICONTROL Default PTC] | Wordt alleen weergegeven wanneer **Amazon Product Tax Code (PTC)** is ingesteld op `Set Default PTC`. Voer de standaard PTC in die moet worden gebruikt voor alle in aanmerking komende Amazon-aanbiedingen. Laat dit veld leeg als uw standaard-PTC is ingesteld in uw [!DNL Amazon Seller Central]-account. <br><br>Wijzigingen in dit veld hebben geen invloed op bestaande aanbiedingen. De vermelding moet [beëindigd](./end-listings-manually.md) zijn en er moet een nieuwe aanbieding worden gemaakt voordat de wijziging van kracht wordt. |
| [!UICONTROL Currency Conversion] | Hiermee kunt u de standaardvaluta [!DNL Commerce] voor winkelobjecten correct converteren naar de standaard Amazon-valuta om je aanbiedingsprijzen in de juiste valuta te publiceren. De valutaomrekening is altijd gebaseerd op de standaardvaluta [!DNL Commerce].<br><br>Je kunt je standaard  [!DNL Commerce] en Amazon valuta&#39;s nog steeds bekijken wanneer andere valuta&#39;s beschikbaar zijn. Als uw standaard [!DNL Commerce] valuta overeenkomt met uw standaard Amazon valuta, laat u Currency Conversion uitgeschakeld.<br><br>Als uw  [!DNL Commerce] standaardvaluta bijvoorbeeld CAD (Canadese dollars) is en uw Amazon-standaardvaluta USD is, moet u Valutaconversie inschakelen en de optie CAD converteren naar USD kiezen. De gepresenteerde opties zijn gebaseerd op de ingebouwde omrekening van valuta&#39;s [!DNL Commerce]. Als u niet de optie ziet die u zoekt, [opstelling de munt in [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){target=&quot;_blank&quot;}. |

**Snelle toegang**  -  [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
