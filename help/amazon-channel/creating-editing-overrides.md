---
title: Overschrijvingen van Amazon-verkoopkanalen maken en bewerken
description: Met overschrijvingen van Amazon-Sales Channel kun je je wijzigingen toepassen op één Amazon-aanbieding of op meerdere aanbiedingen.
feature: Sales Channels, Products, Configuration
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Overschrijvingen maken en bewerken

U kunt een aanbieding maken en overschrijven of een overschrijving bewerken of verwijderen die op een aanbieding is toegepast. Met Overschrijvingen stelt u een gedefinieerde waarde in voor een bepaalde aanbieding.

## Een overschrijving maken voor één aanbieding

De handeling _[!UICONTROL Create Override]_is beschikbaar wanneer u lijsten weergeeft op de tabbladen_[!UICONTROL Inactive]_ , _[!UICONTROL Active]_en_[!UICONTROL Ineligible]_ .

1. Een vermelding op een _[!UICONTROL Products Listings]_pagina (_[!UICONTROL Inactive]_ , _[!UICONTROL Active]_en_[!UICONTROL Ineligible]_ tab) weergeven.

1. Klik in de kolom _[!UICONTROL Action]_op **[!UICONTROL Select]**>**[!UICONTROL Create Override]**om de pagina Overschrijvingen van productaanbiedingen te openen.

   ![ creeer de lijstopheffing van Amazon ](assets/amazon-select-create-override.png){width="220"}

1. Controleer _[!UICONTROL Listing Details]_om te controleren of je de juiste vermelding bekijkt.

1. Bepaal het type overschrijving dat u maakt.

   Je kunt één overschrijvingstype of een combinatie van typen definiëren voor de aanbieding (Prijs, Verwerkingstijd, Voorwaarde, Opmerkingen van verkoper).

   - **Prijs** - klik **[!UICONTROL Change Listing Price]** en ga uw bepaalde prijswaarde voor **[!UICONTROL Price Override]** in.
   - **Behandelingstijd** - klik **[!UICONTROL Change Handling Time]** en ga de bepaalde tijdwaarde (in dagen) voor **[!UICONTROL Handling Time Override]** in.
   - **Voorwaarde** - klik **[!UICONTROL Change Condition]** en kies de correcte optie voor **[!UICONTROL Condition Override]**.
   - **de Nota&#39;s van de Verkoper** - klik **[!UICONTROL Change Seller Notes]** en ga uw notitietekst voor **[!UICONTROL Seller Notes Override]** in.

1. Klik op **[!UICONTROL Save Listing Override]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt gesloten. De status van de vermelding verandert in `Relist in Progress` . De wijziging wordt gepubliceerd naar Amazon met de volgende gegevenssynchronisatie (zoals geconfigureerd in de instellingen voor uitsnijden). De vermelding wordt ook toegevoegd aan het tabblad_[!UICONTROL Overrides]_ .

In het volgende voorbeeld wordt een overschrijving getoond die een nieuwe prijs van `$55` , een nieuwe verwerkingstijd van `1 day` , een nieuwe voorwaarde van `Used; Like New` en nieuwe tekst in de notitie van de verkoper definieert.

![ Voorbeeld Amazon die ](assets/amazon-overrides-edit.png){width="600" zoomable="yes"} van de lijst opneemt

## Een overschrijving voor één aanbieding bewerken of verwijderen {#edit-override-single-listing}

De handeling _[!UICONTROL Edit Overrides]_is beschikbaar wanneer u aanbiedingen weergeeft op het tabblad_[!UICONTROL Overrides]_ .

1. Een vermelding op de pagina _[!UICONTROL Product Listings]_(_[!UICONTROL Overrides]_ tab) weergeven.

