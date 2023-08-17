---
title: Kenmerken voor Amazon-verkoopkanalen maken en bewerken
description: De Sales Channel van Amazon biedt de weergave Kenmerken om u te helpen de huidige kenmerken van Amazon en de gekoppelde handelskenmerken te bekijken.
feature: Sales Channels, Products, Configuration
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Kenmerken maken en bewerken

Maken of bijwerken [!DNL Commerce] kenmerken zoals je via Amazon verkoopt en je winkels bijwerkt. Huidige Amazon-kenmerken en gekoppelde kenmerken bekijken [!DNL Commerce] kenmerken door de [_[!UICONTROL Attributes]_weergave](./attributes-view.md) van de Amazon-homepage van verkoopkanalen. De_[!UICONTROL Action]_ toont de beschikbare acties voor het attribuut. U kunt een nieuwe [!DNL Commerce] -kenmerk voor een ongekoppeld Amazon-kenmerk, of u kunt een bestaand kenmerk bewerken [!DNL Commerce] en de toewijzing ervan aan een Amazon-kenmerk.

Wanneer u kenmerken maakt en bijwerkt, kunt u de kenmerkwaarden controleren voor [!DNL Commerce] en Amazon-producten. Deze waarden kunnen afwijken als u geen waarden synchroniseert en importeert uit Amazon. Zie voor meer informatie over Amazon-waarden voor deze kenmerken [Toewijzing Amazon-kenmerk controleren](./amazon-matching-attributes-values.md). Als u deze waarden wilt wijzigen, kunt u [een toewijzing bewerken of maken](./amazon-manually-update-incomplete-listing.md) tussen Amazon en [!DNL Commerce].

## Een kenmerk maken {#create-an-attribute}

Deze stappen maken een [!DNL Commerce] en toewijzen aan een Amazon-kenmerk. Afhankelijk van configuraties, kunnen de waarden beginnen tussen catalogi te synchroniseren.

1. Op de _Beheerder_ zijbalk, ga naar **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klikken **[!UICONTROL Attributes]** Zoek in het linkermenu een Amazon-kenmerk en klik op **[!UICONTROL Create Attribute]** in de _[!UICONTROL Action]_kolom.

1. De synchronisatie van de Amazon-waarden met de gekoppelde [!DNL Commerce] kenmerk, set **[!UICONTROL Is Active]** tot `Yes`.

   Wanneer ingesteld op `Yes`, worden de waarden gesynchroniseerd op basis van uw configuratie.

1. Kies `Create New Magento Attribute` for **[!UICONTROL Select Magento Product Attribute]**.

   Het kenmerk wordt toegewezen aan de optie **[!UICONTROL Amazon Attribute Name]**.

1. Voer een **[!UICONTROL Magento Product Attribute Name]**.

1. Voer een **[!UICONTROL Magento Product Attribute Code]**.

   Deze waarde moet allemaal in kleine letters en zonder spaties zijn.

1. Voor **[!UICONTROL Attribute Set Ids]**, kiest u een kenmerkset die u wilt toewijzen.

   Kenmerken maken doorgaans deel uit van een kenmerkset, zoals een set voor kleuren met kenmerken voor blauw, groen, geel en rood.

1. Voor **[!UICONTROL Type]**, kiest u het type van de kenmerkwaarde, zoals tekst en getallen.

   Deze optie beïnvloedt de toegestane waarde voor het attribuut.

1. Voor **[!UICONTROL Use for Promo Rule Conditions]**, ingesteld op `Yes` om toe te staan dat het attribuut voor een parameter binnen uw promotionele voorwaarden beschikbaar is.

1. Voor **[!UICONTROL Used in Search]**, ingesteld op `Yes` als het kenmerk en de waarde kunnen worden gebruikt in productzoekopdrachten.

1. Voor **[!UICONTROL Comparable on Storefront]**, ingesteld op `Yes` als de kenmerkwaarde kan worden gebruikt in de Amazon-functie &quot;Vergelijken via&quot;.

1. Kies de optie [!DNL Commerce] [bereik](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) voor het kenmerk en selecteer een of meer winkelweergaven waarin u Amazon-waarden wilt importeren.

   Als het bereik is ingesteld op `Global`de _[!UICONTROL Store View]_kan niet worden gewijzigd nadat het kenmerk is gemaakt.

   Als u `All Store Views (Global)`, worden waarden gesynchroniseerd en opgeslagen in al uw Amazon-winkelweergaven. U kunt waarden alleen synchroniseren met specifieke winkelweergaven.

1. Klik op **[!UICONTROL Save Attribute Settings]**.

Na het opslaan wilt u mogelijk het kenmerk bewerken om de instellingen te bekijken en de overeenkomst tussen Amazon en [!DNL Commerce] waarden voor het kenmerk. U kunt ook aangeven of Amazon-waarden moeten worden overschreven [!DNL Commerce] waarden.

