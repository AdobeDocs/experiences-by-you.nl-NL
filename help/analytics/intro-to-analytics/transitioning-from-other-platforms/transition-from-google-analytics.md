---
title: Uitgebreide handleiding voor de overgang naar [!DNL Adobe Analytics] uit Google [!DNL Analytics]
description: Leer meer over de locatie van equivalente functionaliteit en hoe u deze efficiënt kunt gebruiken bij het overstappen van Google [!DNL Analytics] tot [!DNL Adobe Analytics]
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
exl-id: b2be6081-a1c0-4435-affb-454ed5a74662
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '3290'
ht-degree: 0%

---

# Uitgebreide handleiding voor de overgang naar [!DNL Adobe Analytics] uit Google [!DNL Analytics]{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. Inleiding

Een van de grootste uitdagingen bij het schakelen tussen alle tools is het leren waar equivalente functionaliteit te vinden is en leren hoe u deze efficiënt kunt gebruiken. Deze discussie maakt deel uit van een grotere gids om gebruikers te helpen bij de overgang naar [!DNL Adobe Analytics] (als een nieuwe gebruiker of een gebruiker uit Google [!DNL Analytics]) gemakkelijker. Een diepgaande vergelijking met GA; als het meest waarschijnlijke vergelijkingsinstrument waarmee de meeste gebruikers vertrouwd zijn; wordt verstrekt om gebruikers te helpen bestaande kennis met de nieuwe toolset correleren. Als deze praktijk niet kan worden vervangen, kunt u op deze manier aan de slag gaan en de frustraties die u tijdens deze periode kunt ondervinden, verminderen.

We moeten een snelle vergelijking van terminologie hebben:

| **Beschrijving** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| Er is een gebeurtenismetrische waarde weergegeven die een pagina (of scherm in een app) vertegenwoordigt | Paginaweergave | Voorvertoning |
| Een metrische waarde die een groep interacties op uw website of app vertegenwoordigt die in hetzelfde tijdkader plaatsvinden | Bezoek | Sessie |
| Een metrische waarde die een geïdentificeerd apparaat definieert (op basis van meerdere criteria, waaronder cookies en andere gedragspatronen) om gebruikersinformatie te koppelen. | Unieke bezoeker | Gebruiker |

## 2. De interfaces

Wanneer mensen vergelijken [!DNL Adobe Analytics] en Google [!DNL Analytics], merkt zij op dat [!DNL Adobe]De interface van de gebruiker is eerst ontmoedigend. Dit is waar, maar het is ook; geloof het of niet; een kracht, geen zwakte. [!DNL Adobe] biedt een breed scala aan hulpmiddelen en flexibiliteit in uw gegevensvisualisatie, waardoor u veel meer vrijheid hebt om te bouwen wat u nodig hebt.

Laten we beginnen met de &#39;in-site&#39; rapportage.

### 2.1. Rapportage ter plaatse

#### 2.1.1. Homescherm

Beide [!DNL Adobe Analytics] en Google [!DNL Analytics] Geef een manier op om de eerste weergave aan te passen die een gebruiker ziet wanneer hij of zij zich aanmeldt.

##### 2.1.1.1. Werkruimte / Startscherm aangepaste set ([!DNL Adobe Analytics])

[!DNL Adobe Analytics] veronderstelt niet om een vooraf gebouwd rapport voor alle gebruikers tot stand te brengen om bij login te zien. De standaardhomepage neemt de gebruiker aan het de landende scherm van de Werkruimte dat elke gebruiker alle werkruimterapporten toont die zij creeerde of met hen werden gedeeld. Ook, kan elke gebruiker om het even welk van deze rapporten als hun homescherm plaatsen als zij zo kiezen.

![werkruimte-create-project](assets/ga-to-aa_1.png)

Hieronder vindt u meer informatie over de werkruimte verderop in deze handleiding. Zie punt 2.1.2.1

>[!TIP]
>
>Creeer/deel sommige standaardrapporten voor uw organisatie zodat zij een uitgangspunt hebben om informatie te zien zonder het moeten in de bouw van hun eigen rapporten meteen duiken.



