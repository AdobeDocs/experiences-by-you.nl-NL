---
title: Breng uw gegevensanalyse naar het volgende niveau met Berekende Metriek
description: Leer hoe een peer deskundige Berekende Metriek gebruikt om nieuwe metriek tot stand te brengen zonder hun implementatie te veranderen en de gegevens te gebruiken die reeds worden verzameld om complexe bedrijfsvragen te helpen beantwoorden.
feature-set: Analytics
feature: Calculated Metrics
role: User
level: Beginner
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00Z
jira: KT-13266
thumbnail: KT-13266.jpeg
exl-id: 301ee179-b154-4cf2-b27e-77f38a8945a0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1566'
ht-degree: 0%

---

# Breng uw gegevensanalyse naar het volgende niveau met Berekende Metriek

De meeste nieuwe gebruikers van [!DNL Adobe Analytics] zijn vertrouwd met Segmenten als manier om hun gegevens te segmenteren en te dempen. Vandaag, wil ik u aan berekende metriek introduceren, het volgende beste hulpmiddel in uw analist toolbox.

Met berekende metriek als een geavanceerde functie van [!DNL Adobe Analytics] kunt u nieuwe metriek maken zonder dat u de implementatie wijzigt met behulp van de gegevens die u al hebt verzameld. De Berekende Bouwer van Metriek kan veel verschillende wiskundige en statistische functies gebruiken, zodat kunt u metriek tot stand brengen die zelfs de meest complexe bedrijfsvragen beantwoordt.

## Aan de slag met berekende cijfers

Om met berekende metriek te beginnen, kijken een eenvoudig voorbeeld. Stel dat u wilt begrijpen of gebruikers die zichzelf online bedienen, een hogere gemiddelde orderwaarde (AOV) hebben dan gebruikers die hulp bieden. Ga als volgt te werk om een berekende metrische waarde op te bouwen om deze vraag te beantwoorden:

Om de Berekende Bouwer van Metriek te openen, gebruik de hoogste navigatie om → **Componenten** → **Berekende Metriek** → **+ te klikken toevoegt.** Of, kunt u **+ teken** hierboven **Metriek** in het paneel van Componenten klikken.


![ Calc 01 ](assets/calc01.png) ![ Calc 02 ](assets/calc03.png) ![ Calc 03 ](assets/calc02.png)

![ Calc 04 ](assets/calc04.png)

*Beschrijvingen hieronder voor punten UI*

Zodra de Berekende Bouwer van Metriek opent, voeg en/of doe het volgende toe:

**A.** een naam voor uw berekende metrisch. Deze naam wordt getoond in de lijst van metrieke componenten, zo maak het iets dat aan uzelf en anderen, zoals *AOV van het Centrum van de Vraag* duidelijk zal zijn.

**B.** een beschrijving van berekende metrisch. Deze beschrijving verschijnt wanneer de gebruikers &quot;**i**&quot;naast metrisch in de componentenlijst klikken, zodat zeker is het informatief is. Bijvoorbeeld, voor het Centrum AOV van Vraag, zouden wij kunnen toevoegen *AOV voor het Centrum van de Vraag Begeleide Orden* berekent.

**C.** het metrische formaat: De kiezen decimaal, de tijd, het percentage of de munt, en voegen decimalen en polariteit toe. Hier, zullen wij *Valuta voor het Formaat, 0 voor aantal decimalen, en* ⬆ *Goed (Groen) voor polariteit kiezen.*

**D**. Als u tags gebruikt, waarmee u onderwerpen kunt toepassen en snel berekende metriek kunt zoeken, voegt u de tags toe die hier van toepassing zijn. Wij hebben *AOV* toegevoegd en *het Centrum van de Vraag* markeringen.

**E.** Deze sectie is voor vertoning - aangezien u berekende metrisch in sectie F bouwt, zal de formule hier tonen.

**F.** hier, zult u dimensies (H), metriek (I) of segmenten (J) slepen en laten vallen om uw berekende metrisch evenals de exploitanten voor de formule tot stand te brengen. Als u voor elke meting op het cogumwiel klikt, kunt u de opties Metrisch type (standaard/totaal) en Kenmerk wijzigen. *wij zullen de Opbrengst van het Centrum van de Vraag slepen en laten vallen, dan onder dat, zullen wij* ￼.*. We accepteren het standaard metrische type en attributiemodel.*

**G**. Gebruik deze optie **+Add** om extra voorwaarden of statische aantallen toe te voegen, die wij hier niet nodig hebben.

**K.** en tenslotte, aangezien u uw berekening bouwt, kunt u voorproef de afgelopen 90 dagen&#39; gegevens hier.

