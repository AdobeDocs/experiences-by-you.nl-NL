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
source-git-commit: 47ab8875bc4e41595cd40550330e43a88357b68d
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---


# Velden synchroniseren voor de native CRM-connectors

Gebruikt u Salesforce of Microsoft Dynamics binnen uw organisatie? Als zo, met de inheemse schakelaars van CRM van Marketo Engage (d.w.z. Salesforce, de Dynamica van Microsoft, en Veeva), kunt u marketing en verkoopactiviteiten coördineren door relevante informatie tussen Marketo Engage en CRM foutloos te delen. Alvorens u de aanvankelijke synchronisatie van CRM vormt, zorg ervoor u de gebieden identificeert u tussen de twee systemen wilt synchroniseren om uw gegevensbestand van het Marketo Engage schoon te houden.

Meer informatie over hoe u deze oefening kunt uitvoeren met best practices die door Adobe Professional Services worden voorgesteld. Volg deze instructies om standaardvelden en aangepaste velden te begrijpen en hun relaties tussen Marketo Engage en uw CRM te documenteren.

## Velden identificeren die u wilt synchroniseren voordat u uw CRM integreert met Marketo Engage

Wanneer het integreren van uw CRM met Marketo Engage, zult u waarschijnlijk niet al uw gebieden van CRM aan Marketo Engage hoeven te synchroniseren. Als u strategisch bent over de velden die u nodig hebt, kunt u de gegevensstroom efficiënter verwerken in uw Marketo Engage-instantie.

De eerste synchronisatie tussen uw Marketo Engage en CRM-systeem maakt automatisch koppelingen naar de meeste bestaande standaardvelden (e-mail, Voornaam/achternaam, Bedrijf, enz.). Bovendien synchroniseert de aansluiting ook [Aangepaste velden](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} voor uw Leads, Contacten, Rekeningen, en Kansen door nieuwe gebieden in Marketo Engage te creëren die automatisch aan die gebieden van uw CRM worden in kaart gebracht.

Het identificeren van en het organiseren van de gebieden die u van uw CRM voorafgaand aan het uitvoeren van de aanvankelijke synchronisatie zou willen synchroniseren is een kritieke stap in het Instellingsproces van de Eigen Verbinding. Dit wordt een oefening gegevenswoordenboek genoemd, die u helpt het aantal dubbele velden dat wordt gemaakt tot een minimum te beperken en ervoor te zorgen dat alle volgende stappen voor opnieuw toewijzen zo vloeiend mogelijk verlopen. Deze oefening impliceert typisch input van de Marketing en de teams van de Verkoop en uw Admin van CRM om ervoor te zorgen dat slechts de relevante gebieden aan uw instantie van het Marketo Engage worden gesynchroniseerd.

## Uw gegevenswoordenboek maken

Over het algemeen, is de beste praktijk om de gebieden van CRM slechts te synchroniseren die voor marketing doeleinden zullen worden vereist. Begin met deze oefening om de gebieden van uw CRM te organiseren die aan Marketo Engage zullen moeten worden in kaart gebracht en de aanvankelijke synchronisatie van CRM correct de eerste keer in werking stellen.

>[!NOTE]
>Als u douanegebieden in uw CRM hebt die reeds een gelijkwaardig douanegebied in Marketo Engage hebben alvorens met de aanvankelijke synchronisatie te beginnen, zal een nieuw &quot;dubbel&quot;gebied in Marketo Engage voor het gebied van CRM worden gecreeerd. U kunt het CRM-veld opnieuw toewijzen aan het oorspronkelijke veld van het Marketo Engage en het gedupliceerde veld verbergen zodra de initiële synchronisatie is voltooid, maar u moet contact opnemen met [Klantenondersteuning Adoben](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} om dit te doen. Zie stap 7 voor meer informatie.

**Stap 1:** Bouw een ruwe lijst van gebieden momenteel beschikbaar in uw CRM en merk of u hen in Marketo Engage wilt verschijnen.

* Neem feedback van uw CRM-beheerder, -marketing en -verkoopteams op in het besluitvormingsproces.
* Documenteer de API-namen en veldtypen voor elk veld
* Bepaal welk niveau van toegang Marketo Engage voor deze gebieden (d.w.z. read-Only of Read-Write) zou moeten hebben