##### 2.1.1.2. Schermafbeeldingen op het startscherm (Google [!DNL Analytics])

* Google [!DNL Analytics] Het Homescherm beschikt over enkele vooraf gebouwde visualisaties. Deze omvatten zaken als:
* Gebruikers, sessies, Bounce Rate en Session Duration in de laatste zeven dagen
* Gebruikers op tijdstip van de dag in de laatste 30 dagen
* Huidige gebruikers nu en de bovenste actieve pagina&#39;s
* Verkeerkanaal, bron/medium en verwijzingen in de laatste zeven dagen
* Sessies per land in de laatste zeven dagen
* Bovenste pagina&#39;s voor de laatste zeven dagen
* Ontwikkeling van actieve gebruikers in de afgelopen 30 dagen
* en meer

GA4-gebruikers hebben meer mogelijkheden om hun eigen rapporten aan te passen en toe te voegen aan het Homescherm.

![google-analytics-interfaces](assets/ga-to-aa_2.png)

Dit is waarschijnlijk één ding dat je het meest mist [!DNL Adobe Analytics]. Er is geen beginscherm voor u vooraf gebouwd. U kunt echter eenvoudig een aangepaste werkruimte instellen om te repliceren wat u in de bovenstaande lijst nodig hebt en deze in te stellen als het landingsscherm. Er is meer over dit onderwerp later (of zie Sectie 2.1.2.1) [!DNL Adobe] Werkruimte).

#### 2.1.2. Reporten Builder ter plaatse

Naast de Eenvoudige Rapporten die de analysehulpmiddelen bonden, verstrekt elk hulpmiddel ook krachtigere hulpmiddelen waarmee om uw eigen douanerapporten te bouwen.

##### 2.1.2.1 [!DNL Adobe Analytics] Werkruimte

Dit is de motor van [!DNL Adobe Analytics]sinds de invoering ervan in 2017 is het de weg naar [!DNL Analytics] analyse, en de primaire reden waarom de sectie van Rapporten binnenkort zal worden zonsondergang.

Met dit gereedschap kunt u rapporten opbouwen met bijna volledige vrijheid.

Het rapport kan worden opgedeeld in deelvensters en die deelvensters kunnen een willekeurig aantal visualisaties bevatten. Deelvensters kunnen worden ingesteld op algemene informatie, zoals datumbereik en algemene segmentfilters.

U kunt zowel de deelvensters als de visualisaties in de deelvensters groter of kleiner maken en rond de deelvensters slepen om items naast elkaar weer te geven, of u kunt ze stapelen. Dus als u twee verschillende gegevensreeksen naast elkaar wilt vergelijken, zou u panelen kunnen creëren die 50/50 onderaan het midden verdelen die de twee plaatsen naast elkaar tonen voor gemakkelijke vergelijking.

Gebruikers beschikken over een groot aantal visualisaties:

* Vrije-vormentabel
* Cohorttabel
* Uitval
* Stroom
* Grafieken
   * Gebied (gestapeld en niet gestapeld)
   * Lijn
   * Spreiding
   * Staaf (gestapeld en niet gestapeld)
   * Opsommingsteken
   * Cirkeldiagram
   * Histogram
   * Horizontale balk (gestapeld en niet gestapeld)
* Kaart
* Samenvattingsblokken
   * Samenvattingswijziging
   * Samenvattingstekst
   * Tekst (tekstveld zonder invoervak waarin extra informatie moet worden ingevoerd om context te geven)
* Venn

Elk deelvenster en elke visualisatie kunnen een naam krijgen en er kan een beschrijving op worden toegepast om context te geven aan wat de informatie weergeeft.
In [!DNL Adobe]segmenten (in feite filters voor gegevens) met terugwerkende kracht worden toegepast en deze kunnen in kolommen van uw vrije-vormlijsten worden getrokken om gegevens naast elkaar te vergelijken. Bijvoorbeeld, als een gebruiker twee verschillende categorieën op hun plaats voor verkeer wilde vergelijken; zij konden een segment voor &quot;Categorie A&quot;en een verschillend segment voor &quot;Categorie B&quot;tot stand brengen.

![analytics-page-views-report](assets/ga-to-aa_3.png)

