---
title: Wacht even een segment... met segmentatie om nieuwe inzichten in Analysis Workspace te ontdekken
description: Leer hoe te om segmenten in  [!DNL Adobe Analytics]  te gebruiken om nieuwe inzichten van uw Analysis Workspace visualisaties en vrije vormlijsten te ontdekken.
feature-set: Analytics
feature: Segmentation
role: User
level: Beginner
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00Z
jira: KT-13268
thumbnail: KT-13268.jpeg
exl-id: 3496b6ff-f8d6-48a1-92f4-442a792663e7
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Wacht nu even een segment... Het gebruiken van segmenten om nieuwe inzichten in Analysis Workspace te ontdekken

Of u nu een nieuwe [!DNL Adobe Analytics] -gebruiker bent of een afgewerkte pro, u maakt nogal wat gebruik van segmenten in uw Analysis Workspace-projecten. Zoals [[!DNL Adobe]  Experience League ](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-overview.html?lang=nl-NL) beschrijft, &quot;staan de segmenten u toe om ondergroepen van bezoekers te identificeren die op eigenschappen of websiteinteractie worden gebaseerd.&quot; Hoewel het basisresultaat van deze functie erin bestaat groepen gebruikers te isoleren, bezoeken te brengen of te bezoeken aan uw site, kan een scherpe analist zoals uzelf creatief worden met dit programma en nieuwe manieren vinden om inzicht te krijgen in uw sitetaken. De lijst van mogelijke opties is uitgestrekt, zodat aarzelt niet om te proberen creërend uw en het met anderen bij uw organisatie of online in gemeenschappen zoals de [[!DNL Adobe Analytics]  Gemeenschap ](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics/ct-p/adobe-analytics-community) op Experience League of de [ #Measurement Slack ](https://www.measure.chat/) gemeenschap te delen.

Als u een snelle verfrisser op nodig hebt hoe te om een segment tot stand te brengen, gelieve de documentatie van het Experience League te controleren bij het gebruiken van de [ Bouwer van het Segment ](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html?lang=nl-NL) in Analysis Workspace.

## Segmenten vergelijken en contrasteren

In Analysis Workspace kunt u twee segmenten vergelijken gebruikend &quot;[ de vergelijking van het Segment ](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/panels/segment-comparison/segment-comparison.html?lang=nl-NL)&quot;. Segmentvergelijking vindt u in het gedeelte Deelvensters van de linkernavigatiebalk:

![ Seg 01 ](assets/seg01.png)

Soms hebt u echter geen volledig vergelijkingspaneel nodig om uw eindgebruikers inzicht in de persoonlijke sleutel te geven. Gelukkig kunnen sommige eigenschappen ook in een standaardpaneel worden vergeleken.

De [ het schemavisualisatie van de Venn ](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/visualizations/venn.html?lang=nl-NL) kan helpen tot een snelle vergelijking leiden, toestaand u om de overlappende zittingen, de orden, de gebruikers, enz. te bewegen en te zien. tussen 2-3 aangepaste segmenten. U kunt ook snel segmenten maken door met de rechtermuisknop op een van de overlappende secties te klikken:

![ Seg 02 ](assets/s02.png)

Soms bevindt de belangrijke informatie zich niet in de overlappende gegevens, maar in de gegevens die elkaar niet overlappen. Een snelle manier om dit te bekijken is een exemplaar van één segment tot stand te brengen en het te maken een &quot;Uitsluiten&quot;segment:

![ Seg 03 ](assets/s03.png)

Door het segment &quot;exclude&quot; te stapelen met het andere segment in uw vergelijking, kunt u nu snel berekenen hoeveel bezoeken uw menupagina raakten zonder ook de homepage in de zelfde zitting te bekijken:

![ Seg 04 ](assets/s04.png)

## Stapelaanval

Op dezelfde manier kunt u de elkaar kruisende gegevens van een diagram van Venn tot stand brengen door eenvoudig om het even welke segmenten samen te stapelen. Er is geen limiet voor het aantal segmenten of de afzonderlijke afmetingen die u stapelt. Als ik bijvoorbeeld snel wilde weten welke dagen van de week vorige maand mijn site een bezoek had op een mobiele telefoon, met name een Samsung Galaxy A52s, die mijn menu- en voedingspagina&#39;s wel zag, maar mijn homepage NIET zag, kan ik deze snel als volgt bouwen:

![ Seg 05 ](assets/s05.png)

Maar nog beter, zodra ik die perfecte ondergroep van mijn gebruiker of bezoekbasis vind, kan ik al die waarden selecteren, met de rechtermuisknop klikken, en een segment onmiddellijk creëren:

![ Seg 06 ](assets/s06.png)

![ Seg 07 ](assets/s07.png)

![ Seg 08 ](assets/s08.png)

Dat is veel macht in één segment.

## Een segment getallen voor een aantal segmenten

Vele gebruikers kijken vaak naar nominale, ordinale, of intervalwaarden wanneer het bouwen van segmenten - dingen zoals een bezochte pagina, een leeftijdswaaier van gebruikers, of het aantal bezoeken een gebruiker in het verleden heeft gemaakt. Nochtans, kunt u verhoudingsgegevens ook gebruiken wanneer het creëren van een segment door deze waarden - of zij standaardafmetingen, standaardmetriek, of douanevariabelen en metriek voor uw organisatie zijn te sluiten.

De tijd die bijvoorbeeld op de pagina wordt doorgebracht of de tijd die per bezoek wordt besteed, heeft vooraf gebouwde beschikbare emmers:

![ Seg 09 ](assets/s09.png)

Het is echter mogelijk dat deze niet altijd in de behoeften van uw organisatie passen. De meeste bezoeken van de site zijn wellicht korter dan 10 minuten. U kunt korrelmetingen gebruiken om emmers van verschillende grootte te maken. Hier is gecreeerd om bezoeken te bekijken die tussen 1 minuut, 1 seconde en 1 minuut, 30 seconden duren:

![ Seg 10 ](assets/s10.png)

Zodra gecreeerd, kan ik nu beginnen mijn bezoeken, orden, en andere gebeurtenissen door de verschillende gespikte tijdgroepen te bekijken die ik heb aangepast:

![ Seg 11 ](assets/s11.png)

U kunt zelfs beginnen te onderzoeken hoe uw Zeer belangrijke Indicatoren van Prestaties (KPIs) als factor van hoeveel tijd een gebruiker besteedt, hoeveel pagina&#39;s zij in een bezoek raken, hoeveel tijden zij in het verleden, of een andere numerieke waarde hebben bezocht - fundamenteel toelatend u om metrisch als factor van een andere metrisch te bekijken:

![ Seg 12 ](assets/s12.png)

De mogelijkheden om segmenten te gebruiken om nieuwe inzichten te vinden zijn eindeloos! Dit is gewoon een uitgangspunt. Probeer enkelen op uw en laat de gemeenschap weten wat u ontdekt: [[!DNL Adobe Analytics]  Gemeenschap ](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics/ct-p/adobe-analytics-community) op Experience League of de [&#128279;](https://www.measure.chat/) gemeenschap #Measurement Slack.

Gelukkig segmenteren!

## Auteur

Dit document is geschreven door:

![ Dan Cummings ](assets/seg13.png)

**Dan Cummings**, Sr. Manager van de Techniek van het Product [!DNL Analytics] bij de Bedrijf van McDonald&#39;s

[!DNL Adobe Analytics] Champion
