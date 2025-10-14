---
title: Reissegmenten voor klanten samenstellen
description: Leer hoe te om op gedrag-gebaseerde segmenten van de klantenreis in  [!DNL Adobe Analytics]  tot stand te brengen en uw klanten' ervaring met  [!DNL Adobe]  Experience Cloud te verbeteren door deze geleidelijke gids te volgen.
feature-set: Analytics
feature: Segmentation
role: User
level: Experienced
doc-type: Article
last-substantial-update: 2023-05-02T00:00:00Z
jira: KT-13180
thumbnail: KT-13180.jpeg
exl-id: 34f42d7e-e849-420e-9b3d-f3dcc1882b23
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1224'
ht-degree: 0%

---

# Reissegmenten voor klanten samenstellen

Leer hoe u op gedrag gebaseerde reissegmenten voor klanten maakt in [!DNL Adobe Analytics] en de ervaring van uw klanten met [!DNL Adobe] -Experience Cloud verbetert door deze stapsgewijze handleiding te volgen.

Laten we betere reissegmenten voor klanten maken! In deze reeks, zullen wij [!DNL Adobe Analytics] gebruiken om op gedrag-gebaseerde segmenten te bepalen, publieksgrootte te schatten, en beweging van de spoorgebruiker te volgen. Uiteindelijk kunt u de media personaliseren en de ervaring van uw klanten verbeteren met [!DNL Adobe] Experience Cloud. Houd in mening dat deze segmenten leven en zouden moeten worden bijgewerkt aangezien u meer over uw klanten leert. Hoewel het melden enkele uitdagingen kan zijn, maak u geen zorgen, zal ik u door het begeleiden! Laten we beginnen met het maken van onze eerste set reissegmenten voor klanten, te beginnen met het segment &quot;One Hit Wonders&quot;.

Vandaag, zullen wij placeholders voor onze eerste reeks segmenten van de Reis van de Klant creëren, een [!DNL Adobe Analytics] Workspace bouwen om ons te helpen onze segmenten bepalen, en ons zeer eerste segment bepalen, &quot;One Hit Wonders.&quot;

Aan het einde van deze reeks kunt u reissegmenten voor klanten maken in [!DNL Adobe Analytics] op basis van gedragssignalen. U zult de grootte van elk publiek in elk stadium van de reis kunnen schatten en begrijpen in welk tempo de gebruikers zich tussen die stadia bewegen. En u kunt die klanten die reispubliek naar [!DNL Adobe] Experience Cloud uitvoeren om personalisatie en media het richten toe te laten.

Elk bedrijf is verschillend, en dat betekent dat uw segmenten van de klantenreis verschillend zullen kijken dan de mijne. Dus in plaats van specifieke formules voor te schrijven voor je segmenten, stel je wat dingen voor om naar te kijken en een algemeen proces om ze te bouwen.

Het is ook belangrijk om op te merken dat uw segmenten van de klantenreis levende segmenten zullen zijn. Dit is geen eengemaakte oefening. Aangezien u meer over uw klanten leert, zult u deze segmenten bijwerken. Dit stelt een aantal uitdagingen voor rapportage. De mensen willen consistentie in hun verslagen, en als onze segmentdefinities veranderen, dan zullen de aantallen in de rapporten ook veranderen.

## Aan de slag met segmenten van Bezoek-intentie

De eerste stap aan de bouw van de segmenten van de klantenreis is af te leiden waarom een gast op uw website gebruikend gedragssignalen, en, indien beschikbaar, Stem van de gegevens van de Klant is. We maken een set Bezoek intent-segmenten om alle bezoeken op de website te categoriseren. Op dit moment moeten onze segmenten van de Bezoek Intent elkaar uitsluiten en volledig uitputten. Elk bezoek zou tot één, en slechts één, Bezoek Intent segment moeten behoren.

De segmenten van de Intentie van het Bezoek beschrijven een bezoek, zodat zullen wij de container van Bebezoeken in de segmentdefinitie gebruiken.

Mijn eerste set Bezoek intent-segmenten was:

* One Hit Wonders
* Bewustmaking
* Overwegingen
* Boek (aankoop)
* Behoud (een boeking/aankoop beheren)

Om mijn segmenten van de Intentie van het Bezoek gemakkelijk te maken te gebruiken, stelde ik mijn segmentnamen met &quot;Intent:&quot;vooraf in, gaf hen een aantal om het sorteren toe te laten, en etiketteerde hen &quot;intent&quot;. Mijn segmenten zagen eruit als de onderstaande afbeelding.

