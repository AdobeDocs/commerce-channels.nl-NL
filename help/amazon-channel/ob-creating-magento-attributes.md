---
title: Maken [!DNL Commerce] Attributen voor Amazon
description: Voordat u het Amazon-verkoopkanaal voor instapkaarten voltooit, moet u controleren of u over de vereiste [!UICONTROL Commerce] productkenmerken.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Maken [!DNL Commerce] kenmerken voor Amazon

Voordat u uw [!DNL Amazon Seller Central] accounts, kunt u het beste [!DNL Commerce] [productkenmerken](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;} om uw productaanbiedingen toe te wijzen. Nadat u het instapproces hebt voltooid, kunt u de productkenmerken beheren via de [Attributen](./managing-attributes.md) tabblad van het dialoogvenster [Amazon-verkoopkanaal naar huis](./amazon-sales-channel-home.md) pagina.

In deze instructies wordt gedetailleerd beschreven hoe u kunt maken [!DNL Commerce] kenmerken voor Amazon ASIN en Amazon Condition. Creating additional attributes including Amazon EAN, Amazon ISBN, and Amazon UPC is recommended. You may want to also create an Amazon Price attribute if you want to use your Amazon listing price as a price source for pricing rules. Deze kenmerken worden gebruikt bij het configureren van de instellingen voor aanbiedingen en prijzen tijdens het instappen. Gebruik deze kenmerken ook bij het maken van Amazon-aanbiedingen en bij het bijwerken en synchroniseren van je [!DNL Commerce] catalogus met je Amazon-aanbiedingen.

Catalog Search settings enable you to set matching search parameters that help to map eligible [!DNL Commerce] products with Amazon listings. When mapped, Amazon activates actions related to pricing, quantity, overrides, and order and product synchronization.

Als u deze waarden definieert, neemt de kans op exacte overeenkomsten toe, waardoor de noodzaak van handmatig overeenkomende productaanbiedingen later tot een minimum wordt beperkt. Adding the attributes as part of your onboarding [pre-setup tasks](./amazon-pre-setup-tasks.md), Amazon sales channel has a higher potential for automatically matching your products during onboarding and syncs product data between Amazon and [!DNL Commerce] after onboarding.

Als u alleen het Amazon ASIN-kenmerk maakt (zonder ASIN-waarden per product toe te voegen), kunt u [!DNL Commerce] producten komen mogelijk niet automatisch overeen met je Amazon-aanbiedingen. U kunt uw producten handmatig aanpassen via _Winkelrevisie_. Handmatige overeenkomsten maken echter geen gegevenselementen die nodig zijn voor het delen en synchroniseren van uw productgegevens.

>[!IMPORTANT]
>
>Als u een ASIN-, UPC- of ander gegevenselement voor een handmatig overeenkomend product bijwerkt, moet u de gegevens op beide plaatsen bijwerken: uw [!DNL Commerce] en de aanbieding in uw [!DNL Amazon Seller Central] account.

## Het Amazon ASIN-productkenmerk maken

1. Log into your [!DNL Commerce] Admin.

1. Klikken **[!UICONTROL Stores]** in het linkerzijmenu.

1. In the _[!UICONTROL Attributes]_section, click **[!UICONTROL Product]**.

1. To open the attributes properties, click **[!UICONTROL Add New Attribute]**.

1. Voor **[!UICONTROL Default Label]**, enter `Amazon ASIN` (de naam voor het kenmerk).

1. Voor **[!UICONTROL Catalog Input Type for Store Owner]** kiest u `Text Field`.

1. Voor **[!UICONTROL Values Required]** kiest u `No`.

   Hoewel een Amazon ASIN vereist is om een product op Amazon aan te bieden, zijn sommige catalogusproducten mogelijk niet in Amazon vermeld.

1. Expand the _[!UICONTROL Advanced Attribute Properties]_section and set the options:

   - Voor **[!UICONTROL Attribute Code]**, enter `amazon_asin`.

   - For **[!UICONTROL Scope]**, choose `Global`.

   - Voor **[!UICONTROL Unique Value]** kiest u `No`.

   - Voor **[!UICONTROL Input Validation for Store Owner]** kiest u `None`.

   - Voor **[!UICONTROL Add to Column Options]** kiest u `Yes`.

   - For **[!UICONTROL Use in Filter Options]**, choose `Yes`.

1. Klikken **[!UICONTROL Save Attribute]**.

![Amazon ASIN attribute](assets/creating-asin-attribute.png)

## Create the Amazon Condition product attribute

1. Meld u aan bij uw [!DNL Commerce] Admin.

1. Klikken **[!UICONTROL Stores]** in het linkerzijmenu.

1. In de _[!UICONTROL Attributes]_sectie, klikt u op **[!UICONTROL Product]**.

1. Klik op **[!UICONTROL Add New Attribute]**.

1. Voor **[!UICONTROL Default Label]**, enter `Amazon Condition` (de naam voor het kenmerk).

1. Voor **[!UICONTROL Catalog Input Type for Store Owner]** kiest u `Dropdown`.

   De _[!UICONTROL Manage Options (Values of your Attribute)]_wordt weergegeven.

1. Voor **[!UICONTROL Values Required]** kiest u `No`.

1. For **[!UICONTROL Manage Options (Values for your Attribute)]**, add each of your condition options.

   Tot de standaard Amazon-voorwaarden behoren:

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. Klikken **[!UICONTROL Add Option]**.

1. Select the **[!UICONTROL Is Default]** option for the condition you wish to be the default selection.

1. In de _[!UICONTROL Admin]_voert u de tekst in voor het label van de voorwaarde die u toevoegt (bijvoorbeeld `New`, `Used`, en `Used-Like New`)

1. Klikken **[!UICONTROL Add Option]** om zo nodig meer opties toe te voegen.

1. Uitbreiden _[!UICONTROL Advanced Attribute Properties]_en stelt u de opties in.

   - Voor **[!UICONTROL Attribute Code]**, enter `amazon_condition`.

   - Voor **[!UICONTROL Scope]** kiest u `Global`.

   - Voor **[!UICONTROL Unique Value]** kiest u `No`.

   - Voor **[!UICONTROL Input Validation for Store Owner]** kiest u `None`.

   - Voor **[!UICONTROL Add to Column Options]** kiest u `Yes`.

   - Voor **[!UICONTROL Use in Filter Options]** kiest u `Yes`.

1. Klikken **[!UICONTROL Save Attribute]**.

![Amazon Condition, kenmerk](assets/creating-amazon-condition-attribute.png)

![Volgende pictogram](assets/btn-next.png) [**API-sleutel toevoegen of verifiëren**](./amazon-verify-api-key.md)
