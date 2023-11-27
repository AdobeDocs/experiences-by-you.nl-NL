---
title: Standaardcodesjablonen maken
description: Voor een basislijnimplementatie (d.w.z. wat uw bedrijf de moet-hebben KPIs voor allen beschouwt [!DNL Adobe Analytics] sites), moet uw org waar mogelijk één implementatiemethode hebben.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10532.jpg
kt: 10532
exl-id: edd3df73-6d1a-4a26-a984-810cc7dd382f
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 1%

---

# Standaardcodesjablonen maken

**WAT:** Voor een &quot;basislijn&quot;implementatie (d.w.z. wat uw bedrijf de moet-hebben KPIs voor allen beschouwt [!DNL Adobe Analytics] sites), moet uw org waar mogelijk één implementatiemethode hebben. Gebruik bijvoorbeeld dezelfde gegevenslaagstructuur op verschillende sites en gebruik dezelfde regel/aangepaste code voor tagbeheer om bijvoorbeeld interne zoekopdrachten of informatie over het bezoekersprofiel vast te leggen.

**WAAROM:** Dankzij een herhaalbare en schaalbare basislijnimplementatie wordt het toevoegen van nieuwe elementen of nieuwe sites/apps een gestroomlijnde, lage inspanningsinspanning terwijl uw implementatie ook schoon en gemakkelijk blijft om problemen op te lossen. Met een uniforme methode wordt het ook gemakkelijker voor nieuwe beheerders/ontwikkelaars om online te komen en te begrijpen waarmee zij werken.

**HOE:** Eén indelingssjabloon gebruiken om aan ontwikkelaars door te geven wanneer een nieuwe site of tagverbetering online komt. Een Word-document werkt meestal goed, waarin u de volgende items kunt omtrekken:

* Variabelen die worden geïmplementeerd, hun doel en wanneer. Bijvoorbeeld:

| AA-variabele | Beschrijving | Wanneer/waar moet worden ingesteld | Instellen |
|--- |--- |--- |--- |
| eVar8 | Trefwoorden voor intern zoeken | Bij het landen van de interne pagina met zoekresultaten | gegevenslaag |
| event8 | Aantal interne zoekopdrachten | Bij het landen van de interne pagina met zoekresultaten | Beginregel |

* Details over het instellen. Dit is waar u om het even welke voorwerpen van de gegevenslaag nodig en hun syntaxis evenals om het even welke regels zou specificeren TMS die moeten worden gevormd en de details van de regelopstelling.
* De gevallen van de test om ervoor te zorgen worden behandeld in QA en alle variabelen u verwacht om in een succesvol testgeval te zien. Beschrijf wat een succesvolle implementatie zou moeten omvatten wanneer de ontwikkelaar deze verbetering test.

In het ideale geval hoeft dit document alleen te worden getweend voor de volgende site waar u de basisbeginselen bijwerkt, zoals de naam van de eigenschap, de naamgevingsconventie voor pagina&#39;s, enzovoort. U hoeft het wiel niet telkens opnieuw uit te vinden en u kunt meer tijd besparen.

## Auteurs

Dit document is medegeschreven door:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, digitaal [!DNL Analytics] Platform Manager bij NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, senior consultant bij [!DNL Adobe]
