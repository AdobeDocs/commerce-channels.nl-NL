---
title: Handelskenmerken maken voor Amazon
description: Voordat u het Amazon-verkoopkanaal voor instapkaarten voltooit, moet u controleren of u over de vereiste [!UICONTROL Commerce] productkenmerken.
role: Admin
feature: Sales Channels, Products, Configuration
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Handelskenmerken maken voor Amazon

Voordat u uw [!DNL Amazon Seller Central] accounts, kunt u het beste [!DNL Commerce] [productkenmerken](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) om je productaanbiedingen toe te wijzen. Nadat u het instapproces hebt voltooid, kunt u de productkenmerken beheren via de [Attributen](./managing-attributes.md) tabblad van het [Amazon-verkoopkanaal naar huis](./amazon-sales-channel-home.md) pagina.

In deze instructies wordt gedetailleerd beschreven hoe u kunt maken [!DNL Commerce] kenmerken voor Amazon ASIN en Amazon Condition. Het wordt aanbevolen aanvullende kenmerken te maken, zoals Amazon EAN, Amazon ISBN en Amazon UPC. Je kunt ook een Amazon Price-kenmerk maken als je de prijs van je Amazon-aanbieding wilt gebruiken als prijsbron voor prijsregels. Deze kenmerken worden gebruikt bij het configureren van de instellingen voor aanbiedingen en prijzen tijdens het instappen. Gebruik deze kenmerken ook bij het maken van Amazon-aanbiedingen en bij het bijwerken en synchroniseren van je [!DNL Commerce] catalogus met je Amazon-aanbiedingen.

Met de zoekinstellingen voor catalogi kunt u overeenkomende zoekparameters instellen die u helpen in aanmerking komende parameters toe te wijzen [!DNL Commerce] producten met Amazon-aanbiedingen. Als Amazon een kaart heeft toegewezen, activeert het acties met betrekking tot prijzen, hoeveelheden, overschrijvingen en volgorde en productsynchronisatie.

Als u deze waarden definieert, neemt de kans op exacte overeenkomsten toe, waardoor de noodzaak van handmatig overeenkomende productaanbiedingen later tot een minimum wordt beperkt. Kenmerken toevoegen als onderdeel van uw instapsysteem [vooraf ingestelde taken](./amazon-pre-setup-tasks.md), Amazon verkoopkanaal heeft een groter potentieel om uw producten automatisch aan te passen tijdens het instappen en synchroniseert productgegevens tussen Amazon en [!DNL Commerce] na aan boord gaan.

Als u alleen het Amazon ASIN-kenmerk maakt (zonder ASIN-waarden per product toe te voegen), kunt u [!DNL Commerce] producten komen mogelijk niet automatisch overeen met je Amazon-aanbiedingen. U kunt uw producten handmatig aanpassen via _Winkelrevisie_. Handmatige overeenkomsten maken echter geen gegevenselementen die nodig zijn voor het delen en synchroniseren van uw productgegevens.

>[!IMPORTANT]
>
>Als u een ASIN-, UPC- of ander gegevenselement voor een product bijwerkt dat handmatig overeenkomt, moet u de gegevens op beide plaatsen bijwerken: uw [!DNL Commerce] en de aanbieding in uw [!DNL Amazon Seller Central] account.

## Het Amazon ASIN-productkenmerk maken

1. Log in uw [!DNL Commerce] Admin.

1. Klikken **[!UICONTROL Stores]** in het linkerzijmenu.

1. In de _[!UICONTROL Attributes]_sectie, klikken **[!UICONTROL Product]**.

1. Klik op **[!UICONTROL Add New Attribute]**.

1. Voor **[!UICONTROL Default Label]**, enter `Amazon ASIN` (de naam voor het kenmerk).

1. Voor **[!UICONTROL Catalog Input Type for Store Owner]**, kiest u `Text Field`.

1. Voor **[!UICONTROL Values Required]**, kiest u `No`.

   Hoewel een Amazon ASIN vereist is om een product op Amazon aan te bieden, zijn sommige catalogusproducten mogelijk niet in Amazon vermeld.

1. Breid uit _[!UICONTROL Advanced Attribute Properties]_en stel de opties in:

   - Voor **[!UICONTROL Attribute Code]**, enter `amazon_asin`.

   - Voor **[!UICONTROL Scope]**, kiest u `Global`.

   - Voor **[!UICONTROL Unique Value]**, kiest u `No`.

   - Voor **[!UICONTROL Input Validation for Store Owner]**, kiest u `None`.

   - Voor **[!UICONTROL Add to Column Options]**, kiest u `Yes`.

   - Voor **[!UICONTROL Use in Filter Options]**, kiest u `Yes`.

1. Klik op **[!UICONTROL Save Attribute]**.

![Amazon ASIN, kenmerk](assets/creating-asin-attribute.png){width="600" zoomable="yes"}

## Het productkenmerk Amazon Condition maken

1. Log in uw [!DNL Commerce] Admin.

1. Klikken **[!UICONTROL Stores]** in het linkerzijmenu.

1. In de _[!UICONTROL Attributes]_sectie, klikken **[!UICONTROL Product]**.

1. Klik op **[!UICONTROL Add New Attribute]**.

1. Voor **[!UICONTROL Default Label]**, enter `Amazon Condition` (de naam voor het kenmerk).

1. Voor **[!UICONTROL Catalog Input Type for Store Owner]**, kiest u `Dropdown`.

   De _[!UICONTROL Manage Options (Values of your Attribute)]_wordt weergegeven.

1. Voor **[!UICONTROL Values Required]**, kiest u `No`.

1. Voor **[!UICONTROL Manage Options (Values for your Attribute)]** voegt u elk van uw voorwaardenopties toe.

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

1. Selecteer de **[!UICONTROL Is Default]** voor de voorwaarde die u als standaardselectie wilt gebruiken.

1. In de _[!UICONTROL Admin]_voert u de tekst in voor het label van de voorwaarde die u toevoegt (bijvoorbeeld `New`, `Used`, en `Used-Like New`)

1. Klikken **[!UICONTROL Add Option]** om zo nodig meer opties toe te voegen.

1. Uitbreiden _[!UICONTROL Advanced Attribute Properties]_en stelt u de opties in.

   - Voor **[!UICONTROL Attribute Code]**, enter `amazon_condition`.

   - Voor **[!UICONTROL Scope]**, kiest u `Global`.

   - Voor **[!UICONTROL Unique Value]**, kiest u `No`.

   - Voor **[!UICONTROL Input Validation for Store Owner]**, kiest u `None`.

   - Voor **[!UICONTROL Add to Column Options]**, kiest u `Yes`.

   - Voor **[!UICONTROL Use in Filter Options]**, kiest u `Yes`.

1. Klik op **[!UICONTROL Save Attribute]**.

![Amazon Condition, kenmerk](assets/creating-amazon-condition-attribute.png){width="600" zoomable="yes"}

![Volgende pictogram](assets/btn-next.png) [**API-sleutel toevoegen of verifiëren**](./amazon-verify-api-key.md)
