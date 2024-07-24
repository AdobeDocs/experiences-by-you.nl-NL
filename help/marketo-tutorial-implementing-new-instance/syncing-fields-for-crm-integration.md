---
title: Velden synchroniseren voor de native CRM-connectors
description: Leer hoe te om uw aanvankelijke integratie van CRM te stroomlijnen door de essentiële gebieden van CRM voor te gebruiken Marketo Engage strategisch te selecteren. Voer de oefening van het Woordenboek van Gegevens uit om de gebieden te identificeren u voor een vlotte synchronisatie nodig hebt van CRM die verkoop en marketing teams helpt gericht blijven.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
source-git-commit: 195a1211b8b191032f4d37662b5beee9a0a54de4
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Velden synchroniseren voor de native CRM-connectors

Gebruikt u Salesforce of Microsoft Dynamics binnen uw organisatie? Als zo, met de inheemse schakelaars van CRM van Marketo Engage (d.w.z. Salesforce, de Dynamica van Microsoft, en Veeva), kunt u marketing en verkoopactiviteiten coördineren door relevante informatie tussen Marketo Engage en CRM foutloos te delen. Alvorens u de aanvankelijke synchronisatie van CRM vormt, zorg ervoor u de gebieden identificeert u tussen de twee systemen wilt synchroniseren om uw gegevensbestand van het Marketo Engage schoon te houden.

Meer informatie over hoe u deze oefening kunt uitvoeren met best practices die door Adobe Professional Services worden voorgesteld. Volg deze instructies om standaardvelden en aangepaste velden te begrijpen en hun relaties tussen Marketo Engage en uw CRM te documenteren.

## Velden identificeren die u wilt synchroniseren voordat u uw CRM integreert met Marketo Engage

Wanneer het integreren van uw CRM met Marketo Engage, zult u waarschijnlijk niet al uw gebieden van CRM aan Marketo Engage hoeven te synchroniseren. Als u strategisch bent over de velden die u nodig hebt, kunt u de gegevensstroom efficiënter verwerken in uw Marketo Engage-instantie.

