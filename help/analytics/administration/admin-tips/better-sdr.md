---
title: De Cultuur van Gegevens van de bouw en een Betere Verwijzing van het Ontwerp van de Oplossing
description: Maak een revolutie in uw gegevensstrategie en geef uw team de mogelijkheid om een solide document van de Referentie van het Ontwerp van de Oplossing (SDR) te creëren. Elimineer meethiaten en bevordeer een samenwerkende gegevenscultuur door geleidelijke methodologieën.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25T00:00:00Z
jira: KT-15338
thumbnail: KT-15338.jpeg
exl-id: 99fcf68f-5698-4270-9055-ab224e6323a1
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# Gegevenscultuur opbouwen en een betere referentie voor het ontwerp van oplossingen

_revolutioneer uw gegevensstrategie en machtigt uw team om een stevig document van de Verwijzing van het Ontwerp van de Oplossing te creëren (SDR). Elimineer meethiaten en bevordeer een samenwerkingsgegevenscultuur door geleidelijke methodologieën._

Het is eindelijk tijd. U hebt een solide SDR samengesteld. Een SDR is de gids die u gebruikt om uw metriek en dimensies uit te voeren. Je hebt gedefinieerd wat ze heten, wanneer ze vuur maken, en je ontwikkelaars houden ervan. Je hebt het hele implementatieproces doorlopen, acceptatiecriteria geschreven, door je sproeten gegaan, getest en gedaan! Uw exemplaar van [!DNL Adobe Analytics] zou marketing en productteams moeten krijgen die in de gegevens graven, nieuwe onthullingen over uw klanten krijgen, en alle gebieden van succes en, goed, gebieden van minder succes vinden. Maar je hoort niet de accolades die je verwachtte.

Van één team hoor je klachten zoals:

&quot;Waarom kan ik de omrekeningskoers voor deze trechter niet berekenen?&quot;

&quot;Waarom is er geen metrische waarde voor dit?&quot;

&quot;Ik heb meer details nodig! Een metrische alleen is niet genoeg. Er zijn ten minste drie verschillende dimensies die ik nodig heb om prestaties te begrijpen. Waarom heb je ze niet opgenomen?&quot;

Maar het is het andere team dat nog meer zorgen baart. Van hen hoor je helemaal niets. Erger nog, je ziet grafieken die duidelijk zijn ontleend aan je oude analytische oplossing (die niet meer wordt onderhouden, en elke dag valt verder in een moeras van decrepitude en vuile data). Een gevoel van droevigheid vult je als je kijkt naar de beslissingen die gemaakt kunnen worden met die oorspronkelijke puinhoop.

_wat ging verkeerd?_

_waarom zijn er hiaten in meting?_

_waarom zijn uw teamleden niet het omarmen van dit?_

Ik zal beginnen met jullie iets van de haak te laten. Er is _altijd_ die wat revisie zal zijn. Als uw site of toepassing complex genoeg is om een oplossing voor bedrijfsanalyse te hebben, is het zeker dat u iets zult missen. Maar in dit geval heb je niet genoeg gemist om de meetlacunes die ik beschrijf, uit te leggen.

Wat er mis ging, is veel moeilijker in een spreadsheet te stoppen. In wezen, miste u op uw eerste kans om een samenwerkende gegevenscultuur te bouwen terwijl u SDR bouwde.

Ik wil u door een methode laten lopen die mijn collega&#39;s en ik hebben ontwikkeld om een betere SDR te bouwen met minder tussenruimten en om eindgebruikers te laten investeren (en soms zelfs opgewonden) over hun nieuwe instantie van [!DNL Adobe Analytics]. Laten we eens kijken hoe en waarom je deze methode moet overwegen.

## Hoe

_leer over de metingsconferentie. Gebruik een trechter kaart om elke stap van uw plan visualiseren. Maak modeldashboards die u wilt bekijken als een groep. Creeer een gegevenswoordenboek voor gebruikers._

### De meetconferentie