Nu wij AOV van het Centrum van de Vraag hebben gebouwd, hebben wij ook berekende metrisch voor Online AOV nodig. We zouden dit doen volgens dezelfde stappen die hierboven zijn beschreven.

Daarna, kunnen wij derde berekende metrisch bouwen, of gebruikend de Berekende Bouwer van Metriek of op de vlucht van binnen de vrije vormlijst, om het Centrum van de Vraag en Online AOV te vergelijken zodat komen wij omhoog met iets als dit:

![ Calc 05 ](assets/calc05.png)

In ons voorbeeld zien we een aanzienlijke lift wanneer kopers het callcenter gebruiken om hen te helpen een aankoop te doen. Deze gegevens kunnen dan onze beslissingen over hoe te om klanten te helpen bij hun aankopen door, bijvoorbeeld, popup aanbiedingen of andere geleide ervaringen te krijgen.

## Segmenten gebruiken in berekende cijfers

Nu, kijken hoe wij segmenten in berekende metriek kunnen gebruiken om meer inzicht in klantengedrag, voorkeur, en motivaties te krijgen. Met segmenten en berekende metriek, kunnen wij genoeg over klanten leren om hun ervaring te verbeteren, opbrengst te verhogen, en klantentevredenheid en loyaliteit te verbeteren.

Uit de bovenstaande AOV-voorbeelden weten we al dat de aankoop van gesubsidieerde producten door callcenter doorgaans een hoger AOV heeft. Nochtans, vertellen andere metriek ons dat de meeste gebruikers niet het vraagcentrum voor aankopen gebruiken.

Welke winkelcategorieën - en gebruikerspaden door deze categorieën - resulteren dus in het hoogste AOV?  We kunnen dit ontdekken door segmenten te combineren met berekende meetwaarden.

Om dit te doen, moeten wij eerst bezoek-niveau *tot stand brengen omvatten* en **&#x200B; segmenten voor elke productcategorie uitsluiten. Omvat of sluit wordt bepaald door het &#x200B;** vistuig van Opties** in de juiste hoek van de container te klikken uit. Standaard is Inclusief.

![ Calc 06 ](assets/calc06.png) ![ Calc 07 ](assets/calc07.png)

Zodra wij deze segmenten hebben gecreeerd, kunnen wij berekende metrisch tot stand brengen om u het antwoord op uw vraag te geven. Wij openen de Berekende Bouwer van Metriek en doen het volgende:

1. Onderzoek naar de pas gecreëerde segmenten en sleep en laat vallen degenen die wij in het grijze gebied bij de bovenkant van de **doos van de Definitie** willen gebruiken. Bijvoorbeeld, als wij een AOV voor gebruikers willen creëren die zowel de categorieën van Vrouwen als van Mannen, maar niet Kid&#39;s bezochten, kunnen wij deze drie segmenten aan dat gebied slepen en laten vallen: *omvat Vrouwen*, *omvat Mannen*, en *sluit Kid&#39;s* uit. Wij roepen dit *stapelend segmenten*.

   ![ Calc 09 ](assets/calc09.png) ![ Calc 08 ](assets/calc08.png)

1. Dan, slepen wij en laten vallen de **Online Inkomsten** metrisch in de zelfde container, toen **Online Orden**. Aangezien de containers als wiskundige uitdrukkingen werken om orde van verrichtingen te bepalen, worden de punten in containers verwerkt vóór verdere processen, hoewel wij geen veelvoudige containers of processen in deze berekening hebben.
1. Wij veranderen de exploitant tussen de twee metriek in verdeling (.).
1. Wij selecteren **Valuta** als formaat, **0** decimalen, en **OMHOOG** voor polariteit.
1. Geef de berekende metrisch naam en geef een beschrijving op.
1. Opslaan.

Als we klaar zijn, ziet onze berekende metrische vormgeving er als volgt uit:

![ Calc 10 ](assets/calc10.png)

Nadat wij berekende metriek gebruikend gestapelde segmenten voor elke combinatie van bezoekerscategoriereis creëren en een blik nemen bij de gegevens, kijk wat wij leren! Gebruikers die tijdens hun bezoek zowel de categorie Vrouwen als de categorie Mannen bezoeken, hebben het hoogste AOV en in vergelijking met bezoekers van één categorie is de lift significant:

![ Calc 11 ](assets/calc11.png) ![ Calc 12 ](assets/calc12.png)

Als we dit weten, kunnen we de paginalay-out, de productplaatsing en het promotiemateriaal optimaliseren om meer mensen in deze categorieën te krijgen voordat we uitchecken.

## Waardevol, maar niet overal beschikbaar

**Zo - berekende metriek, zowel eenvoudig als complex, zijn super waardevol voor analisten!**

