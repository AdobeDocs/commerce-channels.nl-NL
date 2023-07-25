---
title: Verkoopkanaal van Amazon - [!UICONTROL Overrides]
description: Amazon Sales Channel biedt het tabblad Overschrijvingen om te bepalen en te beheren hoe u overschrijvingen toepast in uw Amazon-aanbiedingen.
feature: Sales Channels, Price Rules
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# [!UICONTROL Overrides]

De _[!UICONTROL Overrides]_toont je Amazon-aanbiedingen waarop je een overschrijving hebt toegepast. Een overschrijving is een specifieke instelling voor lijsten die u kunt gebruiken om een gedefinieerde waarde in te stellen op een aanbieding. Een overschrijving die wordt toegepast op een aanbieding, definieert de instelling voor de aanbieding, ongeacht andere gedefinieerde aanbiedingsinstellingen of regels waarvoor de aanbieding in aanmerking komt. Wanneer een overschrijving wordt toegepast op een aanbieding, wordt de vermelding weergegeven op het tabblad_[!UICONTROL Overrides]_ tab. De waarde die in de overschrijving is gedefinieerd, wordt in de desbetreffende kolom voor de lijst weergegeven. Er zijn vier soorten overschrijvingen die kunnen worden toegepast: Prijs, Verwerkingstijd, Voorwaarde en Opmerkingen voor verkopers.

## Typen overschrijvingen

