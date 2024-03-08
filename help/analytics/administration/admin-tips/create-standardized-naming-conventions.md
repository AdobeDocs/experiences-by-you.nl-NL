---
title: Standaardnaamconventies maken
description: De gestandaardiseerde Naamgevingsconventies zijn van toepassing op zowel de variabelenaam zelf wanneer deze wordt ingeschakeld in de API voor AA-beheer als op de waarden die worden doorgegeven aan de dimensie.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10531.jpg
kt: 10531
exl-id: 79cec21e-2b52-4e7b-88ad-db137a8cef4e
source-git-commit: c568ed0a06551d910b6f533698ec47c15adecf6c
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Standaardnaamconventies maken

**WAT:** De gestandaardiseerde naamconventies zijn van toepassing op de naam van de variabele zelf wanneer deze wordt ingeschakeld in het dialoogvenster [!DNL Adobe Analytics] (AA) admin UI en de waarden die in de afmeting worden overgegaan. (Paginanamen zouden dus &quot;paginanaam (v1)&quot; zijn als variabelenaam en de ingevoerde paginanamen moeten uniform zijn en een specifieke structuur/hiërarchie volgen, zoals &quot;sitename|homepage&quot; of &quot;sitename|zoekopdracht|zoekresultaten&quot;).

**WAAROM:** Namen van conventies zijn een uitstekende manier om alles uniform te houden en de interface begrijpelijk te houden voor uw gebruikers. Als u deze van het begin creeert en hen in het platform en de code afdwingt, zullen deze gemakkelijker aan schaal zijn.

**HOE:** De interface en het etiketteren doc zouden voor zowel &quot;Naam&quot;als &quot;Beschrijving&quot;moeten aanpassen - dit zal uw gebruikers van het moeten sparen een document van Excel trekken en hen toestaan om uw gegevens direct in de interface te begrijpen. Het wordt ook aanbevolen om alles wat nodig is voor de consistentie te beperken.

Het is altijd het beste om paginanamen ook op het platform consistent te houden (of schermnamen voor apps). U kunt bijvoorbeeld &quot;`property:section:sub section:sub sub section:unique page name`&quot; in een variabele/dimensie. Als al deze gebieden in uw gegevenslaag afzonderlijk zijn, kon u zelfs de paginanaam direct in uw JS dossier/Lancering bouwen. Als al deze elementen ook in hun eigen dimensies zijn ingesteld, kunt u specifieke eigenschappen of gebieden van uw site/app eenvoudiger indelen en meer inzicht krijgen in verkeer en stromen.

Om het even wat dat het voor gebruikers gemakkelijker maakt om de gegevens, met inbegrip van iets te vinden en te begrijpen zoals noemende overeenkomsten, zal het gebruik van [!DNL Adobe Analytics] en levert betere inzichten voor het bedrijf.

## Auteurs

Dit document is medegeschreven door:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, digitaal [!DNL Analytics] Platform Manager bij NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, senior consultant bij [!DNL Adobe]
