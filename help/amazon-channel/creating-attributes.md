---
title: Kenmerken maken en bewerken
description: Amazon Sales Channel biedt de weergave Kenmerken om u te helpen de huidige Amazon-kenmerken en gekoppelde Commerce-kenmerken te bekijken.
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Kenmerken maken en bewerken

Maak of werk [!DNL Commerce]-kenmerken bij terwijl u via Amazon verkoopt en werk uw winkels bij. Bekijk de huidige Amazon-kenmerken en de gekoppelde [!DNL Commerce]-kenmerken via de [_[!UICONTROL Attributes]_-weergave](./attributes-view.md) van de startpagina van het Amazon-verkoopkanaal. In de kolom_[!UICONTROL Action]_ worden de beschikbare acties voor het kenmerk weergegeven. U kunt of een nieuw [!DNL Commerce] attribuut voor een ongekoppeld attribuut van Amazon tot stand brengen en in kaart brengen, of u kunt bestaande [!DNL Commerce] attributen en zijn afbeelding aan een attribuut van Amazon uitgeven.

Wanneer u kenmerken maakt en bijwerkt, kunt u de kenmerkwaarden voor [!DNL Commerce]- en Amazon-producten controleren. Deze waarden kunnen afwijken als u geen waarden synchroniseert en importeert uit Amazon. Zie [Toewijzing Amazon-kenmerk controleren](./amazon-matching-attributes-values.md) voor een overzicht van Amazon-waarden voor deze kenmerken. Als u deze waarden wilt wijzigen, kunt u [een toewijzing](./amazon-manually-update-incomplete-listing.md) tussen Amazon en [!DNL Commerce] bewerken of maken.

## Een kenmerk maken {#create-an-attribute}

Met deze stappen wordt een [!DNL Commerce]-kenmerk gemaakt en toegewezen aan een Amazon-kenmerk. Afhankelijk van configuraties, kunnen de waarden beginnen tussen catalogi te synchroniseren.

1. Ga op de zijbalk _Admin_ naar **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klik **[!UICONTROL Attributes]** in het linkerzijmenu, bepaal de plaats van een attribuut van Amazon, en klik **[!UICONTROL Create Attribute]** in _[!UICONTROL Action]_kolom.

1. Als u de synchronisatie van de Amazon-waarden met het gekoppelde [!DNL Commerce]-kenmerk wilt inschakelen, stelt u **[!UICONTROL Is Active]** in op `Yes`.

   Wanneer ingesteld op `Yes`, worden de waarden gesynchroniseerd op basis van uw configuratie.

1. Kies `Create New Magento Attribute` voor **[!UICONTROL Select Magento Product Attribute]**.

   Het kenmerk verwijst naar het kenmerk dat voor **[!UICONTROL Amazon Attribute Name]** is gekozen.

1. Voer een **[!UICONTROL Magento Product Attribute Name]** in.

1. Voer een **[!UICONTROL Magento Product Attribute Code]** in.

   Deze waarde moet allemaal in kleine letters en zonder spaties zijn.

1. Kies voor **[!UICONTROL Attribute Set Ids]** een kenmerkset die u wilt toewijzen.

   Kenmerken maken doorgaans deel uit van een kenmerkset, zoals een set voor kleuren met kenmerken voor blauw, groen, geel en rood.

1. Kies bij **[!UICONTROL Type]** het type van de kenmerkwaarde, zoals tekst en getallen.

   Deze optie beïnvloedt de toegestane waarde voor het attribuut.

1. Stel **[!UICONTROL Use for Promo Rule Conditions]** in op `Yes` om toe te staan dat het kenmerk beschikbaar is voor een parameter binnen uw promotievoorwaarden.

1. Stel voor **[!UICONTROL Used in Search]** in op `Yes` als het kenmerk en de waarde kunnen worden gebruikt in productzoekopdrachten.

1. Stel voor **[!UICONTROL Comparable on Storefront]** in op `Yes` als de kenmerkwaarde kan worden gebruikt in de Amazon-functionaliteit &quot;Vergelijken door&quot;.

