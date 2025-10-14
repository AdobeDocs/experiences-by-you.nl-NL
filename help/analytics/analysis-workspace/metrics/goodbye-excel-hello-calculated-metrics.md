---
title: Afscheid Excel, hello berekende metriek
description: Leer de voordelen om berekende metriek in  [!DNL Adobe Analytics]  te gebruiken en hoe zij u van een ononderbroken, dynamische mening van uw gegevens in dit artikel kunnen voorzien.
feature-set: Analytics
feature: Calculated Metrics
role: User
level: Experienced
doc-type: Article
last-substantial-update: 2023-05-02T00:00:00Z
jira: KT-13178
thumbnail: KT-13178.jpeg
exl-id: b233d6d0-2e89-473e-b700-9977b402af39
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1274'
ht-degree: 0%

---

# Afscheid Excel, hello berekende metriek

Leer de voordelen van het gebruik van berekende metriek in [!DNL Adobe Analytics] en hoe zij u van een ononderbroken, dynamische mening van uw gegevens in dit artikel kunnen voorzien.

Hé! Waarom ben je nu in Excel? Ik bedoel, ik weet waarom. Je moet rapporteren om de juiste mensen te bereiken. U bent bezig gegevens in te voeren van [!DNL Adobe Analytics] en omzettingspercentages te berekenen, ze in kaart te brengen en ze allemaal voor te bereiden op een PowerPoint dat naar besluitvormers gaat. Ik hoop echt dat je tenminste Report Builder gebruikt om het te doen, maar ik weet dat sommigen van jullie gegevens handmatig kopiëren en plakken van een Workspace naar Excel.

Waarom?

Waarom elke maand een handmatig proces doorlopen? Waarom een statische mening eens per maand in plaats van een ononderbroken, dynamische mening presenteren? Waarom kopieert u dat naar PowerPoint? Waarom niet direct rekeneenheden maken in [!DNL Adobe Analytics] ?

## Berekende metriek zijn krachtig

Berekende metriek zijn krachtig, maar zelfs de basiswiskundige functies zijn echt nuttig en ernstig verbeterend in vergelijking met het uitvoeren van wiskunde in Excel. Laten we eens kijken naar enkele voordelen en enkele gebruiksgevallen:

1. **Berekende Metriek zijn Huidige en Dynamische**

   Wanneer u getallen exporteert uit [!DNL Adobe Analytics] , worden ze op een bepaald moment vergrendeld. U moet absoluut weten hoe uw site of app de maand daarvoor heeft gepresteerd, maar hoe houden besluitvormers bij hoe de zaken medio maand verlopen? Als uw conversiekoers één dag plunst en dan tegen het einde van de maand weer in het gemiddelde terugkeert, weet u dat dan? Die plunge zou waardevolle gegevens kunnen zijn die een belangrijk telemetrieprobleem, of nog belangrijker, een verandering in bezoekersgedrag onthullen. Met berekende metrisch, kunt u dit in kaart brengen en het zien de dag het gebeurt, verlatend u klaar om te antwoorden.

1. **Berekende Metriek sparen u Tijd**

   Ik ben er geweest. Kopiëren/plakken. Voer de formule in of sleep de cel erboven. Klik op het diagram en wijzig het bereik zodat je de laatste twaalf of dertien maanden hebt. Kopieer nu het diagram. Doe het opnieuw. En opnieuw. En opnieuw. Verzend het PowerPoint. Het is vervelend en tijdrovend en het voelt alsof je het elke maand altijd moet doen.

   In plaats daarvan kunt u een Workspace maken die uw berekende metrische waarde gebruikt, de laatste twaalf of dertien volledige maanden als datumbereik hebt, en de gegevens en diagramupdate automatisch laten uitvoeren op de streep van middernacht op de eerste dag van elke maand. De ontvangers kunnen rechtstreeks toegang hebben tot de Workspace. Ze kunnen een PDF-kopie automatisch per e-mail ontvangen op de eerste dag van de maand of nadat u Text Visualizations hebt gebruikt om uw commentaar op de gegevens toe te voegen (u weet wel, het leuke deel van de rapportage).

1. **Berekende Metriek kan op Grote Reeksen gegevens worden toegepast**

   U zou alle productnamen in Excel kunnen uitvoeren en beginnen omzettingspercentages en opbrengst per bezoeker te berekenen, maar dit wordt een gedoe wanneer u 100.000 hebt of zo. Geen kwestie met Berekende Metriek. Zet uw dimensie zoals gebruikelijk in een lijst en gebruik dan uw Berekende Metriek als metriek. Nu hebt u een dynamische sorteerbare tabel die automatisch wordt bijgewerkt wanneer producten of een andere dimensie die u gebruikt, aan uw catalogus worden toegevoegd.

1. **Berekende metriek verhinderen fouten**

   Er treden Excel-fouten op. We zijn er allemaal geweest. Heck, de gehele economie van Griekenland en de reputatie van twee gerespecteerde academici werden verwoest door een fout in de Excel-formule. Je hebt waarschijnlijk geen Europese economie die op je Excel-vaardigheden rijdt, maar er is zeker een beslissing over budgetten die op basis van je cijfers zal verschuiven. Het gebruiken van Berekende Metriek betekent u metrisch kunt bouwen, het QA&#39;d hebben, en dan niet opnieuw ongerust maken over het.