![kenmerkinstellingen maken](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Geeft aan of dit kenmerk live en actief synchroon is tussen Amazon en [!DNL Commerce]. Instellen op `Yes` om de kenmerkwaarden van Amazon en [!DNL Commerce] synchroon blijven voor het geselecteerde kenmerk. |
| Productkenmerk Magento selecteren | Geeft het geselecteerde kenmerk aan dat u wilt koppelen aan de vermelde Amazon-kenmerknaam. Wanneer u een kenmerk maakt, kiest u `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | Hiermee geeft u de naam weer van het Amazon-kenmerk dat u hebt gekozen. De geselecteerde kenmerkkoppelingen naar dit Amazon-kenmerk. U kunt deze waarde niet bewerken via [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | Geeft de kenmerknaam of &quot;label&quot; aan. |
| [!UICONTROL Magento Product Attribute Code] | Geeft de kenmerkcode aan, allemaal in kleine letters zonder spaties. |
| [!UICONTROL Attribute Set Ids] | Geeft de kenmerkset aan waaraan het kenmerk moet worden toegewezen. Kenmerken maken doorgaans deel uit van een kenmerkset, zoals een set voor kleuren met kenmerken voor blauw, groen, geel en rood. |
| [!UICONTROL Type] | Geeft het waardetype van de kenmerkwaarde aan, zoals tekst en getallen. De selectie heeft invloed op de toegestane waarde voor het kenmerk. |
| [!UICONTROL Use for Promo Rule Conditions] | Schakelen tussen `Yes` om toe te staan dat het attribuut voor een parameter binnen uw promotionele voorwaarden beschikbaar is. |
| [!UICONTROL Used in Search] | Geeft aan of het kenmerk en de waarde kunnen worden gebruikt in productzoekopdrachten. |
| [!UICONTROL Comparable on Storefront] | Geeft aan of de kenmerkwaarde kan worden gebruikt in de Amazon-functionaliteit &quot;Vergelijken door&quot;. |
| [!UICONTROL Magento Product Attribute Scope] | Hiermee wordt de [bereik](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) voor het kenmerk. Opties: algemene weergave/winkelweergave<br>Wanneer ingesteld op `Global`, kan de winkelweergave niet worden bewerkt nadat het kenmerk is gemaakt. |
| [!UICONTROL Store Views (to import values into to)] | Wordt alleen weergegeven wanneer het bereik is ingesteld op `Store View`. Kies de optie [winkelweergave](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) waarop de Amazon-kenmerkwaarden worden gesynchroniseerd. Kiezen `All Store Views (Global)` Hiermee wordt de waarde voor alle [!DNL Commerce] archiefweergaven. |

## Een kenmerk bewerken {#edit-an-attribute}

1. Op de _Beheerder_ zijbalk, ga naar **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klikken **[!UICONTROL Attributes]** Zoek in het linkermenu een Amazon-kenmerk en klik op **[!UICONTROL Edit]** in de _[!UICONTROL Action]_kolom.

1. Het synchroniseren van de Amazon-waarden naar de gekoppelde waarden in- of uitschakelen [!DNL Commerce] kenmerk, set **Is actief** tot `Yes` of `No`.

   Wanneer ingesteld op `Yes`, worden de waarden gesynchroniseerd op basis van uw configuratie.

1. Voor **[!UICONTROL Select Magento Product Attribute]**, verifieer of werk de attributen bij om aan gekozen toe te wijzen **[!UICONTROL Amazon Attribute Name]**.

1. Geef aan of u de bestaande kenmerkwaarde van de binnenkomende Amazon wilt overschrijven.

   U wilt bijvoorbeeld de prijzen van Amazon overschrijven naar [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Behoudt de waarde en bewaart verschillende waarden voor uw [!DNL Commerce] en Amazon winkels.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Hiermee overschrijft u de waarde in het dialoogvenster [!DNL Commerce] productcatalogus met de inkomende Amazon-waarde.

1. Kies een of meer **[!UICONTROL Store Views (to import Amazon values into)]**.

   Als het kenmerk is gemaakt met een `Global` de _Winkelweergave_ kan niet worden gewijzigd nadat het kenmerk is gemaakt.

   Als u `All Store Views (Global)`, worden waarden gesynchroniseerd en opgeslagen in alle winkelweergaven. U kunt waarden alleen synchroniseren met specifieke winkelweergaven.

1. Klik op **[!UICONTROL Save Attribute Settings]**.

![kenmerkinstellingen bewerken](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Geeft aan of dit kenmerk live en actief synchroon is tussen Amazon en [!DNL Commerce]. Instellen op `Yes` om de kenmerkwaarden van Amazon en [!DNL Commerce] synchroon blijven voor het geselecteerde kenmerk. |
| [!UICONTROL Select Magento Product Attribute] | Hiermee wordt de geselecteerde [!DNL Commerce] kenmerk dat u wilt koppelen aan de vermelde Amazon-kenmerknaam. Als u de gekoppelde [!DNL Commerce] , kiest u een ander kenmerk in de vervolgkeuzelijst. De waarden worden gesynchroniseerd op basis van configuraties. |
| [!UICONTROL Amazon Attribute Name] | Hiermee wordt de naam van het Amazon-kenmerk weergegeven, zoals gedefinieerd in [!DNL Amazon Seller Central]. De geselecteerde [!DNL Commerce] kenmerkkoppelingen naar dit Amazon-kenmerk. U kunt deze waarde niet bewerken via [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Geeft aan of de Amazon-kenmerkwaarden het bestaande overschrijven [!DNL Commerce] waarden, die van invloed zijn op alle producten met dit [!DNL Commerce] kenmerk.<ul><li>**Bestaande Magento&#39;s niet overschrijven** - (Standaard) De instelling [!DNL Commerce] waarde, verschillende waarden behouden voor [!DNL Commerce] en Amazon winkels.</li><li>**Bestaande Magento&#39;s overschrijven** - Hiermee slaat u de Amazon-waarde op over de [!DNL Commerce] waarde in de [!DNL Commerce] productcatalogus.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Wordt niet weergegeven wanneer u een kenmerk bewerkt als het kenmerk is gemaakt met het gereedschap `Global` bereik. Geeft aan dat de [!DNL Commerce] [bereik](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) is gemaakt en ingesteld op `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | Kies uw [!DNL Commerce] [winkelweergave](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) waarop de Amazon-kenmerkwaarden moeten worden gesynchroniseerd. Kiezen `All Store Views (Global)` Hiermee werkt u de waarde bij in alle weergaven van de winkel. |
