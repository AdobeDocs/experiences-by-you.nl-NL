---
title: Download  [!DNL Adobe Analytics]  implementatie playbook
description: Een Business Requirements Doc (doorgaans BRD genoemd) is een zeer belangrijk stuk documentatie waaraan belangrijke belanghebbenden, zakelijke gebruikers en technische gebruikers willen samenwerken. Het is een plaats voor het documenteren van al uw gewenste KPIs, het melden van vereisten, om het even welk gegevenspunt u wenst om te zien wanneer uw implementatie van aa volledig is.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10530.jpg
kt: 10530
exl-id: 42679c86-e08f-4dda-8e47-f9880409bad6
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1779'
ht-degree: 0%

---

# De afspeelboek van de [!DNL Adobe Analytics] implementatie downloaden

Alvorens begonnen te worden, [ download playbook ](assets/aa-implementation-playbook.xlsx).

## Tabblad Zakelijke vereisten

**WAT:** A BedrijfsVereisten Doc (die algemeen als BRD wordt bedoeld) is een zeer belangrijk stuk van documentatie dat de belangrijkste belanghebbenden, bedrijfsgebruikers en technologiegebruikers aan zullen willen samenwerken. Het is een plaats voor het documenteren van al uw gewenste KPIs, rapporteringsvereisten, en om het even welk gegevenspunt u wenst om te zien wanneer uw [!DNL Adobe Analytics] (AA) implementatie volledig is.

**WAAROM:** dit dient als springend van punt voor de documentatie die volgt (SDR, tech spec, enz.) en is een gemeenschappelijke bron van waarheid voor een overeengekomen eindstaat van AA. In dit document worden gedachten over de verschillende teams in de organisatie georganiseerd, zodat u uw implementatie verder kunt ontwikkelen of verbeteren.

**HOW:** het documenteren van de bedrijfsvereisten wordt algemeen gedaan door het eind - bedrijfsgebruikers van aa, maar het is belangrijk om terugkoppelen van technologiegebruikers te krijgen aangezien er technische uitdagingen kunnen zijn om nota te nemen en bepaalde gegevenspunten kunnen meer inspanning vereisen dan anderen, die factoren in prioriteitstelling.

Vraag jezelf af: &quot;Wat zijn de dingen die we op onze site willen volgen&quot;, &quot;welke datapunten zijn belangrijk voor mij bij het melden van het gebruik&quot;, en het allerbelangrijkste: &quot;hoe zullen deze datapunten beslissingen beïnvloeden&quot;. Het is belangrijk om elk van uw bedrijfsvereisten op een gegevenspunt te verzekeren dat kan worden gebruikt om bedrijfsbesluiten te informeren. Het kan bijvoorbeeld verleidelijk zijn om elke klik op uw site bij te houden, maar aan het einde van de dag, welke inzichten leent u uit die rapportage?

Begin met het invullen van kolom C in de onderstaande screenshot (Bedrijfsvereiste). Dit zou moeten zijn als &quot;hoeveel interne onderzoeken op onze plaats&quot;worden voltooid of &quot;welke interne campagnevlek het meest effectief in termen van beelden is&quot;. Nadat u dit detailniveau hebt ingevuld, kunt u kolom B (Categorie) opnieuw invullen en de vereisten groeperen in categorieën zoals &quot;Zoeken&quot; of &quot;Interne promotie&quot;. Deze categorieën moeten exact overeenkomen met de technische specificaties.

U geeft ook aan of u denkt dat het gebruik van een eVar, gebeurtenis, proxy of combinatie zal leiden tot wat u wilt bijhouden.

En tot slot zal de kolom van de Status van de Implementatie als statuscontrole dienen aangezien u begint om dingen aan uw plaats toe te voegen.

![ Document Bedrijfs van Vereisten ](assets/brd-template.png)

## Variabele toewijzen, tabblad (document/SDR coderen)

**WAT:** Een etiketterend doc (die algemeen als SDR wordt bedoeld) is een kritiek stuk van documentatie dat voor zowel technische als zakelijke gebruikers van aa waardevol is. Het maakt een lijst van elke variabele in gebruik door rapportreeksen samen met alle relevante details voor de veranderlijke montages, hoe de variabele wordt uitgevoerd, en wat zijn doel in rapportering is. Net als uw eigenschappendocument moet dit een levend, goed beheerd Excel-document zijn met een puntpersoon die verantwoordelijk is voor het up-to-date houden van dit document, aangezien tagging-verbeteringen of implementatiewijzigingen worden geïntroduceerd.

**WAAROM:** Dit document zal vele doeleinden dienen, maar het belangrijkste is het volgende:

* Voor iedereen die nog niet vertrouwd is met uw implementatie (nieuwe huur, bedrijfseigenaar die de beschikbare rapporten beter wil begrijpen, enz.) In dit document wordt de beste weergave gegeven van alle variabelen die zijn geïmplementeerd en van hun doel, zodat individuen zichzelf kunnen dienen voor het leren van uw AA-instelling.
* Voor de eigenaar/technische gebruiker van het product van AA, zal dit document als herinnering dienen hoe andere variabelen opstelling zijn en welke variabelen voor gebruik wanneer het toevoegen van een nieuwe dimensie beschikbaar zijn.

