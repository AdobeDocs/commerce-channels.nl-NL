---
title: Amazon-verkoopkanaal - [!UICONTROL Listing Price]
description: Gebruik de instellingen voor de aanbiedingsprijs om de prijsbron en de basisprijs (standaardprijs) voor je Amazon-aanbiedingen te bepalen.
feature: Sales Channels, Products, Price Rules
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1455'
ht-degree: 0%

---

# [!UICONTROL Listing Price]

[!UICONTROL Listing Price] -instellingen maken deel uit van de aanbiedingsinstellingen van je winkel. De lijsten van montages worden betreden van het [ opslagdashboard ](./amazon-store-dashboard.md).

Met deze instellingen wordt gedefinieerd welk prijskenmerk van [!DNL Commerce] moet worden gebruikt als prijsbron. Dit is de basis-prijswaarde (standaardwaarde) voor je Amazon-aanbiedingen. Deze montages worden gebruikt door uw [ het tarief regels ](./pricing-rule-general-settings.md) om uw Amazon lijstprijs met betrekking tot de waarde automatisch aan te passen die voor _[!UICONTROL Magento Price Source]_wordt geplaatst.

U kunt uw [ tariferingswerkingsgebied ](./price-scope.md) als globaal of website vormen. Als uw prijsbereik is ingesteld op `Global` , is er één prijsbron voor al uw winkels/websites. Als uw prijsbereik is ingesteld op `Website` , gebruikt de prijsbron een fallback-logica van de websiteprijs (indien beschikbaar), gevolgd door de standaardprijs (global).

Als een lijstregel wordt geplaatst om op meer dan één website van toepassing te zijn, wordt de orde waarin de websiteprijs wordt gebruikt bepaald door de website prioritaire die plaatsen in de [ lijstingsregel ](./listing-rules.md) wordt bepaald. Met deze regels kunt u productprijzen in de hele catalogus definiëren. Om te zien of gebruikt u het werkingsgebied van de websiteprijs, zie [ het Toepassingsgebied van de Prijs van de Catalogus ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html).

De opties in _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_ en _[!UICONTROL Strike Through Price (MSRP)]_omvatten uw geconfigureerde prijskenmerken. Prijskenmerken zijn [!DNL Commerce] productkenmerken waarvoor de waarde voor Invoertype catalogus voor Winkeleigenaar is ingesteld op `Price` . Zie [ de Types van Invoer van Attributen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/attributes-input-types.html).

## Instellingen voor aanbiedingsprijs configureren {#configure-listing-price-settings}

1. Klik op **[!UICONTROL Listing Settings]** op het opslagdashboard.

1. Vouw de sectie _[!UICONTROL Listing Price]_uit.

1. Kies een optie bij **[!UICONTROL Magento Price Source]** (vereist).

   De standaardwaarde is `Price` . Deze instelling bepaalt de prijsbron die wordt gebruikt voor je Amazon-aanbiedingen. Als u [ het tarief regels ](./pricing-products.md) creeert, worden de regels toegepast op de waarde die voor de hier geselecteerde attributen wordt bepaald. U kunt om het even welk gevormd prijsattribuut selecteren. Als het geselecteerde kenmerk echter niet is ingevuld voor een product, wordt de prijsbron voor het product standaard teruggezet naar `Price` wanneer prijsregels worden toegepast om de gepubliceerde Amazon-aanbiedingsprijs te bepalen.

1. Voor ** [!UICONTROL Minimum Advertised Price (MAP)**], kies een optie.

   Standaard is er geen selectie. Met deze instelling wordt een minimale geadverteerde prijs (MAP) voor een product ingeschakeld. Wanneer je een prijskenmerk definieert en de prijs van je aanbieding voor een product onder de vastgestelde minimumprijs daalt (op basis van je prijsbron en regels), wordt deze waarde de MAP voor de aanbieding. Dit het plaatsen staat u toe om [ het tarief regels ](./pricing-products.md) uit te voeren, terwijl nog het controleren van uw minimumprijs voor een product. Als je wilt voorkomen dat een aanbiedingsprijs te laag is, kies je een prijskenmerk dat je als KAART wilt gebruiken. Als het geselecteerde prijsveld echter niet is gedefinieerd voor een product, wordt de MAP niet gebruikt.

1. Kies bij **[!UICONTROL Strike Through Price (MSRP)]** een optie.

   Standaard is er geen selectie. Deze instelling bepaalt welke prijskenmerk wordt gebruikt als de door de fabrikant voorgestelde detailhandelsprijs (MSRP) voor een product. Als je aanbiedingsprijs lager is dan de gedefinieerde MSRP, wordt je Amazon-aanbieding weergegeven met een doorhaling van de MSRP-prijs met de lagere aanbiedingsprijs, samen met het berekende bedrag en het berekende percentage voor Opslaan. Nochtans, als het geselecteerde het tarief gebied niet voor een product wordt bepaald, wordt MSRP niet berekend.

   >[!NOTE]
   >
   >Dit het plaatsen is slechts op lijsten van toepassing die de [ Buy Box ](./buy-box-competitor-pricing.md) positie hebben gewonnen. De Buy Box wordt door Amazon toegekend aan de verkoper die het product gewoonlijk tegen de beste prijs heeft aangeboden, samen met andere factoren zoals de FBA/First Shipping, de beschikbaarheid en de prestaties van de verkoper.