1. Zorg ervoor dat uw belanghebbenden bij elkaar komen, zowel persoonlijk als virtueel, met als doel na te gaan wat u moet meten. Deze vergadering zou een aantal leidinggevenden moeten omvatten.
1. Heb duidelijke voorbeelden reeds op kleverige nota&#39;s, zoals opbrengst, verkoop, of lood, de belangrijkste productindicatoren (KPIs) u weet zal worden gemeten. Herhaal deze stappen met afmetingen zoals de status Aangemeld, Productcategorieën of zoektermen.
1. Laat iedereen zijn eigen notities toevoegen en groeperen als dat nodig is.
1. Vraag mensen om te stemmen over de dingen die ze belangrijk vinden. Dit zijn onbeperkte stemmen, omdat al deze cijfers en dimensies er waarschijnlijk toe doen.
1. Voor alle meeteenheden en dimensies met een lage stem hebben, hebben de belanghebbenden die hierom hebben gevraagd, uitgelegd waarom deze componenten zouden worden gebruikt. Als er een goed gebruiksgeval is, houd deze componenten. Als er een betere manier is om die gegevens te krijgen, of niemand kan verklaren hoe deze gegevens actionable zijn, of als er een andere goede reden is om de metriek en de afmetingen te verwijderen, doe dit.
1. Voeg deze metriek en dimensies aan uw SDR toe voor een eerste overzicht door de belanghebbenden die aanwezig waren.

### De trechter-kaart

1. Zorg voor een visualisatie van alle treinen, stap voor stap met elk opgenomen frame.
1. Met de ontwerpers en productmanagers, ga door elke stap en bespreek wat iedereen als succes in die trechter beschouwt. Is het de omrekeningskoers? Kies zij een bepaald pad? Gebruikt het bepaalde functies?
1. Stel vragen over welke metriek en afmetingen nodig zijn om de prestaties van de trechter in elke stap van de trechter en in het algemeen te begrijpen.
1. Voeg boven elke stap van de trechter de metriek en de afmetingen toe die bij die stap, met inbegrip van de berekende metriek worden gemeten.
1. Aan het begin van elke trechter, schrijf de rapporten uit die in het dashboard gaan die de productmanager kan gebruiken om prestaties te volgen. Deze rapporten omvatten a [ reserverapport ](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/fallout/fallout-flow), [ huidige maand ](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/components/calendar-date-ranges/custom-date-ranges), [ trended omzettingspercentages ](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/line), en om het even wat specifieker op dat trechter.
1. Voeg de nieuwe metriek en de afmetingen toe u aan SDR hebt ontdekt en verzend het naar de belanghebbenden voor een tweede overzicht.

### De voorvertoningsdashboards

1. Gebruik de trechter-kaart als richtlijn om mockup-dashboards te maken.
1. Er zou een algemene mening, zoals een [ Uitvoerend Samenvattend Dashboard ](driving-success-with-executive-summary-dashboards.md), en dashboards voor elk van de trechters moeten zijn.
1. Er zijn ook enkele specifiekere opties voor uw site of toepassing, zoals de prestaties van producten of inhoud.
1. Geef deze informatie door aan de relevante belanghebbenden en krijg feedback over het ontwerp.
1. Breng de gewenste updates aan en voeg deze toe aan uw SDR als er nieuwe maatstaven of dimensies nodig zijn.
1. Verzend de bijgewerkte voorvertoningsdashboards en SDR voor een laatste revisie.

### Gereedschappen voor gegevensdemocratisering

1. Maak een gegevenswoordenboek. SDR is voor uw ontwikkelaars, maar het gegevenswoordenboek is voor uw eind - gebruikers. Maak het leesbaar zodat iedereen gemakkelijk kan zien welke gegevens beschikbaar zijn en weet hoe deze moeten worden gebruikt. Uw eindgebruikers zouden de definitieve fiatteurs van dit moeten zijn.
1. Annoteren. In elke organisatie zijn er bepaalde data die elk jaar van belang zijn en andere die zullen opduiken. Zorg ervoor dat u de relevante datums van uw belanghebbenden verzamelt en deze als annotaties toevoegt om meer inzicht te krijgen in de gegevens die ze zien.
1. Curate. Als uw SDR groot is, is het misschien overweldigend. Paralyse van keuze is niet alleen van toepassing op uw klanten. Bekijk wat belangrijk is voor elke groep gebruikers en bekijk de elementen die ze zullen zien.

## De reden

_Leer over het verzamelen van vereisten, het bouwen van een gegevenscultuur, die diepgaand denken over gegevens ontlokt, die een gevoel van eigendom over de gegevens creëren, en de gegevens vereenvoudigen._