In vrije-vormtabellen zijn meerdere kolommen en segmentatie mogelijk, indien nodig, om de gegevens op de gewenste manier te visualiseren.

Als u geen onderbreking door datum wilt zien, eenvoudig sleep en laat vallen een andere afmeting of segment daar om de gegevens op een verschillende manier te zien. Gebruik bijvoorbeeld segmenten voor Apparaattype en voeg vervolgens een uitsplitsing toe naar besturingssysteem voor uw mobiele gebruikers/gebruikers van tablets:

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

Met de werkruimte kan uw creativiteit vliegen, u bent niet beperkt tot standaardstoringen. U kunt de visualisaties opbouwen die u nodig hebt om diepgaand in de vergelijkingen te duiken u moet in werking stellen.

>[!TIP]
>
>Wees niet bang om te spelen en te verkennen. Er zijn zoveel manieren om buiten de doos te denken. Bovendien toont de validatie van wat u hebt gemaakt wat u denkt. Ervaar hulp!

U kunt de berekende metriek of de segmenten tot stand brengen die slechts binnen het rapport leven om overstroming van uw segment en berekeningsbewaarplaats te verhinderen. Dit staat u toe om geconcentreerde punten tot stand te brengen die voor specifieke rapporten nodig zijn zonder uw organisatie met dingen te verwarren die niet in andere contexten bruikbaar zijn.

Deze discussie is slechts een inleiding op dit instrument, er zijn andere uitgebreide gidsen om u op gang te brengen. Nadat u deze handleidingen hebt bekeken, kunt u uitgebreide rapporten zoals deze weergeven:

![werkruimte-dashboard](assets/ga-to-aa_5.png)

De werkruimten niet auto-sparen, zodat is het gemakkelijker om een eenmalig, ad-hoc rapport te doen zonder uw rapportbewaarplaats te registreren.

Een andere krachtige eigenschap van werkruimten is de capaciteit om interactieve bepalingen op uw rapporten in de vorm van drop-down toe te passen. Deze drop-down werken niet aan uitgevoerde CSV of dossiers van PDF van uw rapporten. In het live rapport kunt u echter alle visualisaties in een deelvenster bijwerken, zodat hetzelfde rapport onder verschillende omstandigheden wordt weergegeven. Meerdere vervolgkeuzelijsten kunnen worden gebruikt, en op voorwaarde dat de opties elkaar niet uitsluiten, worden de geselecteerde items gestapeld zodat er op een schone manier informatie kan worden gepresenteerd.

>[!IMPORTANT]
>
>Meer lezen over het gebruiken van drop-down en vrije formuitsplitsingen zie <https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680>

##### 2.1.2.2. Google [!DNL Analytics]: Dashboards, Custom Reports en Saved Reports

Google beschikt over een paar gereedschappen voor het maken van rapporten binnen de interface, maar deze werken nog steeds met dezelfde weergave en beperkingen van de rapportsectie.

Nu, voor degenen die in Google geverfd zijn [!DNL Analytics] als je dit leest, zou je kunnen zeggen: &quot;Wacht even even, wat met Google Data Studio, is niet zo&#39;n beter equivalent aan [!DNL Adobe]&#39;s Workspace? Ja, maar de Studio van Gegevens is technisch geen deel van [!DNL Analytics] en maakt verbindingen met verschillende gegevensbronnen mogelijk. Dit hulpmiddel wordt behandeld later in de &quot;Uitgebreide sectie van de Toegang van het Rapport&quot;, specifiek paragraaf 2.2.3.

Met Google-dashboards en aangepaste rapporten kunt u meerdere visualisaties samenvoegen tot één rapport, maar in tegenstelling tot Workspace bent u nog steeds vergrendeld in eenvoudige correlaties en welke gegevens u in welke kolommen kunt plaatsen.

In de Rapporten van de Douane, één van de grootste uitdagingen is wanneer u een filter creeert, is het op alle lusjes van het rapport van toepassing. Er is geen manier om twee verschillende filters binnen het zelfde rapport te vergelijken.

