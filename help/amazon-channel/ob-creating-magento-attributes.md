---
title: Commerce-kenmerken maken voor Amazon
description: Voordat u het Amazon-verkoopkanaal voor instapkaarten voltooit, moet u controleren of u de vereiste [!UICONTROL Commerce] -productkenmerken hebt.
role: Admin
feature: Sales Channels, Products, Configuration
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Commerce-kenmerken maken voor Amazon

Alvorens uw [!DNL Amazon Seller Central] rekeningen op te nemen, is het beste praktijken om [!DNL Commerce] [ productattributen ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) toe te voegen om uw productlijsten in kaart te brengen. Nadat u volledig op het instappen bent, kunt u uw productattributen door het [ lusje van Attributen ](./managing-attributes.md) van het [ de huis van het verkoopkanaal van Amazon ](./amazon-sales-channel-home.md) pagina beheren.

In deze instructies wordt beschreven hoe u [!DNL Commerce] -kenmerken maakt voor Amazon ASIN en Amazon Condition. Het wordt aanbevolen aanvullende kenmerken te maken, zoals Amazon EAN, Amazon ISBN en Amazon UPC. Je kunt ook een Amazon Price-kenmerk maken als je de prijs van je Amazon-aanbieding wilt gebruiken als prijsbron voor prijsregels. Deze kenmerken worden gebruikt bij het configureren van de instellingen voor aanbiedingen en prijzen tijdens het instappen. Gebruik deze kenmerken ook bij het maken van Amazon-aanbiedingen en bij het bijwerken en synchroniseren van uw [!DNL Commerce] -catalogus met uw Amazon-aanbiedingen.

Met de zoekinstellingen voor catalogi kunt u overeenkomende zoekparameters instellen die u helpen in aanmerking komende [!DNL Commerce] -producten toe te wijzen aan Amazon-aanbiedingen. Als Amazon een kaart heeft toegewezen, activeert het acties met betrekking tot prijzen, hoeveelheden, overschrijvingen en volgorde en productsynchronisatie.

Als u deze waarden definieert, neemt de kans op exacte overeenkomsten toe, waardoor de noodzaak van handmatig overeenkomende productaanbiedingen later tot een minimum wordt beperkt. Toevoegend de attributen als deel van uw aan boord gaan [ pre-opstellingstaken ](./amazon-pre-setup-tasks.md), heeft het verkoopkanaal van Amazon een hoger potentieel om uw producten tijdens het aan boord nemen automatisch aan te passen en productgegevens tussen Amazon en [!DNL Commerce] na het aan boord gaan.

Als u alleen het Amazon ASIN-kenmerk maakt (zonder ASIN-waarden per product toe te voegen), komen uw [!DNL Commerce] -producten mogelijk niet automatisch overeen met uw Amazon-aanbiedingen. U kunt uw producten manueel aanpassen door _Overzicht van de Opslag_. Handmatige overeenkomsten maken echter geen gegevenselementen die nodig zijn voor het delen en synchroniseren van uw productgegevens.

>[!IMPORTANT]
>
>Als u een ASIN-, UPC- of ander gegevenselement voor een handmatig overeenkomend product bijwerkt, moet u de gegevens op beide plaatsen bijwerken: de [!DNL Commerce] -catalogus en de vermelding in uw [!DNL Amazon Seller Central] -account.

## Het Amazon ASIN-productkenmerk maken

1. Meld u aan bij uw [!DNL Commerce] Admin.

1. Klik op **[!UICONTROL Stores]** in het menu aan de linkerkant.

1. Klik in de sectie _[!UICONTROL Attributes]_op **[!UICONTROL Product]**.

1. Klik op **[!UICONTROL Add New Attribute]** om de eigenschappen van de kenmerken te openen.

1. Voer bij **[!UICONTROL Default Label]** `Amazon ASIN` in (de naam voor het kenmerk).

1. Kies `Text Field` bij **[!UICONTROL Catalog Input Type for Store Owner]** .

1. Kies `No` bij **[!UICONTROL Values Required]** .

   Hoewel een Amazon ASIN vereist is om een product op Amazon aan te bieden, zijn sommige catalogusproducten mogelijk niet in Amazon vermeld.

1. Vouw de sectie _[!UICONTROL Advanced Attribute Properties]_uit en stel de opties in:

   - Voer bij **[!UICONTROL Attribute Code]** `amazon_asin` in.

   - Kies `Global` bij **[!UICONTROL Scope]** .

   - Kies `No` bij **[!UICONTROL Unique Value]** .

   - Kies `None` bij **[!UICONTROL Input Validation for Store Owner]** .

   - Kies `Yes` bij **[!UICONTROL Add to Column Options]** .

   - Kies `Yes` bij **[!UICONTROL Use in Filter Options]** .

1. Klik op **[!UICONTROL Save Attribute]**.

![ Amazon ASIN attributen ](assets/creating-asin-attribute.png){width="600" zoomable="yes"}

## Het productkenmerk Amazon Condition maken

1. Meld u aan bij uw [!DNL Commerce] Admin.

1. Klik op **[!UICONTROL Stores]** in het menu aan de linkerkant.

1. Klik in de sectie _[!UICONTROL Attributes]_op **[!UICONTROL Product]**.

1. Klik op **[!UICONTROL Add New Attribute]** om de eigenschappen van het kenmerk te openen.

1. Voer bij **[!UICONTROL Default Label]** `Amazon Condition` in (de naam voor het kenmerk).

1. Kies `Dropdown` bij **[!UICONTROL Catalog Input Type for Store Owner]** .

   De sectie _[!UICONTROL Manage Options (Values of your Attribute)]_wordt weergegeven.

1. Kies `No` bij **[!UICONTROL Values Required]** .

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

1. Selecteer de optie **[!UICONTROL Is Default]** voor de voorwaarde die u als standaardselectie wilt gebruiken.

1. Voer in de kolom _[!UICONTROL Admin]_de tekst in voor het label van de voorwaarde die u toevoegt (zoals `New` , `Used` en `Used-Like New` )

1. Klik op **[!UICONTROL Add Option]** om desgewenst meer opties toe te voegen.

1. Vouw de sectie _[!UICONTROL Advanced Attribute Properties]_uit en stel de opties in.

   - Voer bij **[!UICONTROL Attribute Code]** `amazon_condition` in.

   - Kies `Global` bij **[!UICONTROL Scope]** .

   - Kies `No` bij **[!UICONTROL Unique Value]** .

   - Kies `None` bij **[!UICONTROL Input Validation for Store Owner]** .

   - Kies `Yes` bij **[!UICONTROL Add to Column Options]** .

   - Kies `Yes` bij **[!UICONTROL Use in Filter Options]** .

1. Klik op **[!UICONTROL Save Attribute]**.

![ het attribuut van de Voorwaarde van Amazon ](assets/creating-amazon-condition-attribute.png){width="600" zoomable="yes"}

![ Volgende pictogram ](assets/btn-next.png) [**gaat API Sleutel toevoegen of verifiëren**](./amazon-verify-api-key.md)