1. Voor **pas BTW (BTW) toe**, kies een optie:

   - `Disabled` - (Standaard) Kies wanneer je geen BTW op je aanbiedingsprijs wilt toepassen.

   - `Enabled` - Bepaal wanneer je BTW op je aanbiedingsprijs wilt toepassen. BTW wordt in Europese landen doorgaans als BTW gebruikt en wordt toegevoegd aan de uiteindelijke verkoopprijs in Amazon. De BTW is niet op definitieve prijs voor aanbiedingen van toepassing die binnen een intelligente prijsregel worden gebruikt, tenzij de [ vloerprijs ](./floor-price.md) wordt geraakt.

   >[!NOTE]
   >
   >Bedrijven in de Europese Unie (EU) zijn verplicht facturen naar zakelijke kopers te sturen, zodat de klant belasting kan terugbetalen. U kunt deze facturen genereren en de belastingen zelf berekenen of een service voor belastingberekening gebruiken, zoals Amazon Btw Berekening Service. Amazon adviseert omhoog het ondertekenen voor de [ Dienst van de Berekening van de BTW Amazon ](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;). Als u een andere methode kiest, bent u verantwoordelijk voor de naleving van de BTW.>
   >
   >Het kan 10-14 dagen duren voordat Amazon je rekening voor de BTW-berekeningsservice heeft gecontroleerd en geactiveerd.

1. Voer voor **[!UICONTROL VAT Percentage]** de waarde in voor je BTW-tarief.

   De standaardwaarde is `0.00` . Deze waarde wordt gebruikt om het BTW-bedrag te berekenen dat aan de aanbiedingsprijs moet worden toegevoegd. Als `10.2` wordt ingevoerd, wordt een BTW van 10,20% toegepast op de objectprijs. Dit veld is uitgeschakeld wanneer het veld BTW toepassen is ingesteld op `Disabled` .

1. **(Alleen Britse opslag)** Kies voor **[!UICONTROL Amazon Product Tax Code (PTC)]** een optie:

   - `Do Not Manage PTC` - (Standaard) Kies of u een service voor de berekening van BTW van derden gebruikt of dat al uw belastingberekeningen al zijn ingesteld in uw [!DNL Amazon Seller Central] -account. Als je kiest, stuurt Amazon Verkoopkanaal geen gegevens over de productbelastingcode naar je [!DNL Amazon Seller Central] -account.

   - `Set Default PTC` - Kies of u een PTC (Universal Product Tax Code) hebt die u voor al uw producten wilt gebruiken. Wanneer u kiest, moet u _[!UICONTROL Default PTC]_voltooien.

      - Voer bij **[!UICONTROL Default PTC]** de standaardPTC in die moet worden gebruikt voor alle in aanmerking komende Amazon-aanbiedingen. Laat dit veld leeg als uw standaard-PTC is ingesteld in uw [!DNL Amazon Seller Central] -account. Wijzigingen in dit veld hebben geen invloed op bestaande Amazon-aanbiedingen. Om Standaard PTC voor een bestaande lijst te veranderen, moet de lijst [ gebeëindigd ](./end-listings-manually.md) zijn en een nieuwe gemaakte lijst.

   >[!NOTE]
   >
   >Als je gebruik maakt van de Amazon Btw-berekeningsservice, moet je weten wat de belastingcategorie voor je producten is. Een PTC is de ID-code van de Amazon-belastingcategorie voor B2B-aankopen in de EU. Zie [ de Codes van de Belasting van het Product van Amazon ](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US) {target="_blank"}.

1. Kies bij **[!UICONTROL Currency Conversion]** een optie.

   De standaardwaarde is `Disabled` . Deze opties hangen van uw [!DNL Commerce] [ munt ](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) montages af. Als er geen opties beschikbaar zijn, stelt u de valuta-instellingen in.

1. Klik op **[!UICONTROL Save listing settings]** als de bewerking is voltooid.

![ het Aanbieden Prijs ](assets/amazon-listing-price.png){width="500" zoomable="yes"}