Voor oppervlakvergelijkingen, doet het het werk. Deze zijn allemaal vergelijkbaar met de [!DNL Adobe] Oudere dheden, aangepaste rapporten en bladwijzers. De belangrijkste hulpmiddelen die worden verstrekt om uw behoeften te steunen, die binnen de rapportreeks verblijven.

#### 2.1.3. Verslagen

Zowel Google als [!DNL Adobe] Sommige navigeerbare rapporten hebben die per-gebouwde lijsten en basischronologiegrafieken zijn die rond een afmeting worden gebaseerd.

##### 2.1.3.1 [!DNL Adobe Analytics] Rapporten

[!DNL Adobe Analytics] Er is ook een onderdeel Rapporten, maar dit wordt geleidelijk afgeschaft ten gunste van Analysis Workspace. In feite is het einde van de levensduur aangekondigd voor deze interface, aangezien Workspace een krachtiger instrument is. De meeste van deze tabellen kunnen eenvoudiger worden gemaakt en gewijzigd. [!DNL Adobe]De secties zijn veel breder en dit kan ontmoedigend zijn:

![analytische-site-metriek](assets/ga-to-aa_6.png)

Omdat het grootste deel van het bovenstaande toegankelijk is via Workspaces, geef ik een kort overzicht van deze secties en hoe ze betrekking hebben op Google [!DNL Analytics], en de nog steeds relevante verslagen in dit verband onder de aandacht brengen.

Sitemetriek is wat u zou verwachten. Deze heeft betrekking op de standaardmetriek (paginaweergaven, unieke bezoekers, bezoeken en aangepaste gebeurtenissen die u hebt ingesteld). Dit is vergelijkbaar met het gedragsrapport GA, maar bevat ook enkele van wat u in Audience zou vinden (omdat [!DNL Adobe] de metrische typen worden niet opgesplitst).

Hier zie je &#39;Bot&#39;-rapporten. Verkeer van bots wordt uitgesloten van al uw standaardrapporten. Er zijn echter twee rapporten die inzicht verschaffen in wat er gebeurt en welke bots naar uw site komen. Dit is vooral handig als u aangepaste Bot-regels instelt om bekende spamerbots die vaak op uw site worden aangetroffen, uit te sluiten. Je kunt enig inzicht krijgen in wat die bots doen zonder dat je hoofdrapporten overstroomd worden, maar dat verkeer. Beide rapporten zijn momenteel niet beschikbaar via Workspace (maar met de nieuwe rapportmogelijkheden die binnenkort beschikbaar zijn, kunnen gebruikers deze gegevens ook daar ophalen).

Site-inhoud bestaat uit een groep [!DNL Adobe] standaardafmetingen: paginanaam, sitesecties, hiërarchieën, servers en meer. Al deze afmetingen zijn beschikbaar in Workspace.

Mobiel is een groep van specifieke gegevens voor mobiele apparaten, zoals apparaten, apparaattypen en meer. Deze zijn beschikbaar in Workspace.

Paden zijn niet beschikbaar in Workspace. De werkruimte heeft een stroomdiagram waarin u de in- en uitstromen voor één pagina/waarde kunt zien. Met Paden daarentegen kunt u zien welke paden het meest worden gebruikt in uw website. Pagina&#39;s zijn standaard het eerste padrapport dat voor u is ingesteld. U kunt dit echter ook inschakelen voor aangepaste props, zoals een waarde voor Paginatype. U zou kunnen kijken naar het plakken binnen paginatypen. Wat ik persoonlijk leuk vind aan Paden is de eenvoudige manier waarop de informatie wordt gepresenteerd... Het stroomdiagram in de werkruimte (afhankelijk van hoeveel u probeert te bekijken) kan overweldigend worden. Ik raad aan beide uit te proberen... ze hebben elk een nut en waarde afhankelijk van wat u probeert te bereiken. Opgemerkt moet worden dat elke dimensie kan worden gebruikt bij Stromen, terwijl Padden moet worden ingesteld op een proxy in het deelvenster Beheer.