**Stap 2:** Controleer de [Beheer > sectie Veldbeheer](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} van uw Marketo Engage-instantie om eventuele aangepaste velden te identificeren die eerder rechtstreeks in het systeem zijn gemaakt en die u in de synchronisatie wilt opnemen.

* Documenteer de API-namen en veldtypen voor elk veld.
* Geef velden aan die al een equivalent veld hebben in uw CRM.
* Geef velden aan die nog geen equivalent veld hebben in uw CRM.


**Stap 3:** Beginnen het Woordenboek van Gegevens met de standaardkaartgebieden te bouwen

* Aangezien het Marketo Engage een vlakke gegevensbestand gebruikt, adviseert men dat u uw Woordenboek van Gegevens als volgt formatteert:

   * Eerste kolom: veldnamen Marketo&#39;s Engage
   * Tweede kolom: Marketo Engage API-namen
   * Derde kolom: [Veldtype Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} (d.w.z. Boolean, Valuta, Datum, enz.)
   * In verdere kolommen, herhaal voor de objecten van CRM types (Lood, Contact, Rekening, Opportunity) met een extra kolom voor het niveau van toegang u Marketo Engage zou willen hebben (d.w.z. Lezen, schrijven, uitgeven)
  <br>

  Hier volgt een voorbeeld van hoe het eruit zou zien:
  ![Tabel gegevenswoordenboek](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Begin door de standaardgebieden toe te voegen die automatisch voor uw CRM zullen worden in kaart gebracht:

   * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Bevestig elk standaardgebied in Marketo Engage het gebied in uw CRM aanpast dat u met zou willen synchroniseren. Het veld &quot;Unsubscribed&quot; in Marketo Engage kan bijvoorbeeld het veld &quot;E-mail weigeren&quot; in uw CRM zijn.
* De naam, rechten en [gegevenstype](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} indien nodig.

**Stap 4:** Extra velden toevoegen aan het gegevenswoordenboek

* Neem de weergavenaam, de gewenste CRM-rechten en het gegevenstype voor elk veld op.
* Als een veld bestaat in CRM maar niet in een Marketo Engage, vult u de weergave van het Marketo Engage en de API-namen met dezelfde waarden in het CRM-veld.
* Als een veld in het Marketo Engage bestaat maar niet in de CRM-weergave, vult u de CRM-weergavenaam met de gewenste waarde in, maar laat u de CRM-API-naam leeg tot nadat het veld is gemaakt.
* Als beide systemen equivalente velden bevatten, neemt u deze op dezelfde regel op en geeft u aan dat ze opnieuw moeten worden toegewezen in de sectie &quot;Notities&quot; uiterst rechts van het gegevenswoordenboek.

>[!NOTE]
>Als u een veld Filter synchroniseren wilt maken ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}), moet u deze in deze stap opnemen, maar laat de API-namen leeg totdat het veld wordt gemaakt in uw CRM.

**Stap 5:** Controleer het gegevenswoordenboek met uw CRM-beheerder

* Creeer gebieden in CRM voor die reeds in Marketo Engage bestaan en werk het Woordenboek van Gegevens met de Vertoning en API namen voor het nieuwe gebied van CRM bij.
* Veldtoewijzing uitvoeren tussen de objecten Lead en Contact in uw CRM ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}). Wanneer een lead wordt geconverteerd naar een contactpersoon, zorgt dit ervoor dat de velden kunnen worden geconsolideerd in één veld in het Marketo Engage.
* Controleer of het Marketo Sync Profile (Synchronisatieprofiel) de juiste rechten heeft voor elk veld zoals vermeld in het gegevenswoordenboek:
   * [Profielmachtigingen instellen in Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Profielmachtigingen instellen in Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Profielmachtigingen instellen in Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}

**Stap 6:** De eerste synchronisatie uitvoeren

