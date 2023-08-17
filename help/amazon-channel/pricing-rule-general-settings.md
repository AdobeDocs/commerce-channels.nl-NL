---
title: Amazon-Sales Channel - Algemene instellingen voor prijsregel
description: Met de algemene instellingen van de prijsregel definieert u de primaire kenmerken van een prijsregel voor aanbiedingen.
feature: Sales Channels, Price Rules, Configuration
exl-id: 915b3eed-997e-4f94-a23f-0553a9dfe30c
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Algemene instellingen voor prijsregel

Definieer de naam, beschrijving, actieve datums en prioriteit voor de regel.

## Het gedeelte Algemene instellingen van prijsregel invullen

1. Voor **[!UICONTROL Rule Name]** (vereist), ga de naam voor de regel in.

   Deze naam is alleen bedoeld voor uw interne identificatie. Hoe beschrijvender de regelnaam, hoe beter.

1. Voor **[!UICONTROL Description]**, voer een gedetailleerde beschrijving van uw regel in.

   Deze beschrijving kan informatie bevatten over de producten die in aanmerking komen, de actieve datums, de formule voor het berekenen van de aangepaste prijs of andere informatie die u nuttig zou vinden als u de regel wilt wijzigen.

1. Voor **[!UICONTROL Status]** kiest u een optie:

   - `Active` - Kies deze optie als je de prijsregel wilt toepassen op in aanmerking komende producten en je aanbiedingsprijzen wilt aanpassen voordat je deze publiceert naar Amazon.

   - `Inactive` - Kies deze optie als u de prijsregel niet wilt toepassen op in aanmerking komende producten. Deze optie zal zeer waarschijnlijk worden gebruikt wanneer het wijzigen van een prijsregel of het uitzetten van het na een beperkte bevordering.

1. Voor **[!UICONTROL From]** en **[!UICONTROL To]** Voer een begin- en einddatum in voor de prijsregel.

   U kunt ook op het kalenderpictogram klikken om een datum in de dynamische kalender te selecteren. Deze automatische start- en stopoptie is nuttig bij het opzetten van promoties in beperkte tijd of seizoensgebonden tijd met een bepaalde begin- en einddatum.

1. Voor **[!UICONTROL Priority]** Voer een numerieke waarde voor de regelprioriteit in.

   Prioriteitswaarde gelijk aan `1` is de hoogste prioriteit. Wanneer u veelvoudige actieve het tarief regels hebt, kunt u deze prioritaire waarde gebruiken om te bepalen welke regel eerst wordt toegepast. Dit veld is vereist voor het gebruik van de _[!UICONTROL Discard Subsequent Rules]_gebruiken.

1. Voor **[!UICONTROL Discard Subsequent Rules]** kiest u een optie:

   - `Yes` - Kies deze optie als u geen andere prijsregels wilt toepassen die op een product van toepassing kunnen zijn. Als latere regels worden genegeerd, betekent dit dat, wanneer meerdere prijsregels op hetzelfde product van toepassing zijn, alleen de prijsregel met de hoogste gedefinieerde prioriteitswaarde op het product wordt toegepast. Met deze optie wordt voorkomen dat meerdere prijsregels worden gestapeld en onbedoelde extra kortingen bieden.

   - `No` - Kies deze optie als u meerdere prijsregels wilt toepassen op hetzelfde product. Deze optie kan ertoe leiden dat meerdere kortingen worden gestapeld en toegepast.

>[!NOTE]
>
>Als u volgende regels wilt verwijderen, moet een prijsregel een definitie hebben **Prioriteit** waarde.

![Algemene instellingen voor prijsregel](assets/amazon-pricing-rule-general.png){width="600" zoomable="yes"}

| Veld | Beschrijving |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Name] | (Vereist) Voer een naam voor de regel in die wordt gebruikt voor interne identificatie. Hoe beschrijvender de regelnaam, hoe beter. Bijvoorbeeld: &quot;25% korting op jaarultimo.&quot; |
| [!UICONTROL Description] | Voer een gedetailleerde beschrijving in die de regel (die ook voor interne doeleinden wordt gebruikt) uitlegt. Bijvoorbeeld: &quot;Verkoop einde jaar, 25% korting op alle objecten in de categorie Boeken.&quot; |
| [!UICONTROL Status] | Opties:<ul><li>**[!UICONTROL Inactive]** - De prijsregel geldt niet voor je aanbiedingen. Deze optie kan worden gebruikt wanneer u een prijsregel wijzigt of deze uitschakelt na een beperkte promotie.</li><li>**[!UICONTROL Active]** - De prijsregel geldt voor je aanbiedingen en pas de prijs van je aanbieding aan voordat je op Amazon publiceert.</li></ul> |
| [!UICONTROL From] | Voer de begindatum in waarop de prijsregel begint. Als u bijvoorbeeld een verkoop wilt uitvoeren in de laatste maand van het jaar, stelt u de optie `From` datum tot 1 december, zodat de prijsregel automatisch van toepassing is op je Amazon-aanbiedingen vanaf 1 december. |
| [!UICONTROL To] | Voer de einddatum in waarop de prijsregel eindigt. Als u het vorige voorbeeld doorloopt en de verkoop wilt beperken tot de laatste maand van het jaar, stelt u de optie `To` datum 31 december, zodat de prijsregel op 31 december verstrijkt. |
| [!UICONTROL Priority] | Voer een waarde in voor de prioriteit van de prijsregel. Een prioriteitswaarde gelijk aan `1` is de hoogste prioriteit. Wanneer u veelvoudige het tarief regels hebt, kunt u de prioritaire waarde gebruiken om te bepalen welke regel eerst wordt toegepast. Dit veld is vereist voor het gebruik van de **Volgende regels negeren** gebruiken. |
| [!UICONTROL Discard Subsequent Rules] | Gebruikt om veelvoudige het tarief regels toe te staan of te verhinderen en extra kortingen te verstrekken. Als u volgende regels wilt verwijderen, moet voor een prijsregel een waarde zijn gedefinieerd voor **[!UICONTROL Priority]**. Opties:<ul><li>**[!UICONTROL Yes]** - Kies wanneer u geen andere prijsregels wilt toepassen die op een product van toepassing kunnen zijn. Als latere regels worden genegeerd, betekent dit dat wanneer meerdere prijsregels op hetzelfde product van toepassing zijn, alleen de prijsregel met de hoogste gedefinieerde prioritaire waarde wordt toegepast.</li><li>**[!UICONTROL No]** - Kies wanneer u meerdere prijsregels wilt toepassen op hetzelfde product. Deze optie kan ertoe leiden dat er meerdere kortingen op je aanbiedingsprijs worden toegepast.</li></ul> |
