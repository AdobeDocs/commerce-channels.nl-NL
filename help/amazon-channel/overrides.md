---
title: Overschrijvingen
description: Amazon Sales Channel biedt het tabblad Overschrijvingen om te bepalen en te beheren hoe u overschrijvingen toepast in uw Amazon-aanbiedingen.
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Overschrijvingen

Op het tabblad _[!UICONTROL Overrides]_worden de Amazon-aanbiedingen weergegeven waarop u een overschrijving hebt toegepast. Een overschrijving is een specifieke instelling voor lijsten die u kunt gebruiken om een gedefinieerde waarde in te stellen op een aanbieding. Een overschrijving die wordt toegepast op een aanbieding, definieert de instelling voor de aanbieding, ongeacht andere gedefinieerde aanbiedingsinstellingen of regels waarvoor de aanbieding in aanmerking komt. Wanneer een overschrijving wordt toegepast op een lijst, wordt de vermelding weergegeven op het tabblad_[!UICONTROL Overrides]_. De waarde die in de overschrijving is gedefinieerd, wordt in de desbetreffende kolom voor de lijst weergegeven. Er zijn vier soorten overschrijvingen die kunnen worden toegepast: Prijs, Verwerkingstijd, Voorwaarde en Opmerkingen voor verkopers.

## Typen overschrijvingen

