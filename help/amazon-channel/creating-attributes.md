---
title: Kenmerken voor Amazon-verkoopkanalen maken en bewerken
description: Amazon-Sales Channel biedt de weergave Kenmerken om u te helpen de huidige Amazon-kenmerken en gekoppelde Commerce-kenmerken te bekijken.
feature: Sales Channels, Products, Configuration
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# Kenmerken maken en bewerken

Maak of werk [!DNL Commerce] -kenmerken bij terwijl u via Amazon verkoopt en werk uw winkels bij. Bekijk de huidige Amazon-kenmerken en gekoppelde [!DNL Commerce] -kenmerken via de [_[!UICONTROL Attributes]_view ](./attributes-view.md) van de startpagina van het Amazon-verkoopkanaal. In de kolom_[!UICONTROL Action]_ worden de beschikbare acties voor het kenmerk weergegeven. U kunt een nieuw [!DNL Commerce] -kenmerk maken en toewijzen voor een ongekoppeld Amazon-kenmerk, of een bestaand [!DNL Commerce] -kenmerk en de toewijzing ervan aan een Amazon-kenmerk bewerken.

Wanneer u kenmerken maakt en bijwerkt, kunt u de kenmerkwaarden voor [!DNL Commerce] - en Amazon-producten controleren. Deze waarden kunnen afwijken als u geen waarden synchroniseert en importeert uit Amazon. Om de waarden van Amazon voor deze attributen te herzien, zie [ het Reviseren van de Toewijzing van Attributen van Amazon ](./amazon-matching-attributes-values.md). Als u die waarden wilt veranderen, kunt u [ uitgeven of een afbeelding ](./amazon-manually-update-incomplete-listing.md) tussen Amazon en [!DNL Commerce] tot stand brengen.

## Een kenmerk maken {#create-an-attribute}

Met deze stappen maakt u een [!DNL Commerce] -kenmerk en wijst u dit toe aan een Amazon-kenmerk. Afhankelijk van configuraties, kunnen de waarden beginnen tussen catalogi te synchroniseren.

1. Voor _Admin_ sidebar, ga **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klik op **[!UICONTROL Attributes]** in het linkermenu, zoek een Amazon-kenmerk en klik op **[!UICONTROL Create Attribute]** in de kolom _[!UICONTROL Action]_.

1. Als u de synchronisatie van de Amazon-waarden met het gekoppelde [!DNL Commerce] -kenmerk wilt inschakelen, stelt u **[!UICONTROL Is Active]** in op `Yes` .

   Als u deze optie instelt op `Yes` , worden de waarden gesynchroniseerd op basis van uw configuratie.

1. Kies `Create New Magento Attribute` voor **[!UICONTROL Select Magento Product Attribute]** .

   Het kenmerk verwijst naar het kenmerk dat u hebt gekozen voor **[!UICONTROL Amazon Attribute Name]** .

1. Voer een **[!UICONTROL Magento Product Attribute Name]** in.

1. Voer een **[!UICONTROL Magento Product Attribute Code]** in.

   Deze waarde moet allemaal in kleine letters en zonder spaties zijn.

1. Kies bij **[!UICONTROL Attribute Set Ids]** een kenmerkset die u wilt toewijzen.

   Kenmerken maken doorgaans deel uit van een kenmerkset, zoals een set voor kleuren met kenmerken voor blauw, groen, geel en rood.

1. Kies bij **[!UICONTROL Type]** het type kenmerkwaarde, zoals tekst en getallen.

   Deze optie beïnvloedt de toegestane waarde voor het attribuut.

1. Stel voor **[!UICONTROL Use for Promo Rule Conditions]** in op `Yes` om toe te staan dat het kenmerk beschikbaar is voor een parameter binnen uw promotievoorwaarden.

1. Stel voor **[!UICONTROL Used in Search]** in op `Yes` als het kenmerk en de waarde kunnen worden gebruikt in productzoekopdrachten.

1. Stel voor **[!UICONTROL Comparable on Storefront]** de waarde in op `Yes` als de kenmerkwaarde kan worden gebruikt in de Amazon-functionaliteit &quot;Vergelijken via&quot;.