verkeersbronnen, [!DNL Campaign]s, en de rapporten van de Kanalen van de Marketing zijn allen gelijkaardig aan het rapport van de Aankoop bij het product van Google. De bronnen van het verkeer richten zich op Werkelijke Referenties; [!DNL Campaign]s Focus op uw [!DNL Campaign] De codes, en de Kanalen van de Marketing richten zich ook op [!DNL Campaign] Codes, maar passen ook extra logica toe zoals die door u wordt bepaald op hoe te om de informatie te verwerken. [!DNL Adobe] biedt meer vrijheid voor het instellen van uw regels. Google doet daarentegen veel voor je, en dit is een verandering in denken. Standaard wordt Google toegewezen aan [!DNL Campaign] De codes zijn zes maanden. [!DNL Adobe]De toewijzing wordt standaard ingesteld op één week. Dit kan worden gewijzigd in uw beheerinstellingen, maar in Workspace kunt u in feite een aangepaste toewijzing boven op elke dimensie toepassen, zodat u veel meer flexibiliteit &#39;ter plekke&#39; hebt.

Bezoeker retentie- en bezoekersprofielrapporten lijken op de Publiek-rapporten in Google [!DNL Analytics]. De aandacht wordt meer gericht op de terugkeerfrequentie, terwijl het Profiel van de Bezoeker meer op de Geografie en de Technologie van de gebruikers wordt gericht.

De rapporten van de Omzetting van de douane en van het Verkeer van de Douane zijn beide rapporten van de douanedimensie. Conversies zijn eVars. U kunt een aangepaste vervaldatum instellen op de waarde hit, visit, month en year. Deze waarde blijft voor een gebruiker in persistentie voor het gevormde tijdkader tenzij beschreven. Verkeersvariabelen zijn profielen. U kunt deze ook instellen voor Pathing Reports of als lijstitems die meerdere waarden splitsen op basis van een scheidingsteken naar keuze.

Media is bedoeld voor video&#39;s of audiobestanden waarin u speciale mediatracering hebt ingesteld.

De Rapporten van de douane is een sectie waar een gebruiker de kolommen en de onderverdelingen kan aanpassen die zij binnen de rapportinterface hebben gecreeerd en het opslaan als douanerapport. Zoals hierboven vermeld, moet er echter alles op maat worden gemaakt, aangezien Workspace zoveel krachtigere breuken en correlaties mogelijk maakt. Dit was een goede oplossing voordat Workspace bestond.

De sectie Bladwijzers is vergelijkbaar met Aangepaste rapporten, waar vaak gebruikte rapporten als bladwijzers kunnen worden gemarkeerd in de interface Rapporten, zodat ze gemakkelijker kunnen worden gevonden.

Dashboard was een oud product dat mensen in staat stelde gegevensrapporten te combineren tot één visualisatie. Nochtans, is de functionaliteit in Werkruimte (Sectie 2.1.2.1) zo gemakkelijker om met te werken, dat dit slechts als toegangspunt aan erfenisrapporten bestaat die zouden moeten worden herbouwd alvorens deze eigenschap zonsondergang is.

Met doelen kunnen mensen binnen een bepaald tijdsbestek een rapport maken op basis van een doel. De teams controleren campagnes om te zien of zijn zij op spoor om hun verkeersdoelstellingen te bereiken.

Alle rapporten hier stonden voor veelvoudige metrische kolommen en afmetingsonderverdelingen toe. De eenvoud van de visualisaties en een aantal logica achter de elementen die gecorreleerd kunnen zijn, kunnen echter soms frustrerend zijn.

##### 2.1.3.2. Google [!DNL Analytics] Rapporten

Google [!DNL Analytics] Deze rapporten worden in de volgende secties gesplitst: Realtime, Audience, Acquisition, Behavior en Conversations (in GA3) en in Levenscyclus (met de subsecties: Acquisitie, Betrokkenheid, Monetisering, Behoud) en Gebruiker (met de subsecties: Demografie en Tech).

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

U kunt kleine aanpassingen maken aan deze visualisaties, een secundaire afbraak toevoegen, de visualisatie wijzigen, een filter voor de gegevens maken en nog veel meer. U kunt uw aanpassingen opslaan als Opgeslagen Rapport.