1. Klik in de kolom _[!UICONTROL Action]_op **[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt geopend.

   ![ selecteer een de lijstopheffing van Amazon ](assets/amazon-select-edit-overrides.png){width="125"}

1. Controleer _[!UICONTROL Listing Details]_om te controleren of je de juiste aanbieding overschrijft.

1. Als u de instellingen van _[!UICONTROL Override]_wilt bewerken, definieert u de secties voor het type dat u wilt wijzigen (Prijs, Verwerkingstijd, Voorwaarde, Notities van verkoper).

   Selecteer `No Change To <override type>` (de standaardinstelling) om het overschrijvingstype ongewijzigd te laten. Met deze instelling blijft de eerder gedefinieerde overschrijvingswaarde ongewijzigd.

   - **Prijs** - klik **[!UICONTROL Change Listing Price]** en ga uw bepaalde prijswaarde voor **[!UICONTROL Price Override]** in.
   - **Behandelingstijd** - klik **[!UICONTROL Change Handling Time]** en ga de bepaalde tijdwaarde (in dagen) voor **[!UICONTROL Handling Time Override]** in.
   - **Voorwaarde** - klik **[!UICONTROL Change Condition]** en kies de correcte optie voor **[!UICONTROL Condition Override]**.
   - **de Nota&#39;s van de Verkoper** - klik **[!UICONTROL Change Seller Notes]** en ga uw notitietekst voor **[!UICONTROL Seller Notes Override]** in.

1. Om een met voeten getreden type te verwijderen, **verwijdert** voor elk van de types u wilt verwijderen. Als deze niet wordt verwijderd, blijft de eerder gedefinieerde waarde in de overschrijving staan.

1. Klik op **[!UICONTROL Save Listing Override]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt gesloten. De status van de vermelding verandert in `Relist in Progress` . De wijziging wordt gepubliceerd naar Amazon met de volgende gegevenssynchronisatie (zoals geconfigureerd in de instellingen voor uitsnijden). Als deze nog niet wordt vermeld, worden de lijsten ook toegevoegd aan het tabblad_[!UICONTROL Overrides]_ .

Het piggybacks op _leidt tot een Voorbeeld van de Opheffing_. In het volgende voorbeeld wordt een bewerking getoond van de eerder gemaakte overschrijving die een nieuwe prijs van `$50` definieert, wordt de handeling Tijd genegeerd en worden de vorige voorwaarde en de voorwetenschap van de verkoper genegeerd.

![ het uitgeven of het verwijderen van een opheffing ](assets/amazon-overrides-edit-2.png){width="600" zoomable="yes"}
__

## Een overschrijving voor meerdere aanbiedingen bewerken of verwijderen {#edit-override-multiple-listings}

De handeling _[!UICONTROL Edit Listing Overrides]_is beschikbaar op de tabbladen_[!UICONTROL Inactive]_ , _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ en _[!UICONTROL Ineligible]_.

>[!NOTE]
>
>Omdat u overschrijvingen voor meerdere aanbiedingen wijzigt, wordt de sectie _[!UICONTROL Listing Details]_niet weergegeven zoals wanneer u één aanbieding wijzigt.

1. Geef de vermelding weer op een _[!UICONTROL Products Listings]_-pagina (_[!UICONTROL Inactive]_ , _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ en _[!UICONTROL Ineligible]_-tabblad).

1. Schakel het selectievakje in de linkerkolom in voor alle aanbiedingen die u wilt wijzigen.

1. Klik onder _[!UICONTROL Actions]_op **[!UICONTROL Edit Listing Overrides]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt geopend.

   ![ selecteer een de lijstopheffing van Amazon ](assets/amazon-actions-edit-listing-overrides.png){width="200"}

1. Als u de instellingen van _[!UICONTROL Override]_wilt bewerken, definieert u de secties voor het type dat u wilt wijzigen (Prijs, Verwerkingstijd, Voorwaarde, Notities van verkoper).

   Selecteer `No Change To <override type>` (standaardwaarde) als u dezelfde instelling wilt gebruiken. Met deze instelling blijft de eerder gedefinieerde overschrijvingswaarde ongewijzigd.

   - **Prijs** - klik **[!UICONTROL Change Listing Price]** en ga uw bepaalde prijswaarde voor **[!UICONTROL Price Override]** in.
   - **Behandelingstijd** - klik **[!UICONTROL Change Handling Time]** en ga de bepaalde tijdwaarde (in dagen) voor **[!UICONTROL Handling Time Override]** in.
   - **Voorwaarde** - klik **[!UICONTROL Change Condition]** en kies de correcte optie voor **[!UICONTROL Condition Override]**.
   - **de Nota&#39;s van de Verkoper** - klik **[!UICONTROL Change Seller Notes]** en ga uw notitietekst voor **[!UICONTROL Seller Notes Override]** in.

1. Als u een overschrijvingstype wilt verwijderen, klikt u op **[!UICONTROL Remove]** voor elk type dat u wilt verwijderen. Als deze niet wordt verwijderd, blijft de eerder gedefinieerde waarde in de overschrijving staan.

1. Klik op **[!UICONTROL Save Listing Override]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt gesloten. De status van de aanbiedingen verandert in `Relist in Progress` . De wijziging wordt gepubliceerd naar Amazon met de volgende gegevenssynchronisatie (zoals geconfigureerd in de instellingen voor uitsnijden). Als deze nog niet wordt vermeld, worden de lijsten ook toegevoegd aan het tabblad_[!UICONTROL Overrides]_ .

### Typen overschrijven

| Negeren | Beschrijving |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Override] | Een prijsoverschrijving definieert de prijs voor de aanbiedingen. Deze overschrijving heeft voorrang op alle geautomatiseerde instellingen totdat de overschrijving wordt verwijderd.<br><br> om de prijs van uw product met voeten te treden, verkies **[!UICONTROL Change Listing Price]** en ga de nieuwe prijs voor **[!UICONTROL Price Override]** in. |
| [!UICONTROL Handling Time Override] | Met een overschrijvingstijd van de verwerkingstijd wordt de tijd (in dagen) voor het verwerken en verzenden van producten gedefinieerd. Een het behandelen tijdopheffing neemt voorrang over alle geautomatiseerde en standaard behandelingstijdinstellingen tot de opheffing wordt verwijderd.<br><br> de waarde die in het _[!UICONTROL Handling Time Override]_vakje bestaat is of uw standaard behandelingstijd die in uw [ wordt bepaald lijst van montages ](./listing-settings.md) of uw bepaalde met voeten getreden behandelingstijd. Als je een overschrijving van de afhandelingstijd verwijdert, wordt de aanbieding standaard afgehandeld volgens de verwerkingstijd die in de aanbiedingsinstellingen is opgegeven.<br><br> om een het behandelen tijdopheffing te bepalen, verkies **[!UICONTROL Change Handling Time]**en ga de nieuwe behandelingstijd (in dagen) voor **[!UICONTROL Handling Time Override]**in. |
| [!UICONTROL Condition Override] | Om de Lijstvoorwaarde met voeten te treden, verkies **[!UICONTROL Change Condition]** en kies de nieuwe voorwaarde van **Voorkeur met voeten treedt**. |
| [!UICONTROL Seller Notes Override] | Voor producten in uw catalogus die met een andere voorwaarde dan `New` zijn gedefinieerd, kan een verkopersopmerking worden toegevoegd om het product en de toestand ervan voor potentiële kopers nader te beschrijven. U kunt een overschrijving voor verkopersnotities invoeren voor een voorwaardenproduct van `New` , maar Amazon geeft de notitie niet weer.<br><br> Om de Nota&#39;s van de Verkoper met voeten te treden, verkies **[!UICONTROL Change Seller Notes]** en ga de nieuwe nota voor **[!UICONTROL Seller Notes Override]** in. |
