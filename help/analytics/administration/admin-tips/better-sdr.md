---
title: Gegevenscultuur opbouwen en een betere referentie voor het ontwerp van oplossingen
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
source-git-commit: 484f93bc2828d2565486eff8ae4801a8d203d280
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 0%

---


# Gegevenscultuur opbouwen en een betere referentie voor het ontwerp van oplossingen

**Maak een revolutie in uw gegevensstrategie en geef uw team de mogelijkheid om een document met een solide referentie-ontwerp (SDR) voor oplossingen te maken. Elimineer meethiaten en bevordeer een samenwerkende gegevenscultuur door geleidelijke methodologieën.**

Het is eindelijk tijd. U stelt een stevige Referentie van het Ontwerp van de Oplossing (SDR) samen. Dit is de gids die je gebruikt om je metriek en dimensies te implementeren, wat ze heten, wanneer ze branden, en je devs hielden ervan. Je hebt het hele implementatieproces doorlopen, acceptatiecriteria geschreven, door je sproeten, het hele ding QAing, en het is klaar! Het was veel werk, en nu is het klaar. Uw exemplaar van Adobe Analytics zou marketing en product moeten krijgen die omhoog en neer springen aangezien zij in de gegevens graven, nieuwe onthullingen over uw klanten krijgen, en alle gebieden van succes en, goed, gebieden van minder succes vinden. Maar je hoort niet de accolades die je verwachtte.

Van één kamp hoor je klachten.

&quot;Waarom kan ik de omrekeningskoers voor deze trechter niet berekenen?&quot;

&quot;Waarom is er geen metrische waarde voor dit?&quot;

&quot;Ik heb hier veel meer details over nodig! Een metrische alleen is niet genoeg. Er zijn minstens drie verschillende dimensies die ik nodig heb om prestaties te begrijpen. Waarom heb je ze niet opgenomen?&quot;

Maar het is het andere kamp dat een nog grotere bron van zorg is. Van hen hoor je helemaal niets. Maar nog veel erger: je ziet grafieken die heel duidelijk zijn ontleend aan je oude analytische oplossing, die niet meer wordt onderhouden, en elke dag valt verder in een moeras van decrepitude en vuile data. Een gevoel van dromen vult je als je nadenkt over de beslissingen die met die rommel gemaakt kunnen worden.

Wat ging er mis? Waarom zijn er gaten in de meting? Waarom staan uw teamleden dit niet toe?

Ik zal beginnen met jullie een beetje van de haak te laten. Er is *altijd* een herziening. Als uw site of toepassing complex genoeg is om een zakelijke analyseoplossing te nodig hebben, is het in principe zeker dat u iets zult missen. Maar niet genoeg om de meetlacunes te verklaren waar ik het hier over heb. Wat er mis ging, is veel moeilijker in een spreadsheet te stoppen. U hebt uw eerste kans gemist om een samenwerkende gegevenscultuur tezelfdertijd te bouwen u SDR bouwde. Ik wil u door een methode laten lopen die ik en mijn collega&#39;s hebben ontwikkeld om zowel een betere SDR met minder hiaten op te bouwen als eindgebruikers te laten investeren en soms zelfs enthousiast te maken over hun nieuwe exemplaar van Adobe Analytics. Laten we over de poten en de weg gaan.

**Hoe**

***De meetconferentie:***

