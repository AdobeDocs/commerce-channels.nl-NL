---
title: Amazon-orderinstellingen
description: Gebruik de Orde-instellingen om te bepalen hoe Amazon-bestellingen worden geïmporteerd in en verwerkt in uw Commerce-winkel.
feature: Sales Channels, Orders, Inventory, Configuration
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: a93ba31a95f32cc6ea285aed2399255021985693
workflow-type: tm+mt
source-wordcount: '1388'
ht-degree: 0%

---

# Amazon-orderinstellingen

De montages van de orde bepalen als en hoe de orden van Amazon in worden ingevoerd en in [!DNL Commerce] worden verwerkt en op het [ opslagdashboard ](./amazon-store-dashboard.md) kunnen worden betreden.

De instellingen voor het importeren van bestellingen worden standaard ingesteld op `Enabled` . Dit betekent dat uw Amazon-bestellingen worden weergegeven op het opslagdashboard en dat er corresponderende [!DNL Commerce] -bestellingen worden gemaakt. De ingevoerde orden kunnen in het [!DNL Commerce] [ Orders ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) werkschema worden beheerd.

>[!NOTE]
>
>Ongeacht de instellingen van uw bestelling worden Amazon-bestellingen die vóór de integratie van uw winkel bestonden, niet geïmporteerd.

Nadat [ opslagintegratie ](./store-integration.md) volledig is, kunt u uw ordemontages veranderen. Als u de instellingen voor uw bestelling instelt op `Disabled` , worden Amazon-bestellingen weergegeven op het opslagdashboard, maar moeten ze worden beheerd in uw [!DNL Amazon Seller Central] -account.

Wanneer een bestelling wordt gemaakt op Amazon, wordt deze niet onmiddellijk geïmporteerd in [!DNL Commerce] . Amazon wijst de status `Pending` toe aan nieuwe bestellingen. Nadat Amazon de bestelling en de betalingsmethode heeft geverifieerd, wordt de status van de bestelling gewijzigd in `Unshipped` . Deze statuswijziging activeert het importeren van de order en [!DNL Commerce] maakt een overeenkomende, overeenkomende volgorde.

De orden die van Amazon worden ingevoerd kunnen in het [!DNL Commerce] [ werkschema van orden ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) worden beheerd. Zie ook [ Orden beheren ](./managing-orders.md).

## Orderinstellingen configureren {#configure-order-settings}

1. Klik op **[!UICONTROL Order Settings]** op het opslagdashboard.

1. Kies bij **[!UICONTROL Import Amazon Orders]** (vereist) een optie:

   - `Disabled` - Kies wanneer u geen corresponderende bestellingen wilt maken in [!DNL Commerce] wanneer nieuwe bestellingen worden ontvangen van Amazon. Als u deze optie kiest, worden alle andere velden op deze pagina uitgeschakeld.

   - `Enabled` - (Standaard) Kies wanneer u corresponderende [!DNL Commerce] -bestellingen wilt maken wanneer nieuwe bestellingen worden ontvangen van Amazon. [!DNL Commerce] -orders worden gemaakt op basis van Amazon-status en -voorraadniveaus.

     >[!NOTE]
     >
     >De Orden van Amazon van de invoer moeten aan `Enabled` worden geplaatst om de orden van Amazon in het [!DNL Commerce] [ orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) werkschema te beheren. Als u deze instelt op `Disabled` , hebben uw Amazon-bestellingen geen corresponderend [!DNL Commerce] ordernummer en kunnen deze niet worden beheerd in [!DNL Commerce] . U beheert deze bestellingen in uw [!DNL Amazon Seller Central] -account.

1. Kies bij **[!UICONTROL Import Amazon Orders Into Magento Store]** met welke [!DNL Commerce] de Amazon-bestellingen worden opgeslagen wanneer de corresponderende volgorde wordt gemaakt in [!DNL Commerce] .

   Dit het plaatsen blijft aan de Mening van de Opslag voor de geselecteerde website in gebreke wanneer u [ de opslag van Amazon ](./store-integration.md) toevoegde. Als u deze instelling wilt wijzigen, is de lijst met opties afhankelijk van de opslaginstellingen die u in de configuratie hebt ingesteld in [!DNL Commerce] . Zie [ Sporen ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html).

