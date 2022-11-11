---
title: Orderinstellingen
description: Gebruik de Orde-instellingen om te bepalen hoe Amazon-orders worden geïmporteerd in en verwerkt in uw Commerce-winkel.
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Orderinstellingen

De instellingen voor bestellingen bepalen of en hoe Amazon-bestellingen worden geïmporteerd in en verwerkt in [!DNL Commerce] en kan worden geraadpleegd op de [opslagdashboard](./amazon-store-dashboard.md).

De instellingen voor het importeren van de volgorde zijn ingesteld op `Enabled` standaard, wat betekent dat uw Amazon-bestellingen worden weergegeven op het opslagdashboard en dat de bijbehorende bestellingen worden gemaakt [!DNL Commerce] bestellingen. Geïmporteerde orders kunnen worden beheerd in het dialoogvenster [!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} workflow.

>[!NOTE]
>
>Ongeacht de instellingen van uw bestelling worden Amazon-bestellingen die vóór de integratie van uw winkel bestonden, niet geïmporteerd.

Na [winkelintegratie](./store-integration.md) is voltooid, kunt u de instellingen voor uw bestelling wijzigen. Als u de instellingen voor uw bestelling instelt op `Disabled`, Amazon-orders worden weergegeven op het winkeldashboard, maar moeten worden beheerd in uw [!DNL Amazon Seller Central] account.

Wanneer een bestelling op Amazon wordt gemaakt, wordt deze niet onmiddellijk geïmporteerd in [!DNL Commerce]. Amazon wijst een `Pending` status voor nieuwe bestellingen. Nadat Amazon de bestelling en de betalingsmethode heeft geverifieerd, wordt de status van de bestelling gewijzigd in `Unshipped`. Deze statuswijziging leidt tot het importeren van de order, en [!DNL Commerce] maakt een overeenkomende, overeenkomende volgorde.

Uit Amazon geïmporteerde bestellingen kunnen worden beheerd in het dialoogvenster [!DNL Commerce] [orderwerkstroom](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}. Zie ook [Bestellingen beheren](./managing-orders.md).

## Orderinstellingen configureren {#configure-order-settings}

1. Klikken **[!UICONTROL Order Settings]** op het opslagdashboard.

1. Voor **[!UICONTROL Import Amazon Orders]** (vereist) kiest u een optie:

   - `Disabled` - Kies wanneer u geen corresponderende bestellingen wilt maken in [!DNL Commerce] wanneer nieuwe bestellingen van Amazon worden ontvangen. Als u deze optie kiest, worden alle andere velden op deze pagina uitgeschakeld.

   - `Enabled` - (Standaard) Kies wanneer u de corresponderende tekst wilt maken [!DNL Commerce] bestellingen wanneer nieuwe bestellingen van Amazon worden ontvangen. [!DNL Commerce] bestellingen worden aangemaakt op basis van Amazon-status en aandelenniveaus.

      >[!NOTE]
      >
      >Amazon-orders importeren moet zijn ingesteld op `Enabled` om Amazon-orders te beheren in het dialoogvenster [!DNL Commerce] [orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} workflow. Wanneer ingesteld op `Disabled`, hebben uw Amazon-bestellingen geen overeenkomende [!DNL Commerce] ordernummer en kan niet worden beheerd in [!DNL Commerce]. U beheert deze bestellingen in uw [!DNL Amazon Seller Central] account.

1. Voor **[!UICONTROL Import Amazon Orders Into Magento Store]**, kiest u welke [!DNL Commerce] de Amazon-orders opslaan als er een corresponderende volgorde wordt gemaakt in [!DNL Commerce].

   Deze instelling wordt standaard ingesteld op de Winkelweergave voor de website die u selecteert wanneer u [toegevoegd aan de Amazon-winkel](./store-integration.md). Als u deze instelling wilt wijzigen, is de lijst met opties afhankelijk van de optie [!DNL Commerce] slaat u opstelling in uw configuratie op. Zie [Winkels](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){target=&quot;_blank&quot;}.

