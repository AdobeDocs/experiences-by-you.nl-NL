---
title: Modellen voor het scoren van personen voor programma's voor Marketo's Engage samenstellen
description: Met Adobe Marketo Engage kunt u uw scoremodel(en) helemaal vanaf de grond samenstellen. Voordat u direct in Marketo Engage gaat om uw scoreprogramma's te maken, moet u de belangrijkste score instellen, zoals Demografische score, Gedragsscore en Totaal aantal personen. Meer informatie over de strategieën die worden gebruikt door Marketo Engage Champions voor het ontwikkelen van Scoremodellen die uw bedrijf nodig heeft.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14810
thumbnail: KT-14810.jpeg
source-git-commit: 47ab8875bc4e41595cd40550330e43a88357b68d
workflow-type: tm+mt
source-wordcount: '2111'
ht-degree: 0%

---

# Een model voor het scoren van personen maken

Met persoonlijke scoring kunt u de mensen identificeren die het meest betrokken zijn bij uw bedrijf en uw ideale klantprofiel zijn, zodat u deze leads kunt delen met uw verkoopteam en de beste deals kunt sluiten. Samen met de verkoop, bepaalt u wat u aan hen door een lood/persoon te gebruiken scoring programma in Adobe Marketo Engage leidt af te geven. Dit kan worden bepaald door een minimum aan gedragscoring, demografische scoring of beide.

In deze zelfstudie zullen we u drie oefeningen doorlopen die door Marketo Engage Champions Christina Zuniga en Katja Keesom worden voorgesteld. Volg verder om te bepalen welke activiteiten en kenmerken belangrijke indicatoren zijn die een vooruitzicht in aankoop (gedragscoring) geinteresseerd is en het juiste pasje voor u (demografische scoring), en rekenschap geven van de nuances over de markten.

## Waarom ontwikkelen en gebruiken van een persoon die model scoring?

U hebt misschien veel leads in uw database, maar hoe weet u welke klaar zijn om uw producten en services nu te kopen? Aangezien uw marketing organisatie probeert om loodkwaliteit en verkoopbereidheid te optimaliseren, is dit waar het het scoren model in spel komt.

Door mensen in uw gegevensbestand van het Marketo Engage te scoren, kunt u meten hoe gekwalificeerd uw geproduceerde lood is en criteria plaatsen voor wanneer zij verkoopklaar zijn. Hierdoor kan uw verkoopteam zich richten op de leads die het meest waarschijnlijk zullen sluiten terwijl het marketingteam de andere mensen in de database blijft voeden via hun marketingprogramma&#39;s.

## Oefening 1 - Bepalen van de interesse van de koper met gedragscores

Gedragscoring geeft een numerieke waarde aan traceerbare acties die in het vooruitzicht worden gesteld en die wijzen op interesse in uw producten en services en de intentie om te kopen. Als u bijvoorbeeld de website bezoekt, wordt interesse getoond en kunt u de prijspagina bezoeken met de bedoeling. Als u daarentegen de pagina met carrières bezoekt, geeft dit mogelijk aan dat de persoon niet gaat kopen.

**Stap 1** - Een lijst maken met mogelijke activiteiten die van belang zijn voor uw verkoopproces of die van belang zijn voor uw organisatie. Het kan handig zijn om samen met uw verkoopteam te bepalen welke activiteiten aangeven dat een lead de intentie heeft om te kopen, zodat u de criteria kunt afstemmen op de verkoop en prioriteiten kunt stellen op basis van hun opmerkingen over gesloten deals. Hier volgen enkele suggesties voor vragen die u aan uw verkoopteam kunt stellen:

* Welke activiteiten wijzen op een goed of slecht gevolg voor u?
* Welk type inhoud dat door een lead wordt verbruikt, heeft een sterkere intentie om te kopen?

**Stap 2** - Objecten weergeven die aangeven dat er een vooruitzicht is, zijn niet geïnteresseerd in uw product. Ben zeker om activiteiten te vermelden die door Marketo Engage traceerbaar zijn.