1. Kies bij **[!UICONTROL Customer Creation]** een optie:

   - `No Customer Creation (guest)` - (Standaard) Kies wanneer u geen klantenaccount wilt maken in [!DNL Commerce] met behulp van de geïmporteerde klantgegevens uit de Amazon-volgorde. Als u [!DNL Commerce] kiest, wordt een geïmporteerde Amazon-bestelling op dezelfde manier verwerkt als een uitcheckbewerking voor gasten in [!DNL Commerce] .

   - `Build New Customer Account` - Kies wanneer u een nieuwe klantenaccount wilt maken in [!DNL Commerce] met de klantgegevens die u met de Amazon-volgorde hebt geïmporteerd. Met deze optie kunt u uw klantendatabase samenstellen op basis van uw Amazon-bestellingen.

1. Kies bij **[!UICONTROL Order Number Source]** een optie:

   - `Build Using Magento Order Number` - (Standaard) Kies wanneer u een uniek [!DNL Commerce] volgnummer wilt maken voor de corresponderende Amazon-volgorde met de [!DNL Commerce] incrementeel toegewezen volgorde-id.

   - `Build Using Amazon Order Number` - Kies wanneer u het [!DNL Commerce] -ordernummer wilt maken met het corresponderende door Amazon toegewezen ordernummer.

   >[!NOTE]
   >
   >Nadat een bestelling is geïmporteerd, wordt het Amazon-ordernummer weergegeven in de lijst _[!UICONTROL Recent Orders]_op het winkeldashboard. Het [!DNL Commerce] orderaantal toont wanneer het bekijken van de ordedetails in de [!DNL Commerce] [ 3} werkruimte van Orden {.](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)