Deze bieden snel en gemakkelijk inzicht in uw gegevens. Nochtans, kunt u dingen zoals Gebruikers aan paginameningen voor een pagina in de zelfde lijst vergelijken, en u kunt niet meer dan één extra dimensie toevoegen om extra gegevens te zien.

Deze zijn goed voor snelle analytische gegevens, maar als je echt diep moet graven, lijden ze aan de beperkingen.

### 2.2. Uitgebreide toegang tot rapporten

Naast &quot;Rapportering ter plaatse&quot;, bieden de meeste hulpmiddelen uitgebreide functionaliteit aan die u toestaat om uw analyse buiten de hulpmiddelen te nemen en iets te bouwen een beetje meer aangepast.

#### 2.2.1. [!DNL Adobe Analytics] Report Builder (Microsoft® Excel-extensie)

De werkruimte is een geweldig hulpmiddel, maar soms moet u uw gegevens in een aangepaste spreadsheet krijgen, misschien zodat u veelvoudige bronnen van gegevens kunt verenigen. Hier speelt Report Builder een rol.

Report Builder is een insteekmodule voor Microsoft® Excel waarmee u verbindingen met uw [!DNL Adobe Analytics] gegevens die moeten worden opgehaald in tabelgegevens die u kunt manipuleren in Excel. Over het algemeen om dit efficiënt te gebruiken zou u de gegevens in sommige ruwe gegevenslusjes trekken, dan gebruiks excel celverwijzingen om gegevens van deze lusjes in één enkel geconsolideerd rapport te trekken, dan grafieken en visualisaties tot stand te brengen.

>[!NOTE]
>
>Report Builder heeft een speciale machtiging die op uw gebruikers moet worden toegepast om toegang te krijgen tot deze plug-in. Dit moet worden toegestaan aan gebruikers die hebben geleerd hoe u het gereedschap op de juiste manier kunt gebruiken.

#### 2.2.2. [!DNL Adobe Analytics] API-verbinding

Indien nodig [!DNL Adobe Analytics] gegevens die door iets anders dan Excel moeten worden verteerd, en u wilt de verwerkte gegevens met inbegrip van de beide regeluitsluitingen, gebruiken [!DNL Adobe]API om de gegevens rechtstreeks aan te trekken. Verwerk de gegevens vervolgens met een script of voeg deze toe aan een database voor gebruik met een ander systeem.

Opgemerkt moet worden dat de API nog steeds correlatiegegevens ophaalt die de uitsplitsingen en segmenten toepassen zoals die in de pull-aanvraag zijn gespecificeerd.

[!DNL Adobe]De werkruimte van &#39;s (Sectie 2.1.2.1) gebruikt API om de rapporten te bouwen, en als u zuivert wijze in Werkruimte toelaat, toont het u de nauwkeurige gebruikte API vraag. Dit is een snelle manier om uw API vraag uit te bouwen. Door Werkruimte te gebruiken om de gegevens te bouwen en te bevestigen u wilt trekken, dan gebruikt u die API vraag om de gegevens uit te krijgen aan uw eigen verwerking.


#### 2.2.3. Google [!DNL Analytics] Data Studio

Als u langs hebt gelezen, weet u reeds van bovenaf dat ik de Studio van Gegevens als gelijkwaardig aan noemde [!DNL Adobe]s Workspace. Met Data Studio kunt u in Google gaan werken [!DNL Analytics] gegevens, maar ook gegevens uit andere bronnen. Dit is handig als u de analysegegevens wilt consolideren met andere verzamelde gegevens. Met Google [!DNL Analytics]Hetzelfde soort visualisatiebeperkingen zijn er. De manier waarop de rijen en kolommen worden gevormd is nog steeds beperkt.

Het is nog steeds een krachtig instrument, en ik zou mensen er op geen enkele manier van weerhouden het te gebruiken. Mijn persoonlijke ervaring is dat ik het rigide gedrag vrij beperkend vind.


#### 2.2.4. Google-uitbreiding voor werkbladen

