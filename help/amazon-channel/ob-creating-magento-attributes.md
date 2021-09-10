---
title: Create [!DNL Commerce] Attributen voor Amazon
description: Voordat u het Amazon-verkoopkanaal voor instapkaarten voltooit, moet u controleren of u de vereiste [!UICONTROL Commerce] productkenmerken hebt.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# [!DNL Commerce]-kenmerken maken voor Amazon

Voordat u uw [!DNL Amazon Seller Central]-accounts instapt, kunt u het beste [!DNL Commerce] [productkenmerken toevoegen](https://docs.magento.com/user-guide/stores/attributes-product.html){:target=&quot;_blank&quot;} om uw productaanbiedingen toe te wijzen. Nadat u het aan boord gaan hebt voltooid, kunt u uw productkenmerken beheren via het tabblad [Kenmerken](./managing-attributes.md) van de pagina [Amazon Verkoopkanaal home](./amazon-sales-channel-home.md).

In deze instructies wordt beschreven hoe u [!DNL Commerce]-kenmerken voor Amazon ASIN en Amazon Condition maakt. Het wordt aanbevolen aanvullende kenmerken te maken, zoals Amazon EAN, Amazon ISBN en Amazon UPC. Je kunt ook een Amazon Price-kenmerk maken als je de prijs van je Amazon-aanbieding wilt gebruiken als prijsbron voor prijsregels. Deze kenmerken worden gebruikt bij het configureren van de instellingen voor aanbiedingen en prijzen tijdens het instappen. Gebruik deze kenmerken ook bij het maken van Amazon-aanbiedingen en bij het bijwerken en synchroniseren van uw [!DNL Commerce]-catalogus met uw Amazon-aanbiedingen.

Met de zoekinstellingen voor catalogi kunt u overeenkomende zoekparameters instellen waarmee in aanmerking komende [!DNL Commerce]-producten kunnen worden toegewezen aan Amazon-aanbiedingen. Als Amazon een kaart heeft toegewezen, activeert het acties met betrekking tot prijzen, hoeveelheden, overschrijvingen en volgorde en productsynchronisatie.

Als u deze waarden definieert, neemt de kans op exacte overeenkomsten toe, waardoor de noodzaak van handmatig overeenkomende productaanbiedingen later tot een minimum wordt beperkt. Als u de kenmerken toevoegt als onderdeel van uw instaptaken [pre-setup taken](./amazon-pre-setup-tasks.md), biedt Amazon-verkoopkanaal een groter potentieel om uw producten automatisch op elkaar af te stemmen tijdens het instappen en synchroniseren van productgegevens tussen Amazon en [!DNL Commerce] na het instappen.

Als u alleen het Amazon ASIN-kenmerk maakt (zonder ASIN-waarden per product toe te voegen), komen uw [!DNL Commerce]-producten mogelijk niet automatisch overeen met uw Amazon-aanbiedingen. U kunt uw producten handmatig aanpassen via _Revisie opslaan_. Handmatige overeenkomsten maken echter geen gegevenselementen die nodig zijn voor het delen en synchroniseren van uw productgegevens.

>[!IMPORTANT]
>
>Als u een ASIN-, UPC- of ander gegevenselement voor een handmatig overeenkomend product bijwerkt, moet u de gegevens op beide plaatsen bijwerken: uw [!DNL Commerce]-catalogus en de aanbieding in uw [!DNL Amazon Seller Central]-account.

## Het Amazon ASIN-productkenmerk maken

1. Meld u aan bij uw [!DNL Commerce]-beheerder.

1. Klik **[!UICONTROL Stores]** in het linkerzijmenu.

1. Klik in de sectie _[!UICONTROL Attributes]_op **[!UICONTROL Product]**.

1. Klik op **[!UICONTROL Add New Attribute]** om de eigenschappen van de kenmerken te openen.

1. Typ **[!UICONTROL Default Label]** (de naam voor het kenmerk).`Amazon ASIN`

1. Kies **[!UICONTROL Catalog Input Type for Store Owner]** bij `Text Field`.

1. Kies **[!UICONTROL Values Required]** bij `No`.

   Hoewel een Amazon ASIN vereist is om een product op Amazon aan te bieden, zijn sommige catalogusproducten mogelijk niet in Amazon vermeld.

1. Vouw de sectie _[!UICONTROL Advanced Attribute Properties]_uit en stel de opties in:

   - Typ `amazon_asin` bij **[!UICONTROL Attribute Code]**.

   - Kies **[!UICONTROL Scope]** bij `Global`.

   - Kies **[!UICONTROL Unique Value]** bij `No`.

   - Kies **[!UICONTROL Input Validation for Store Owner]** bij `None`.

   - Kies **[!UICONTROL Add to Column Options]** bij `Yes`.

   - Kies **[!UICONTROL Use in Filter Options]** bij `Yes`.

1. Klik op **[!UICONTROL Save Attribute]**.

![Amazon ASIN, kenmerk](assets/creating-asin-attribute.png)

## Het productkenmerk Amazon Condition maken

1. Meld u aan bij uw [!DNL Commerce]-beheerder.

1. Klik **[!UICONTROL Stores]** in het linkerzijmenu.

1. Klik in de sectie _[!UICONTROL Attributes]_op **[!UICONTROL Product]**.

1. Klik op **[!UICONTROL Add New Attribute]** om de kenmerkeigenschappen te openen.

1. Typ **[!UICONTROL Default Label]** (de naam voor het kenmerk).`Amazon Condition`

1. Kies **[!UICONTROL Catalog Input Type for Store Owner]** bij `Dropdown`.

   De sectie _[!UICONTROL Manage Options (Values of your Attribute)]_wordt weergegeven.

1. Kies **[!UICONTROL Values Required]** bij `No`.

1. Voeg bij **[!UICONTROL Manage Options (Values for your Attribute)]** elk van uw voorwaardenopties toe.

   Tot de standaard Amazon-voorwaarden behoren:

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. Klik op **[!UICONTROL Add Option]**.

1. Selecteer de optie **[!UICONTROL Is Default]** voor de voorwaarde u wenst om de standaardselectie te zijn.

1. Voer in de kolom _[!UICONTROL Admin]_de tekst in voor het label van de voorwaarde die u toevoegt (zoals `New`, `Used` en `Used-Like New`)

1. Klik **[!UICONTROL Add Option]** om meer opties toe te voegen, zoals nodig.

1. Vouw de sectie _[!UICONTROL Advanced Attribute Properties]_uit en stel de opties in.

   - Typ `amazon_condition` bij **[!UICONTROL Attribute Code]**.

   - Kies **[!UICONTROL Scope]** bij `Global`.

   - Kies **[!UICONTROL Unique Value]** bij `No`.

   - Kies **[!UICONTROL Input Validation for Store Owner]** bij `None`.

   - Kies **[!UICONTROL Add to Column Options]** bij `Yes`.

   - Kies **[!UICONTROL Use in Filter Options]** bij `Yes`.

1. Klik op **[!UICONTROL Save Attribute]**.

![Amazon Condition, kenmerk](assets/creating-amazon-condition-attribute.png)

![Volgende ](assets/btn-next.png) [**pictogramDoorgaan met toevoegen of verifiëren van API-sleutel**](./amazon-verify-api-key.md)