**HOW:** begin door van alle [!DNL Adobe] uit-van-de-doos variabelen (pagina, product, geo, enz.), evenals eVars, steunen, gebeurtenissen, en lijstvariabelen in een doc van Excel een lijst te maken. Dit zou één lusje per plaats/rapportreeks moeten hebben.
Voor elk van deze afmetingen voeg ik de volgende kolommen toe:
* **Naam:** verstrek een eenvoudige en korte naam die door de meesten kan worden begrepen. Dit moet zo intuïtief zijn dat een nieuwe gebruiker de variabele kan ophalen en begrijpen wat de variabele moet vastleggen.
* **Beschrijving:** Meer detail rond wat de variabele wordt gebruikt voor en welke gegevens het volgt. Ik houd dit kort en eenvoudig en heb het de beschrijving die in de interface wordt gebruikt aanpassen. In het ideale geval wil ik niet dat mijn gebruikers ooit het etiketterende document hoeven te raadplegen. Dus als er een nieuwe dimensie wordt ingesteld op de achterkant van de beheerder, voeg ik daar dezelfde beschrijving aan toe. Op deze manier kan de gebruiker rechtstreeks in Workspace op het informatiepictogram klikken om te begrijpen wat een dimensie is - geen Excel-document meer nodig!

![ Vereenvoudigde Pagina URL ](assets/page-url-simplified.png)

* **Code:** de code van de achterkant die de waarde plaatst. Dit kan het gebied van de gegevenslaag op de pagina zijn, of u kunt roepen dat dit met een regel van de Lancering, een verwerkingsregel, enz. wordt gedaan.
* **de rapporten van de Classificatie:** vraag uit om het even welke classificatierapporten die of met de Indeler van de Indeling of de Bouwer van de Regel van de Indeling worden gedaan
* **Reikwijdte van de Oplossing:** ik vind het nuttig om van alle eigenschappen (minstens degenen die meer dan standaardvariabelen gebruiken) in kleine kolommen een lijst te maken en een controleteken voor elke dimensie toe te voegen die op dat bezit wordt geplaatst. Op deze manier kunt u eenvoudig filteren op een specifieke eigenschap en snel zien waar een bepaalde dimensie wordt ingesteld.
* **Configuratie:** montages Admin UI voor elke variabele (d.w.z. voor eVars - vervalsing, toewijzing, handel, enz.)

Screenshot van voorbeeld SDR:
![ Steekproef SDR.](assets/sample-sdr.png)

Het wordt ook aangeraden dit coderingsdocument te gebruiken om gratis variabelen en eventuele junkvariabelen bij te houden. Wanneer een afmeting niet meer nuttig is, zal dev gewoonlijk enige tijd nodig hebben om het te schrappen. Zelfs daarna kan caching voorkomen, of u kunt zich realiseren dat de dimensie ook elders werd geplaatst. Het opschonen van dimensies is niet eenvoudig en vereist vaak geduld. Hier volgen enkele tips om je junk verborgen te houden onder het bed, zodat je gebruikers niet in verwarring raken terwijl ze het bijhouden.

