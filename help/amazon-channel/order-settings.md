---
title: Orderinstellingen
description: Gebruik de Orde-instellingen om te bepalen hoe Amazon-orders worden geïmporteerd in en verwerkt in uw Commerce-winkel.
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Orderinstellingen

De instellingen voor Volgorde bepalen of en hoe Amazon-orders worden geïmporteerd in en verwerkt in [!DNL Commerce] en kunnen worden geopend op het [opslagdashboard](./amazon-store-dashboard.md).

De instellingen voor het importeren van bestellingen worden standaard ingesteld op `Enabled`. Dit betekent dat uw Amazon-bestellingen op het opslagdashboard worden weergegeven en corresponderende [!DNL Commerce]-bestellingen worden gemaakt. Geïmporteerde orders kunnen worden beheerd in de [!DNL Commerce] [Bestellingen](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} workflow.

>[!NOTE]
>
>Ongeacht de instellingen van uw bestelling worden Amazon-bestellingen die vóór de integratie van uw winkel bestonden, niet geïmporteerd.

Nadat [store integration](./store-integration.md) volledig is, kunt u uw ordemontages veranderen. Als u de instellingen voor uw bestelling instelt op `Disabled`, worden Amazon-bestellingen weergegeven op het opslagdashboard, maar moeten deze worden beheerd in uw [!DNL Amazon Seller Central]-account.

Wanneer een orde op Amazon wordt gecreeerd, wordt het niet onmiddellijk ingevoerd in [!DNL Commerce]. Amazon wijst de status `Pending` toe aan nieuwe bestellingen. Nadat Amazon de bestelling en de betalingsmethode heeft geverifieerd, wordt de status van de bestelling gewijzigd in `Unshipped`. Deze statuswijziging activeert de order die wordt geïmporteerd en [!DNL Commerce] maakt een overeenkomende, overeenkomende volgorde.

Uit Amazon geïmporteerde bestellingen kunnen worden beheerd in de [!DNL Commerce] [workflow voor bestellingen](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}. Zie ook [Bestellingen beheren](./managing-orders.md).

## Orderinstellingen configureren {#configure-order-settings}

1. Klik **[!UICONTROL Order Settings]** op het opslagdashboard.

1. Kies voor **[!UICONTROL Import Amazon Orders]** (vereist) een optie:

   - `Disabled` - Kies wanneer u geen corresponderende bestellingen wilt maken  [!DNL Commerce] wanneer u nieuwe bestellingen ontvangt van Amazon. Als u deze optie kiest, worden alle andere velden op deze pagina uitgeschakeld.

   - `Enabled` - (Standaard) Kies wanneer u corresponderende  [!DNL Commerce] bestellingen wilt maken wanneer u nieuwe bestellingen ontvangt van Amazon. [!DNL Commerce] bestellingen worden aangemaakt op basis van Amazon-status en aandelenniveaus.

      >[!NOTE]
      >
      >Amazon-orders voor importeren moeten worden ingesteld op `Enabled` om Amazon-orders te beheren in de [!DNL Commerce] [orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} workflow. Als u de waarde `Disabled` hebt, hebben uw Amazon-bestellingen geen corresponderend [!DNL Commerce]-ordernummer en kunnen deze niet worden beheerd in [!DNL Commerce]. U beheert deze bestellingen in uw [!DNL Amazon Seller Central]-account.

1. Kies bij **[!UICONTROL Import Amazon Orders Into Magento Store]** aan welke [!DNL Commerce] de Amazon-orders moeten worden gekoppeld wanneer de corresponderende volgorde wordt gemaakt in [!DNL Commerce].

   Deze instelling wordt standaard ingesteld op Winkelweergave voor de geselecteerde website wanneer u [de Amazon-winkel](./store-integration.md) hebt toegevoegd. Als u deze instelling wilt wijzigen, is de lijst met opties afhankelijk van de [!DNL Commerce]-opslaginstellingen die u in uw configuratie hebt ingesteld. Zie [Opslag](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){:target=&quot;_blank&quot;}.