**Voorbeeld 1a - Activiteiten die de intentie aangeven te kopen**

| **Activiteiten die de intentie om te kopen aangeven** | **Activiteiten die geen koopvoornemen aangeven** |
| --- | --- |
| Bezoek de prijspagina | Geen interactie in de afgelopen 90 dagen |
| Jaarlijkse klantgebeurtenis bijwonen | Pagina met carrières bezoeken |
| Registreren voor webinar | Abonnementen opzeggen |
| Artikel downloaden |     |
| Demoformulier voor aanvraag invullen |     |

**Stap 3** - Analyseer en kies een drempelscore voor de afkoopactie.

* Zodra een lood genoeg interesse door sommige activiteiten uit te voeren u in Stap 1 bepaalde en de totale score deze drempel overschrijdt, zult u hen aan verkoop afgeven. Deze drempel is eenvoudig een getal dat u helpt een benchmark in te stellen voor de scores die u toewijst aan individuele gedragingen.
* Uw drempelnummer moet groot genoeg zijn, zodat iemand meerdere interacties met uw merk moet uitvoeren om aan deze voorwaarde te voldoen. Het is bijvoorbeeld onwaarschijnlijk dat één e-mailbericht voldoende is geopend. Als u net begon, probeer werkend met een drempel van 100 en bouwend uw persoon die van daar scoring.
* Het plaatsen van een hoge of lage drempel hangt af van welke leiden uw verkoopteam het meest in het ontvangen en ontwikkelen in bedrijfskansen geinteresseerd is. Als u over bestaande gegevens over uw recente verkoopovereenkomsten beschikt, analyseert u deze en bekijkt u welke acties mensen hebben ondernomen in geslaagde overeenkomsten. Dit kan u helpen om te bepalen hoeveel aanraakpunten in een gekwalificeerde verkooplood gaan en u helpen van hieruit extrapoleren wat uw drempelnummer zou moeten zijn.

**Voorbeeld 1b - Drempel voor verkoopuitstel:**

| Gemiddeld aantal aanraakpunten voor gekwalificeerd lood | 4 |
| --- | --- |
| Drempel voor verkoopuitstel | 50 |

**Stap 4** - Een score toewijzen aan elke activiteit die wordt vermeld in &#39;Voorbeeld 1a - Activiteiten die de intentie om te kopen aangeven&#39;.

* Gebruik een positieve gedragsscore voor de activiteiten die op interesse wijzen om de algemene loodscore van een vooruitzicht te verhogen, en een negatieve score om op oninteresse te wijzen.
* Gebruikend uw drempel van &quot;Voorbeeld 1b - Drempel voor verkoopoverdracht&quot;als benchmark, bepaal uw gedragsscores met betrekking tot het belang van hun acties. Voorbeelden die een demo aanvragen, moeten bijvoorbeeld rechtstreeks naar de verkoop gaan. Het toewijzen van die actie aan een puntwaarde die gelijk is aan uw perspectiefdrempel voor het afhandelen, heeft de meeste zin. Ondertussen is het downloaden van een witboek niet zo&#39;n sterke indicator van koopbelangstelling en zou het daarom minder waard moeten zijn.

**Voorbeeld 1c - Scoreactiviteiten die de koopintentie aangeven:**

| Drempel voor verkoopuitstel = 50 punten |     |
| --- | --- |
| Activiteit | Score |
| Ingevuld &quot;request a demo form&quot; | +50 |
| Geen interactie in de afgelopen 90 dagen | \-10 |
| Een witboek downloaden | +5 |
| Bezoek ons op een tradeshow | +15 |

**Stap 5** - Onthoud, scoring is een herhalend proces. U kunt scores en drempels voortdurend controleren en aanpassen terwijl u meer gegevens voor analyse verzamelt.

## Oefening 2 - Het identificeren van het juiste pasvorm met Demografische Scores