| Type | Beschrijving |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Prijs | Een overschrijving waarmee de prijs van de aanbieding wordt ingesteld, waarbij alle andere prijsinstellingen voor de aanbieding worden genegeerd. <br><br>**Voorbeeld**: U hebt een prijsregel van 20% voor kortingen gedefinieerd die van toepassing is op alle producten in een specifieke categorie van uw catalogus. Je hebt een nieuw product op de markt en de vraag is hoog. Daarom wil je niet dat de verlaagde prijs op de aanbieding wordt toegepast, ook al valt het product in die categorie. Je kunt de aanbieding selecteren, [een prijsoverschrijving maken](./creating-editing-overrides.md#edit-override-single-listing)en definieer de aanbiedingsprijs in een prijsoverschrijving. |
| Verwerkingstijd | Een overschrijving waarmee de verwerkingstijd voor een aanbieding wordt ingesteld, waarbij de standaardverwerkingstijd die in de aanbiedingsinstellingen is ingesteld, wordt genegeerd.<br><br>**Voorbeeld**: De standaardverwerkingstijd voor aanbiedingen is ingesteld op 2 dagen. Je hebt een product dat kwetsbaar is en een extra dag nodig heeft om de speciale verpakking voor de verzending te garanderen. Je kunt de aanbieding bekijken, [een verwerkingstijd overschrijven](./creating-editing-overrides.md#edit-override-single-listing)en definieert de verwerkingstijd op drie dagen.<br><br>**Opmerking:** Niet beschikbaar voor producten die zijn ingesteld op `Fulfilled by Amazon`. |
| Voorwaarde | Een overschrijving waarmee de voorwaardenwaarde van een lijst wordt ingesteld, ongeacht het voorwaardelement dat aan de lijst is toegewezen.<br><br>**Voorbeeld**: De meeste producten in uw catalogus zijn Nieuwe voorwaarde, maar u hebt een product dat in Gereviseerde staat is. Je kunt de aanbieding bekijken, [een voorwaardenoverschrijving maken](./creating-editing-overrides.md#edit-override-single-listing)en definieer de voorwaarde Gereviseerd voor de aanbieding.<br><br>**Opmerking:** Niet beschikbaar voor producten die zijn ingesteld op `Fulfilled by Amazon`. |
| Opmerkingen van verkoper | Een overschrijving die de instelling _Opmerkingen van verkoper_ van de aanbieding. Dit veld kan worden gebruikt om aanvullende informatie toe te voegen met betrekking tot het product of de toegepaste overschrijving, die doorgaans wordt gebruikt om de conditie van &quot;niet-nieuwe&quot; producten te beschrijven. Tekst in dit veld wordt weergegeven met de vermelding voor de winkels. Opmerkingen van verkopers kunnen niet worden toegevoegd voor een aanbieding met een voorwaardenwaarde van `New`. <br><br>**Voorbeeld**: U hebt een product waarin `Refurbished` voorwaarde. Normaal gesproken bevatten producten in deze voorwaarde geen handleidingen of documenten, maar u hebt een andere leverancier voor dit product die een handleiding bevat. Je kunt de aanbieding bekijken, [een overschrijving voor verkopersnotities maken](./creating-editing-overrides.md#edit-override-single-listing)en voeg uw tekstnotitie die uniek is voor deze aanbieding toe aan de handleiding, zodat de verkoper weet dat deze is opgenomen.<br><br>**Opmerking**: Als een product een bepaalde voorwaarde heeft van `New`, kun je overschrijvingen van verkopersaantekeningen invoeren, maar Amazon geeft geen verkopersaantekeningen voor een `New` product. |

U kunt een overschrijving maken, bewerken of verwijderen [enkele aanbieding](./creating-editing-overrides.md#edit-override-single-listing). Op de _[!UICONTROL Inactive]_,_[!UICONTROL Active]_, en _[!UICONTROL Ineligible]_tabs, kunt u klikken **[!UICONTROL Select]**in de_[!UICONTROL Action]_ kolom en kies **[!UICONTROL Create Override]**. De _[!UICONTROL Edit Overrides]_De handeling is alleen beschikbaar als een aanbieding een overschrijving heeft en wordt weergegeven op het tabblad_[!UICONTROL Overrides]_ tab.

U kunt ook een overschrijving maken, bewerken of verwijderen [meerdere aanbiedingen](./creating-editing-overrides.md#edit-override-multiple-listings). Op de _[!UICONTROL Inactive]_,_[!UICONTROL Active]_, en _[!UICONTROL Ineligible]_tabs, kunt u klikken **[!UICONTROL Select]**in de_[!UICONTROL Action]_ kolom en kies **[!UICONTROL Edit Listing Overrides]**.

Als je een overschrijving verwijdert, weet de aanbieding dat ze de waarden moet gebruiken die door de instellingen en regels van je aanbieding worden gedefinieerd.

Wanneer u een overschrijving definieert, kunt u ook één type overschrijving of een combinatie van de typen invoeren.

Zie [Overschrijvingen maken en bewerken](./creating-editing-overrides.md).

>[!NOTE]
>
>Als je aanbiedingen in behandeling hebt, wordt het aantal aanbiedingen weergegeven in een bericht boven de tabbladen.

![Het tabblad Overschrijvingen](assets/amazon-overrides.png){width="600" zoomable="yes"}

Homepages van Amazon-verkoopkanalen delen [besturingselementen voor werkruimte](./workspace-controls.md) waarmee u de weergegeven gegevens kunt aanpassen.

## Standaardkolommen

| Kolom | Beschrijving |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br>ASIN staat voor de Amazon Standard Identification Numbers. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Condition Override] | De nieuwe voorwaarde die in de opheffing wordt bepaald. Als de overschrijving die op de lijst is toegepast geen voorwaardenoverschrijving is, `Not Selected` in deze kolom. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Seller Notes Override] | De nieuwe verkopersnotities die in de overschrijving zijn gedefinieerd. Als de overschrijving die op de lijst is toegepast, niet dit type overschrijving is, is deze kolom leeg. |
| [!UICONTROL Handling Override] | De nieuwe verwerkingstijd die is gedefinieerd in de overschrijving (in dagen). Als de overschrijving die op de lijst is toegepast, geen overschrijving is, is deze kolom leeg. |
| [!UICONTROL List Price Override] | De nieuwe aanbiedingsprijs die in de overschrijving is gedefinieerd. Als de overschrijving die op de aanbieding wordt toegepast geen prijsoverschrijving is, `N/A` in deze kolom. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, gaat u naar _[!UICONTROL Action]_kolom, klikt u op **[!UICONTROL Select]**en kies een optie:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