1. Voor **[!UICONTROL Customer Creation]** kiest u een optie:

   - `No Customer Creation (guest)` - (Standaard) Kies wanneer u geen klantenaccount wilt maken in [!DNL Commerce] de geïmporteerde klantgegevens uit de Amazon-bestelling gebruiken. Indien gekozen, [!DNL Commerce] verwerkt een geïmporteerde Amazon-bestelling op dezelfde manier als een uitcheckprocedure voor gasten [!DNL Commerce].

   - `Build New Customer Account` - Kies wanneer u een nieuwe klantenaccount wilt maken in [!DNL Commerce] met de klantgegevens die met de Amazon-bestelling zijn geïmporteerd. Met deze optie kunt u uw klantendatabase samenstellen op basis van uw Amazon-bestellingen.

1. Voor **[!UICONTROL Order Number Source]** kiest u een optie:

   - `Build Using Magento Order Number` - (Standaard) Kies wanneer u een unieke [!DNL Commerce] ordernummer voor de bijbehorende Amazon-order met behulp van de [!DNL Commerce] incrementeel toegewezen order-id.

   - `Build Using Amazon Order Number` - Kies wanneer u de [!DNL Commerce] volgordenummer met het corresponderende door Amazon toegewezen ordernummer.
   >[!NOTE]
   >
   >Nadat een bestelling is geïmporteerd, wordt het Amazon-ordernummer weergegeven in het dialoogvenster _[!UICONTROL Recent Orders]_op het opslagdashboard. De [!DNL Commerce] het ordernummer wordt weergegeven wanneer u de ordergegevens in het dialoogvenster [!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} werkruimte.

