---
title: Skapa Workfront-objekt med hjälp av Adobe Workfront Planning Record Automations
description: Du kan konfigurera automatisering i Adobe Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller poster i Workfront Planning. Objekten och posterna som skapas kopplas automatiskt till befintliga planeringsposter.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 0%

---

# Skapa objekt med automatisering av Adobe Workfront Planning Record

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Du kan konfigurera automatisering i Adobe Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller registrerar Workfront Planning. De skapade objekten eller posterna länkas automatiskt till de poster som du aktiverar automatiseringen från.

Du kan konfigurera och aktivera automatiseringen på postens sida i Workfront Planning. Det anslutna objektet som skapas placeras i det anslutna fältet för den posttyp som du kör automatiseringen från.

Du kan till exempel skapa en automatisering som tar en Workfront Planning-kampanj och skapar ett projekt i Workfront för att spåra kampanjens utveckling. Projektet kopplas till Workfront Planning Campingkampanj i fältet Connected Project i kampanjen.

Mer information om anslutna poster finns i [Översikt över anslutna poster](/help/quicksilver/planning/records/connected-records-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td> Standard
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p> 
   <p>Redigera åtkomst i Workfront för de objekttyper som du vill skapa (projekt, portföljer, program). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter för den arbetsyta som du vill lägga till poster i. </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Att tänka på när du skapar objekt och poster med hjälp av en automatisering

* Det nya objektet eller postnamnet är samma som det postnamn som du skapade det från. <!--take this out when they add the field mapping - no longer just the name of the original record-->
* Nya objekt åsidosätter inte befintliga objekt i samma fält.
* Automatiseringen skapar ytterligare objekt endast i fälten för många till många eller en till många anslutningstyper.

## Konfigurera automatisering i Workfront Planning

Du måste konfigurera en automatisering för en posttyp i Workfront Planning innan du kan använda den för att skapa objekt.

{{step1-to-planning}}

1. Klicka på ett posttypskort och klicka sedan på namnet på en post.

   Posttypssidan öppnas.
1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Hantera automatisering**.

   En lista över tillgängliga automatiseringar öppnas.

1. Klicka på **Ny automatisering** i skärmens övre högra hörn. Rutan **Ny automatisering** öppnas.
1. Uppdatera följande fält:

   * Ersätt **Namnlös automatisering** med texten som du vill ska visas på automatiseringsknappen. Användare klickar på den här knappen när de använder automatiseringen för att skapa ett Workfront-objekt eller en Planning-post.
   * **Beskrivning**: Lägg till en beskrivning för att identifiera syftet med automatiseringen.
1. Klicka på **Spara**.
Sidan med information om automatisering öppnas.

1. Uppdatera följande fält i avsnittet **Utlösare** på informationssidan för automatiseringen:

   * **Utlösare**: Välj den åtgärd som ska utlösa automatiseringen. Välj till exempel **Knapp klicka**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Uppdatera följande fält i avsnittet **Åtgärder**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Objekttyp**: Markera det objekt som du vill att automatiseringen ska skapa. Detta är ett obligatoriskt fält.

     Du kan skapa följande objekt från Workfront Planning-poster:

      * Projekt
      * Portfolio
      * Program
      * Grupp
      * Post
1. (Villkorligt) Beroende på vilken typ av objekt du vill skapa uppdaterar du följande fält:

   * **Projekt**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet som det nya projektet ska visas i. Detta är ett obligatoriskt fält
      * **Mall som projektet ska skapas från**: Välj en projektmall som Workfront ska använda för att skapa projektet.
   * **Portfolio**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet där den nya portföljen visas. Detta är ett obligatoriskt fält.
      * **Anpassat formulär att koppla till den nya portföljen**: Välj ett anpassat formulär att koppla till den nya portföljen. Du måste skapa ett anpassat portföljformulär innan du kan markera det.
   * **Program**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet som det nya programmet visas i. Detta är ett obligatoriskt fält.
      * **Programportfölj**: Välj en portfölj där det nya programmet ska läggas till. Detta är ett obligatoriskt fält.
      * 
         * **Anpassat formulär att koppla till det nya programmet**: Välj ett anpassat formulär att koppla till det nya programmet. Du måste skapa ett anpassat programformulär innan du kan markera det.
   * **Grupp**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet där den nya gruppen visas. Detta är ett obligatoriskt fält.
      * **Anpassat formulär att koppla till den nya gruppen**: Välj ett anpassat formulär att koppla till det nya programmet. Du måste skapa ett anpassat programformulär innan du kan markera det.
   * **Post**:
      * **Ansluten posttyp**: Välj den posttyp som du vill skapa.
      * **Anslutet fält där posten skapas**: Det här är det anslutna fältet där den nya posten visas. Detta är ett obligatoriskt fält. <!--this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label-->
      * **Mappa fält**
         * **Överför från**: Välj fält från den posttyp som automatiseringen skapas för för att mappa dem till fälten för den anslutna posttypen.
      * **Överför till**: Välj fält från den nyligen skapade posten som ska innehålla information från den post som du kör automatiseringen från.
1. (Valfritt och villkorligt) Om du har valt att skapa en post klickar du på **Lägg till fält** för att mappa ytterligare uppslagsfält från en post till en annan.
1. (Valfritt och villkorligt) Om du inte har något anslutningsfält för en Workfront-objekttyp klickar du på ikonen **Skapa ett anslutningsfält** ![](assets/create-a-connection-field-icon.png) för att lägga till ett fält.
1. Klicka på **Spara** i det övre högra hörnet på sidan med automatiseringsinformation.

   Automatiseringen visas i listan över automatiseringar och finns tillgänglig för arkivering.
1. (Valfritt) Gör så här om du vill redigera, inaktivera eller ta bort en automatisering:

   1. Håll markören över namnet på en sparad automatisering i listan över automatiseringar och klicka sedan på menyn **Mer** ![](assets/more-menu.png) .

   1. Klicka på **Redigera** för att uppdatera information om och konfigurera fält i automatiseringen.
   1. Klicka på **Inaktivera** om du vill ta bort automatiseringen från tabellvyn och hindra användare från att använda den för att skapa poster eller objekt. Om du vill göra den tillgänglig igen klickar du på menyn **Mer** ![](assets/more-menu.png) igen och sedan på **Aktivera**.
   1. Klicka på **Ta bort** om du vill ta bort automatiseringen. En borttagen automatisering kan inte återställas. Poster som har skapats med automatiseringen är fortfarande kopplade till den post som ursprungligen valdes.

## Skapa ett objekt eller en post med en Workfront Planning Automation

1. Öppna den posttypssida som innehåller de poster du vill använda för att skapa Workfront-objekt eller Planning-poster i Workfront Planning.
1. Öppna tabellvyn.
1. Markera en eller flera poster.

   Ett blått fält visas längst ned i tabellen med ytterligare knappar, inklusive automatiseringsknappar.
1. Klicka på knappen för automatisering i skärmens nedre högra hörn.

   ![Automatiseringsknappen](assets/automation-custom-button.png)

   Ett bekräftelsemeddelande visas längst ned på skärmen om automatiseringen lyckades skapa ett objekt eller en post.

   Det nya objektet visas i det anslutna fältet som du angav i inställningarna för knappen för automatisering. Du kan behöva uppdatera sidan innan du kan visa det nya objektet.

   >[!NOTE]
   >
   >Vi rekommenderar att du kontrollerar att objektet har skapats och anslutits som förväntat.

1. (Valfritt) Klicka på det nya objektet i det anslutna fältet. Objektsidan öppnas och du kan göra ytterligare ändringar i det nya objektet.

<!--you might need to add something about notifications and emails?!-->