1. Zorg ervoor dat uw belanghebbenden bij elkaar komen, hetzij persoonlijk, hetzij praktisch met het doel na te gaan wat u moet meten. Dit zou sommige uitvoeringen moeten omvatten.
1. Heb sommige duidelijke voorbeelden op het bord op kleverige nota&#39;s reeds, dingen zoals opbrengst, verkoop, of lood, zeer kernPKIs u weet zal worden gemeten. Herhaal deze stappen met dimensies, zoals de aanmeldingsstatus, productcategorieën of zoektermen.
1. Iedereen eigen notities laten toevoegen, zonodig groeperen
1. Laat mensen stemmen over de dingen die ze belangrijk vinden. Dit zijn onbeperkte stemmen, omdat misschien al deze cijfers en dimensies belangrijk zijn.
1. Voor wie weinig stemmen heeft, hebben de belanghebbenden die om hen vroegen verklaren wat zij hen zullen gebruiken. Als er een goede gebruikszaak is, houd het binnen. Als er een betere manier is om die gegevens te verkrijgen, kunnen ze niet uitleggen hoe ze kunnen optreden, of er is nog een andere goede reden om ze weg te laten, het van het bord te halen.
1. Voeg deze metriek en dimensies aan uw SDR toe voor een eerste overzicht door de belanghebbenden die aanwezig waren

***De Trechter Map***

1. Krijg een visualisatie van alle trechters, stap voor stap met elke inbegrepen staat
1. Met de ontwerpers en productmanagers, ga door elke stap en praat door wat zij als succes op die trechter beschouwen. Is het de omrekeningskoers? Kies zij een bepaald pad? Gebruikt het bepaalde functies?
1. Stel vragen over welke metriek en afmetingen nodig zijn om de prestaties van de trechter in elke stap van de trechter en in het algemeen te begrijpen.
1. Voeg boven elke stap van de trechter de metriek en de afmetingen toe die bij die stap, met inbegrip van de berekende metriek zullen worden gemeten.
1. Aan het begin van elke trechter, schrijf de rapporten uit die in het dashboard zullen gaan dat de productmanager zal gebruiken om prestaties, dingen zoals een reserve rapport, huidige maand en trended omzettingspercentages, en om het even wat specifieker voor die trechter te volgen.
1. Voeg de nieuwe metriek en de afmetingen toe u aan SDR hebt ontdekt en verzend het naar de belanghebbenden voor een tweede overzicht.

***De voorbeelddashboards***

1. Met de Kanaalkaart als richtlijn maakt u mockup-dashboards.
1. Er moet een algemene weergave zijn, zoals een Executive Summary Dashboard, en dashboards voor elk van de trechters.
1. Er zijn ook enkele specifiekere opties voor uw site of toepassing, zoals de prestaties van producten of inhoud.
1. Geef deze informatie door aan de relevante belanghebbenden en krijg feedback over het ontwerp.
1. Breng de gewenste updates aan en voeg deze toe aan uw SDR als er nieuwe maatstaven of dimensies nodig zijn.
1. Verzend de bijgewerkte voorvertoningsdashboards en SDR voor een laatste revisie.

***Hulpmiddelen voor gegevensdemocratisering***

1. Maak een gegevenswoordenboek. De SDR is voor uw modellen. Het gegevenswoordenboek is bestemd voor uw eindgebruikers. Zorg dat deze leesbaar is voor eindgebruikers, zodat ze gemakkelijk kunnen zien welke gegevens beschikbaar zijn en weten hoe ze deze kunnen gebruiken. Uw eindgebruikers zouden de definitieve fiatteurs van dit moeten zijn.
1. Annotaties. In elke organisatie zijn er bepaalde data die elk jaar van belang zijn en andere die zullen opduiken. Zorg ervoor dat u de relevante bestanden van uw belanghebbenden verzamelt en deze als annotaties toevoegt om meer inzicht te krijgen in de gegevens die ze zien.
1. Curatie. Als uw SDR groot is, is het misschien overweldigend. Paralyse van keuze is niet alleen van toepassing op uw klanten. Bekijk wat belangrijk is voor elke groep gebruikers en bekijk de elementen die ze zullen zien.

**Waarom**

***Om vereisten te verkrijgen***