Nu u de activiteiten hebt gedefinieerd die de koopintentie aangeven, moet u het scoremodel voltooien met uw ideale perspectiefprofielen. Om te bepalen of een vooruitzicht voor verder verkoopgesprek geschikt is, is het belangrijk om demografische scores naast gedragsscores toe te wijzen zodat de modelhulp de beste lood in termen van passend en intent bepaalt.

**Stap 1** - Maak een lijst van eigenschappen voor uw ideale vooruitzichten.

* Denk na aanbiedingsattributen zoals hun industrie, bedrijf, afdeling, en rol. Zorg ervoor dat deze eigenschappen overeenkomen met de beschikbare demografische velden in uw Marketo Engage-exemplaar.
* Het werk met uw verkoopteam om te bepalen welke lood aan verkooponderzoeken het meest beantwoordt en belangrijkste contacten tijdens verkoopkansen zijn.
   * Het kan nuttig zijn om recente gesloten gewonnen kansen te analyseren om te zien welke eigenschappen uw beste klanten hebben. Bijvoorbeeld:
      * Door gesloten verloren kansen voor patronen te graven, kunt u demografische gegevens vinden die u wilt vermijden.
      * Beslissingsmakers en interne kampioenen identificeren die je verkoopinspanningen sturen. Diep duik in de gegevens en breng uw bevindingen naar een workshop met een deel van uw verkoopteam om uw conclusies te valideren of te verfijnen.
   * U kunt uw verkoopteam ook interviewen met de volgende voorbeeldvragen:
      * Met welke afdeling zijn ze meestal bezig?
      * Wat zijn de functies van de mensen die betrokken zijn bij productdemo&#39;s en wie zijn de mensen die zich bij de aankoop moeten afmelden?

**Voorbeeld 2a - Ideale perspectiefkenmerken**

| **Categorie** | **Ideale perspectiefkenmerken** |
| --- | --- |
| Industrie | Ruimtevaart, industrie |
| Bedrijfsomvang | 100 - 999, 1.000 - 9.999 |
| Functie | Director, vicepresident, C-niveau |
| Afdeling | HR |

**Stap 2** - Wijs een score toe aan elk kenmerk afhankelijk van de relevantie ervan in uw ideale perspectiefprofiel. Gebruik positieve scores voor wenselijke kenmerken en negatieve scores voor kenmerken die de lood minder geschikt maken voor uw product.

**Voorbeeld 2b - Muziek toewijzen aan ideale en ongewenste perspectiefkenmerken**

| **Kenmerk** | **Score** |
| --- | --- |
| Industrie - ruimtevaart | +10 |
| Industrie - Industrie | +5 |
| Bedrijfsomvang - 100 - 999 | +5 |
| Bedrijfsomvang - 1.000 - 9.999 | +10 |
| Bedrijfsomvang - &lt;10 | \-10 |

## Oefening 3 - De lokale flexibiliteit van uw het scoren model opnemen

Met de basismodellen voor gedrag en demografisch scoren die u hebt voltooid, kunt u deze naar een hoger niveau tillen door lokale flexibiliteit toe te staan. De bedrijfswaarden kunnen in verschillende markten variëren wanneer een organisatie globaal werkt. In de volgende oefening, zult u leren hoe te om scores toe te passen om de echte bedrijfswaarde van de belangrijkste activiteiten of kenmerken in verschillende situaties te weerspiegelen.

Heb je de voorkeur aan een videodemo voor deze oefening? Aanpassen als Marketo Engage Champion Katja Keesom laat zien hoe u lokale flexibiliteit inbouwt in het scoremodel.