1. Kies het [!DNL Commerce] [ werkingsgebied ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) voor de attributen, en selecteer dan één of meerdere Mening van de Opslag om de waarden van Amazon in in te voeren.

   Als het bereik is ingesteld op `Global` , kan _[!UICONTROL Store View]_niet worden gewijzigd nadat het kenmerk is gemaakt.

   Als u `All Store Views (Global)` kiest, worden waarden gesynchroniseerd en opgeslagen in al uw Amazon-winkelweergaven. U kunt waarden alleen synchroniseren met specifieke winkelweergaven.

1. Klik op **[!UICONTROL Save Attribute Settings]** als de bewerking is voltooid.

Nadat u het kenmerk hebt opgeslagen, wilt u het kenmerk mogelijk bewerken om de instellingen te bekijken en de Amazon- en [!DNL Commerce] -waarden voor het kenmerk te vergelijken. U kunt ook aangeven of Amazon-waarden [!DNL Commerce] -waarden moeten overschrijven.

![ creeer attributenmontages ](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Geeft aan of dit kenmerk live is en actief synchroniseert tussen Amazon en [!DNL Commerce] . Stel in op `Yes` om ervoor te zorgen dat de kenmerkwaarden van Amazon gelijk blijven en dat [!DNL Commerce] synchroon blijft voor het geselecteerde kenmerk. |
| Productkenmerk Magento selecteren | Geeft het geselecteerde kenmerk aan dat u wilt koppelen aan de vermelde Amazon-kenmerknaam. Kies `Create New Magento Attribute` wanneer u een kenmerk maakt. |
| [!UICONTROL Amazon Attribute Name] | Hiermee geeft u de naam weer van het Amazon-kenmerk dat u hebt gekozen. De geselecteerde kenmerkkoppelingen naar dit Amazon-kenmerk. U kunt deze waarde niet bewerken via [!DNL Commerce] . |
| [!UICONTROL Magento Product Attribute Name] | Geeft de kenmerknaam of &quot;label&quot; aan. |
| [!UICONTROL Magento Product Attribute Code] | Geeft de kenmerkcode aan, allemaal in kleine letters zonder spaties. |
| [!UICONTROL Attribute Set Ids] | Geeft de kenmerkset aan waaraan het kenmerk moet worden toegewezen. Kenmerken maken doorgaans deel uit van een kenmerkset, zoals een set voor kleuren met kenmerken voor blauw, groen, geel en rood. |
| [!UICONTROL Type] | Geeft het waardetype van de kenmerkwaarde aan, zoals tekst en getallen. De selectie heeft invloed op de toegestane waarde voor het kenmerk. |
| [!UICONTROL Use for Promo Rule Conditions] | Schakel over naar `Yes` als u wilt dat het kenmerk beschikbaar is voor een parameter binnen uw promotievoorwaarden. |
| [!UICONTROL Used in Search] | Geeft aan of het kenmerk en de waarde kunnen worden gebruikt in productzoekopdrachten. |
| [!UICONTROL Comparable on Storefront] | Geeft aan of de kenmerkwaarde kan worden gebruikt in de Amazon-functionaliteit &quot;Vergelijken door&quot;. |
| [!UICONTROL Magento Product Attribute Scope] | Wijst op het [ werkingsgebied ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) voor de attributen. Opties: Globale Mening / de Mening van de Opslag <br> Wanneer geplaatst aan `Global`, kan de Mening van de Opslag niet worden uitgegeven nadat het attribuut wordt gecreeerd. |
| [!UICONTROL Store Views (to import values into to)] | Wordt alleen weergegeven wanneer het bereik is ingesteld op `Store View` . Kies de [ opslagmening ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) waaraan de de attributenwaarden van Amazon worden gesynchroniseerd. Als u `All Store Views (Global)` kiest, wordt de waarde bijgewerkt in alle [!DNL Commerce] -winkelweergaven. |

## Een kenmerk bewerken {#edit-an-attribute}

1. Voor _Admin_ sidebar, ga **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klik op **[!UICONTROL Attributes]** in het linkermenu, zoek een Amazon-kenmerk en klik op **[!UICONTROL Edit]** in de kolom _[!UICONTROL Action]_.

1. Om het synchroniseren van de waarden van Amazon aan het verbonden [!DNL Commerce] attribuut toe te laten of onbruikbaar te maken, is de reeks **Actief** aan `Yes` of `No`.

   Als u deze optie instelt op `Yes` , worden de waarden gesynchroniseerd op basis van uw configuratie.

1. Verifieer of werk voor **[!UICONTROL Select Magento Product Attribute]** het kenmerk bij om het toe te wijzen aan de gekozen **[!UICONTROL Amazon Attribute Name]** .

1. Geef aan of u de bestaande kenmerkwaarde van de binnenkomende Amazon wilt overschrijven.

   U kunt bijvoorbeeld de prijzen van Amazon in [!DNL Commerce] niet overschrijven.

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Behoudt de waarde en behoudt verschillende waarden voor de [!DNL Commerce] - en Amazon-winkels.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Hiermee vervangt u de waarde in de productcatalogus van [!DNL Commerce] door de inkomende Amazon-waarde.

1. Kies een of meer **[!UICONTROL Store Views (to import Amazon values into)]** indien beschikbaar voor bewerken.

   Als het attribuut met a `Global` werkingsgebied werd gecreeerd, kan de _Mening van de Opslag_ niet worden veranderd nadat het attribuut wordt gecreeerd.

   Als u `All Store Views (Global)` kiest, worden waarden gesynchroniseerd en opgeslagen in alle weergaven van de winkel. U kunt waarden alleen synchroniseren met specifieke winkelweergaven.

1. Klik op **[!UICONTROL Save Attribute Settings]** als de bewerking is voltooid.

![ geef attributenmontages uit ](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Geeft aan of dit kenmerk live is en actief synchroniseert tussen Amazon en [!DNL Commerce] . Stel in op `Yes` om ervoor te zorgen dat de kenmerkwaarden van Amazon gelijk blijven en dat [!DNL Commerce] synchroon blijft voor het geselecteerde kenmerk. |
| [!UICONTROL Select Magento Product Attribute] | Geeft het geselecteerde [!DNL Commerce] -kenmerk aan dat u wilt koppelen aan de vermelde Amazon-kenmerknaam. Als u het gekoppelde [!DNL Commerce] -kenmerk wilt wijzigen, kiest u een ander kenmerk in de vervolgkeuzelijst. De waarden worden gesynchroniseerd op basis van configuraties. |
| [!UICONTROL Amazon Attribute Name] | Hiermee geeft u de naam van het Amazon-kenmerk weer, zoals gedefinieerd in [!DNL Amazon Seller Central] . Het geselecteerde [!DNL Commerce] -kenmerk is gekoppeld aan dit Amazon-kenmerk. U kunt deze waarde niet bewerken via [!DNL Commerce] . |
| [!UICONTROL Overwrite Existing Value] | Geeft aan of de Amazon-kenmerkwaarden bestaande [!DNL Commerce] -waarden overschrijven, wat van invloed is op alle producten met dit [!DNL Commerce] -kenmerk.<ul><li>**overschrijft geen Bestaande Waarden van het Magento** - (Gebrek) behoudt de [!DNL Commerce] waarde, die verschillende waarden voor [!DNL Commerce] en Amazon bewaart.</li><li>**beschrijft Bestaande Waarden van het Magento** - bewaart de waarde van Amazon over de [!DNL Commerce] waarde in de [!DNL Commerce] productcatalogus.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Wordt niet weergegeven wanneer u een kenmerk bewerkt als het kenmerk is gemaakt met het bereik `Global` . Wijst erop dat het [!DNL Commerce] [ werkingsgebied ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) werd gecreeerd en aan `Store View` werd geplaatst. |
| [!UICONTROL Store Views (to import values into to)] | Kies uw [!DNL Commerce] [ opslagmening ](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) waaraan om de attributenwaarden van Amazon te synchroniseren. Als u `All Store Views (Global)` kiest, wordt de waarde bijgewerkt in alle winkelweergaven. |