1. Kies [!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;} voor het attribuut, en selecteer dan één of meerdere Mening van de Opslag om de waarden van Amazon in in te voeren.

   Als het bereik is ingesteld op `Global`, kan _[!UICONTROL Store View]_niet worden gewijzigd nadat het kenmerk is gemaakt.

   Als u `All Store Views (Global)` kiest, worden waarden gesynchroniseerd en opgeslagen in al uw Amazon-winkelweergaven. U kunt waarden alleen synchroniseren met specifieke winkelweergaven.

1. Klik op **[!UICONTROL Save Attribute Settings]** als u klaar bent.

Nadat u het kenmerk hebt opgeslagen, wilt u het kenmerk mogelijk bewerken om de instellingen te bekijken en de Amazon- en [!DNL Commerce]-waarden voor het kenmerk aan te passen. U kunt ook aangeven of Amazon-waarden [!DNL Commerce]-waarden moeten overschrijven.

![kenmerkinstellingen maken](assets/amazon-attribute-settings-create.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Is Active] | Geeft aan of dit kenmerk live en actief wordt gesynchroniseerd tussen Amazon en [!DNL Commerce]. Stel in op `Yes` om ervoor te zorgen dat de kenmerkwaarden van Amazon gesynchroniseerd blijven en [!DNL Commerce] gesynchroniseerd blijven voor het geselecteerde kenmerk. |
| Magento-productkenmerk selecteren | Geeft het geselecteerde kenmerk aan dat u wilt koppelen aan de vermelde Amazon-kenmerknaam. Kies `Create New Magento Attribute` wanneer u een kenmerk maakt. |
| [!UICONTROL Amazon Attribute Name] | Hiermee geeft u de naam weer van het Amazon-kenmerk dat u hebt gekozen. De geselecteerde kenmerkkoppelingen naar dit Amazon-kenmerk. U kunt deze waarde niet bewerken via [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | Geeft de kenmerknaam of &quot;label&quot; aan. |
| [!UICONTROL Magento Product Attribute Code] | Geeft de kenmerkcode aan, allemaal in kleine letters zonder spaties. |
| [!UICONTROL Attribute Set Ids] | Geeft de kenmerkset aan waaraan het kenmerk moet worden toegewezen. Kenmerken maken doorgaans deel uit van een kenmerkset, zoals een set voor kleuren met kenmerken voor blauw, groen, geel en rood. |
| [!UICONTROL Type] | Geeft het waardetype van de kenmerkwaarde aan, zoals tekst en getallen. De selectie heeft invloed op de toegestane waarde voor het kenmerk. |
| [!UICONTROL Use for Promo Rule Conditions] | Schakel over naar `Yes` om toe te staan dat het kenmerk beschikbaar is voor een parameter binnen uw promotievoorwaarden. |
| [!UICONTROL Used in Search] | Geeft aan of het kenmerk en de waarde kunnen worden gebruikt in productzoekopdrachten. |
| [!UICONTROL Comparable on Storefront] | Geeft aan of de kenmerkwaarde kan worden gebruikt in de Amazon-functionaliteit &quot;Vergelijken door&quot;. |
| [!UICONTROL Magento Product Attribute Scope] | Wijst op [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;} voor het attribuut. Opties: Globale weergave / Winkelweergave<br>Wanneer deze is ingesteld op `Global`, kan de Winkelweergave niet worden bewerkt nadat het kenmerk is gemaakt. |
| [!UICONTROL Store Views (to import values into to)] | Wordt alleen weergegeven wanneer het bereik is ingesteld op `Store View`. Kies [store view](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} waaraan de Amazon-kenmerkwaarden worden gesynchroniseerd. Als u `All Store Views (Global)` kiest, wordt de waarde bijgewerkt in alle [!DNL Commerce]-opslagweergaven. |

## Een kenmerk bewerken {#edit-an-attribute}

1. Ga op de zijbalk _Admin_ naar **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klik **[!UICONTROL Attributes]** in het linkerzijmenu, bepaal de plaats van een attribuut van Amazon, en klik **[!UICONTROL Edit]** in _[!UICONTROL Action]_kolom.

1. Als u de synchronisatie van de Amazon-waarden met het gekoppelde [!DNL Commerce]-kenmerk wilt in- of uitschakelen, stelt u **Is Active** in op `Yes` of `No`.

   Wanneer ingesteld op `Yes`, worden de waarden gesynchroniseerd op basis van uw configuratie.

1. Verifieer of werk voor **[!UICONTROL Select Magento Product Attribute]** het kenmerk bij om het toe te wijzen aan de gekozen **[!UICONTROL Amazon Attribute Name]**.

1. Geef aan of u de bestaande kenmerkwaarde van de binnenkomende Amazon wilt overschrijven.

   U kunt bijvoorbeeld de prijzen van Amazon in [!DNL Commerce] niet overschrijven.

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Hiermee behoudt u de waarde en behoudt u verschillende waarden voor uw  [!DNL Commerce] en Amazon-winkels.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Hiermee overschrijft u de waarde in de  [!DNL Commerce] productcatalogus met de inkomende Amazon-waarde.

1. Kies een of meer **[!UICONTROL Store Views (to import Amazon values into)]**, indien beschikbaar voor bewerken.

   Als het attribuut met een `Global` werkingsgebied werd gecreeerd, kan _de Mening van de Opslag_ niet worden veranderd nadat het attribuut wordt gecreeerd.

   Als u `All Store Views (Global)` kiest, synchroniseert het en bewaart waarden aan alle opslagmeningen. U kunt waarden alleen synchroniseren met specifieke winkelweergaven.

1. Klik op **[!UICONTROL Save Attribute Settings]** als u klaar bent.

![kenmerkinstellingen bewerken](assets/amazon-attribute-settings-edit.png)

| Veld | Beschrijving |
|--- |--- |
| [!UICONTROL Is Active] | Geeft aan of dit kenmerk live en actief wordt gesynchroniseerd tussen Amazon en [!DNL Commerce]. Stel in op `Yes` om ervoor te zorgen dat de kenmerkwaarden van Amazon gesynchroniseerd blijven en [!DNL Commerce] gesynchroniseerd blijven voor het geselecteerde kenmerk. |
| [!UICONTROL Select Magento Product Attribute] | Geeft het geselecteerde [!DNL Commerce]-kenmerk aan dat u wilt koppelen aan de vermelde Amazon-kenmerknaam. Als u het gekoppelde [!DNL Commerce]-kenmerk wilt wijzigen, kiest u een ander kenmerk in de vervolgkeuzelijst. De waarden worden gesynchroniseerd op basis van configuraties. |
| [!UICONTROL Amazon Attribute Name] | Hiermee geeft u de naam van het Amazon-kenmerk weer zoals gedefinieerd in [!DNL Amazon Seller Central]. De geselecteerde [!DNL Commerce] attribuutverbindingen aan dit attribuut van Amazon. U kunt deze waarde niet bewerken via [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Geeft aan of de Amazon-kenmerkwaarden bestaande [!DNL Commerce]-waarden overschrijven, wat van invloed is op alle producten met dit [!DNL Commerce]-kenmerk.<ul><li>**Bestaande Magento-waarden**  niet overschrijven - (standaardinstelling) behoudt de  [!DNL Commerce] waarde en behoudt verschillende waarden voor  [!DNL Commerce] en Amazon-winkels.</li><li>**Bestaande Magento-waarden**  overschrijven - Hiermee slaat u de Amazon-waarde op over de  [!DNL Commerce] waarde in de  [!DNL Commerce] productcatalogus.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Wordt niet weergegeven wanneer u een kenmerk bewerkt als het kenmerk is gemaakt met het bereik `Global`. Geeft aan dat [!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;} is gemaakt en ingesteld op `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | Kies uw [!DNL Commerce] [opslagmening](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} waarnaar de Amazon-kenmerkwaarden moeten worden gesynchroniseerd. Als u `All Store Views (Global)` kiest, wordt de waarde bijgewerkt in alle winkelweergaven. |
