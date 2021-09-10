---
title: Overschrijvingen maken en bewerken
description: Met Amazon Sales Channel overschrijven kun je je wijzigingen toepassen op één Amazon-aanbieding of op meerdere aanbiedingen.
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Overschrijvingen maken en bewerken

U kunt een aanbieding maken en overschrijven of een overschrijving bewerken of verwijderen die op een aanbieding is toegepast. Met Overschrijvingen stelt u een gedefinieerde waarde in voor een bepaalde aanbieding.

## Een overschrijving maken voor één aanbieding

De actie _[!UICONTROL Create Override]_is beschikbaar wanneer het bekijken van lijsten op_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, en_[!UICONTROL Ineligible]_ lusjes.

1. Een vermelding op een _[!UICONTROL Products Listings]_-pagina (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_en_[!UICONTROL Ineligible]_-tabblad) weergeven.

1. Klik in de kolom _[!UICONTROL Action]_op **[!UICONTROL Select]**>**[!UICONTROL Create Override]**om de pagina Overschrijvingen van productaanbiedingen te openen.

   ![Amazon-aanbieding overschrijven](assets/amazon-select-create-override.png)

1. Controleer _[!UICONTROL Listing Details]_om ervoor te zorgen dat je de juiste aanbieding bekijkt.

1. Bepaal het type overschrijving dat u maakt.

   Je kunt één overschrijvingstype of een combinatie van typen definiëren voor de aanbieding (Prijs, Verwerkingstijd, Voorwaarde, Opmerkingen van verkoper).

   - **Prijs**  - klik  **[!UICONTROL Change Listing Price]** en ga uw bepaalde prijswaarde voor in  **[!UICONTROL Price Override]**.
   - **Behandelingstijd**  - Klik  **[!UICONTROL Change Handling Time]** en ga de bepaalde tijdwaarde (in dagen) voor in  **[!UICONTROL Handling Time Override]**.
   - **Voorwaarde**  - Klik  **[!UICONTROL Change Condition]** en kies de correcte optie voor  **[!UICONTROL Condition Override]**.
   - **Opmerkingen**  van verkoper - Klik  **[!UICONTROL Change Seller Notes]** en voer de tekst van je notities in voor  **[!UICONTROL Seller Notes Override]**.

1. Klik op **[!UICONTROL Save Listing Override]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt gesloten. De status van de vermelding verandert in `Relist in Progress`. De wijziging wordt gepubliceerd naar Amazon met de volgende gegevenssynchronisatie (zoals geconfigureerd in de instellingen voor uitsnijden). De vermelding wordt ook toegevoegd aan het tabblad_[!UICONTROL Overrides]_.

In het volgende voorbeeld wordt een overschrijving getoond die een nieuwe prijs van `$55`, een nieuwe verwerkingstijd van `1 day`, een nieuwe voorwaarde van `Used; Like New`, en nieuwe tekst van de Nota van de Verkoper bepaalt.

![Voorbeeld Amazon-aanbieding overschrijven](assets/amazon-overrides-edit.png)

## Een overschrijving voor één aanbieding bewerken of verwijderen {#edit-override-single-listing}

De actie _[!UICONTROL Edit Overrides]_is beschikbaar wanneer het bekijken van lijsten op_[!UICONTROL Overrides]_ tabel.

1. Een vermelding op de pagina _[!UICONTROL Product Listings]_weergeven (_[!UICONTROL Overrides]_ tabblad).