Dit is duidelijk, maar er zijn andere effectieve manieren om eisen te stellen. Persoonlijk heb ik er één gebruikt voor één interviews, vragenlijsten en revisies op bestaande rapporten. Dat zal werken, maar ik denk niet zo goed als de methoden die ik zojuist heb geschetst. Ik denk eerlijk gezegd niet dat de kloof in het verzamelen van vereisten zo groot is. De methode die ik heb beschreven zal je 95% van de manier daar brengen, en deze andere methodes zullen u 90% van de manier krijgen. Wat is de grote reden?

***Gegevenscultuur samenstellen***

Met dit proces:

- Spark diep nadenken over hoe succes kan worden gemeten
- Zorgen voor een gevoel van betrokkenheid bij uw belanghebbenden
- Het voor belanghebbenden gemakkelijker maken om hun gegevens te begrijpen

***Diep nadenken over gegevens***

Voor veel van de mensen in je bedrijf is data iets wat ze consumeren. Ze gebruiken het. Ze analyseren het. Ze denken er niet diep over na. Sommige van hen erven rapporten en processen van hun voorgangers zij niet veranderd wegens de behoefte aan continuïteit. Ze hoefden nooit na te denken over de reden van de data.

Dit proces biedt hen de kans om echt *begrijpen* gegevens. Wat is succes als je de vragen stelt? Hoe zou je weten of je succesvol was? Hoe zou je weten wat te veranderen als je niet succesvol was? Dit is een oefening die aan het begin van het creëren van elke plaats, app, en product zou moeten worden gedaan, maar veel te vaak is niet. Door deze vragen te stellen, helpt u hun begrip van niet alleen de gegevens, maar ook hun eigen product te vergroten.

***Een gevoel van eigendom maken over de gegevens***

Dit is niet iets dat van bovenaf is overgeleverd. Dit is niet iets wat drie maanden geleden een dertigminieme vergadering was. Dit is niet die vervelende vragenlijst die ze een week lang hebben opgehangen om te beantwoorden en die ze haast hebben gemaakt, omdat ze een demo hadden om naar te gaan zodat ze de datum van publicatie van de sprint konden maken. Dit is het product van hun diepgewortelde gedachte en hun werk met jullie en hun collega&#39;s, het ding waar ze meerdere keren over hebben gekeken, doorlopende feedback voor hebben gegeven, en dat ze hebben goedgekeurd nadat die feedback was opgenomen. Het is van hen! Dat het nuttig is, komt door hen. Het is *hun* gegevens en het is het proces dat ze heeft gemaakt.

***De gegevens begrijpelijker maken***

U hebt hen ook getoond hoe zij het zullen gebruiken en hoe het door de voorproefdashboards zal kijken. Elke nieuwe oplossing is *hard*. Er is zoveel te leren en gezien de enorme aanpassingsmogelijkheden van Adobe Analytics, kan de leercurve vrij steil zijn. Daar heb je 80% van verwijderd. Zelfs voordat de eerste coderegel is geschreven, weten uw belanghebbenden hoe hun dashboards eruit zullen zien. Ze zullen weten hoe ze ze kunnen lezen en betekenis ervan krijgen. Ze zullen weten hoe succes er letterlijk uitziet, omdat ze je hebben verteld welke maatstaven en dimensies succes definiëren, en je hebt hen verteld hoe dat voor hen zichtbaar zal zijn. De levering van de daadwerkelijke dashboards is een verfrisser, niet een eng nieuwe leertaak.

Dit is niet de snelste manier om een SDR bij elkaar te krijgen. Het is een hoop werk en vereist veel coördinatie van schema&#39;s, vooral omdat het van essentieel belang is dat je een paar directeuren in de mix hebt. Uiteindelijk is een oplossing voor bedrijfsanalyses echter een enorme investering in tijd en geld, en u wilt ervoor zorgen dat adoptie en tevredenheid hoog zijn. Deze methode is een hele stap in de goede richting.

**Auteur**

Dit document is geschreven door:

![gitai-headshot](assets/gitai-headshot.png)

Gitai Ben-Ammi, Business Architecture Associate Manager bij Accenture

Adobe Analytics Champion


