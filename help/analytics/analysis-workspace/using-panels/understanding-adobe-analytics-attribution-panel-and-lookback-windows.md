---
title: Deelvenster Adobe Analytics-toewijzing en terugzoekvensters
description: Leer hoe u het deelvenster Kenmerken en het terugzoekvenster kunt gebruiken om het gedrag van de klant te begrijpen en aan te passen hoe de dimensie-items krediet krijgen voor succesgebeurtenissen.
feature-set: Analytics
feature: Attribution
role: User
level: Experienced
doc-type: Article
last-substantial-update: 2023-06-20T00:00:00Z
jira: KT-13181
thumbnail: KT-13181.jpeg
exl-id: 2a62e563-bad9-424f-94ca-2af68d4a83b5
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 0%

---

# [!DNL Adobe Analytics] Deelvenster Kenmerken en terugzoekvensters

Toen ik eerst aan het [ attributiepaneel ](https://experienceleague.adobe.com/docs/analytics-platform/using/cja-workspace/panels/attribution.html?lang=en) en **raadplegingsvenster** dacht, werd ik onmiddellijk herinnerd aan het concept &quot;*tijdreis&quot;*; dan, natuurlijk, werd ik ook herinnerd aan onze typische reactie op vele nieuwe hulpmiddelen zoals dit eenvoudig het proberen uit te stellen om het te gebruiken, omdat zij zo gecompliceerd kijken.

Ik bedoel eerlijk gezegd, kijk gewoon naar al die opties, switches, deelvensters, lezingen en knoppen.  En serieus, laten we het hebben over die gecompliceerde knipperende lichten, slangen, kooien... WACHT!  Dit is niet het moment om afleiding te krijgen in het praten over tijdmachines, we hebben gewoon geen tijd... of doen we dat?

Ik zal het **attributiepaneel** toegeven is een vrij complex hulpmiddel; nochtans, onze typische baan als analisten, dag in en dag uit, moet een andere van onze favoriete en hoogst complexe hulpmiddelen gebruiken om ook een blik te nemen op wat in het verleden gebeurde. Dat gereedschap heet ***[!DNL Adobe Analytics]**!  Dus ja, om onze zeer relevante vraag te beantwoorden, denk ik dat deze twee dingen zeggen dat we genoeg tijd hebben.

Daarom waarom zouden wij iets als een beetje angst moeten toestaan om de manier van zulke verbazingwekkende, gesofisticeerde, en krachtige hulpmiddelen als deze te verhinderen die ons letterlijk toestaan om *achteruit* in tijd, elke dag te kijken?

Want dit is TIJDREIS, mensen!  We hebben het allemaal over dat soort dingen.  Juist??!

Dus, wat wachten we op - een glanzende metalen auto, een politiedoos, of een oude telefoontoestel met de bedrading van een oude paraplu als antenne om op onze deur te komen?

Nee!  We hebben nog iets beters, dus laten we er maar aan vasthouden!

Nou... je krijgt het idee.


Nu wij allen over tijdreis enthousiast zijn, nemen een diepe adem, stap terug een beetje, bepaal wat het **werkelijk 2&rbrace; attributiepaneel 0&rbrace; *is, en breken dingen neer een klein beetje:***

![ Attributie ](assets/attribution.png)

*Figuur 1 - Getallen die inline met tekst verder onder* worden getoond

In **attributie**, overweeg eenvoudig hoe de gebeurtenissen/de acties door een individu, verscheidene individuen, of één van om het even welk aantal verschillende gebeurtenissen in tijd zouden kunnen worden veroorzaakt.

Volgens [[!DNL Adobe] ](https://experienceleague.adobe.com/docs/analytics-platform/using/cja-workspace/attribution/overview.html?lang=en), *attributie* geeft analisten de capaciteit aan om aan te passen hoe *Dimension* punten krediet voor *succesgebeurtenissen* ontvangen.


>[!WARNING]
>
>Enkel een snelle nota om uit te roepen dat **attributiemodellen** zo vaak met **marketing kanalen** worden geassocieerd dat ik opzettelijk *doorstreept* ❷ KANAAL in het beeld hierboven om het te illustreren **attributie** analyse tegen meeste andere ***afmeting*** kan uitvoeren.


In feite, is zelden om het even welke bepaalde klantenreis echt lineair en zelfs minder vaak voorspelbaar.  Meer zo, zal elke klant bij hun eigen tempo te werk gaan; vaak, zouden zij terug kunnen verdubbelen, kunnen stagneren, wegvallen, of andere niet-lineair gedrag aangaan. Deze biologische acties maken het moeilijk of praktisch onmogelijk om de impact van marketinginspanningen op de hele reis van de klant te kennen. Het belemmert ook de inspanningen om meerdere gegevenskanalen aan elkaar te koppelen.

Dat klopt.  Laat je &#39;domino&#39;-analogieën bij de deur staan en open voor concepten die meer op de lijn liggen van het vlindereffect en de snaartheorie - maar net als alle andere dingen moeten we beginnen met een aantal basisprincipes.

## **modellen van de Attributie**

Wanneer wij het **attributiepaneel** gebruiken, kunnen wij beginnen verscheidene verschillende dingen waar te nemen.  Bijvoorbeeld, tonen de **attributiemodellen** aan ons hoe onze *omzettingen* (d.w.z., ❶ **succesmetriek**) over *hits* in om het even welke bepaalde groep kunnen worden verdeeld.

Eenvoudig gezet, als **10 mensen** a **BIG RODE KNOP** aan stap door een deur, onze **attributiemodellen** ons zullen vertellen welke van die **10 mensen** wij &quot;krediet&quot;willen toewijzen - of beter gezegd, hoe *veel* &quot;krediet&quot;wij hen willen toewijzen - voor het drukken van genoemde knoop.

![ Knoop ](assets/button.png)

Het houden van dit in mening, zijn hier een paar voorbeelden van hoe de ❸ **attributiemodellen** die **10 mensen** zouden kunnen beïnvloeden:

- **Eerste aanraking**: Dit model werkt precies als het door **100% krediet** aan de *eerste* persoon te geven die door de deur liep.  De verkopers zijn waarschijnlijker deze benadering voor tactieken zoals ***sociale media*** of ***vertoning*** te gebruiken; nochtans, is het ook een grote tactiek om vaak voor de doeltreffendheid van de productaanbeveling ter plaatse te gebruiken.
- **Laatste aanraking**: Deze tactiek werkt ook precies als het klinkt, maar in plaats daarvan geeft **100% krediet** aan de LAATSTE persoon die door de deur liep.  Dit model wordt typisch gebruikt om dingen als ***natuurlijk (biologisch) onderzoek*** en andere *kortetermijn* marketing cycluscampagnes te analyseren.
- **Lineair**: Dit model verdeelt gelijk krediet over ELKE ENKELE PERSOON die door de deur liep.

  >[!CAUTION]
  >
  >Hier wordt echter de nodige voorzichtigheid geboden, omdat u de resultaten zeer snel kunt verspreiden wanneer u deze tactiek toepast, rekening houdend met hoe langer de tactiek loopt en hoe groter het publiek dat deze bereikt.

- **u-Vormd**: Deze benadering wijst **40%** van het krediet aan de *eerste persoon* in de deur toe, spreads **20%** van het krediet over *iedereen binnen tussen*, en geeft dan **40%** aan **laatste** door. Dit model zal het vaakst in situaties worden gebruikt wanneer u a **lange omzetting/verkoopcyclus** die *verscheidene aanraakpunten* langs de weg bevat.  In dit geval, is uw doel ***eerste*** en ***laatste*** marketing tactiek primair te benadrukken die aan de klant het omzetten bijdroeg.
- **J** - **Vormde** en **Omgekeerde J**:
   - Denk over **u-Gegraveerd**, maar in plaats daarvan wijst dit model **60%** krediet aan de *laatste persoon* lopend door de deur, **20%** aan *eerst* toe, en dan *verdeelt* resterende **20%** over {11 4} iedereen anders *in het midden.*  **Omgekeerde J** doet het nauwkeurige tegenovergestelde.

     Het doel is hier het grootste deel van uw nadruk, of bij het *begin* of het *eind* van uw campagne te zetten; nochtans, wilt u nog een bepaalde hoeveelheid krediet aan het bijdragende punt op het tegenovergestelde eind toewijzen terwijl het erkennen van de &quot;kleine jongens&quot;langs de manier.

- **Verval van de Tijd**: Nu, zou ik remiss zijn als ik dit niet deelde. Dit model heeft letterlijk een halfwaardetijd die exponentieel vervalt - in de loop der tijd!  In dit geval, is de *standaard* parameter voor het halfleven van dit model **7 dagen**.  De manier het werkt is *gewicht* op elk **marketing kanaal** dan toe te passen, *gebaseerd op de hoeveelheid tijd* die na *aanvankelijke touchpoint* overgaat en wanneer de klant omzet.

  **Verval van de Tijd** en **U-Gegrafeerde attributiemodellen** zowel worden typisch gebruikt om langer-bedachte campagnes te meten, maar aangezien u kunt zien, hebben zij lichtjes verschillende doelstellingen, die op hoe zij uiteindelijk ** de waarde van het resultaat wegen.

- **Douane**: U kiest en kiest wie krediet gaat krijgen.  Het is jouw campagne!

Voor extra informatie over deze en andere attribuutmodellen, [ klik hier ](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/attribution/models.html?lang=en)

Om dit nog interessanter te maken, praten we over het terugdraaien van de klok!

## **Lookback vensters**

Nu is het tijd om je geest op een hoger niveau te zetten.  Hier voegen we letterlijk het tijdreiselement toe aan onze analyse - en opnieuw beginnen we met de basis.

***[!DNL Adobe]*** bepaalt ❹ **raadplegingsvensters** als &quot;de hoeveelheid tijd een omzetting zou moeten terugkijken om aanraakpunten te omvatten. Attributiemodellen die meer krediet geven aan eerste interacties zien grotere verschillen bij het weergeven van verschillende terugkijkvensters.&quot;


Met andere woorden, **raadplegingsvensters** bepalen de tijdspanne waarin *omzettingen* worden overwogen en *context* aan de attributieanalyse verstrekken. ***[!DNL Adobe Analytics]*** biedt drie soorten **raadplegingsvensters** aan:

- **het raadplegingsvenster van het Bezoek:** kijkt terug naar het begin van a ***bezoek*** wanneer een omzetting gebeurde, die inzichten in de directe interactie verstrekken die tot omzettingen leiden.

  Herinner dit typisch het kortste **raadplegingsvenster** aan gebruik is.
- **het terugkijkvenster van de bezoeker:** bekijkt alle ***bezoeken*** file tot de eerste van de maand binnen de geselecteerde **datumwaaier**, die een veel bredere mening van de interactie van de klant aanbieden en de hulp identificeert patronen in tijd.
- **het raadplegingsvenster van de Douane:** staat u toe om het **attributievenster** voorbij de het melden **datumwaaier** tot a *maximum* van **90 dagen** uit te breiden.  Het verstrekt *flexibiliteit* in het vangen van touchpoints die *buiten* de geselecteerde **datumwaaier** voorkwamen, die een uitvoerige analyse verzekeren.

Door een bepaald **raadplegingsvenster** aan te passen, kunnen de analisten het effect van één of meerdere touchpoints binnen specifieke tijdkaders dan onderzoeken en grotere inzichten in krijgen hoe de verschillende tijdsduur attributieresultaten beïnvloeden.

## **die het allen samen brengen**

Wat betekent dit voor ons als analisten?

Het **attributiepaneel** en **raadplegingsvenster** geven ons de macht om voorbij de alledaagse, oppervlakte-vlakke gegevens te kijken, en dieper in de klantenreis te duiken. Door te begrijpen welke aanraakpunten het grootste effect op *omzettingen* hadden, kunnen wij geïnformeerde besluiten over onze marketing strategieën nemen en middelen effectiever toewijzen.

Herinner me, nadat u uw **attributiemodellen** en **geselecteerde raadplegingsvensters** hebt, kunt u uw gegevens nog verder manipuleren door het met een ❺ **segment te filtreren,** of een andere component te filtreren u op dit punt wenst.  Bovendien beschikt u over alle functies van een traditionele Workspace nadat het paneel is weergegeven.

## **definitief het zetten van het in praktijk**

Nu u de concepten neer hebt, veronderstel u een marketing campagne in werking stelt en probeert om te bepalen welk kanaal *het meest effectief* voor het drijven van omzettingen is. Met hulp van het **attributiepaneel**, niet alleen kunt u het **laatste aanraken** zien, maar ook **eerste aanraking**, **zelfde aanraking**, en een ander **model** u verkiest om te bepalen welke **kanalen** *het meest efficiënte* zijn in het drijven van uw *conversie sions*. Dan, kan deze informatie worden gebruikt om *uw campagnes te optimaliseren en algemene prestaties eenvoudig te verbeteren door de klok met het **raadplegingsvenster**&#x200B;van uw keus terug te draaien!*

Nu je hebt gezien wat het kan doen, mag je niet misleid of geïntimideerd worden door de schijnbaar complexe kenmerken van het attributiepaneel.  **Gezicht het**.  *Embrace* het.  **Begrijp** het.
MAAR DE MEESTE VAN ALLES - *gebruik het aan uw voordeel.* het **attributiepaneel** en **raadplegingsvenster** zijn de sleutels om een diepgaander inzicht in uw klanten en hun reis met uw merk te ontsluiten.

Nu, kunnen wij &quot;[ terug in tijd ](https://youtu.be/gVryJmZNFdU)&quot;met vertrouwen reizen en de macht van onze trusty tijdmachine (a.k.a. *** [!DNL Adobe Analytics]***) gebruiken om gegeven-gedreven besluiten te nemen.

## Auteur

Dit document is geschreven door:

![ Jeff Bloomer ](assets/jeff-headshot.png)

**Jeff Bloomer**, Manager, Digitaal [!DNL Analytics] bij Kroger Persoonlijke Financiën

[!DNL Adobe Analytics] Champion