>[!VIDEO](https://video.tv.adobe.com/v/3426914/?learn=on)

**Stap 1** - Neem de activiteiten en kenmerken van oefeningen 1 en 2 en bepaal voor elk punt of zij per locatie of productlijn verschillen.

**Voorbeeld 3a - Signalen op mondiale en lokale markten:**

| **Signaal** | **Algemeen** | **Lokaal** |
| --- | --- | --- |
| Activiteiten | <ul><li>Formulier &quot;Verzoek om demo&quot; ingevuld</li><li>Geen interactie in de afgelopen 90 dagen (ongeveer 3 maanden)</li></ul> | <ul><li>Bezoek ons op de beurs</li><li>Een witboek downloaden</li></ul> |
| Kenmerken | <ul><li>Afdeling</li><li>Functie</li></ul> | <ul><li>Industrie</li><li>Bedrijfsomvang</li></ul> |

**Stap 2** - Definieer uw scorematrix voor lokale markten:

* Stel een andere matrix in voor demografische en gedragselementen.
* Bepaal de onderwerpen van prioriteiten voor u om de input van het lokale team te vragen op.
* Bepaal het aantal waarden die worden gebruikt om binnen uw onderwerpen te schatten.
* Wijs individuele waarden toe door relatieve waarde uit te lijnen met algemene scores.
* Overweeg gemeenschappelijke scenario&#39;s te bepalen wanneer de vooruitzichten met uw merk in wisselwerking staan en uw algemeen het scoren voor hen te testen.
   * Zo is het bijvoorbeeld gebruikelijk dat iemand uw website op een inhoudspagina invoert, vervolgens naar een productpagina klikt en een brochure downloadt. U zou hen richten met een webinar uitnodiging, en zij antwoorden aan het door te registreren, maar niet het bijwonen. Bedenk of uw verkoop al met deze persoon wil spreken of niet en evalueer of uw het scoren model deze vooruitzichten aan de juiste algemene score krijgt om dat niveau van interesse te weerspiegelen.

**Voorbeeld 3b - Demografische scorematrix:**

| **Demografische matrix** | **Prioriteit 1** | **Prioriteit 2** | **Prioriteit 3** |
| --- | --- | --- | --- |
| Hoge waarden | 20 punten | 10 punten | 7 punten |
| Normale waarden | 10 punten | 7 punten | 3 punten |
| Lage waarden | 5 punten | 3 punten | 1 punt |

**Stap 3** - Verzamel input van uw lokale of regionale verkoopteams om een holistische mening te ontwikkelen. In voorbeeld 3c worden geen individuele scores vermeld. Dit staat het verkoopteam toe om zich op de relatieve waarde van de verschillende onderwerpen tijdens het overzichtsproces te concentreren. Nochtans, zou u uw volledig model moeten hebben dat als achtergrondmaterialen voor andere beheerders van de Marketo Engage wordt gedocumenteerd.

* Vergrendel wat niet kan worden aangepast voor algemene consistentie (hier in de kolom &quot;Onderwerp implementeren&quot;).
* Markeer (hier in de kolommen &quot;Prioriteit&quot; en &quot;Score&quot;) wat kan worden aangepast aan lokale invloeden.

**Voorbeeld 3c - Relatieve waarde van het scoren van onderwerpen:**

<table>
 <tr>
    <th>Aantal</th>
    <th>Onderwerp implementeren</th>
    <th>Demografisch/gedrag</th>
    <th>Onderwerp</th>
    <th>Prioriteit</th>
    <th>Waarden</th>
    <th>Scores</th>
 </tr>
 <tr>
    <td rowspan="6">1</td>
    <td rowspan="6"><b>VEREIST</b></td>
    <td rowspan="6">Demografisch</td>
    <td rowspan="6">Industrie</td>
    <td rowspan="6"><b>2</b></td>
    <td>Technologie</td>
    <td><b>Hoog</b></td>
  </tr>
  <tr>
    <td>Mode</td>
    <td><b>Hoog</b></td>
  </tr>
  <tr>
    <td>Detailhandel</td>
    <td><b>Normaal</b></td>
  </tr>  
  <tr>
    <td>Productie</td>
    <td><b>Normaal</b></td>
  </tr>
  <tr>
    <td>Gezondheidszorg</td>
    <td><b>Laag</b></td>
  </tr>
  <tr>
    <td>...</td>
    <td><b>Laag</b></td>
  </tr>
<tr>
    <td rowspan="3">2</td>
    <td rowspan="3"><b>Ja</td>
    <td rowspan="3">Demografisch</td>
    <td rowspan="3">Bedrijfsomvang (werknemers)</td>
    <td rowspan="3"><b>3</td>
    <td>&gt; 1000 werknemers</td>
    <td><b>Hoog</td>
  </tr>
  <tr>
    <td>250-999 werknemers</td>
    <td><b>Normaal</td>
  </tr>
  <tr>
    <td>1-249 werknemers</td>
    <td><b>Laag</td>
  </tr>  
<tr>
    <td rowspan="3">3</td>
    <td rowspan="3"><b>Nee</b></td>
    <td rowspan="3">Gedrag</td>
    <td rowspan="3">Paginabezoeken op uw website</td>
    <td rowspan="3"><b>2</b></td>
    <td>&gt;Productinformatiepagina's</td>
    <td><b>Laag</b></td>
  </tr>
  <tr>
    <td>Prijspagina's</td>
    <td><b>Normaal</b></td>
  </tr>
  <tr>
    <td>Pagina Demo-verzoek</td>
    <td><b>Hoog</b></td>
  </tr>
</table>

## Wat is de volgende?

* Download de [oefenblad voor persoonlijke scores](./assets/build-person-scoring-model-and-local-flexibility-in-adobe-marketo-engage.docx){target="_blank} om uw scoremodel offline te ontwikkelen.
* Maak uw persoonlijke scores in het Marketo Engage. Dit controleren [zelfstudie](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch){target="_blank} en [demo](https://experienceleague.adobe.com/en/docs/events/marketo-and-mochas-recordings/2023/lead-scoring){target="_blank} aan de slag. U kunt een programma voor het scoren van leads/personen importeren [template](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program){target="_blank} van de Bibliotheek van de Verwijzing van het Marketo Engage om de programmabouw te versnellen.
* Maak twee versies van het scoreprogramma:
   * Een centraal programma dat alle scoring uitvoert die niet lokaal kan worden bijgewerkt.
   * Een lokale kopie met de scorende elementen die configureerbaar zijn.
* Stel uw scorewaarden in als tokens in het scoreprogramma. Dit zorgt voor consistentie, zelfs wanneer u de scores in de loop van de tijd aanpast.
   * Een gemeenschappelijk voorbeeld van verdeelde scores heeft een token voor activiteiten van hoge waarde die automatisch aan uw drempel voldoen, zoals het aanvragen van een demo of het boeken van een vergadering met uw verkoopteam. Zelfs als u de vereiste minimumscore wijzigt om aan uw drempel te voldoen, kunt u alle activiteiten met een hoge waarde eenvoudig tegelijk bijwerken door één token bij te werken.
* Pas uw lokale slimme campagne aan voor elke locatie:
   * Bepaal welke demografie en gedragsactiviteiten slechts één keer moeten scoren (d.w.z. industrie) en welke scores elke keer dat een vooruitzicht kwalificeert (d.w.z. een webinar bijwonen). Dit verzekert potentiële contacten die door de verandering van de gegevenswaarde worden teweeggebracht voor verkoop relevant zijn.
   * Zorg ervoor dat je keuzes elkaar uitsluiten.
   * Breng uw updates in beide stroomstappen zodat de Score van de Persoon op een identieke manier aan de Demografische Score wordt bijgewerkt. Op die manier blijft de persoonlijke score in overeenstemming met de combinatie van gedragsscore en demografische score.
* Test de slimme campagne zodra u klaar bent met het ontwikkelen van uw programma. Ga bijvoorbeeld naar uw demo-formulier, vul het in met een teste-mail en controleer de score van de testpersoon in [Marketo Engage-database](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring#step-view-the-person-info){target="_blank}.
* Nadat u uw model hebt opgebouwd, kunt u overwegen een waarschuwing in te stellen om naar de verkoop te gaan zodra de score van de persoon de drempel voor het afleveren van de verkoop heeft bereikt. Meer informatie over het instellen van een waarschuwing met deze [zelfstudie](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert){target="_blank}.

### Auteurs

{{christina-zuniga}}

{{katja-keesom}}

{{amy-chiu}}