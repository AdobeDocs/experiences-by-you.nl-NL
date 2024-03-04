---
title: Problemen oplossen voor marketeers
description: Kennis van de meest voorkomende fouten kan u helpen sneller problemen op te lossen en uw productiviteit te verhogen. Deze het oplossen van problemenuiteinden om u te helpen gelijkaardige fouten effectief oplossen aangezien zij voorkomen.
solution: Campaign Standard
feature-set: Campaign
feature: Workflows
role: User
level: Beginner, Intermediate, Experienced
doc-type: Article
last-substantial-update: 2023-05-18T00:00:00Z
jira: KT-13256
thumbnail: KT-13256.jpeg
source-git-commit: a27a5538a7009d00d01227865ced4c5039147496
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# Oplossen van problemen voor marktspelers: 5 algemene workflowfouten en leveringsfouten

Door: [Suraj Patra](https://www.linkedin.com/in/suraj-p-51612053/){target="_blank"}, senior consultant, Meijer

Als Senior Engineer en klant expert op [!DNL Adobe] Experience Cloud producten de afgelopen vijf jaar, ik laat zakelijke gebruikers toe bij [Meijer](https://www.meijer.com/){target="_blank"}, een in 1934 opgerichte Amerikaanse supercentrum-keten, om complexe marketing- en transactiecampagnes met ACS te voeren. Enkele projecten waaraan ik heb gewerkt, zijn onder andere aangepaste campagnes voor het opslaan van aanbiedingen en het bestellen van gegevens voor personalisatie, geïntegreerd met [!DNL Adobe] Audience Manager, en klanteninzicht voor segmentopname.


In mijn tijd die ACS gebruikt, heb ik fouten ervaren die tijdrovend en frustrerend kunnen zijn om op te lossen. Kennis van de meest voorkomende fouten kan u helpen sneller problemen op te lossen en uw productiviteit te verhogen. Hieronder vindt u de tips voor het oplossen van problemen waarmee u vergelijkbare fouten op effectieve wijze kunt oplossen.

## Fout bij gegevenstype komt niet overeen

**Foutcode:**
`PGS-220000 PostgreSQL error: ERROR: operator does not exist: character varying = bigint`

**Oorzaak:**
Deze fouttypen worden in een workflow weergegeven wanneer u probeert het gebruik van velden met verschillende gegevenstypen te combineren. Wanneer u bijvoorbeeld een bestand uploadt met een bestand dat een tekenreeksveld heeft, en u probeert het tekenreeksveld te koppelen aan een profielveld met een gegevenstype int.

![data-type-mismatch-error](/help/_assets/kt-13256/data-type-mismatch.png)

**Oplossing:**
Wijzig het gegevenstype van het veld bij activiteit Bestand laden in het gegevenstype dat u wilt gebruiken. Open de activiteit Bestand laden. Ga naar het tabblad &#39;COLUMN DEFINITION&#39; en wijzig het gegevenstype van het gewenste veld.


![data-type-mismatch-solution](/help/_assets/kt-13256/data-type-mismatch-solution.png)

## Fout bij aanpassen van levering

**Foutcode:**
`The schema for profiles specified in the transition ('') is not compatible with the schema defined in the delivery template ('nms:recipient'). They should be identical.`

**Oorzaak:**
Deze fout treedt op wanneer u een e-mail naar een adres verzendt, maar de e-mail of een andere id niet in overeenstemming is met een profiel. Als u een e-mailbericht wilt verzenden, moet de e-mail of de id altijd zijn gekoppeld aan een profiel.

![workflow met afstemmingsactiviteit](/help/_assets/kt-13256/del-persn-error-wf.png)

**Oplossing:**
Een gemeenschappelijke identiteitskaart moet bestaan van het geladen dossier met de ontvankelijke lijst. Deze algemene sleutel voegt het ladingsdossier aan de ontvankelijke lijst binnen de verzoeningsactiviteit toe. E-mails worden mogelijk niet verzonden naar records die niet bestaan in de tabel met ontvangers waarvoor deze afstemmingsstap binnen de workflow is vereist. Hierbij stemt u de activiteit van het inkomende laadbestand af met een id zoals een e-mailadres uit het profiel. De `nms:recipient` Het schema verwijst naar de profiellijst en het in overeenstemming brengen van de inkomende verslagen met profiel maakt het tijdens e-mailvoorbereiding beschikbaar.

Raadpleeg de schermafbeelding voor afstemmingsactiviteiten, zoals hieronder wordt weergegeven.

![workflow met reconciliatiedetails](/help/_assets/kt-13256/del-persn-error-wf-solution.png)

Meer informatie over [verzoening](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/data-management-activities/reconciliation.html?lang=en).

## Gegevensfout algemeen veld

**Foutcode:**
`The document types of inbound events (''and'') are incompatible (step 'Exclusion'). Unable to perform the operation. `

**Oorzaak:**
Dit probleem treedt op tijdens het gebruik van het **uitsluitingsactiviteit** in ACS werkschema&#39;s, wanneer het uitvoeren van een uitsluiting die op identiteitskaart wordt gebaseerd, wanneer de Primaire reeks en de uitgesloten reeks niet de zelfde gebiedsnamen hebben.


![Gegevensfout algemeen veld](/help/_assets/kt-13256/dataset-error.png)

**Oplossing:**

Deze fout kan op twee manieren worden opgelost:

1. Dezelfde veldnaam gebruiken in zowel primaire als uitgesloten velden en dat veld als id gebruiken

   OF

2. Gebruik de methode voor JOINS-uitsluiting om het veld te selecteren waarop u de records wilt uitsluiten.

![Gegevenssetfout algemeen veld - Oplossing ](/help/_assets/kt-13256/dataset-error-solution.png)

## Fout veldnaam gedropt

**Foutcode:**
`XTK-170036 Unable to parse expression 'i__name'`

**Oorzaak:**

Mislukkingspunten kunnen optreden in een **verrijkingsactiviteit**. Een van de meest voorkomende wordt hieronder weergegeven.

![Fout veldnaam gedropt](/help/_assets/kt-13256/field-name-dropped-error.png)

Dit gebeurt wanneer u handmatig een expressienaam bewerkt in de activiteit. De afbeelding toont aan dat de expressie is gewijzigd van `name `tot `i__name`.

**Oplossing:**

U kunt deze fout op drie manieren oplossen:

1. Wijzig de naam weer in de oorspronkelijke expressie.

2. Als u een nieuwe naam wilt gebruiken, wijzigt u de waarden in het dialoogvenster **verrijkingsactiviteit**.

3. Als je je niet herinnert wat er veranderd is, zou je best de activiteit opnieuw kunnen creëren.

## Fout bij tijdelijk neerzetten van tabel 

**Foutcode:**
`XTK-170024 The temporary schema "temp:deliveryEmail1" is not defined in the current context.`

**Oorzaak:**
Dit is een algemene fout in gecompliceerde workflows met verrijking of andere activiteiten. Dit betekent waarschijnlijk dat sommige werkstromen voor activiteit niet correct worden opgeslagen tijdens meerdere wijzigingen in de werkstroom.

![Fout bij tijdelijk neerzetten van tabel ](/help/_assets/kt-13256/temp-table-dropped-error.png)

**Oplossing:**
Deze fout kan op vele manieren optreden, dus er is geen eenvoudige oplossing. Als het een eenvoudige werkstroom is, dan zou het beter zijn om de activiteit opnieuw te vormen. In een gecompliceerde workflow is het beter om de workflowactiviteiten naar een nieuwe workflow te kopiëren, deze op te slaan en opnieuw uit te voeren.