Deze cijfers zijn echter niet in alle gebieden van [!DNL Adobe Analytics] beschikbaar. U kunt berekende metriek niet gebruiken in:

- Uitval in Analysis Workspace
- Cohortanalyse in Analysis Workspace
- Data Warehouse
- Real Time-rapporten
- Huidige gegevensrapporten
- [!DNL Analytics] voor doel
- Report Builder

## Aanbevolen werkwijzen voor berekende metriek

Nu u weet hoe waardevol berekende metriek kan zijn, nemen een blik bij sommige beste praktijken in het bouwen van hen.

1. **controleer uw formulesyntaxis.** Zorg ervoor dat de syntaxis van de formule zowel correct is als de syntaxis van [!DNL Adobe Analytics] volgt om ervoor te zorgen dat u betekenisvolle informatie krijgt.
1. **verifieer de orde van verrichtingen.** Zorg ervoor dat u containers zorgvuldig gebruikt en plaats de items in de juiste wiskundige volgorde van bewerkingen.
1. **niet dubbel-tellingsgegevens**. U kunt dubbel-tellende gegevens vermijden door ervoor te zorgen dat de formule die in berekende metrisch wordt gebruikt niet de zelfde gegevens veelvoudige tijden telt. Dit wordt vaak bereikt door *te combineren omvat* en *sluit* voorwaarden in berekende metrisch of door het gebruik van segmenten uit.
1. **granulariteit van de tijdcontrole.** Zorg ervoor dat de berekende metrische waarde dezelfde tijdgranulariteit heeft als de bronmetriek die in de formule wordt gebruikt.
1. **Gebruik nauwkeurige gegevens:** u zult slechts waardevolle resultaten krijgen als u nauwkeurige en betrouwbare gegevens in de berekening gebruikt.

## Aangepaste beste praktijken voor segmenten

Houd bij het maken van segmenten in [!DNL Adobe Analytics] rekening met de volgende aanbevolen procedures:

1. **houd het eenvoudig.** Vermijd overcomplicaties van het segment. Houd het zo eenvoudig mogelijk en gebruik alleen de voorwaarden die nodig zijn om de nauwkeurigheid te waarborgen.
1. **Gebruik de correcte containertypes**. Gebruik het juiste containertype (bezoeker, bezoek of hit) in de segmentdefinitie om onjuiste resultaten te voorkomen.
1. **niet dubbel-tellingsgegevens**. Zoals met berekende metriek, zorg ervoor het segment niet de zelfde gegevens veelvoudige tijden telt. U kunt containers opnemen en uitsluiten.
   1. Wanneer omvat container wordt gebruikt, omvat het ** *alle inhoud van het bezoek* als om het even welke slag de voorwaarde binnen het bezoek aanpast.
   1. Wanneer een exclusief container wordt gebruikt, sluit het *alle inhoud van het bezoek* uit als om het even welke slag de voorwaarde binnen het bezoek aanpast.
1. **Nest containers behoorlijk**. Bepaal welke gegevens worden opgenomen met behulp van de buitenste container en pas vervolgens geneste regels toe op de resterende gegevens. Aangezien de genestelde regels worden toegepast, doet de segmentstroom dienst als trechter, en de verdere regels zijn niet op om het even welke klappen van toepassing die de eerste regel uitsloot.
1. **zorg ervoor uw gegevens bijgewerkt zijn.** Zorg ervoor dat u nauwkeurige en actuele gegevens in de segmentdefinitie gebruikt voor nauwkeurige resultaten.
1. **Test het segment.** Test het segment altijd om te controleren of het naar behoren werkt voordat u het naar anderen loslaat.
1. **overweeg prestaties.** Segmenten vertragen mogelijk de verwerking van rapporten, dus houd er rekening mee dat dit van invloed is wanneer u ze maakt.

## Key Takeaways

Het combineren van segmenten en berekende metriek in [!DNL Adobe Analytics] kan absoluut tot robuustere en effectievere gegevensanalyse leiden. Door uw gegevens te segmenteren en te dicteren en berekeningen te maken voor vergelijking, kunt u meer inzicht krijgen in het gedrag van klanten dat u kunt gebruiken om uw marketingcampagnes te optimaliseren en op maat gemaakte dashboards en rapporten te maken. Houd er echter rekening mee dat berekende metriek niet op alle gebieden van [!DNL Adobe Analytics] beschikbaar zijn en zorg ervoor dat u de beste werkwijzen volgt om ervoor te zorgen dat u nauwkeurige en nuttige gegevens krijgt.


## Auteur

Dit document is geschreven door:

![ Debbie Kern ](assets/calc13.jpeg)

**Debbie Kern**, Hogere [!DNL Adobe Analytics] Manager bij Adswerve

![ Adswerve ](assets/calc14.png)