![&#x200B; intent segmenten &#x200B;](assets/intent-segments.png)

**ga vooruit en creeer uw Segmenten van de Intentie van het Bezoek gebruikend de container van Bezoekers met een placeholder definitie van de Meningen van de Pagina >= 1.**

Zoals we zullen zien, is het bouwen van deze segmenten een herhalend en onderling verbonden proces. Ik zal het proces beschrijven om deze segmenten te bouwen in een toekomstig artikel.

## Bezoek Intent Segment Data Quality Workspace

![&#x200B; de werkruimte van de de intentie van het bezoek &#x200B;](assets/visit-intent-workspace.png)

Ik gebruikte een eenvoudige werkruimte om ervoor te zorgen dat ik mijn segmenten van de Intentie van het Bezoek goed definieerde. Herinner me, moet elk bezoek tot één, en slechts één, segment van de Intentie van het Bezoek behoren. De werkruimte die ik heb ingesteld, zorgt ervoor dat alle bezoeken worden verantwoord en dat er geen overlapping tussen de segmenten is.

Ik noemde deze werkruimte &quot;DATA QUALITY: Visit Intent Segments&quot; met de tags &quot;data quality&quot;, &quot;visit intent&quot; en &quot;customer trip&quot;. Later maken we een &quot;Visit Intent-dashboard&quot;, zodat het voorvoegsel &quot;DATA QUALITY&quot; aangeeft dat deze werkruimte bedoeld is voor het instellen en onderhouden van de segmenten. Het is een administratief dashboard dat vrij weinig bedrijfsinzicht heeft maar belangrijk is om ervoor te zorgen dat de segmenten worden gehandhaafd. Het is een goed idee om routinematig terug te komen naar dit dashboard, of opstellingsalarm, om ervoor te zorgen uw segmenten correct gedefiniëerd blijven.

De belangrijkste visualisatie in deze werkruimte is de segmentoverlap in de vrije vorm visualisatie in het midden links. Gebruikend metrisch van Bebezoeken, creeer kolomfilters voor elk van uw segmenten van de Intentie van het Bezoek, plus het Al segment van Bezoeken in de meest rechtse kolom. Maak rijen voor elk segment Intentie bezoeken aan de linkerkant. U hebt nu een visuele kruiscursor. Wanneer uw segmenten correct worden gevormd, zullen er slechts gegevens in één kolom en één rij, bij de doorsnede van elk segment van de Intentie van het Bezoek met zich zijn.

De volgende belangrijkste visualisaties zijn de summiere metriek bij de hoogste linkerzijde. De samenvatting van Gesegmenteerde Bezoeken neemt zijn waarde uit de Al kolom van Bezoeken in de Overlap van het Segment onmiddellijk hieronder visualisatie. De samenvatting van alle bezoeken heeft zijn eigen verborgen lijst.

![&#x200B; alle bezoeken &#x200B;](assets/all-visits.png)

Rechtsboven heb ik aanvullende metriek toegevoegd aan elk van de segmenten om wat &quot;smaak&quot; te geven aan hoe de segmenten zich vormgeven. In het bijzonder, omdat deze segmenten elkaar wederzijds uitsluiten, verwacht ik slechts boekingen voor het segment van de Intentie van de Boek (vrees niet, zullen wij aan omzettingspercentages krijgen wanneer wij deze op bezoeker-gebaseerde segmenten van de Intentie van Bezoek maken.

Onthoud dat we zojuist plaatsaanduidingssegmenten hebben gemaakt. In eerste instantie zal je werkruimte er gek uitzien. Alle segmenten met bezoekintentie overlappen 100% omdat ze dezelfde definitie hebben. Dit is correct, en precies wat u op dit punt in het proces wilt zien. Terwijl we de segmentdefinities maken, zult u beginnen te zien dat deze segmenten vorm krijgen.

![&#x200B; de definities van het de intentsegment van het Bezoek &#x200B;](assets/visit-intent-segment-defs.png)

## Uw eerste segment met bezoekintentie maken

Het bepalen van de segmenten van de Intentie van het Bezoek is een beetje van een proces van eliminatie, en er is veel onderlinge afhankelijkheid tussen hen. Dus ik bouwde deze segmenten niet in de volgorde van de reis, ik bouwde ze op volgorde van de eenvoudigst gedefinieerde tot de meest uitdagende. Dat gaf me deze orde:

1. Intentie: 0 - één hits
1. Intentie: 3 - Boken
1. Intentie: 4 - Behoud
1. Intentie: 2 - Overwegingen
1. Intentie: 1 - Bewustmaking

Heel willekeurig, hé? Het bepalen van deze segmenten van de Intentie van Bezoek was een iteratief, rug-en-over, proces, en vaak vereiste een aanpassing aan één segment updates aan andere segmenten. Dit zal duidelijker worden aangezien ik beschrijf hoe ik elk van deze segmenten definieer.

Vandaag, zullen wij onze eerste, en gemakkelijkste, segment bepalen, One Hit Wonders

## Het One Hit Wonders-segment opbouwen

Mijn eerste segment, &quot;One Hit Wonders&quot;, was eenvoudig te definiëren. Het is gewoon een bezoek met slechts één paginaweergave. We weten echt niet waarom die gebruiker op de website stond, omdat ze op de boog stuitten. Ik veronderstel wij een intent konden veronderstellen die op hun ingangspagina wordt gebaseerd, maar met slechts één paginamening, is er enkel niet genoeg informatie om een geïnformeerde raad over intentie te maken.

![&#x200B; de definitie van het Segment &#x200B;](assets/segment-def.png)

Nadat u dit segment hebt gedefinieerd, ziet u hoe uw Visit Intent-Workspace vorm krijgt.

![&#x200B; Meer segmentdefinities &#x200B;](assets/more-segment-defs.png)

Het samenstellen van klantenswitches met [!DNL Adobe Analytics] is een uitdagend maar belonend proces. Door op gedrag-gebaseerde segmenten tot stand te brengen, publieksgrootte te schatten, en gebruikersbewegingen te volgen, kunnen de ondernemingen media personaliseren en klantenervaring verbeteren. Elk bedrijf is uniek, en er zijn geen specifieke formules voor het creëren van segmenten, maar richtlijnen en een te volgen proces. De segmenten zouden moeten worden bijgewerkt aangezien de ondernemingen meer over hun klanten leren, die rapporteringsuitdagingen voorstelt. Door het proces te volgen om de segmenten van de Intentie van het Bezoek te bouwen, kunnen de ondernemingen algemene klantenervaring verbeteren.

## Auteur

Dit document is geschreven door:

![&#x200B; Aaron Fossum &#x200B;](assets/aaron-headshot.png)

**Aaron Fossum**, Director, Digitaal [!DNL Analytics]

[!DNL Adobe Analytics] Champion