### Nu we de voordelen van het gebruik van berekende metriek hebben bekeken, laten we eens kijken hoe we ze in de praktijk kunnen brengen

**Geval 1 van het Gebruik: De Tarieven van de Omzetting**

De meeste conversiekoersen zijn gewoon een eenvoudige verdeling. Verdeel het aantal omzettingen door het aantal bezoekers of bezoeken. Verdeel het aantal paginaweergaven voor de laatste pagina van een trechter door het aantal pagina&#39;s dat wordt weergegeven voor de eerste pagina van een trechter. Verdeel het aantal interne campagneklikcontroles door het aantal beelden. Al deze gegevens kunnen eenvoudig als berekende metriek worden gedaan en in een dashboard worden geplaatst met lage gegevenslatentie, het bijwerken van visualisaties, en grotere aandeelbaarheid.

**Geval 2 van het Gebruik: Intern Onderzoek**

Intern zoeken is een van de belangrijkste hulpmiddelen om uw site te begrijpen. In de zoekresultaten van de site kunt u zien waar uw bezoekers geïnteresseerd in zijn en of ze deze gemakkelijk kunnen vinden met navigatie of niet. U moet kunnen bepalen of uw plaatsonderzoek goed werkt en het gebruiken van een beetje basistoevoeging en een afdeling kan u dat antwoord geven.

Laten we beginnen met zoekresultaten. U wilt weten of een zoekterm resultaten oplevert of niets oplevert. Dat zijn meestal aparte gebeurtenissen. Wilt u de moeite nemen om een derde gebeurtenis voor alle interne zoekopdrachten op de site te krijgen? Geef uw modellen in plaats daarvan een onderbreking en gebruik Berekende metriek om Intern Onderzoek toe te voegen: Resultaten en Intern Onderzoek: Geen resultaten samen om Totaal Interne Zoekopdrachten te krijgen.

Welk percentage van onderzoeken keert geen resultaten terug? Splitsen op interne zoekopdracht: geen resultaten met die nieuwe Totaal aantal interne zoekopdrachten berekend met metrisch. Nu weet u of het dringend is om nieuwe inhoud te maken die aansluit bij die zoektermen, of dat uw inhoudsteam hogere prioriteiten kan aanpakken.

We willen weten hoeveel van die zoekopdrachten met resultaten klikdoorzoekingen krijgen en meestal ook daar een aparte maatstaf voor hebben. Gebruik Berekende Metriek om het aantal klikthrough door het aantal tijden te verdelen dat de termijn onderzoeksresultaten omhoog bracht en het als percentage toont. Nu hebt u het klikthrough tarief voor elke interne onderzoekstermijn op uw plaats. U kunt de zoektermen isoleren die tot ongewenste resultaten leiden. Er zijn alle historische gegevens voor je beschikbaar zodat je ze in kaart kunt brengen. Als je verbeteringen aanbrengt, kun je gemakkelijk zien of ze werken door te kijken hoe die snelheid omhoog of omlaag gaat.

Verdeel het aantal interne zoekopdrachten door het aantal zoekbezoekers. U hebt zoekopdrachten per bezoeker voor elke term. Als dat getal hoog is (hoe dichter het bij 1,0 komt, hoe beter), hebt u een van de twee mogelijke problemen. Of de resultaten die worden geklikt zijn slecht en uw bezoekers doen veelvoudige onderzoeken om de beste resultaten te vinden, of zij kunnen niet de pagina&#39;s vinden die zij door nav zoeken.

Hoe kunt u meten of die zeer belangrijke pagina&#39;s door uw nav kunnen worden gevonden? Maak een berekende metrische waarde voor paginaweergaven die volgde op een paginaweergave met zoekresultaten. Verdeel dat door totale paginameningen voor die pagina. Nu kent u het percentage paginaweergaven dat afkomstig is uit zoekresultaten. Als u een hoog percentage hebt, hebt u waarschijnlijk wat werk aan navigatie te doen.

### Berekende cijfers zijn krachtig

Ik hoop dat dit u enkele mogelijkheden heeft getoond om fundamentele wiskundige functies in Berekende Metriek te gebruiken en dat u zult beginnen wat zelf te bouwen. Dit begint slechts de mogelijkheden van de berekening te beschrijven u in Berekende Metriek kunt doen, zelfs met vier eenvoudige functies. Berekende metriek kan u helpen bezoekersgedrag op een volledig nieuw niveau begrijpen en zodra u het hangende hebt, hebt u de deur geopend om complexere functies te gebruiken die ook voor u beschikbaar zijn.

## Auteur

Dit document is geschreven door:

![&#x200B; Gittai hoofdschot &#x200B;](assets/gittai.png)

**Gitai Ben-Ammi**, Belangrijkste Consultant bij de Katalysator van Concentrix

[!DNL Adobe Analytics] Champion