1. Kies voor **[!UICONTROL Customer Creation]** een optie:

   - `No Customer Creation (guest)` - (Standaard) Kies wanneer u geen klantenaccount wilt maken  [!DNL Commerce] met de geïmporteerde klantgegevens in de Amazon-volgorde. Als u [!DNL Commerce] kiest, wordt een geïmporteerde Amazon-bestelling op dezelfde manier verwerkt als een uitcheckbewerking voor gasten in [!DNL Commerce].

   - `Build New Customer Account` - Kies wanneer u een nieuwe klantenaccount wilt maken  [!DNL Commerce] met de klantgegevens die met de Amazon-bestelling zijn geïmporteerd. Met deze optie kunt u uw klantendatabase samenstellen op basis van uw Amazon-bestellingen.

1. Kies voor **[!UICONTROL Order Number Source]** een optie:

   - `Build Using Magento Order Number` - (Standaard) Kies wanneer u een uniek  [!DNL Commerce] ordernummer voor de bijbehorende Amazon-volgorde wilt maken met de  [!DNL Commerce] incrementeel toegewezen bestellings-id.

   - `Build Using Amazon Order Number` - Kies wanneer u het  [!DNL Commerce] ordernummer wilt maken met het corresponderende door Amazon toegewezen volgnummer.
   >[!NOTE]
   >
   >Nadat een orde wordt ingevoerd, toont het de ordeaantal van Amazon in _[!UICONTROL Recent Orders]_lijst op het opslagdashboard. Het ordernummer [!DNL Commerce] wordt weergegeven wanneer de ordergegevens worden weergegeven in de werkruimte [!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}.