1. Kies bij **[!UICONTROL Order Status]** (vereist) een optie:

   - `Default Order Status` - (Standaard) Kies wanneer u de status van de standaardvolgorde voor nieuwe bestellingen wilt toewijzen aan nieuw gemaakte bestellingen die u uit Amazon hebt geïmporteerd. De standaardstatus voor nieuwe bestellingen (tenzij u een aangepaste orderstatus voor nieuwe bestellingen hebt gemaakt) is `Pending` . Zie [ Orden van de Verwerking ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

   - `Custom Order Status` - Kies wanneer u wilt dat nieuwe orders die u uit Amazon hebt geïmporteerd, een andere status krijgen dan de standaardstatus.

   - `Processing Order Status` - Ingeschakeld wanneer **[!UICONTROL Order Status]** is ingesteld op `Custom Order Status` . Kies de status die u wilt gebruiken voor nieuwe bestellingen die uit Amazon zijn geïmporteerd. De opties in dit veld zijn gebaseerd op de standaardopties voor de status in [!DNL Commerce] . Zie [ Status van de Orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). U kunt ook een aangepaste orderstatus maken die hier voor selectie wordt weergegeven. Om een status van de douaneorde tot stand te brengen, zie [ Status van de Orde van de Douane ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html#custom-order-status).

1. Klik op **[!UICONTROL Save order settings]** als de bewerking is voltooid.

![ de montages van de Orde ](assets/amazon-order-settings.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | Opties:<ul><li>**[!UICONTROL Disabled]** - Kies wanneer u geen corresponderende bestellingen wilt maken in [!DNL Commerce] wanneer nieuwe bestellingen worden ontvangen van Amazon. Als u deze optie kiest, worden alle andere velden op deze pagina uitgeschakeld.</li><li>**[!UICONTROL Enabled]** - (Standaard) Kies wanneer u corresponderende [!DNL Commerce] -bestellingen wilt maken wanneer nieuwe bestellingen worden ontvangen van Amazon. [!DNL Commerce] -orders worden gemaakt op basis van Amazon-status en -voorraadniveaus.</li></ul><br><br>`Enabled` moet worden gekozen om Amazon-orders te beheren in [!DNL Commerce] . Wanneer `Disabled` wordt gekozen, worden uw Amazon-bestellingen weergegeven op het opslagdashboard, maar moeten de bestellingen worden beheerd in uw [!DNL Amazon Seller Central] -account. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Kies welke [!DNL Commerce] opslag de orden van Amazon worden geassocieerd met wanneer zij in de [!DNL Commerce] [ 3} werkruimte van Orden {worden gecreeerd. ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Dit plaatsen blijft aan de Mening van de Opslag voor de [!DNL Commerce] geselecteerde website in gebreke wanneer u [ de opslag van Amazon ](./store-integration.md) toevoegde. Als u deze instelling wilt wijzigen, is de lijst met opties afhankelijk van de opslaginstellingen die u in de configuratie hebt ingesteld in [!DNL Commerce] . Zie [ Sporen ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html). |
| [!UICONTROL Customer Creation] | Opties:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Standaard) Kies wanneer u geen klantenaccount wilt maken in [!DNL Commerce] met behulp van de geïmporteerde klantgegevens uit de Amazon-volgorde. Als u deze optie kiest, geeft [!DNL Commerce] de opdracht een geïmporteerde Amazon-bestelling op dezelfde manier te verwerken als een uitcheckbewerking voor gasten.</li><li>**[!UICONTROL Build New Customer Account]** - Kies wanneer u een nieuwe klantenaccount wilt maken in uw [!DNL Commerce] -klantdatabase met de klantgegevens die u met de Amazon-order hebt geïmporteerd. Met deze optie kunt u uw [!DNL Commerce] -klantdatabase samenstellen op basis van uw Amazon-bestellingen.</li></ul> |
| Order Number Source | Opties:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Standaard) Kies wanneer u een uniek [!DNL Commerce] volgnummer wilt maken voor de corresponderende Amazon-volgorde met de [!DNL Commerce] incrementeel toegewezen volgorde-id. </li><li>**bouwt het Gebruiken van het Aantal van de Orde van Amazon** - verkies wanneer u het [!DNL Commerce] ordeaantal wilt creëren gebruikend het overeenkomstige Amazon-Toegewezen orderaantal.</li></ul> |
| In behandeling zijnde bestellingen | Opties:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Kies wanneer u niet wilt dat het [!DNL Commerce] -voorraadaantal wordt beïnvloed door uw Amazon-bestellingen. Kies of u Amazon gebruikt voor uw uitvoeringsproces (FBA). Als je kiest en je ontvangt een Amazon-bestelling, heeft de bestelde hoeveelheid geen invloed op de hoeveelheid van je [!DNL Commerce] voorraad.</li><li>**[!UICONTROL Reserve Quantity]** - Kies wanneer u het orderaantal in de Amazon-volgorde wilt &#39;gereserveerd&#39; in uw [!DNL Commerce] -voorraad. Als je kiest en je ontvangt een Amazon-bestelling, wordt de bestelde hoeveelheid in je [!DNL Commerce] voorraad &#39;gereserveerd&#39; om te voorkomen dat je [!DNL Commerce] -voorraad te veel verkoopt. Het gereserveerde aantal is niet beschikbaar voor aankoop via uw [!DNL Commerce] winkel.</li></ul> |
| [!UICONTROL Order Status] | Opties:<ul><li>**[!UICONTROL Default Order Status]** - (Standaard) Kies wanneer u de status van de standaardvolgorde voor nieuwe bestellingen wilt toewijzen aan nieuw gemaakte bestellingen die u wilt importeren uit Amazon. De standaardstatus voor nieuwe bestellingen (tenzij u een aangepaste orderstatus voor nieuwe bestellingen hebt gemaakt) is `Pending` . Zie [ Orden van de Verwerking ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).</li><li>**[!UICONTROL Custom Order Status]** - Kies wanneer u wilt dat nieuwe orders die u uit Amazon hebt geïmporteerd, een andere status krijgen dan de standaardstatus. Als u **[!UICONTROL Processing Order Status]** kiest, kunt u de status kiezen die u wilt gebruiken voor nieuwe bestellingen die u uit Amazon hebt geïmporteerd.</li></ul> |
| [!UICONTROL Processing Orders Status] | Wordt ingeschakeld wanneer _[!UICONTROL Order Status]_is ingesteld op `Custom Order Status` . Kies de orderstatus die u wilt toewijzen aan nieuwe bestellingen. De opties in dit veld zijn afhankelijk van de standaardopties voor de status in [!DNL Commerce] . Zie [ Status van de Orde ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). U kunt ook een aangepaste orderstatus maken die hier wordt weergegeven. Om een status van de douaneorde tot stand te brengen, zie [ Status van de Orde van de Douane ] |

## [!DNL Commerce] bestellen

[!DNL Commerce] -orders worden gemaakt voor Amazon-orders op basis van de volgende status en inventarisvoorwaarden.

### Maken van bestellingen met Inventory management

>[!NOTE]
>
>Alleen ondersteund in Adobe Commerce en Magento Open Source 2.3.x-integratie.

| Afuitvoeringskanaal | [!DNL Commerce] Inventarisstatus | Status Amazon-bestelling | [!UICONTROL Create Magento Order] Instelling | Voorraad gereserveerd |
|---------------------|-------------------------------------------|---------------------|-------------------------------------------|--------------------|
| FBA | In-voorraad <br> uit-van-voorraad <br> leidt niet | In behandeling | Nee | Nee |
| FBA | In-voorraad <br> uit-van-voorraad <br> leidt niet | PendingAvailability | Nee | Nee |
| FBA | In-voorraad <br> uit-van-voorraad <br> leidt niet | Geannuleerd | Nee | Nee |
| FBA | In-voorraad <br> uit-van-voorraad <br> leidt niet | Fout | Nee | Nee |
| FBA | In-voorraad <br> uit-van-voorraad <br> leidt niet | Niet verscheept | Nee | Nee |
| FBA | In-voorraad <br> uit-van-voorraad <br> leidt niet | GedeeltelijkVerzonden | Nee | Nee |
| FBA | In voorraad <br> beheert niet | Verzonden | Ja | Nee |
| FBA | Buiten de voorraad | Verzonden | Nee | Nee |
| FBM | In-voorraad <br> uit-van-voorraad <br> leidt niet | In behandeling | Nee | Nee |
| FBM | In-voorraad <br> uit-van-voorraad <br> leidt niet | PendingAvailability | Nee | Nee |
| FBM | In-voorraad <br> uit-van-voorraad <br> leidt niet | Geannuleerd | Nee | Nee |
| FBM | In-voorraad <br> uit-van-voorraad <br> leidt niet | Fout | Nee | Nee |
| FBM | In voorraad <br> beheert niet | Niet verscheept | Ja | Ja |
| FBM | Buiten de voorraad | Niet verscheept | Nee | Nee |
| FBM | In voorraad <br> beheert niet | GedeeltelijkVerzonden | Ja | Ja |
| FBM | Buiten de voorraad | GedeeltelijkVerzonden | Nee | Nee |
| FBM | In voorraad <br> beheert niet | Verzonden | Ja | Ja |
| FBM | Buiten de voorraad | Verzonden | Nee | Nee |

>[!NOTE]
>Als een Amazon-bestelling wordt geïmporteerd in de status `Partially Shipped` of `Shipped` , geldt de voorraadboeking die wordt gemaakt voor alle items in de bestelling. Amazon biedt geen compensatie voor objecten die eerder zijn verzonden.
>
>Als een bestelling wordt uitgevoerd door Amazon (FBA) maar een item de status `out of stock` heeft, kan [!DNL Commerce] geen corresponderende volgorde maken. Dit is een beperking van de integratie van Inventory management.