| Type | Beschrijving |
|---|---|
| Prijs | Een overschrijving waarmee de prijs van de aanbieding wordt ingesteld, waarbij alle andere prijsinstellingen voor de aanbieding worden genegeerd. <br><br>**Voorbeeld**: U hebt een prijsregel van 20% voor kortingen gedefinieerd die van toepassing is op alle producten in een specifieke categorie van uw catalogus. Je hebt een nieuw product op de markt en de vraag is hoog. Daarom wil je niet dat de verlaagde prijs op de aanbieding wordt toegepast, ook al valt het product in die categorie. U kunt de aanbieding selecteren, [een prijsoverschrijving maken](./creating-editing-overrides.md#edit-override-single-listing) en de aanbiedingsprijs definiëren in een prijsoverschrijving. |
| Verwerkingstijd | Een overschrijving waarmee de verwerkingstijd voor een aanbieding wordt ingesteld, waarbij de standaardverwerkingstijd die in de aanbiedingsinstellingen is ingesteld, wordt genegeerd.<br><br>**Voorbeeld**: Je standaardverwerkingstijd voor aanbiedingen is ingesteld op 2 dagen. Je hebt een product dat kwetsbaar is en een extra dag nodig heeft om de speciale verpakking voor de verzending te garanderen. U kunt de lijst bekijken, [een behandelingstijd met voeten treden](./creating-editing-overrides.md#edit-override-single-listing), en de behandelingstijd bepalen op drie dagen.<br><br>**Opmerking:** niet beschikbaar voor producten die zijn ingesteld op  `Fulfilled by Amazon`. |
| Voorwaarde | Een overschrijving waarmee de voorwaardenwaarde van een lijst wordt ingesteld, ongeacht het voorwaardelement dat aan de lijst is toegewezen.<br><br>**Voorbeeld**: De meeste producten in uw catalogus zijn Nieuwe voorwaarde, maar u hebt een product dat in Gereviseerde staat is. U kunt de vermelding weergeven, [een voorwaardenoverschrijving maken](./creating-editing-overrides.md#edit-override-single-listing) en de voorwaarde Gereviseerd voor de aanbieding definiëren.<br><br>**Opmerking:** niet beschikbaar voor producten die zijn ingesteld op  `Fulfilled by Amazon`. |
| Opmerkingen van verkoper | Een overschrijving die de sectie _Seller Notes_ van de aanbieding bepaalt. Dit veld kan worden gebruikt om aanvullende informatie toe te voegen met betrekking tot het product of de toegepaste overschrijving, die doorgaans wordt gebruikt om de conditie van &quot;niet-nieuwe&quot; producten te beschrijven. Tekst in dit veld wordt weergegeven met de vermelding voor de winkels. Notities van verkopers kunnen niet worden toegevoegd voor een aanbieding met een voorwaardenwaarde van `New`. <br><br>**Voorbeeld**: Je hebt een product dat in  `Refurbished` staat is. Normaal gesproken bevatten producten in deze voorwaarde geen handleidingen of documenten, maar u hebt een andere leverancier voor dit product die een handleiding bevat. Je kunt de aanbieding bekijken, [een overschrijving met opmerkingen voor de verkoper maken](./creating-editing-overrides.md#edit-override-single-listing) en je tekstopmerking die uniek is voor deze aanbieding in de handleiding toevoegen zodat de verkoper weet dat deze is opgenomen.<br><br>**Opmerking**: Als voor een product een gedefinieerde voorwaarde geldt van  `New`, kun je overschrijvingen van verkopersaantekeningen invoeren, maar geeft Amazon geen verkopersaantekeningen voor een  `New` product weer. |

U kunt een overschrijving maken, bewerken of verwijderen voor een [enkele vermelding](./creating-editing-overrides.md#edit-override-single-listing). Op _[!UICONTROL Inactive]_,_[!UICONTROL Active]_, en _[!UICONTROL Ineligible]_lusjes, kunt u **[!UICONTROL Select]**in &lt;a4 klikken en **[!UICONTROL Create Override]**kiezen._[!UICONTROL Action]_ De handeling _[!UICONTROL Edit Overrides]_is alleen beschikbaar wanneer op een lijst een overschrijving is toegepast en wordt weergegeven op het tabblad_[!UICONTROL Overrides]_.

U kunt ook een overschrijving naar [meerdere aanbiedingen](./creating-editing-overrides.md#edit-override-multiple-listings) maken, bewerken of verwijderen. Op _[!UICONTROL Inactive]_,_[!UICONTROL Active]_, en _[!UICONTROL Ineligible]_lusjes, kunt u **[!UICONTROL Select]**in &lt;a4 klikken en **[!UICONTROL Edit Listing Overrides]**kiezen._[!UICONTROL Action]_

Als je een overschrijving verwijdert, weet de aanbieding dat ze de waarden moet gebruiken die door de instellingen en regels van je aanbieding worden gedefinieerd.

Wanneer u een overschrijving definieert, kunt u ook één type overschrijving of een combinatie van de typen invoeren.

Zie [Overschrijvingen maken en bewerken](./creating-editing-overrides.md).

>[!NOTE]
>
>Als je aanbiedingen in behandeling hebt, wordt het aantal aanbiedingen weergegeven in een bericht boven de tabbladen.

![Het tabblad Overschrijvingen](assets/amazon-overrides.png)

Amazon-homepages van verkoopkanalen hebben gemeenschappelijke [besturingselementen voor werkruimten](./workspace-controls.md) waarmee u de weergegeven gegevens kunt aanpassen.

## Standaardkolommen

| Kolom | Beschrijving |
|---|---|
| [!UICONTROL Amazon Seller SKU] | De SKU (Stock Keeping Unit) die door Amazon aan een product wordt toegewezen om het product, de opties, de prijs, en de fabrikant te identificeren. |
| [!UICONTROL ASIN] | Een uniek blok van 10 letters en/of cijfers dat items identificeert.<br><br>ASIN staat voor de Amazon Standard Identification Numbers. Een ASIN is een uniek blok van 10 letters en/of getallen dat items identificeert. Voor boeken, is ASIN het zelfde als het aantal ISBN, maar voor alle andere producten wordt een nieuwe ASIN gecreeerd wanneer het punt aan hun catalogus wordt geupload. Je vindt een artikel in ASIN op de productdetailpagina op Amazon, samen met meer informatie over het object. |
| [!UICONTROL Condition Override] | De nieuwe voorwaarde die in de opheffing wordt bepaald. Als de overschrijving die op de lijst is toegepast geen voorwaardenoverschrijving is, wordt `Not Selected` in deze kolom weergegeven. |
| [!UICONTROL Product Listing Name] | De naam van het product. |
| [!UICONTROL Seller Notes Override] | De nieuwe verkopersnotities die in de overschrijving zijn gedefinieerd. Als de overschrijving die op de lijst is toegepast, niet dit type overschrijving is, is deze kolom leeg. |
| [!UICONTROL Handling Override] | De nieuwe verwerkingstijd die is gedefinieerd in de overschrijving (in dagen). Als de overschrijving die op de lijst is toegepast, geen overschrijving is, is deze kolom leeg. |
| [!UICONTROL List Price Override] | De nieuwe aanbiedingsprijs die in de overschrijving is gedefinieerd. Als de overschrijving die op de aanbieding wordt toegepast geen prijsoverschrijving is, wordt `N/A` in deze kolom weergegeven. |
| [!UICONTROL Action] | Lijst met beschikbare acties die kunnen worden toegepast op een specifieke aanbieding. Als u een handeling wilt toepassen, klikt u in de kolom _[!UICONTROL Action]_op **[!UICONTROL Select]**en kiest u een optie:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