* Alle afmetingen/gebeurtenissen die niet worden gebruikt, zijn &#39;free&#39; of &#39;being delete&#39;
   * Als de dimensie in de afgelopen 90 dagen junkwaarden heeft, wordt ze &#39;verwijderd&#39;
   * Als de dimensie de afgelopen 90 dagen vrij en duidelijk is, is ze &quot;vrij&quot;
   * Markeer deze als dusdanig onder &#39;Naam&#39; in het gecodeerde document, zodat u er gemakkelijk voor kunt filteren. Ik houd deze ongecontroleerd in het etiketteren document (de gegevensfilter van Excel) zodat de gebruikers hen niet zien
   * Markeer deze als de naam van de eVar in de interface, zodat gebruikers deze niet vinden in een zoekopdracht (dus &#39;(v6)&#39;) en verwijder de beschrijving in de interface
* Op deze manier kunt u, wanneer u een nieuwe dimensie nodig hebt, eenvoudig filteren op &#39;gratis&#39; in de kolom &#39;Naam&#39; om een schone dimensie te zoeken die u kunt gebruiken
* Voor de &#39;verwijderde&#39; afmetingen en gebeurtenissen raadt ik u aan deze bij te houden met Workspace:
   * Maak een project dat alleen zichtbaar is voor beheerders met 3 tabellen: eVars, props en gebeurtenissen. Ik gebruik &#39;instances&#39; voor de specifieke eVars en voor &#39;props&#39; maak ik bijvoorbeeld HIT-segmenten met &#39;prop5 bestaat&#39;.
   * Datum instellen op Laatste 90 dagen
   * Gebruik het bovenstaande als rijen in de 3 tabellen, samen met exemplaren
   * Zodra er iets &#39;0&#39; is, merk ik het als &#39;gratis&#39; in het gelabelde document en verwijder het uit het Workspace-project

Op deze manier zijn je gegevens altijd schoon, en je hebt een duidelijk idee van je rommel.

![ Variabelen en gebeurtenissen overzicht ](assets/variables-and-events-overview.png)

## Tabblad Eigenschappen

**WAT:** de eigenschappen van A zouden een lijst van al uw digitale eigenschappen - websites, mobiele apps, andere hulpmiddelen (praatje, terugkoppelen, enz.) moeten maken, of die eigenschappen met [!DNL Adobe Analytics] of niet worden geëtiketteerd. Dit zou als gecentraliseerd, levend document over zaken en technologiegebruikers moeten dienen.

**WAAROM:** Dit zal u een duidelijke mening van de reis van uw gebruiker over al uw digitale eigenschappen geven, en wat [!DNL Adobe Analytics] doet en niet behandelt zodat kunt u beginnen het etiketteren aan om het even welke eigenschappen voorrang te geven waar het mist. Door uw digitale ecosysteem op deze manier op te zetten, kunt u potentiële mogelijkheden in het etiketteren van strategie identificeren om een volledig overzicht van de reis van uw gebruiker te krijgen. Bijvoorbeeld - hebt u een globale rapportreeks nodig om over veelvoudige domeinen/plaatsen te volgen? Is er een overdracht van bezoekersidentiteitskaart nodig tussen domeinen of app aan hybride ervaring? Moeten interne URL-filters worden bijgewerkt voor interdomeintracering?

**HOW:** identificeer een eigenaar van doc om bestuur en één enkele bron van verantwoordelijkheid voor het beheren van updates te verstrekken.
Hier geeft u het volgende weer op het tabblad Eigenschappen:
* **naam van het Bezit:** dit kan een domein, sub-domein, toepassingsnaam, enz. zijn. Zelfs binnen het zelfde domein, als sommige delen van het afzonderlijk worden beheerd (zoals door een verschillend team, of een verschillende technologie), zouden deze uit moeten worden gescheiden.
* **Verbinding (URL)** aan bezit waar beschikbaar
* **Eigenaar &amp; Contacten:** maak een lijst van de belangrijkste eigenaar of de contacten voor het bezit
* **methode van de Markering:** Velen van ons hebben verschillende codemethodes en implementaties op zijn plaats (Lanceren, JS- dossiers, AEP, enz.). U kunt dit indien nodig verder naar beneden splitsen (zoals door codeversie of het systeem van het markeringsbeheer), maar dit is bedoeld om spoor van al uw verschillende codemethodes en versies te houden, waar de code moet worden bijgewerkt, en hoe het moet worden gehandhaafd. Als u [!DNL Adobe] Starten gebruikt, geeft u de naam van de eigenschap Starten op.

Denk eraan dat u alle digitale eigenschappen opneemt, zelfs als deze niet zijn gecodeerd met [!DNL Adobe Analytics] . Zo krijgt u meer inzicht in uw digitale landschap en in de manier waarop uw gebruikers met al uw eigenschappen omgaan.

Het wordt aanbevolen dit document zo eenvoudig mogelijk te houden en het niet met teveel informatie op te slaan, zodat het gemakkelijk te interpreteren blijft door verschillende delen van de organisatie. [!DNL Analytics] -teams begrijpen het digitale landschap vaak beter dan andere teams. Dit document wordt daarom vaak door andere teams en managers gebruikt om een grondig overzicht te geven.

>[!TIP]
>
>Maak een naam-/eigenschapsdimensie van de site in [!DNL Adobe Analytics] . Als u een speciale dimensie (meestal een eVar) in [!DNL Adobe Analytics] hebt die de naam van de site/app aangeeft, kunt u segmenteren, problemen oplossen, virtuele rapportsuite maken, enz. De voordelen zijn eindeloos, vooral wanneer het combineren van veelvoudige plaatsen in één (globale) rapportreeks. De sleutel zorgt ervoor dat uw ontwikkelingsteams altijd deze waarde in de eigenschappen afmeting plaatsen, met inbegrip van alle paginaladingen (s.t vraag/trackState) en alle douanegebeurtenissen (s.tl vraag/trackAction). Verwerkingsregels kunnen een waardevol hulpmiddel zijn om u te helpen deze waarden behoorlijk en consequent plaatsen.

[ bekijk deze video door Doug Moore ](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/implementation/implementation-basics/creating-a-business-requirements-document.html) {target="_blank"} voor meer informatie bij het invullen van implementatieplaybook.

## Auteurs

Dit document is medegeschreven door:

![ Christel Guidon ](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager bij NortonLifeLock
[!DNL Adobe Analytics] Champion

![ Rachel Fenwick ](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, senior consultant bij [!DNL Adobe]
