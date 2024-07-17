---
title: Logboek CRM-synchronisatiefouten voor eenvoudige probleemoplossing
description: Leer hoe te om een logboek van de fouten van de Synchronisatie van CRM te gebruiken om de synchronisatiekwesties van CRM te onderzoeken en het te houden regelmatig lopend.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Logboek CRM-synchronisatiefouten voor eenvoudige probleemoplossing

Als a [!DNL Marketo Engage] beheerder, die als uw instantie synchroon met uw CRM is zou een zeer belangrijk deel van uw [ dagelijkse routine ](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508) moeten zijn {target="_blank"}. Terwijl de [ sectie van Meldingen ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html) {target="_blank"} (vind het op de hoogste juiste hoek van uw [!DNL Marketo Engage] interface) waar u zult beginnen om frequente synchronisatiekwesties te vinden en te onderzoeken, is er een pro tip die u zou kunnen helpen de instantiekwaliteit op een georganiseerde manier beheren. [!DNL Adobe] Marketo Champion (2019-2022), Amy Goldfine raadt beheerders aan een logboek van de fouten van de Synchronisatie van CRM bij te houden om het oplossen van problemen gemakkelijker te maken.

![ Schermafbeelding van het lusje van de Fouten van de Synchronisatie ](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Waarom een overzicht bijhouden van CRM-synchronisatiefouten?

Door de fouten van de Synchronisatie van CRM te registreren, kunnen [!DNL Marketo Engage] beheerders de kwesties en de tendensen met de beheerders van CRM herzien om de worteloorzaak te bevestigen. Volg de onderstaande stappen om uw problemen met CRM Sync voor uw instantie te documenteren.

## Hoe te om een logboek van de Fouten van de Synchronisatie van CRM te houden

Alvorens u begonnen wordt, download het [ malplaatje van het Logboek van de Fouten van de Synchronisatie van CRM ](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Stap 1:** ga naar de *[!UICONTROL Admin]sectie* in [!DNL Marketo Engage]. Klik onder *[!UICONTROL Integration]* op *[!DNL Salesforce]* , *[!DNL Microsoft Dynamics]* of *[!DNL Veeva]* , afhankelijk van welke [!DNL CRM] u gebruikt, en vervolgens op de tab *[!UICONTROL Sync Errors]* .

**Stap 2:** u kunt verkiezen om de verslagen van fouten als a  [!DNL CSV]  dossier door het [!UICONTROL Filter] paneel ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors) {target="_blank"} uit te voeren. [ Als u slechts een paar uur hebt, kunt u het beste rechtstreeks vanaf het tabblad *[!UICONTROL Sync Errors]* kopiëren en plakken.

**Stap 3:** neem nota van de datum dat de fout voorkwam.

**Stap 4:** ga het aantal persoonverslagen in die door die fout worden beïnvloed. (Soms zal uw CRM slechts een fout voor één persoon veroorzaken. Soms zullen er veel mensen met dezelfde fout tegelijk zijn.)

**Stap 5:** neem nota van het e-mailadres van één persoon die door de fout wordt beïnvloed. Dit maakt het voor u gemakkelijk om de fouten met de beheerder van CRM van verwijzingen te voorzien en te bespreken.

**Stap 6:** de verbindingen van het Deeg met het persoonverslag in [!DNL Marketo Engage] en [!UICONTROL CRM Lead/Contact] verslag van die persoon.

**Stap 7:** in de laatste kolom, kleef de daadwerkelijke tekst van de fout.

## Wat is de volgende?

**identificeer de Codes van de Fout:** om de foutencodes te begrijpen, bekijk omhoog de beschrijvingen in de van de ontwikkelaarsdocumentatie [ antwoord-Niveau Codes lijst van de Fout ](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes) {target="_blank"} en vind typische volgende stappen om de fouten op te lossen.

## Auteurs

**Amy Goldfine**\
[!DNL Adobe] Marketo Champion (2019-2022)
*Oprichter, MarketingOpsAdvice.com*

![ Amy Goldfine ](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Beheer van toepassings- en retentiemarkering op[!DNL Adobe]*

![ Amy Chiu ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