### Verzamelvereisten

Het is duidelijk dat er vereisten moeten worden verzameld, maar er zijn verschillende effectieve manieren om dat te doen. Ik heb één-op-één interviews, vragenlijsten, en revisies van bestaande rapporten gebruikt. Die strategieën werken, maar niet zo goed als de methoden die ik zojuist heb geschetst. Maar ik denk niet dat het verschil tussen de methodes voor het verzamelen van vereisten significant is. De methode die ik heb beschreven geeft je 95% van de manier waarop je daar zit, en deze andere methoden brengen je 90% van de weg.

Dus, wat is _waarom_?

### Gegevenscultuur opbouwen

In dit proces, u:

* Spark diep nadenken over hoe succes kan worden gemeten
* Zorgen voor een gevoel van betrokkenheid bij uw belanghebbenden
* Het voor belanghebbenden gemakkelijker maken om hun gegevens te begrijpen

### Spark diep nadenken over gegevens

Voor veel van de mensen in je bedrijf is data iets wat ze consumeren. Ze gebruiken het. Ze analyseren het. Ze denken er niet diep over na. Sommige mensen hebben rapporten en processen van hun voorgangers geërfd, maar hebben ze niet gewijzigd omwille van de continuïteit. Misschien moesten deze mensen nooit aan _denken waarom_ van de gegevens.

Dit proces geeft hen een kans om __ gegevens echt te begrijpen. Vragen stellen als: Wat is succes? Hoe zou je weten of je succesvol was? Hoe zou je weten wat te veranderen als je niet succesvol was? Deze vragen moeten aan het begin van het creëren van elke plaats, toepassing, en product-maar veel te vaak worden beantwoord zij niet. Door deze vragen te stellen, helpt u iemands begrip van niet alleen de gegevens, maar ook hun product te verdiepen.

### Een gevoel van eigendom over de gegevens maken

Een gevoel van eigendom is niet iets dat een persoon gemakkelijk verkrijgt. Het is niet gevonden in die dertig minuten durende vergadering die drie maanden geleden bijwoonde. Het is niet gemaakt door dat een vervelende vragenlijst die ze te snel beantwoord hebben vanwege andere dringende werkproblemen, zoals demos en de datums van de sprint.

Eigendom is het product van iemands diepste gedachte en zijn werk met u en collega&#39;s. Het is het ding waar ze meerdere malen naar hebben gekeken, waar ze voortdurend feedback op hebben gegeven, en waar ze mee hebben ingestemd nadat die feedback was opgenomen. Het is van hen! Dat het nuttig is, komt door hen. Het is _hun_ gegevens en het is dat proces dat het hun maakte.

### De gegevens vereenvoudigen

U hebt hen ook getoond hoe zij het proces zullen gebruiken en wat het als door de [ voorproefdashboards ](#the-preview-dashboards) zal kijken. Om het even welke nieuwe oplossing is hard __. Er is zoveel te leren, en gezien de enorme aanpasbaarheid van [!DNL Adobe Analytics], kan de leercurve steil zijn. Daar heb je 80% van verwijderd. Zelfs voordat de eerste coderegel is geschreven, weten uw belanghebbenden hoe hun dashboards eruit zullen zien. Ze zullen weten hoe ze ze kunnen lezen en betekenis ervan krijgen. Ze zullen weten hoe succes er letterlijk uitziet, omdat ze je hebben verteld welke maatstaven en dimensies succes definiëren. Je hebt ze verteld hoe dat succes voor hen zichtbaar zal zijn. De levering van de daadwerkelijke dashboards is een verfrisser, niet een eng nieuwe leertaak.

Dit is niet noodzakelijk de snelste manier om een SDR samen te krijgen. Het is een hoop werk en vereist veel coördinatie van schema&#39;s, vooral omdat het essentieel is dat je een aantal leidinggevenden in de mix hebt. Uiteindelijk is een oplossing voor bedrijfsanalyses echter een enorme investering in tijd en geld, en u wilt ervoor zorgen dat adoptie en tevredenheid hoog zijn. Deze methode is een hele stap in de goede richting.

**Auteur**

Dit document is geschreven door:

![ gitai-hoofd ](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, Business Architecture Associate Manager bij Accenture

[!DNL Adobe Analytics] Champion
