---
title: Uitgebreide gids voor het overgaan naar  [!DNL Adobe Analytics]  van Google  [!DNL Analytics]
description: Leer over de plaats van gelijkwaardige functionaliteit en hoe te om het efficiënt te gebruiken wanneer het overgaan van Google  [!DNL Analytics]  aan  [!DNL Adobe Analytics]
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
exl-id: 646bdc8f-c95e-40be-b2f7-8e4ba5653d91
source-git-commit: 02e3a6dfa59df45113242bd8e874e18e9e1efd58
workflow-type: tm+mt
source-wordcount: '3323'
ht-degree: 0%

---

# Uitgebreide handleiding voor het overschakelen van Google naar [!DNL Adobe Analytics] [!DNL Analytics]{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. Inleiding

Een van de grootste uitdagingen bij het schakelen tussen alle tools is het leren waar equivalente functionaliteit te vinden is en leren hoe u deze efficiënt kunt gebruiken. Deze discussie maakt deel uit van een uitgebreidere handleiding waarmee gebruikers gemakkelijker kunnen overstappen op [!DNL Adobe Analytics] (als een nieuwe gebruiker of een gebruiker die uit Google komt [!DNL Analytics] ). Een diepgaande vergelijking met GA; als het meest waarschijnlijke vergelijkingsinstrument waarmee de meeste gebruikers vertrouwd zijn; wordt verstrekt om gebruikers te helpen bestaande kennis met de nieuwe toolset correleren. Als deze praktijk niet kan worden vervangen, kunt u op deze manier aan de slag gaan en de frustraties die u tijdens deze periode kunt ondervinden, verminderen.

We moeten een snelle vergelijking van terminologie hebben:

| **Beschrijving** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| Er is een gebeurtenismetrische waarde weergegeven die een pagina (of scherm in een app) vertegenwoordigt | Paginaweergave | Voorvertoning |
| Een metrische waarde die een groep interacties op uw website of app vertegenwoordigt die in hetzelfde tijdkader plaatsvinden | Bezoek | Sessie |
| Een metrische waarde die een geïdentificeerd apparaat definieert (op basis van meerdere criteria, waaronder cookies en andere gedragspatronen) om gebruikersinformatie te koppelen. | Unieke bezoeker | Gebruiker |

## 2. De interfaces

Wanneer mensen [!DNL Adobe Analytics] en Google [!DNL Analytics] vergelijken, merken ze op dat de interface van [!DNL Adobe] eerst ontmoedigend is. Dit is waar, maar het is ook; geloof het of niet; een kracht, geen zwakte. [!DNL Adobe] biedt een groot aantal gereedschappen en flexibiliteit in uw gegevensvisualisatie, waardoor u veel meer vrijheid hebt om te bouwen wat u nodig hebt.

Laten we beginnen met de &#39;in-site&#39; rapportage.

### 2.1. Rapportage ter plaatse

#### 2.1.1. Homescherm

Zowel [!DNL Adobe Analytics] als Google [!DNL Analytics] bieden een manier om de eerste weergave aan te passen die een gebruiker ziet wanneer hij of zij zich aanmeldt.

##### 2.1.1.1. Homescherm Workspace / Aangepaste set ([!DNL Adobe Analytics])

[!DNL Adobe Analytics] veronderstelt niet om een vooraf gebouwd rapport tot stand te brengen voor alle gebruikers om bij login te zien. De standaardstartpagina neemt de gebruiker naar het Workspace-landingsscherm, waarin elke gebruiker alle werkruimterapporten ziet die hij heeft gemaakt of met hem heeft gedeeld. Ook, kan elke gebruiker om het even welk van deze rapporten als hun homescherm plaatsen als zij zo kiezen.