| Veld | Beschrijving |
|---------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Magento Price Source] | Hiermee bepaalt u de prijsbron die wordt gebruikt bij het maken van je Amazon-aanbiedingen. De standaardwaarde is `Price` . Als u een ander kenmerk kiest, zoals `Amazon Price` of `Special Price` , wordt de gedefinieerde waarde voor het kenmerk gebruikt voor de Amazon-aanbieding. Als het geselecteerde kenmerk echter niet is gedefinieerd, wordt `Price` gebruikt. |
| [!UICONTROL Minimum Advertised Price (MAP)] | Het kenmerk [!DNL Commerce] voor MAP-prijzen. Als je de optie Winkelbasis kiest, wordt je Amazon-aanbieding automatisch ingesteld op de MAP-prijs als de prijs van de aanbieding lager is dan de MAP-prijs. |
| [!UICONTROL Strike Through Price (MSRP)] | Het [!DNL Commerce] attribuut dat de prijs MSRP vertegenwoordigt. Als de Amazon-aanbiedingsprijs lager is dan het MSRP, wordt een doorhaling van de MSRP-prijs en de aanbiedingsprijs weergegeven. Dit het plaatsen wordt ook gebruikt om &quot;u te berekenen sparen&quot;hoeveelheid en percentage, maar deze eigenschap is slechts op lijsten van toepassing die de [ Buy Box ](./buy-box-competitor-pricing.md) positie hebben gewonnen. |
| [!UICONTROL Apply Value Added Tax (VAT)] | BTW wordt gebruikt door verkopers in de Europese Unie.<br><br> Kies `Disabled` als je geen BTW wilt toevoegen aan aanbiedingsprijzen.<br><br> Kies `Enabled` en voer vervolgens het BTW-percentage in voor het toepassen van BTW op je aanbiedingsprijzen. |
| [!UICONTROL VAT Percentage] | Geef het percentage op dat moet worden gebruikt om het BTW-bedrag te berekenen dat aan de aanbiedingsprijs voor je Amazon-aanbiedingen moet worden toegevoegd. <br><br> Als je `5` invoert, wordt een BTW van 5% toegepast op de uiteindelijke prijs van de aanbieding nadat alle prijsregels zijn toegepast. De btw is niet op de definitieve prijs voor lijsten van toepassing die binnen een intelligente prijsregel worden gebruikt, tenzij de [ vloer ](./floor-price.md) of [ plafond ](./optional-ceiling-price.md) wordt geraakt. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Wordt alleen weergegeven voor winkels in het Verenigd Koninkrijk) Hiermee wordt bepaald of gegevens over de productbelastingcode door het verkoopkanaal van Amazon naar uw [!DNL Amazon Seller Central] -account worden verzonden. <br><br> Uitgezochte **beheert PTC** niet als u de dienst van de de belastingberekening van de derde gebruikt of reeds al uw belastingberekeningen hebt die in uw [!DNL Amazon Seller Central] rekening worden geplaatst. Wanneer deze optie is ingeschakeld, stuurt Amazon Sales Channel geen gegevens over de productbelastingcode naar uw [!DNL Amazon Seller Central] -account.<br><br> Uitgezochte **Vastgestelde StandaardPTC** als u een universele code van de productbelasting hebt u voor al uw producten wilt gebruiken.<br><br> zie [ Codes van de Belasting van het Product van Amazon ](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US) {target="_blank"}. |
| [!UICONTROL Default PTC] | Slechts verschijnt wanneer **de Code van de Belasting van het Product van Amazon (PTC)** aan `Set Default PTC` wordt geplaatst. Voer de standaard-PTC in die moet worden gebruikt voor alle in aanmerking komende Amazon-aanbiedingen. Laat dit veld leeg als uw standaard-PTC is ingesteld in uw [!DNL Amazon Seller Central] -account. <br><br> de veranderingen die aan dit gebied worden aangebracht beïnvloeden geen bestaande lijsten. De lijst moet [ gebeëindigd ](./end-listings-manually.md) zijn en een nieuwe lijst die voor de verandering wordt gecreeerd om van kracht te worden. |
| [!UICONTROL Currency Conversion] | Met de standaardvaluta van je [!DNL Commerce] winkel kun je je aanbiedingsprijzen op de juiste manier in Amazon converteren naar de standaardvaluta. De valutaomrekening is altijd gebaseerd op de standaardvaluta van [!DNL Commerce] .<br><br> u kunt nog uw gebrek [!DNL Commerce] bekijken en de valuta van Amazon wanneer andere valuta&#39;s beschikbaar zijn. Als uw standaard [!DNL Commerce] -valuta overeenkomt met uw standaard Amazon-valuta, laat u Currency Conversion uitgeschakeld.<br><br> Bijvoorbeeld, als uw [!DNL Commerce] standaardmunt CAD (Canadese dollars) is en uw Amazon standaardmunt USD is, moet u de Omzetting van de Valuta toelaten en de CAD van het Tarief van de Omzetting kiezen aan USD. De weergegeven opties zijn gebaseerd op de ingebouwde [!DNL Commerce] valutaomrekeningen. Als u niet de optie ziet die u zoekt, [ opstelling de munt in  [!DNL Commerce] ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html). |

**Snelle Toegang** - [!UICONTROL Listing Settings] secties

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