* Zorg ervoor dat alle velden die u wilt synchroniseren met Marketo Engage, de juiste rechten hebben in uw CRM-toepassing, zoals gedefinieerd in het gegevenswoordenboek.
* Zorg ervoor dat alle velden die u wilt instellen  ***niet*** houden van synchronisatie met Marketo Engage [verborgen in het Marketo Sync Profile](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. Het is veel gemakkelijker om later nieuwe velden aan de synchronisatie toe te voegen dan het is om velden te verwijderen die per ongeluk zijn gesynchroniseerd.
* Verbindt u uw CRM met het gebied van de Filter van de Synchronisatie? Als u synchroniseert met Salesforce, neemt u contact op met de Klantenondersteuning van de Adobe om ervoor te zorgen dat de filterfunctionaliteit is ingeschakeld voordat u de eerste synchronisatie start.


**Stap 7:** De sectie Veldbeheer in Marketo Engage controleren

* Bevestig of werk de Naam van de Vertoning &amp; API voor de nieuwe gesynchroniseerde gebieden bij.
* Identificeer om het even welke gedupliceerde gebieden die opnieuw in kaart moeten brengen. In een paar scenario&#39;s komen gedupliceerde velden voor:
   * De gebieden van de douane in CRM zouden tot een nieuw (potentieel dubbel) gebied in Marketo Engage leiden de eerste keer zij synchroniseren neer als een gelijkwaardig gebied reeds in Marketo Engage bestond.
   * Aangepaste velden alleen in Marketo (dus een veld dat rechtstreeks in Marketo Engage is gemaakt) en een equivalent veld kan worden gesynchroniseerd via de CRM.



**Stap 8:** Neem contact op met de Klantenondersteuning van de Adobe om een nieuwe toewijzing uit te voeren als gedupliceerde velden worden weergegeven

* Neem contact op met de Technische Ondersteuning voor de volgende informatie voor velden die opnieuw moeten worden toegewezen:
   * Geef de namen van de vertoning &amp; API voor nieuwe dubbele gebieden door CRM worden gecreeerd die.
   * De naam van de vertoning voor het gebied van het Marketo Engage dat u het gebied van CRM om zou willen in kaart brengen aan.
   * Zie dit voorbeeld [HIER](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}.
* Als het opnieuw toewijzen is voltooid, controleert u de API-namen voor de opnieuw toegewezen velden in het Marketo Engage en werkt u de waarden in de kolom &quot;API-naam&quot; van het gegevenswoordenboek bij om ervoor te zorgen dat dit de meest nauwkeurige gegevens bevat.

## Wat is de volgende?

* Bouw uw Woordenboek van Gegevens om uw gebieden voor de integratie van CRM te organiseren.
* Begrijp me met het aanvankelijke synchronisatieproces voor uw CRM

>[!BEGINTABS]

>[!TAB Salesforce]

Leer hoe Marketo Engage en Salesforce samenwerken om uw verkoop- en marketinggegevens synchroon te houden.

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**Koppelingen in de video:**

* [Werken met Salesforce Sync](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.html){target="_blank"}

* [Marketo-velden toevoegen aan Salesforce (Enterprise/Onbeperkt)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.html){target="_blank"}

* [Een Marketo-gebruiker maken in Salesforce (Enterprise/Onbeperkt)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.html){target="_blank"}

* [Connect Marketo en Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.html){target="_blank"}

* [Gebruikers moeten de Connected App instellen aan de Salesforce-zijde voordat ze verdergaan met Marketo en Salesforce Sync.](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.html){target="_blank"}

* [Status van Salesforce-synchronisatie](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status.html){target="_blank"}

* [Een veld verbergen en verbergen opheffen](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field.html){target="_blank"}

* [Zelfstudie: Meer informatie over het synchroniseren van Marketo naar uw CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Leer hoe de synchronisatie van Microsoft Dynamics 365 werkt en vorm de opstelling behoorlijk om de twee systemen toe te staan om met elkaar te spreken.

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**Koppelingen in de video:**

* [Werken met Microsoft Dynamics Sync](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync.html){target="_blank"}

* [Download de Marketo Lead Management Solution](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution.html){target="_blank"}

* [Marketo Solution for Microsoft Dynamics bijwerken](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.html){target="_blank"}

* [Toestemming verlenen voor client-id en toepassingsregistratie](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration.html)

* [Microsoft Dynamics Sync valideren](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync.html){target="_blank"}

* [Synchronisatiestatus](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status.html){target="_blank"}

* [Problemen met validatie synchroniseren van dynamiek verhelpen](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues.html){target="_blank"}

* [Een filter voor aangepaste dynamicasynchronisatie maken](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynmaics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [De URL van de organisatieservice weergeven](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url.html){target="_blank"}

* [Te synchroniseren velden bewerken voordat deze worden verwijderd in Dynamiek](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics.html){target="_blank"}

* [Zelfstudie: Meer informatie over het synchroniseren van Marketo naar uw CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!ENDTABS]

### Auteurs

{{peter-livadas}}

{{amy-chiu}}