![&#x200B; werkruimte-creeer-project &#x200B;](assets/ga-to-aa_1.png)

Hieronder vindt u meer informatie over de werkruimte verderop in deze handleiding. Zie punt 2.1.2.1

>[!TIP]
>
>Creeer/deel sommige standaardrapporten voor uw organisatie zodat zij een uitgangspunt hebben om informatie te zien zonder het moeten in de bouw van hun eigen rapporten meteen duiken.



##### 2.1.1.2. Schermafbeeldingen op het startscherm (Google [!DNL Analytics])

* Google [!DNL Analytics] Home Screen beschikt over enkele kant-en-klare visualisaties. Deze omvatten zaken als:
* Gebruikers, sessies, Bounce Rate en Session Duration in de laatste zeven dagen
* Gebruikers op tijdstip van de dag in de laatste 30 dagen
* Huidige gebruikers nu en de bovenste actieve pagina&#39;s
* Verkeerskanaal, Source/Medium en verwijzingen in de afgelopen zeven dagen
* Sessies per land in de laatste zeven dagen
* Bovenste pagina&#39;s voor de laatste zeven dagen
* Ontwikkeling van actieve gebruikers in de afgelopen 30 dagen
* en meer

GA4-gebruikers hebben meer mogelijkheden om hun eigen rapporten aan te passen en toe te voegen aan het Homescherm.

![&#x200B; google-analytics-interfaces &#x200B;](assets/ga-to-aa_2.png)

Dit is waarschijnlijk één ding dat u het meest mist in [!DNL Adobe Analytics]. Er is geen beginscherm voor u vooraf gebouwd. U kunt echter eenvoudig een aangepaste Workspace instellen om te repliceren wat u in de bovenstaande lijst nodig hebt en deze in te stellen als landingsscherm. Meer informatie over dit onderwerp vindt u later (of zie Sectie 2.1.2.1 [!DNL Adobe] Workspace).

#### 2.1.2. Reporten Builder ter plaatse

Naast de Eenvoudige Rapporten die de analysehulpmiddelen bonden, verstrekt elk hulpmiddel ook krachtigere hulpmiddelen waarmee om uw eigen douanerapporten te bouwen.

##### 2.1.2.1. [!DNL Adobe Analytics] Workspace

Dit is de drijvende kracht van [!DNL Adobe Analytics], sinds de introductie ervan in 2017 is het het pad geworden voor [!DNL Analytics] -analyse, en de primaire reden waarom de sectie Reports binnenkort zal worden verst.

Met dit gereedschap kunt u rapporten opbouwen met bijna volledige vrijheid.

Het rapport kan worden opgedeeld in deelvensters en die deelvensters kunnen een willekeurig aantal visualisaties bevatten. Deelvensters kunnen worden ingesteld op algemene informatie, zoals datumbereik en algemene segmentfilters.

U kunt zowel de deelvensters als de visualisaties in de deelvensters groter of kleiner maken en rond de deelvensters slepen om items naast elkaar weer te geven, of u kunt ze stapelen. Dus als u twee verschillende gegevensreeksen naast elkaar wilt vergelijken, zou u panelen kunnen creëren die 50/50 onderaan het midden verdelen die de twee plaatsen naast elkaar tonen voor gemakkelijke vergelijking.

Gebruikers beschikken over een groot aantal visualisaties:

* Vrije-vormentabel
* Cohortabel
* Fallout
* Stroom
* Grafieken
   * Gebied (gestapeld en niet gestapeld)
   * Lijn
   * Spreiding
   * Staaf (gestapeld en niet gestapeld)
   * Opsommingsteken
   * Donut
   * Histogram
   * Horizontale balk (gestapeld en niet gestapeld)
* Kaart
* Samenvattingsblokken
   * Samenvattingswijziging
   * Samenvattingstekst
   * Tekst (tekstveld zonder invoervak waarin extra informatie moet worden ingevoerd om context te geven)
* Venn

Elk deelvenster en elke visualisatie kunnen een naam krijgen en er kan een beschrijving op worden toegepast om context te geven aan wat de informatie weergeeft.
In [!DNL Adobe] zijn segmenten (in feite gegevensfilters) retroactief van toepassing. Deze kunnen in kolommen van vrije-vormtabellen worden getrokken om gegevens naast elkaar te vergelijken. Bijvoorbeeld, als een gebruiker twee verschillende categorieën op hun plaats voor verkeer wilde vergelijken; zij konden een segment voor &quot;Categorie A&quot;en een verschillend segment voor &quot;Categorie B&quot;tot stand brengen.

![&#x200B; analytics-page-views-rapport &#x200B;](assets/ga-to-aa_3.png)

In vrije-vormtabellen zijn meerdere kolommen en segmentatie mogelijk, indien nodig, om de gegevens op de gewenste manier te visualiseren.

Als u geen onderbreking door datum wilt zien, eenvoudig sleep en laat vallen een andere afmeting of segment daar om de gegevens op een verschillende manier te zien. Gebruik bijvoorbeeld segmenten voor Apparaattype en voeg vervolgens een uitsplitsing toe naar besturingssysteem voor uw mobiele gebruikers/gebruikers van tablets:

![&#x200B; analytics-compare-page-views-rapport &#x200B;](assets/ga-to-aa_4.png)

Workspace laat je creativiteit vliegen, je bent niet beperkt tot &#39;standaard&#39; indelingen. U kunt de visualisaties opbouwen die u nodig hebt om diepgaand in de vergelijkingen te duiken u moet in werking stellen.

>[!TIP]
>
>Wees niet bang om te spelen en te verkennen. Er zijn zoveel manieren om buiten de doos te denken. Bovendien toont de validatie van wat u hebt gemaakt wat u denkt. Ervaar hulp!

U kunt de berekende metriek of de segmenten tot stand brengen die slechts binnen het rapport leven om overstroming van uw segment en berekeningsbewaarplaats te verhinderen. Dit staat u toe om geconcentreerde punten tot stand te brengen die voor specifieke rapporten nodig zijn zonder uw organisatie met dingen te verwarren die niet in andere contexten bruikbaar zijn.

Deze discussie is slechts een inleiding op dit instrument, er zijn andere uitgebreide gidsen om u op gang te brengen. Nadat u deze handleidingen hebt bekeken, kunt u uitgebreide rapporten zoals deze weergeven:

![&#x200B; werkruimte-dashboard &#x200B;](assets/ga-to-aa_5.png)

De werkruimten niet auto-sparen, zodat is het gemakkelijker om een eenmalig, ad-hoc rapport te doen zonder uw rapportbewaarplaats te registreren.

Een andere krachtige eigenschap van werkruimten is de capaciteit om interactieve bepalingen op uw rapporten in de vorm van drop-down toe te passen. Deze drop-down werken niet aan uitgevoerde CSV of dossiers van PDF van uw rapporten. In het live rapport kunt u echter alle visualisaties in een deelvenster bijwerken, zodat hetzelfde rapport onder verschillende omstandigheden wordt weergegeven. Meerdere vervolgkeuzelijsten kunnen worden gebruikt, en op voorwaarde dat de opties elkaar niet uitsluiten, worden de geselecteerde items gestapeld zodat er op een schone manier informatie kan worden gepresenteerd.

>[!IMPORTANT]
>
>Meer informatie over het gebruiken van drop-down en freeform onderverdelingen zie <https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680>

##### 2.1.2.2. Google [!DNL Analytics]: dashboards, Custom Reports en Saved Reports

Google beschikt over een paar gereedschappen voor het maken van rapporten binnen de interface, maar deze werken nog steeds met dezelfde weergave en beperkingen van de rapportsectie.

Nu, voor degenen die in Google [!DNL Analytics] zijn geverfd als je dit leest, zou je kunnen zeggen: &quot;Wacht eens even, wat met Google Data Studio, is dat niet beter dan de Workspace van [!DNL Adobe]?&quot; Ja, maar de Studio van Gegevens is technisch geen deel van het [!DNL Analytics] hulpmiddel, en het staat voor verbindingen aan verschillende gegevensbronnen toe. Dit hulpmiddel wordt behandeld later in de &quot;Uitgebreide sectie van de Toegang van het Rapport&quot;, specifiek paragraaf 2.2.3.

Met Google-dashboards en aangepaste rapporten kunt u meerdere visualisaties samenvoegen tot één rapport, maar in tegenstelling tot Workspace bent u nog steeds vergrendeld in eenvoudige correlaties en welke gegevens u in welke kolommen kunt plaatsen.

In de Rapporten van de Douane, één van de grootste uitdagingen is wanneer u een filter creeert, is het op alle lusjes van het rapport van toepassing. Er is geen manier om twee verschillende filters binnen het zelfde rapport te vergelijken.

Voor oppervlakvergelijkingen, doet het het werk. Deze zijn allemaal vergelijkbaar met de oude [!DNL Adobe] dashboards, aangepaste rapporten en bladwijzers. De belangrijkste hulpmiddelen die worden verstrekt om uw behoeften te steunen, die binnen de rapportreeks verblijven.

#### 2.1.3. Verslagen

Zowel Google als [!DNL Adobe] hebben enkele rapporten waarin u kunt navigeren. Dit zijn afzonderlijke tabellen en standaardtijdlijngrafieken die rond een dimensie zijn gebaseerd.

##### 2.1.3.1. [!DNL Adobe Analytics] Rapporten

[!DNL Adobe Analytics] heeft ook een sectie Rapporten, hoewel dit ten gunste van Analysis Workspace wordt afgebouwd. In feite is het einde van de levensduur aangekondigd voor deze interface, aangezien Workspace een krachtiger instrument is. De meeste van deze tabellen kunnen eenvoudiger worden gemaakt en gewijzigd. De secties van [!DNL Adobe] zijn veel breder en dit kan ontmoedigend zijn:

![&#x200B; analytics-plaats-metriek &#x200B;](assets/ga-to-aa_6.png)

Omdat het meeste van het bovenstaande toegankelijk is via Workspaces, geef ik een kort overzicht van deze secties en hoe ze zich verhouden tot Google [!DNL Analytics] en benadruk hier de nog steeds relevante rapporten.

Sitemetriek is wat u zou verwachten. Deze heeft betrekking op de standaardmetriek (paginaweergaven, unieke bezoekers, bezoeken en aangepaste gebeurtenissen die u hebt ingesteld). Dit is gelijkaardig aan het rapport van het Gedrag GA, maar omvat ook wat van wat u in Publiek (aangezien [!DNL Adobe] niet de metrische types) zou vinden.

Hier zie je &#39;Bot&#39;-rapporten. Verkeer van bots wordt uitgesloten van al uw standaardrapporten. Er zijn echter twee rapporten die inzicht verschaffen in wat er gebeurt en welke bots naar uw site komen. Dit is vooral handig als u aangepaste Bot-regels instelt om bekende spamerbots die vaak op uw site worden aangetroffen, uit te sluiten. Je kunt enig inzicht krijgen in wat die bots doen zonder dat je hoofdrapporten overstroomd worden, maar dat verkeer. Beide rapporten zijn momenteel niet beschikbaar via Workspace (maar met de nieuwe rapportmogelijkheden die binnenkort beschikbaar zijn, kunnen gebruikers deze gegevens ook ophalen).

Site-inhoud bestaat uit een groep [!DNL Adobe] standaardafmetingen: paginanaam, sitesecties, hiërarchieën, servers en nog veel meer. Al deze dimensies zijn beschikbaar in Workspace.

Mobiel is een groep van specifieke gegevens voor mobiele apparaten, zoals apparaten, apparaattypen en meer. Deze zijn beschikbaar in Workspace.

Paden zijn niet beschikbaar in Workspace. Workspace heeft een stroomdiagram waarin u de in- en uitstromen voor één pagina/waarde kunt zien. Met Paden daarentegen kunt u zien welke paden het meest worden gebruikt in uw website. Pagina&#39;s zijn standaard het eerste padrapport dat voor u is ingesteld. U kunt dit echter ook inschakelen voor aangepaste props, zoals een waarde voor Paginatype. U zou kunnen kijken naar het plakken binnen paginatypen. Wat ik persoonlijk leuk vind aan Paden is de eenvoudige manier waarop de informatie wordt gepresenteerd... Het stroomdiagram in de werkruimte (afhankelijk van hoeveel u probeert te bekijken) kan overweldigend worden. Ik raad aan beide uit te proberen... ze hebben elk een nut en waarde afhankelijk van wat u probeert te bereiken. Opgemerkt moet worden dat elke dimensie kan worden gebruikt bij Stromen, terwijl Padden moet worden ingesteld op een proxy in het deelvenster Beheer.

De bronnen van het verkeer, [!DNL Campaign] s, en de rapporten van de Kanalen van de Marketing zijn allen gelijkaardig aan het rapport van de Aankoop bij het product van Google. De bronnen van het verkeer concentreert zich op Werkelijke Verwijzingen, [!DNL Campaign] concentreert zich op uw [!DNL Campaign] Codes, en de Kanalen van de Marketing richten zich ook op [!DNL Campaign] Codes, maar past ook extra logica toe zoals die door u op wordt bepaald hoe te om de informatie te verwerken. [!DNL Adobe] biedt meer vrijheid voor het instellen van uw regels. Google doet daarentegen veel voor je, en dit is een verandering in denken. Standaard is de Google-toewijzing voor [!DNL Campaign] -codes zes maanden. De toewijzing van [!DNL Adobe] wordt standaard ingesteld op één week. Dit kan worden gewijzigd in uw beheerinstellingen, maar in Workspace kunt u een aangepaste toewijzing boven op elke dimensie toepassen, zodat u veel meer flexibiliteit hebt.

Bezoeker retentie- en bezoekersprofiel rapporteert hetzelfde als de Audience-rapporten in Google [!DNL Analytics] . De aandacht wordt meer gericht op de terugkeerfrequentie, terwijl het Profiel van de Bezoeker meer op de Geografie en de Technologie van de gebruikers wordt gericht.

De rapporten van de Omzetting van de douane en van het Verkeer van de Douane zijn beide rapporten van de douanedimensie. Conversies zijn eVars. U kunt een aangepaste vervaldatum instellen op de waarde hit, visit, month en year. Deze waarde blijft voor een gebruiker in persistentie voor het gevormde tijdkader tenzij beschreven. Verkeersvariabelen zijn profielen. U kunt deze ook instellen voor Pathing Reports of als lijstitems die meerdere waarden splitsen op basis van een scheidingsteken naar keuze.

Media is bedoeld voor video&#39;s of audiobestanden waarin u speciale mediatracering hebt ingesteld.

De Rapporten van de douane is een sectie waar een gebruiker de kolommen en de onderverdelingen kan aanpassen die zij binnen de rapportinterface hebben gecreeerd en het opslaan als douanerapport. Zoals hierboven vermeld, moet er echter alles op maat gemaakt worden, aangezien Workspace zoveel machtigere breuken en correlaties mogelijk maakt. Dit was een goede oplossing voordat Workspace bestond.

De sectie Bladwijzers is vergelijkbaar met Aangepaste rapporten, waar vaak gebruikte rapporten als bladwijzers kunnen worden gemarkeerd in de interface Rapporten, zodat ze gemakkelijker kunnen worden gevonden.

Dashboard was een oud product dat mensen in staat stelde gegevensrapporten te combineren tot één visualisatie. Nochtans, is de functionaliteit in Workspace (Sectie 2.1.2.1) zo gemakkelijker om met te werken, dat dit slechts als toegangspunt aan erfenisrapporten bestaat die zouden moeten worden herbouwd alvorens deze eigenschap wordt geplaatst.

Met doelen kunnen mensen binnen een bepaald tijdsbestek een rapport maken op basis van een doel. De teams controleren campagnes om te zien of zijn zij op spoor om hun verkeersdoelstellingen te bereiken.

Alle rapporten hier stonden voor veelvoudige metrische kolommen en afmetingsonderverdelingen toe. De eenvoud van de visualisaties en een aantal logica achter de elementen die gecorreleerd kunnen zijn, kunnen echter soms frustrerend zijn.

##### 2.1.3.2. Google [!DNL Analytics] - rapporten

Google [!DNL Analytics] splitst deze rapporten in de volgende secties: Realtime, Audience, Acquisition, Behavior en Conversations (in GA3) en in Levenscyclus (met de subsecties: Acquisitie, Betrokkenheid, Monetisering, Behoud) en Gebruiker (met de subsecties: Demografie en Tech).

![&#x200B; google-analytics-interface-compare &#x200B;](assets/ga-to-aa_7.png)

U kunt kleine aanpassingen maken aan deze visualisaties, een secundaire afbraak toevoegen, de visualisatie wijzigen, een filter voor de gegevens maken en nog veel meer. U kunt uw aanpassingen opslaan als Opgeslagen Rapport.

Deze bieden snel en gemakkelijk inzicht in uw gegevens. Nochtans, kunt u dingen zoals Gebruikers aan paginameningen voor een pagina in de zelfde lijst vergelijken, en u kunt niet meer dan één extra dimensie toevoegen om extra gegevens te zien.

Deze zijn goed voor snelle analytische gegevens, maar als je echt diep moet graven, lijden ze aan de beperkingen.

### 2.2. Uitgebreide toegang tot rapporten

Naast &quot;Rapportering ter plaatse&quot;, bieden de meeste hulpmiddelen uitgebreide functionaliteit aan die u toestaat om uw analyse buiten de hulpmiddelen te nemen en iets te bouwen een beetje meer aangepast.

#### 2.2.1. [!DNL Adobe Analytics] Report Builder (Microsoft® Excel-extensie)

Workspace is een fantastisch hulpmiddel, maar soms moet u uw gegevens in een aangepaste spreadsheet krijgen, misschien zodat u meerdere gegevensbronnen kunt samenvoegen. Hier speelt Report Builder een rol.

Report Builder is een insteekmodule voor Microsoft® Excel waarmee u verbindingen kunt maken met uw [!DNL Adobe Analytics] -gegevens om tabelgegevens te verkrijgen die u in Excel kunt manipuleren. Over het algemeen om dit efficiënt te gebruiken zou u de gegevens in sommige ruwe gegevenslusjes trekken, dan gebruiks excel celverwijzingen om gegevens van deze lusjes in één enkel geconsolideerd rapport te trekken, dan grafieken en visualisaties tot stand te brengen.

>[!NOTE]
>
>Report Builder heeft een speciale machtiging die op uw gebruikers moet worden toegepast om toegang te krijgen tot deze plug-in. Dit moet worden toegestaan aan gebruikers die hebben geleerd hoe u het gereedschap op de juiste manier kunt gebruiken.

#### 2.2.2. [!DNL Adobe Analytics] API-verbinding

Als u [!DNL Adobe Analytics] -gegevens wilt laten samenvoegen door iets anders dan Excel en u wilt dat de verwerkte gegevens inclusief de beide regeluitsluitingen, gebruikt u de API van [!DNL Adobe] om de gegevens rechtstreeks aan te trekken. Verwerk de gegevens vervolgens met een script of voeg deze toe aan een database voor gebruik met een ander systeem.

Opgemerkt moet worden dat de API nog steeds correlatiegegevens ophaalt die de uitsplitsingen en segmenten toepassen zoals die in de pull-aanvraag zijn gespecificeerd.

De Workspace van [!DNL Adobe] (Section 2.1.2.1) gebruikt de API om de rapporten samen te stellen. Als u de foutopsporingsmodus inschakelt in Workspace, worden de exacte gebruikte API-aanroepen weergegeven. Dit is een snelle manier om uw API vraag uit te bouwen. Door Workspace te gebruiken om de gegevens te bouwen en te bevestigen u wilt trekken, dan gebruikt u die API vraag om de gegevens uit te krijgen aan uw eigen verwerking.


#### 2.2.3. Google [!DNL Analytics] Data Studio

Als je al verder hebt gelezen, weet je al van bovenaf dat ik Data Studio noemde als een equivalent van de Workspace van [!DNL Adobe] . Met Data Studio kunt u gegevens uit Google [!DNL Analytics] , maar ook gegevens uit andere bronnen, ophalen. Dit is handig als u de analysegegevens wilt consolideren met andere verzamelde gegevens. Bij Google [!DNL Analytics] zijn echter dezelfde visualisatiebeperkingen van toepassing. De manier waarop de rijen en kolommen worden gevormd is nog steeds beperkt.

Het is nog steeds een krachtig instrument, en ik zou mensen er op geen enkele manier van weerhouden het te gebruiken. Mijn persoonlijke ervaring is dat ik het rigide gedrag vrij beperkend vind.


#### 2.2.4. Google-uitbreiding voor werkbladen

Als ik voor mijn eigen gebruik gegevens uitgebreid van Google [!DNL Analytics] moet ophalen, is mijn persoonlijke keuze de Google Spreadsheet Extension. Hoewel ik veelvoudige verbindingen aan mijn lijsten GA moet maken, kan ik de cellen van de ruwe gegevens van verwijzingen voorzien en de rapporten uitbouwen ik nodig. Vervolgens visualiseer ik ze met behulp van de grafische mogelijkheden van Google Spreadsheet.


## 3. Uitvoer van onbewerkte gegevens

Wanneer u echt onbewerkte gegevens nodig hebt, bieden zowel [!DNL Adobe] als Google de mogelijkheid om informatie op deze manier op te halen.

### 3.1. [!DNL Adobe] Gegevensfeed

In paragraaf 2.2.2 merkte ik op dat de [!DNL Adobe Analytics] API uit &quot;verwerkte gegevens&quot; werd gehaald. De feed Raw-gegevens bevat gegevens die worden verwerkt door de verwerkingsregels die zijn ingesteld in het deelvenster Beheer, maar deze onbewerkte gegevens bevatten alle gegevens die overal anders zijn uitgesloten.

Dit betekent dat al uw Boot-uitsluitingen, interne IP-gefilterde gegevens en andere uitgesloten gegevens zich in de onbewerkte gegevensfeeds bevinden. Er zijn vlaggen om deze gegevens te identificeren, zodat als u een gegevensmeer bouwt, kan het technische team logica tot stand brengen om deze gegevens dienovereenkomstig te verwerken.

De onbewerkte gegevensfeeds kunnen worden aangepast om alle kolommen met gegevens te verzenden, of alleen specifieke kolommen als u een meer gerichte feed nodig hebt.

De feeds kunnen rechtstreeks naar FTP, SFTP of S3 worden verzonden.


### 3.2. Google Big Query

Helaas heb ik geen ervaring met dit Google-instrument. In theorie zou de gegevensfeed vergelijkbaar moeten zijn met de gegevensfeed van [!DNL Adobe] , zodat uw engineeringteam toegang heeft tot onbewerkte gegevens van uw Google [!DNL Analytics] -account.

Nochtans, eerder dan het verstrekken van een volledige stortplaats van ruwe gegevens, staat het uw ingenieurs toe om tot de gegevens via SQL vragen toegang te hebben om gerichte ruwe gegevens of alle kolommen van ruwe gegevens te trekken.

## 4. Conclusie

Zoals elk systeem, is de praktijk nodig om met het hulpmiddel comfortabel te worden. Hopelijk helpt deze handleiding u om aan de slag te gaan of biedt u tips om uw gebruik van [!DNL Adobe Analytics] te verbeteren.

Ik wil echter benadrukken dat ik het gebruik van zowel [!DNL Adobe Analytics] als Google [!DNL Analytics] in uw implementatiestrategie zou aanbevelen (zelfs als de Google [!DNL Analytics] alleen de gratis versie is). Hierdoor hebt u een back-upsysteem om ervoor te zorgen dat u over gegevens beschikt, aangezien geen enkel systeem onfeilbaar is.

Naast deze handleiding beschikt u over veel bronnen die u kunnen helpen uw strategie te verbeteren:

* [[!DNL Adobe]  Experience League &#x200B;](https://experienceleague.adobe.com/nl#home) - bevat leerprogramma&#39;s, video&#39;s, documentatie, en communautaire forums
* [[!DNL Adobe]  Groepen van de Gebruiker &#x200B;](https://analytics-augs.adobe.com/) - een hub van gemeenschap-in werking gestelde gebeurtenissen om gebruikers te helpen met elkaar verbinden en hun implementaties verbeteren.
* [[!DNL Adobe Analytics]  Kanaal van de Groepen van de Gebruiker YouTube &#x200B;](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) - kon geen [!DNL Adobe Analytics] zitting van de gebruikersgroep maken? Bekijk vorige gebruikersgroepssessies over de hele wereld opnieuw voor meer informatie over hoe uw collega&#39;s het gereedschap gebruiken.
* [&#x200B; het kanaal van de Slack van het Praatje van de Meting &#x200B;](https://www.measure.chat/) - verbind met [!DNL Adobe Analytics] gebruikers over de wereld en deel industrieleerlingen, stel vragen van uw edelen, en sluit zich bij meting geconcentreerde belangengroepen aan.
* en meer!

## Auteur

Dit document is geschreven door:

![&#x200B; Jennifer Dungan &#x200B;](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan, Optimization Manager [!DNL Analytics] bij Torstar

[!DNL Adobe Analytics] Champion