Voor mijn eigen gebruik, wanneer ik gegevens uitgebreid uit Google moet halen [!DNL Analytics]Mijn persoonlijke keuze is de Google Spreadsheet Extension. Hoewel ik veelvoudige verbindingen aan mijn lijsten GA moet maken, kan ik de cellen van de ruwe gegevens van verwijzingen voorzien en de rapporten uitbouwen ik nodig. Vervolgens visualiseer ik ze met behulp van de grafische mogelijkheden van Google Spreadsheet.


## 3. Uitvoer van onbewerkte gegevens

Wanneer u echt onbewerkte gegevens nodig hebt, beide [!DNL Adobe] en Google bieden de mogelijkheden om informatie op deze manier te verzamelen.

### 3.1 [!DNL Adobe] Gegevensfeed

In paragraaf 2.2.2 heb ik vermeld dat de [!DNL Adobe Analytics] API van &quot;verwerkte gegevens&quot;. De feed Raw-gegevens bevat gegevens die worden verwerkt door de verwerkingsregels die zijn ingesteld in het deelvenster Beheer, maar deze onbewerkte gegevens bevatten alle gegevens die overal anders zijn uitgesloten.

Dit betekent dat al uw Boot-uitsluitingen, interne IP-gefilterde gegevens en andere uitgesloten gegevens zich in de onbewerkte gegevensfeeds bevinden. Er zijn vlaggen om deze gegevens te identificeren, zodat als u een gegevensmeer bouwt, kan het technische team logica tot stand brengen om deze gegevens dienovereenkomstig te verwerken.

De onbewerkte gegevensfeeds kunnen worden aangepast om alle kolommen met gegevens te verzenden, of alleen specifieke kolommen als u een meer gerichte feed nodig hebt.

De feeds kunnen rechtstreeks naar FTP, SFTP of S3 worden verzonden.


### 3.2. Google Big Query

Helaas heb ik geen ervaring met dit Google-instrument. In theorie zou het vergelijkbaar moeten zijn met [!DNL Adobe]&#39;s Data Feed, waarmee uw engineeringteam toegang heeft tot onbewerkte gegevens van uw Google [!DNL Analytics] account.

Nochtans, eerder dan het verstrekken van een volledige stortplaats van ruwe gegevens, staat het uw ingenieurs toe om tot de gegevens via SQL vragen toegang te hebben om gerichte ruwe gegevens of alle kolommen van ruwe gegevens te trekken.

## 4. Conclusie

Zoals elk systeem, is de praktijk nodig om met het hulpmiddel comfortabel te worden. Hopelijk helpt deze gids u beginnen of verstrekt uiteinden om uw gebruik van te verbeteren [!DNL Adobe Analytics].

Ik wil echter benadrukken dat ik het gebruik van beide wil aanbevelen [!DNL Adobe Analytics] en Google [!DNL Analytics] in uw implementatiestrategie (zelfs als de Google [!DNL Analytics] is alleen de gratis versie). Hierdoor hebt u een back-upsysteem om ervoor te zorgen dat u over gegevens beschikt, aangezien geen enkel systeem onfeilbaar is.

Naast deze handleiding beschikt u over veel bronnen die u kunnen helpen uw strategie te verbeteren:

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/#home) - Bevat zelfstudies, video&#39;s, documentatie en communityforums
* [[!DNL Adobe] Gebruikersgroepen](https://analytics-augs.adobe.com/) - Een hub van op gemeenschap-in werking gestelde gebeurtenissen om gebruikers te helpen met elkaar verbinden en hun implementaties verbeteren.
* [[!DNL Adobe Analytics] YouTube-kanaal gebruikersgroepen](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) - Kan geen [!DNL Adobe Analytics] gebruikersgroepsessie? Bekijk vorige gebruikersgroepssessies over de hele wereld opnieuw voor meer informatie over hoe uw collega&#39;s het gereedschap gebruiken.
* [Chat-Slack meten, kanaal](https://www.measure.chat/) - Verbinding maken met [!DNL Adobe Analytics] gebruikers over de hele wereld en delen branche-lessen, stellen vragen aan uw collega&#39;s en voegen zich bij meetgerichte belangengroepen.
* en meer!

## Auteur

Dit document is geschreven door:

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan, Optimization Manager [!DNL Analytics] bij Torstar

[!DNL Adobe Analytics] Champion