1. Voor **[!UICONTROL Order Status]** (vereist) kiest u een optie:

   - `Default Order Status` - (Standaardinstelling) Kies wanneer u wilt dat aan nieuw gemaakte bestellingen die u uit Amazon hebt geïmporteerd, de standaardvolgordestatus voor nieuwe bestellingen wordt toegewezen. De standaardstatus voor nieuwe orders (tenzij u een aangepaste orderstatus voor nieuwe orders hebt gemaakt) is `Pending`. Zie [Bezig met verwerken van bestellingen](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}.

   - `Custom Order Status` - Kies wanneer u wilt dat nieuwe orders die u uit Amazon hebt geïmporteerd, een andere status krijgen dan de standaardstatus.

   - `Processing Order Status` - Ingeschakeld wanneer **[!UICONTROL Order Status]** is ingesteld op `Custom Order Status`. Kies de status die u wilt gebruiken voor nieuwe bestellingen die uit Amazon zijn geïmporteerd. De opties in dit veld zijn gebaseerd op de standaardopties voor de status in [!DNL Commerce]. Zie [Status van bestelling](https://docs.magento.com/user-guide/sales/order-status.html). U kunt ook een aangepaste orderstatus maken die hier voor selectie wordt weergegeven. Als u een aangepaste orderstatus wilt maken, raadpleegt u [Status van aangepaste bestelling](https://docs.magento.com/user-guide/sales/order-status-custom.html){target=&quot;_blank&quot;}.

1. Klik op **[!UICONTROL Save order settings]**.

![Orderinstellingen](assets/amazon-order-settings.png)

| Veld | Beschrijving |
|---|---|
| [!UICONTROL Import Amazon Orders] | Opties:<ul><li>**[!UICONTROL Disabled]** - Kies wanneer u geen corresponderende bestellingen wilt maken in [!DNL Commerce] wanneer nieuwe bestellingen van Amazon worden ontvangen. Als u deze optie kiest, worden alle andere velden op deze pagina uitgeschakeld.</li><li>**[!UICONTROL Enabled]** - (Standaard) Kies wanneer u de corresponderende tekst wilt maken [!DNL Commerce] bestellingen wanneer nieuwe bestellingen van Amazon worden ontvangen. [!DNL Commerce] bestellingen worden aangemaakt op basis van Amazon-status en aandelenniveaus.</li></ul><br><br>`Enabled` moet worden gekozen voor het beheren van Amazon-orders in [!DNL Commerce]. Wanneer `Disabled` wordt gekozen, worden uw Amazon-bestellingen weergegeven op het opslagdashboard, maar de bestellingen moeten worden beheerd in uw [!DNL Amazon Seller Central] account. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Kiezen welke [!DNL Commerce] bestellingen van Amazon opslaan waaraan wordt gekoppeld wanneer ze worden gemaakt in het dialoogvenster [!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} werkruimte. Deze instelling wordt standaard ingesteld in de winkelweergave voor de [!DNL Commerce] website geselecteerd wanneer u [toegevoegd aan de Amazon-winkel](./store-integration.md). Als u deze instelling wilt wijzigen, is de lijst met opties afhankelijk van de optie [!DNL Commerce] slaat u opstelling in uw configuratie op. Zie [Winkels](https://docs.magento.com/user-guide/stores/stores-all-stores.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Customer Creation] | Opties:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Standaard) Kies wanneer u geen klantenaccount wilt maken in [!DNL Commerce] de geïmporteerde klantgegevens uit de Amazon-bestelling gebruiken. Als u deze optie kiest, krijgt deze de volgende informatie [!DNL Commerce] om een geïmporteerde Amazon-bestelling te verwerken op dezelfde manier als een uitcheckbewerking voor gasten.</li><li>**[!UICONTROL Build New Customer Account]** - Kies wanneer u een nieuwe klantenaccount wilt maken in uw [!DNL Commerce] met de klantgegevens die met de Amazon-order zijn geïmporteerd. Met deze optie kunt u uw [!DNL Commerce] van uw Amazon-bestellingen.</li></ul> |
| Bron van ordernummer | Opties:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Standaard) Kies wanneer u een unieke [!DNL Commerce] ordernummer voor de bijbehorende Amazon-order met behulp van de [!DNL Commerce] incrementeel toegewezen order-id. </li><li>**Samenstellen met Amazon Order Number** - Kies wanneer u de [!DNL Commerce] volgordenummer met het corresponderende door Amazon toegewezen ordernummer.</li></ul> |
| In behandeling zijnde bestellingen | Opties:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Kies wanneer u uw [!DNL Commerce] voorraadhoeveelheid die wordt beïnvloed door je Amazon-bestellingen. Kies of u Amazon gebruikt voor uw uitvoeringsproces (FBA). Wanneer je kiest en je een Amazon-bestelling ontvangt, heeft het bestelde aantal geen invloed op je [!DNL Commerce] voorraadhoeveelheid.</li><li>**[!UICONTROL Reserve Quantity]** - Kies wanneer u het orderaantal in de Amazon-volgorde wilt &quot;gereserveerd&quot; in uw [!DNL Commerce] voorraadhoeveelheid. Wanneer je kiest en je een Amazon-bestelling ontvangt, wordt het bestelde aantal in je [!DNL Commerce] voorraadhoeveelheid om je [!DNL Commerce] voorraad van &#39;over-sales&#39;. De hoeveelheid &quot;gereserveerd&quot; kan niet worden aangeschaft via uw [!DNL Commerce] storefront.</li></ul> |
| [!UICONTROL Order Status] | Opties:<ul><li>**[!UICONTROL Default Order Status]** - (Standaardinstelling) Kies wanneer u wilt dat aan nieuw gemaakte bestellingen die u uit Amazon hebt geïmporteerd, de status van de standaardvolgorde wordt toegewezen voor nieuwe bestellingen. De standaardstatus voor nieuwe orders (tenzij u een aangepaste orderstatus voor nieuwe orders hebt gemaakt) is `Pending`. Zie [Bezig met verwerken van bestellingen](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]** - Kies wanneer u wilt dat nieuwe orders die u uit Amazon hebt geïmporteerd, een andere status krijgen dan de standaardstatus. Indien gekozen, **[!UICONTROL Processing Order Status]** Hiermee kunt u de status kiezen die u wilt gebruiken voor nieuwe bestellingen die uit Amazon zijn geïmporteerd.</li></ul> |
| [!UICONTROL Processing Orders Status] | Ingeschakeld als _[!UICONTROL Order Status]_is ingesteld op `Custom Order Status`. Kies de orderstatus die u wilt toewijzen aan nieuwe bestellingen. De opties in dit veld zijn afhankelijk van de standaardstatusopties in het veld [!DNL Commerce]. Zie [Status van bestelling](https://docs.magento.com/user-guide/sales/order-status.html){target=&quot;_blank&quot;}. U kunt ook een aangepaste orderstatus maken die hier wordt weergegeven. Als u een aangepaste orderstatus wilt maken, raadpleegt u [Status van aangepaste bestelling](https://docs.magento.com/user-guide/sales/order-status-custom.html){target=&quot;_blank&quot;}. |

## [!DNL Commerce] bestellen

[!DNL Commerce] voor Amazon-bestellingen worden bestellingen gemaakt op basis van de volgende status en inventarisvoorwaarden.

### Maken van bestellingen met Inventory management

>[!NOTE]
>
>Alleen ondersteund in Adobe Commerce en Magento Open Source 2.3.x-integratie.

| Afuitvoeringskanaal | [!DNL Commerce] Inventarisstatus | Status Amazon-bestelling | [!UICONTROL Create Magento Order] Instelling | Voorraad gereserveerd |
|---|---|---|---|---|
| FBA | In voorraad<br>Buiten de voorraad<br>Niet beheren | In behandeling | Nee | Nee |
| FBA | In voorraad<br>Buiten de voorraad<br>Niet beheren | PendingAvailability | Nee | Nee |
| FBA | In voorraad<br>Buiten de voorraad<br>Niet beheren | Geannuleerd | Nee | Nee |
| FBA | In voorraad<br>Buiten de voorraad<br>Niet beheren | Fout | Nee | Nee |
| FBA | In voorraad<br>Buiten de voorraad<br>Niet beheren | Niet verscheept | Nee | Nee |
| FBA | In voorraad<br>Buiten de voorraad<br>Niet beheren | GedeeltelijkVerzonden | Nee | Nee |
| FBA | In voorraad<br>Niet beheren | Verzonden | Ja | Nee |
| FBA | Buiten de voorraad | Verzonden | Nee | Nee |
| FBM | In voorraad<br>Buiten de voorraad<br>Niet beheren | In behandeling | Nee | Nee |
| FBM | In voorraad<br>Buiten de voorraad<br>Niet beheren | PendingAvailability | Nee | Nee |
| FBM | In voorraad<br>Buiten de voorraad<br>Niet beheren | Geannuleerd | Nee | Nee |
| FBM | In voorraad<br>Buiten de voorraad<br>Niet beheren | Fout | Nee | Nee |
| FBM | In voorraad<br>Niet beheren | Niet verscheept | Ja | Ja |
| FBM | Buiten de voorraad | Niet verscheept | Nee | Nee |
| FBM | In voorraad<br>Niet beheren | GedeeltelijkVerzonden | Ja | Ja |
| FBM | Buiten de voorraad | GedeeltelijkVerzonden | Nee | Nee |
| FBM | In voorraad<br>Niet beheren | Verzonden | Ja | Ja |
| FBM | Buiten de voorraad | Verzonden | Nee | Nee |

>[!NOTE]
>Als een Amazon-bestelling wordt geïmporteerd in een `Partially Shipped` of `Shipped` status, de voorraadboeking die wordt gemaakt, geldt voor alle items in de bestelling. Amazon biedt geen compensatie voor objecten die eerder zijn verzonden.
>
>Als een bestelling wordt vervuld door Amazon (FBA), maar een item zich bevindt in `out of stock` status, [!DNL Commerce] kan geen corresponderende volgorde maken. Dit is een beperking van de integratie van Inventory management.