1. Kies voor **[!UICONTROL Order Status]** (vereist) een optie:

   - `Default Order Status` - (Standaardinstelling) Kies wanneer u wilt dat aan nieuw gemaakte bestellingen die u uit Amazon hebt geïmporteerd, de standaardvolgordestatus voor nieuwe bestellingen wordt toegewezen. De standaardstatus voor nieuwe orders (tenzij u een aangepaste orderstatus voor nieuwe orders hebt gemaakt) is `Pending`. Zie [Verwerkingsopdrachten](https://docs.magento.com/user-guide/sales/order-processing.html){:target=&quot;_blank&quot;}.

   - `Custom Order Status` - Kies wanneer u wilt dat nieuwe orders die u uit Amazon hebt geïmporteerd, een andere status krijgen dan de standaardstatus.

   - `Processing Order Status` - Ingeschakeld wanneer  **[!UICONTROL Order Status]** deze is ingesteld op  `Custom Order Status`. Kies de status die u wilt gebruiken voor nieuwe bestellingen die uit Amazon zijn geïmporteerd. De opties in dit gebied zijn gebaseerd op de standaardstatusopties in [!DNL Commerce]. Zie [Status van bestelling](https://docs.magento.com/user-guide/sales/order-status.html). U kunt ook een aangepaste orderstatus maken die hier voor selectie wordt weergegeven. Zie [Status aangepaste volgorde](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;} om een aangepaste orderstatus te maken.

1. Klik op **[!UICONTROL Save order settings]** als u klaar bent.

![Orderinstellingen](assets/amazon-order-settings.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Import Amazon Orders] | Opties:<ul><li>**[!UICONTROL Disabled]** - Kies wanneer u geen corresponderende bestellingen wilt maken  [!DNL Commerce] wanneer u nieuwe bestellingen ontvangt van Amazon. Als u deze optie kiest, worden alle andere velden op deze pagina uitgeschakeld.</li><li>**[!UICONTROL Enabled]** - (Standaard) Kies wanneer u corresponderende  [!DNL Commerce] bestellingen wilt maken wanneer u nieuwe bestellingen ontvangt van Amazon. [!DNL Commerce] bestellingen worden aangemaakt op basis van Amazon-status en aandelenniveaus.</li></ul><br><br>`Enabled` moet worden gekozen voor het beheren van Amazon-bestellingen in  [!DNL Commerce]. Wanneer `Disabled` wordt gekozen, worden uw Amazon-bestellingen weergegeven op het opslagdashboard, maar moeten de bestellingen worden beheerd in uw [!DNL Amazon Seller Central]-account. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Kies aan welke [!DNL Commerce] de Amazon-orders moeten worden gekoppeld wanneer ze worden gemaakt in de werkruimte [!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}. Deze instelling wordt standaard ingesteld op Winkelweergave voor de [!DNL Commerce]-website die is geselecteerd wanneer u de Amazon-winkel [toevoegt. ](./store-integration.md) Als u deze instelling wilt wijzigen, is de lijst met opties afhankelijk van de [!DNL Commerce]-opslaginstellingen die u in uw configuratie hebt ingesteld. Zie [Opslag](https://docs.magento.com/user-guide/stores/stores-all-stores.html){:target=&quot;_blank&quot;}. |
| [!UICONTROL Customer Creation] | Opties:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Standaard) Kies wanneer u geen klantenaccount wilt maken  [!DNL Commerce] met de geïmporteerde klantgegevens in de Amazon-volgorde. Als u deze optie kiest, wordt [!DNL Commerce] gevraagd een geïmporteerde Amazon-bestelling op dezelfde manier te verwerken als een uitcheckbewerking voor gasten.</li><li>**[!UICONTROL Build New Customer Account]** - Kies wanneer u een nieuwe klantenaccount in uw  [!DNL Commerce] klantendatabase wilt maken met de klantgegevens die u met de Amazon-order hebt geïmporteerd. Met deze optie kunt u uw [!DNL Commerce]-klantendatabase samenstellen op basis van uw Amazon-bestellingen.</li></ul> |
| Bron van ordernummer | Opties:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Standaard) Kies wanneer u een uniek  [!DNL Commerce] ordernummer voor de bijbehorende Amazon-volgorde wilt maken met de  [!DNL Commerce] incrementeel toegewezen bestellings-id. </li><li>**Build Using Amazon Order Number**  - Kies wanneer u het  [!DNL Commerce] ordernummer wilt maken met het corresponderende door Amazon toegewezen ordernummer.</li></ul> |
| In behandeling zijnde bestellingen | Opties:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Kies wanneer je niet wilt dat het  [!DNL Commerce] voorraadaantal wordt beïnvloed door je Amazon-bestellingen. Kies of u Amazon gebruikt voor uw uitvoeringsproces (FBA). Wanneer u een Amazon-bestelling hebt gekozen, heeft de bestelde hoeveelheid geen invloed op uw [!DNL Commerce]-voorraadhoeveelheid.</li><li>**[!UICONTROL Reserve Quantity]** - Kies wanneer u het orderaantal in de Amazon-volgorde wilt &#39;gereserveerd&#39; in het aantal  [!DNL Commerce] aandelen. Wanneer u een Amazon-bestelling hebt gekozen, wordt de bestelde hoeveelheid in uw [!DNL Commerce] voorraadhoeveelheid &quot;gereserveerd&quot; om te voorkomen dat uw [!DNL Commerce]-voorraad &quot;te koop&quot; wordt. De &quot;gereserveerde&quot; hoeveelheid kan niet worden aangeschaft via uw [!DNL Commerce] winkel.</li></ul> |
| [!UICONTROL Order Status] | Opties:<ul><li>**[!UICONTROL Default Order Status]** - (Standaardinstelling) Kies wanneer u wilt dat aan nieuw gemaakte bestellingen die u uit Amazon hebt geïmporteerd, de status van de standaardvolgorde wordt toegewezen voor nieuwe bestellingen. De standaardstatus voor nieuwe orders (tenzij u een aangepaste orderstatus voor nieuwe orders hebt gemaakt) is `Pending`. Zie [Verwerkingsopdrachten](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]** - Kies wanneer u wilt dat nieuwe orders die uit Amazon zijn geïmporteerd een andere status krijgen dan de standaardstatus. Als u **[!UICONTROL Processing Order Status]** kiest, kunt u de status kiezen die u wilt gebruiken voor nieuw gemaakte bestellingen die uit Amazon zijn geïmporteerd.</li></ul> |
| [!UICONTROL Processing Orders Status] | Wordt ingeschakeld wanneer _[!UICONTROL Order Status]_is ingesteld op `Custom Order Status`. Kies de orderstatus die u wilt toewijzen aan nieuwe bestellingen. De opties in dit gebied hangen van de standaardstatusopties in [!DNL Commerce] af. Zie [Order Status](https://docs.magento.com/user-guide/sales/order-status.html){:target=&quot;_blank&quot;}. U kunt ook een aangepaste orderstatus maken die hier wordt weergegeven. Zie [Status aangepaste volgorde](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;} om een aangepaste orderstatus te maken. |

## [!DNL Commerce] bestellen

[!DNL Commerce] voor Amazon-bestellingen worden bestellingen gemaakt op basis van de volgende status en inventarisvoorwaarden.

### Maken van bestellingen met inventarisbeheer

>[!NOTE]
>
>Alleen ondersteund in Adobe Commerce- en Magento Open Source 2.3.x-integratie.

| Afuitvoeringskanaal | [!DNL Commerce] Inventarisstatus | Status Amazon-bestelling | [!UICONTROL Create Magento Order] Instelling | Voorraad gereserveerd |
|---|---|---|---|---|
| FBA | In stock<br>Out-of-stock<br>Niet beheren | In behandeling | Nee | Nee |
| FBA | In stock<br>Out-of-stock<br>Niet beheren | PendingAvailability | Nee | Nee |
| FBA | In stock<br>Out-of-stock<br>Niet beheren | Geannuleerd | Nee | Nee |
| FBA | In stock<br>Out-of-stock<br>Niet beheren | Fout | Nee | Nee |
| FBA | In stock<br>Out-of-stock<br>Niet beheren | Niet verscheept | Nee | Nee |
| FBA | In stock<br>Out-of-stock<br>Niet beheren | GedeeltelijkVerzonden | Nee | Nee |
| FBA | In stock<br>Niet beheren | Verzonden | Ja | Nee |
| FBA | Buiten de voorraad | Verzonden | Nee | Nee |
| FBM | In stock<br>Out-of-stock<br>Niet beheren | In behandeling | Nee | Nee |
| FBM | In stock<br>Out-of-stock<br>Niet beheren | PendingAvailability | Nee | Nee |
| FBM | In stock<br>Out-of-stock<br>Niet beheren | Geannuleerd | Nee | Nee |
| FBM | In stock<br>Out-of-stock<br>Niet beheren | Fout | Nee | Nee |
| FBM | In stock<br>Niet beheren | Niet verscheept | Ja | Ja |
| FBM | Buiten de voorraad | Niet verscheept | Nee | Nee |
| FBM | In stock<br>Niet beheren | GedeeltelijkVerzonden | Ja | Ja |
| FBM | Buiten de voorraad | GedeeltelijkVerzonden | Nee | Nee |
| FBM | In stock<br>Niet beheren | Verzonden | Ja | Ja |
| FBM | Buiten de voorraad | Verzonden | Nee | Nee |

>[!NOTE]
>Als een Amazon-bestelling wordt geïmporteerd in de status `Partially Shipped` of `Shipped`, geldt de voorraadboeking die wordt gemaakt voor alle items in de bestelling. Amazon biedt geen compensatie voor objecten die eerder zijn verzonden.
>
>Als een bestelling wordt vervuld door Amazon (FBA) maar een item de status `out of stock` heeft, kan [!DNL Commerce] geen corresponderende bestelling maken. Dit is een beperking van de integratie van voorraadbeheer.