1. Klik in de kolom _[!UICONTROL Action]_op **[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt geopend.

   ![Overschrijving Amazon-aanbieding selecteren](assets/amazon-select-edit-overrides.png)

1. Controleer _[!UICONTROL Listing Details]_om ervoor te zorgen dat je de juiste aanbieding overschrijft.

1. Als u uw _[!UICONTROL Override]_-instellingen wilt bewerken, definieert u de secties voor het type dat u wilt wijzigen (Prijs, Verwerkingstijd, Voorwaarde, Notities van verkoper).

   Selecteer `No Change To <override type>` (de standaardinstelling) om een overschrijvingstype gelijk te houden. Met deze instelling blijft de eerder gedefinieerde overschrijvingswaarde ongewijzigd.

   - **Prijs**  - klik  **[!UICONTROL Change Listing Price]** en ga uw bepaalde prijswaarde voor in  **[!UICONTROL Price Override]**.
   - **Behandelingstijd**  - Klik  **[!UICONTROL Change Handling Time]** en ga de bepaalde tijdwaarde (in dagen) voor in  **[!UICONTROL Handling Time Override]**.
   - **Voorwaarde**  - Klik  **[!UICONTROL Change Condition]** en kies de correcte optie voor  **[!UICONTROL Condition Override]**.
   - **Opmerkingen**  van verkoper - Klik  **[!UICONTROL Change Seller Notes]** en voer de tekst van je notities in voor  **[!UICONTROL Seller Notes Override]**.

1. Als u een overschrijvingstype wilt verwijderen, klikt u op **Verwijderen** voor elk type dat u wilt verwijderen. Als deze niet wordt verwijderd, blijft de eerder gedefinieerde waarde in de overschrijving staan.

1. Klik op **[!UICONTROL Save Listing Override]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt gesloten. De status van de vermelding verandert in `Relist in Progress`. De wijziging wordt gepubliceerd naar Amazon met de volgende gegevenssynchronisatie (zoals geconfigureerd in de instellingen voor uitsnijden). Als deze nog niet wordt vermeld, worden de aanbiedingen ook toegevoegd aan het tabblad_[!UICONTROL Overrides]_.

Het migreren op _leidt tot een Voorbeeld van de Opheffing_. In het volgende voorbeeld wordt een bewerking getoond van de eerder gemaakte overschrijving die een nieuwe prijs van `$50` definieert, wordt de handeling Tijd genegeerd en worden de vorige voorwaarde en verkopersnotities genegeerd.

![Een overschrijving](assets/amazon-overrides-edit-2.png)
__ bewerken of verwijderen

## Een overschrijving voor meerdere aanbiedingen bewerken of verwijderen {#edit-override-multiple-listings}

De handeling _[!UICONTROL Edit Listing Overrides]_is beschikbaar op de tabbladen_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ en _[!UICONTROL Ineligible]_.

>[!NOTE]
>
>Omdat u overschrijvingen voor meerdere aanbiedingen wijzigt, wordt de sectie _[!UICONTROL Listing Details]_niet weergegeven zoals wanneer u één aanbieding wijzigt.

1. Geef de vermelding weer op een _[!UICONTROL Products Listings]_-pagina (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ en _[!UICONTROL Ineligible]_tab).

1. Schakel het selectievakje in de linkerkolom in voor alle aanbiedingen die u wilt wijzigen.

1. Klik onder _[!UICONTROL Actions]_op **[!UICONTROL Edit Listing Overrides]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt geopend.

   ![Overschrijving Amazon-aanbieding selecteren](assets/amazon-actions-edit-listing-overrides.png)

1. Als u uw _[!UICONTROL Override]_-instellingen wilt bewerken, definieert u de secties voor het type dat u wilt wijzigen (Prijs, Verwerkingstijd, Voorwaarde, Notities van verkoper).

   Selecteer `No Change To <override type>` (standaardwaarde) om hetzelfde item niet te overschrijven. Met deze instelling blijft de eerder gedefinieerde overschrijvingswaarde ongewijzigd.

   - **Prijs**  - klik  **[!UICONTROL Change Listing Price]** en ga uw bepaalde prijswaarde voor in  **[!UICONTROL Price Override]**.
   - **Behandelingstijd**  - Klik  **[!UICONTROL Change Handling Time]** en ga de bepaalde tijdwaarde (in dagen) voor in  **[!UICONTROL Handling Time Override]**.
   - **Voorwaarde**  - Klik  **[!UICONTROL Change Condition]** en kies de correcte optie voor  **[!UICONTROL Condition Override]**.
   - **Opmerkingen**  van verkoper - Klik  **[!UICONTROL Change Seller Notes]** en voer de tekst van je notities in voor  **[!UICONTROL Seller Notes Override]**.

1. Als u een overschrijvingstype wilt verwijderen, klikt u op **[!UICONTROL Remove]** voor elk type dat u wilt verwijderen. Als deze niet wordt verwijderd, blijft de eerder gedefinieerde waarde in de overschrijving staan.

1. Klik op **[!UICONTROL Save Listing Override]**.

   De pagina _[!UICONTROL Product Listing Overrides]_wordt gesloten. De status van de aanbiedingen verandert in `Relist in Progress`. De wijziging wordt gepubliceerd naar Amazon met de volgende gegevenssynchronisatie (zoals geconfigureerd in de instellingen voor uitsnijden). Als deze nog niet wordt vermeld, worden de aanbiedingen ook toegevoegd aan het tabblad_[!UICONTROL Overrides]_.

### Typen overschrijven

| Negeren | Beschrijving |
|--- |--- |
| [!UICONTROL Price Override] | Een prijsoverschrijving definieert de prijs voor de aanbiedingen. Deze overschrijving heeft voorrang op alle geautomatiseerde instellingen totdat de overschrijving wordt verwijderd.<br><br>Als u de prijs van uw product wilt overschrijven, kiest u  **[!UICONTROL Change Listing Price]** en voert u de nieuwe prijs in voor  **[!UICONTROL Price Override]**. |
| [!UICONTROL Handling Time Override] | Met een overschrijvingstijd van de verwerkingstijd wordt de tijd (in dagen) voor het verwerken en verzenden van producten gedefinieerd. Een het behandelen tijdopheffing neemt voorrang over alle geautomatiseerde en standaard behandelingstijdinstellingen tot de opheffing wordt verwijderd.<br><br>De waarde die in het  _[!UICONTROL Handling Time Override]_vak staat, is de standaardverwerkingstijd die in de  [aanbiedingsinstellingen is gedefinieerd of de ](./listing-settings.md) door u gedefinieerde verwerkingstijd voor overschrijven. Als je een overschrijving van de afhandelingstijd verwijdert, wordt de aanbieding standaard afgehandeld volgens de verwerkingstijd die in de aanbiedingsinstellingen is opgegeven.<br><br>Als u een verwerkingstijd wilt overschrijven, kiest u **[!UICONTROL Change Handling Time]**en voert u de nieuwe verwerkingstijd (in dagen) in voor **[!UICONTROL Handling Time Override]**. |
| [!UICONTROL Condition Override] | Als u de aanbiedingsvoorwaarde wilt overschrijven, kiest u **[!UICONTROL Change Condition]** en kiest u de nieuwe voorwaarde uit **Voorwaardelijke overschrijving**. |
| [!UICONTROL Seller Notes Override] | Voor producten in uw catalogus die zijn gedefinieerd met een andere voorwaarde dan `New`, kan een verkopersopmerking worden toegevoegd om het product en de toestand ervan voor potentiële kopers nader te beschrijven. U kunt een overschrijving voor verkopersnotities invoeren voor een voorwaardenproduct `New`, maar Amazon geeft de notitie niet weer.<br><br>Als je de verkopersnotities wilt overschrijven, kies je  **[!UICONTROL Change Seller Notes]** en voer je de nieuwe notitie in voor  **[!UICONTROL Seller Notes Override]**. |