De eerste synchronisatie tussen uw Marketo Engage en CRM-systeem maakt automatisch koppelingen naar de meeste bestaande standaardvelden (e-mail, Voornaam/achternaam, Bedrijf, enz.). Bovendien, synchroniseert de schakelaar ook ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary) {target="_blank"} de Gebieden van de Douane [ voor uw Leads, Contacten, Rekeningen, en Kansen door nieuwe gebieden in Marketo Engage te creëren die automatisch aan die gebieden van uw CRM in kaart worden gebracht.

Het identificeren van en het organiseren van de gebieden die u van uw CRM voorafgaand aan het uitvoeren van de aanvankelijke synchronisatie zou willen synchroniseren is een kritieke stap in het Instellingsproces van de Eigen Verbinding. Dit wordt een oefening gegevenswoordenboek genoemd, die u helpt het aantal dubbele velden dat wordt gemaakt tot een minimum te beperken en ervoor te zorgen dat alle volgende stappen voor opnieuw toewijzen zo vloeiend mogelijk verlopen. Deze oefening impliceert typisch input van de Marketing en de teams van de Verkoop en uw Admin van CRM om ervoor te zorgen dat slechts de relevante gebieden aan uw instantie van het Marketo Engage worden gesynchroniseerd.

## Uw gegevenswoordenboek maken

Over het algemeen, is de beste praktijk om de gebieden van CRM slechts te synchroniseren die voor marketing doeleinden zullen worden vereist. Begin met deze oefening om de gebieden van uw CRM te organiseren die aan Marketo Engage zullen moeten worden in kaart gebracht en de aanvankelijke synchronisatie van CRM correct de eerste keer in werking stellen.

>[!NOTE]
>Als u douanegebieden in uw CRM hebt die reeds een gelijkwaardig douanegebied in Marketo Engage hebben alvorens met de aanvankelijke synchronisatie te beginnen, wordt een nieuw &quot;dubbel&quot;gebied gecreeerd in Marketo Engage voor het gebied van CRM. U kunt het gebied van CRM aan het originele gebied van het Marketo Engage opnieuw in kaart brengen en het dubbele gebied verbergen zodra de aanvankelijke synchronisatie volledig is, maar u moet ](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console) {target="_blank"} de Steun van de Klant van de Adobe contacteren [ om dit te doen. Zie stap 7 voor meer informatie.

**Stap 1:** Bouw een ruwe lijst van gebieden momenteel beschikbaar in uw CRM en teken of u hen in Marketo Engage zou willen verschijnen.

* Neem feedback van uw CRM-beheerder, -marketing en -verkoopteams op in het besluitvormingsproces.
* Documenteer de API-namen en veldtypen voor elk veld
* Bepaal welk niveau van toegang Marketo Engage voor deze gebieden (d.w.z. read-Only of Read-Write) zou moeten hebben


**Stap 2:** herzie [ Admin > sectie van het Beheer van het Gebied ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce) {target="_blank"} van uw instantie van het Marketo Engage om het even welke douanevelden te identificeren die eerder direct in het systeem worden gecreeerd dat u in de synchronisatie zou willen omvatten.

* Documenteer de API-namen en veldtypen voor elk veld.
* Geef velden aan die al een equivalent veld hebben in uw CRM.
* Geef velden aan die nog geen equivalent veld hebben in uw CRM.


**Stap 3:** Begin bouwend het Woordenboek van Gegevens met de standaardkaartgebieden

* Aangezien het Marketo Engage een vlakke gegevensbestand gebruikt, adviseert men dat u uw Woordenboek van Gegevens als volgt formatteert:

   * Eerste kolom: veldnamen Marketo&#39;s Engage
   * Tweede kolom: Marketo Engage API-namen
   * Derde Kolom: [ Type van het Gebied van het Marketo Engage ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary) {target="_blank"} (d.w.z. Van Boole, Valuta, Datum, enz.)
   * In verdere kolommen, herhaal voor de objecten van CRM types (Lood, Contact, Rekening, Opportunity) met een extra kolom voor het niveau van toegang u Marketo Engage zou willen hebben (d.w.z. Lezen, schrijven, uitgeven)
  <br>

  Hier volgt een voorbeeld van hoe het eruit zou zien:
  ![ Lijst van het Woordenboek van Gegevens ](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Begin door de standaardgebieden toe te voegen die automatisch voor uw CRM zullen worden in kaart gebracht:

   * [ Salesforce ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping) {target="_blank"}
   * [ Dynamica van Microsoft ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping) {target="_blank"}
   * [ Veeva ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping) {target="_blank"}

* Bevestig elk standaardgebied in Marketo Engage het gebied in uw CRM aanpast dat u met zou willen synchroniseren. Het veld &quot;Unsubscribed&quot; in Marketo Engage kan bijvoorbeeld het veld &quot;E-mail weigeren&quot; in uw CRM zijn.
* Pas de naam van CRM API, voorrechten, en [ gegevenstype ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary) aan {target="_blank"} waar nodig.

**Stap 4:** voeg extra gebieden aan het Woordenboek van Gegevens toe

* Neem de weergavenaam, de gewenste CRM-rechten en het gegevenstype voor elk veld op.
* Als een veld bestaat in CRM maar niet in een Marketo Engage, vult u de weergave van het Marketo Engage en de API-namen met dezelfde waarden in het CRM-veld.
* Als een veld in het Marketo Engage bestaat maar niet in de CRM-weergave, vult u de CRM-weergavenaam met de gewenste waarde in, maar laat u de CRM-API-naam leeg tot nadat het veld is gemaakt.
* Als beide systemen equivalente velden bevatten, neemt u deze op dezelfde regel op en geeft u aan dat ze opnieuw moeten worden toegewezen in de sectie &quot;Notities&quot; uiterst rechts van het gegevenswoordenboek.

>[!NOTE]
>Als u op het creëren van een gebied van de Filter van de Synchronisatie ([ Salesforce ](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758) {target="_blank"} plant | [ de Dynamiek van Microsoft ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter) {target="_blank"}), zorg ervoor om het in deze stap te omvatten maar verlaat de namen van API leeg tot het gebied in uw CRM wordt gecreeerd.

**Stap 5:** herzie het Woordenboek van Gegevens met uw Admin van CRM

* Creeer gebieden in CRM voor die reeds in Marketo Engage bestaan en werk het Woordenboek van Gegevens met de Vertoning en API namen voor het nieuwe gebied van CRM bij.
* Voer gebiedstoewijzing tussen Lood en de voorwerpen van het Contact in uw CRM uit ([ Salesforce ](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758) {target="_blank"} | [ de Dynamiek van Microsoft ](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1) {target="_blank"}). Wanneer een lead wordt omgezet in een contactpersoon, zorgt dit ervoor dat de velden kunnen worden geconsolideerd in één veld in het Marketo Engage.
* Controleer of het Marketo Sync Profile (Synchronisatieprofiel) de juiste rechten heeft voor elk veld zoals vermeld in het gegevenswoordenboek:
   * [ vastgestelde profieltoestemmingen in Salesforce ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions) {target="_blank"}
   * [ vastgestelde profieltoestemmingen in de Dynamica van Microsoft ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft) {target="_blank"}
   * [ plaats profieltoestemmingen in Veva ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage#set-profile-permissions) {target="_blank"}

**Stap 6:** voer de aanvankelijke synchronisatie uit

* Zorg ervoor dat alle velden die u wilt synchroniseren met Marketo Engage, de juiste rechten hebben in uw CRM-toepassing, zoals gedefinieerd in het gegevenswoordenboek.
* Zorg ervoor dat alle gebieden u **niet** met Marketo Engage zou willen synchroniseren [ verborgen van het Profiel van de Synchronisatie van Marketo ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync) {target="_blank"} zijn. Het is veel gemakkelijker om later nieuwe velden aan de synchronisatie toe te voegen dan het is om velden te verwijderen die per ongeluk zijn gesynchroniseerd.
* Verbindt u uw CRM met het gebied van de Filter van de Synchronisatie? Als u synchroniseert met Salesforce, neemt u contact op met de klantenondersteuning van de Adobe om ervoor te zorgen dat de filterfunctionaliteit is ingeschakeld voordat u de eerste synchronisatie start.


**Stap 7:** herzie de sectie van het Beheer van het Gebied in Marketo Engage

* Bevestig of werk de Naam van de Vertoning &amp; API voor de nieuwe gesynchroniseerde gebieden bij.
* Identificeer om het even welke gedupliceerde gebieden die opnieuw in kaart moeten brengen. In een paar scenario&#39;s komen gedupliceerde velden voor:
   * De gebieden van de douane in CRM zouden tot een nieuw (potentieel dubbel) gebied in Marketo Engage leiden de eerste keer zij synchroniseren neer als een gelijkwaardig gebied reeds in Marketo Engage bestond.
   * Aangepaste velden alleen in Marketo (dus een veld dat rechtstreeks in Marketo Engage is gemaakt) en een equivalent veld kan worden gesynchroniseerd via de CRM.



**Stap 8:** De Steun van de Klant van de Adobe van het Contact om remapping uit te voeren als de dubbele gebieden verschijnen

* Neem contact op met de Technische Ondersteuning voor de volgende informatie voor velden die opnieuw moeten worden toegewezen:
   * Geef de namen van de vertoning &amp; API voor nieuwe dubbele gebieden door CRM worden gecreeerd die.
   * De naam van de vertoning voor het gebied van het Marketo Engage dat u het gebied van CRM om zou willen in kaart brengen aan.
   * Gelieve te verwijzen naar dit voorbeeld [ HIER ](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284) {target="_blank"}.
* Als het opnieuw toewijzen is voltooid, controleert u de API-namen voor de opnieuw toegewezen velden in het Marketo Engage en werkt u de waarden in de kolom &quot;API-naam&quot; van het gegevenswoordenboek bij om ervoor te zorgen dat dit de meest nauwkeurige gegevens bevat.

## Wat is de volgende?

* Bouw uw Woordenboek van Gegevens om uw gebieden voor de integratie van CRM te organiseren.
* Begrijp me met het aanvankelijke synchronisatieproces voor uw CRM

>[!BEGINTABS]

>[!TAB  Salesforce ]

Leer hoe Marketo Engage en Salesforce samenwerken om uw verkoop- en marketinggegevens synchroon te houden.

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**Verbindingen die in de video worden gebruikt:**

* [ Begrijpend de Synchronisatie Salesforce ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync) {target="_blank"}

* [ voeg de Gebieden van Marketo aan Salesforce (Onderneming/Onbeperkt) toe ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited) {target="_blank"}

* [ creeer een Gebruiker van Marketo in Salesforce (Onderneming/Onbeperkt) ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited) {target="_blank"}

* [ verbind Marketo en Salesforce (Onderneming/Onbeperkt) ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited) {target="_blank"}

* [ De gebruikers zouden omhoog Verbonden App op de kant Salesforce moeten opstelling alvorens zij aan Marketo en de Synchronisatie Salesforce te werk gaan.](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0) {target="_blank"}

* [ de Status van de Synchronisatie van Salesforce ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status) {target="_blank"}

* [ Verberg en maak een Gebied ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field) {target="_blank"} ongedaan

* [ Leerprogramma: Leer over het synchroniseren van Marketo aan uw CRM ](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn) {target="_blank"}

+++

>[!TAB  de Dynamica van Microsoft ]

Leer hoe de synchronisatie van Microsoft Dynamics 365 werkt en vorm de opstelling behoorlijk om de twee systemen toe te staan om met elkaar te spreken.

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**Verbindingen die in de video worden gebruikt:**

* [ Begrijpend de Synchronisatie van de Dynamica van Microsoft ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync) {target="_blank"}

* [ Download de Oplossing van het Beheer van de Lood van Marketo ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution) {target="_blank"}

* [ werk de Oplossing van Marketo voor de Dynamica van Microsoft ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics) bij {target="_blank"}

* [ Toestemming van de toelage voor identiteitskaart van de Cliënt en de Registratie van de Toepassing ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration)

* [ bevestigt de Synchronisatie van de Dynamica van Microsoft ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync) {target="_blank"}

* [ de Status van de Synchronisatie ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status) {target="_blank"}

* [ de Kwesties van de Synchronisatie van de Dynamica van de Reparatie ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues) {target="_blank"}

* [ creeer een Filter van de Synchronisatie van de Dynamiek van de Douane ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter.html) {target="_blank"}

* [ Mening URL van de Dienst van de Organisatie ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url) {target="_blank"}

* [ het uitgeven Gebieden om te synchroniseren alvorens hen in Dynamica te schrappen ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics) {target="_blank"}

* [ Leerprogramma: Leer over het synchroniseren van Marketo aan uw CRM ](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn) {target="_blank"}

+++

>[!ENDTABS]

### Auteurs

{{peter-livadas}}

{{amy-chiu}}
