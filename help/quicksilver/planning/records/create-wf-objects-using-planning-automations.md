---
title: Skapa Workfront-objekt med hjälp av Adobe Workfront Planning Record Automations
description: Du kan konfigurera automatisering i Adobe Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller poster i Workfront Planning. Objekten och posterna som skapas kopplas automatiskt till befintliga planeringsposter. I den här artikeln beskrivs hur du kan hantera automatiseringar, inklusive hur du redigerar, inaktiverar, tar bort och utlöser dem för att skapa objekt och poster.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 585a65c497211c84cffafeeaa5016218fd66acd2
workflow-type: tm+mt
source-wordcount: '2197'
ht-degree: 0%

---

# Skapa objekt med automatisering av Adobe Workfront Planning Record

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Du kan konfigurera automatisering i Adobe Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller poster i Workfront Planning när de aktiveras från en Planning-post. De skapade objekten eller posterna ansluts automatiskt till de poster som du aktiverar automatiseringen från.

Du kan konfigurera och aktivera automatiseringen på posttypens sida i Workfront Planning. Det anslutna objektet som skapas placeras i det anslutna fältet för den posttyp som du kör automatiseringen från.

Du kan till exempel skapa en automatisering som tar en Workfront Planning-kampanj och skapar ett projekt i Workfront för att spåra kampanjens utveckling. Projektet kopplas till Workfront Planning Campingkampanj i fältet Connected Project i kampanjen.

Mer information om anslutna poster finns i [Översikt över anslutna poster](/help/quicksilver/planning/records/connected-records-overview.md).

Du kan skapa följande med automatisering i Workfront Planning:

* Ett <span class="preview">eller flera</span> projekt
* En grupp
* Ett program
* En portfölj
* Ett projekt
* En post

## Åtkomstkrav

+++ Expandera för att visa åtkomstkrav..

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
   <p>Redigera åtkomst med Skapa objekt i Workfront för de objekttyper som du vill skapa (projekt, portfolior, program). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter på arbetsytan för att skapa automatisering. </p>
   <p>Contribute eller högre behörigheter till arbetsytan <!--<span class="preview">and to the record type</span>--> där du vill skapa objekt med hjälp av befintliga automatiseringar. </p>  
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (program eller projekt).</p>
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
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

* Namnet på det objekt eller den post som skapas av en automatisering är samma som det postnamn som du skapar objektet från när du skapar ett enskilt objekt.

<div class="preview">

* När du skapar flera projekt får de automatiskt följande namn:

  `[ Name of the record ] Name of the field choice`

  Mer information finns i avsnittet [Använd en Workfront Planning Automation för att skapa ett objekt eller en post](#use-a-workfront-planning-automation-to-create-an-object-or-a-record) i den här artikeln.

</div>

* Nya objekt eller poster åsidosätter inte befintliga objekt i samma fält. Om samma automatisering aktiveras flera gånger för samma post läggs nya objekt eller poster i samma kopplade fält i den ursprungliga posten till, förutom de som skapades tidigare.

<!--hide this for now; they are trying to remove this militation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

## Konfigurera automatisering i Workfront Planning

Du måste konfigurera en automatisering för en posttyp i Workfront Planning innan du kan använda den för att skapa objekt.

{{step1-to-planning}}

1. Klicka på ett posttypskort och klicka sedan på namnet på en post.

   Posttypssidan öppnas.
1. Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Hantera automatisering**.

   En lista över tillgängliga automatiseringar för den valda posttypen öppnas.

1. Klicka på **Ny automatisering** i skärmens övre högra hörn. Rutan **Ny automatisering** öppnas.
1. Uppdatera följande fält:

   * Ersätt **Namnlös automatisering** med texten som du vill ska visas på automatiseringsknappen. Användare klickar på den här knappen när de använder automatiseringen för att skapa ett Workfront-objekt eller en Planning-post.
   * **Beskrivning**: Lägg till en beskrivning för att identifiera syftet med automatiseringen.
1. Klicka på **Spara**.
Sidan med information om automatisering öppnas.

1. Uppdatera följande fält i avsnittet **Utlösare** på informationssidan för automatiseringen:

   * **Utlösare**: Välj den åtgärd som ska utlösa automatiseringen. Välj till exempel **Knapp klicka**. <!--update this step with a list of all possible triggers; right now only Button click is available-->

1. Uppdatera följande fält i avsnittet **Åtgärder**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Åtgärder**: Välj den åtgärd som du vill att Workfront ska utföra när automatiseringen aktiveras. Detta är ett obligatoriskt fält.
Välj någon av följande åtgärder:

      * <span class="preview">Skapa flera projekt</span>
      * <span class="preview">Skapa ett enskilt projekt</span>
      * Skapa projekt
      * Skapa post
      * Skapa program
      * Skapa portfölj
      * Skapa grupp

     >[!TIP]
     >
     >När du har sparat automatiseringen kan du inte längre ändra åtgärden som är vald i det här fältet.

1. (Villkorligt) Beroende på vilken åtgärd du valde kan du uppdatera följande fält:

   * **Skapa <span class="preview">ett enskilt</span> projekt**: <!--replace to the left: Create a single project-->
      * **Anslutet fält där projektet skapas**: Det här är det anslutna fältet som det nya projektet ska visas i. Detta är ett obligatoriskt fält.
      * **Projektmall**: Välj en projektmall som Workfront ska använda för att skapa projektet.

   <div class="preview">

   * Skapa flera projekt:
      * **Anslutet fält där projektet skapas**: Det här är det anslutna fältet som det nya projektet ska visas i. Detta är ett obligatoriskt fält.
      * **Fält vars val skapar posterna**: Välj ett fält med flera eller enstaka val från den valda posttypen. Workfront skapar ett projekt för varje fältval som är markerat på den post från vilken du utlöser automatiseringen.

     >[!TIP]
     >
     >Ett projekt skapas bara för de alternativ som är markerade i flervalsfältet eller envalsfältet i den post som du kör automatiseringen från, och inte för alla möjliga val för det fältet.
     >

      * **Använd samma mall**: Välj det här alternativet om du vill använda samma mall för varje nytt projekt. Om alternativet är avmarkerat väljer du en **projektmall** för varje fältval.
      * **Projektmall**: Om du valde alternativet **Använd samma mall** väljer du en projektmall som Workfront ska använda för att skapa projekten.

   </div>

   * **Skapa portfölj**:
      * **Anslutet fält där portföljen skapas**: Det här är det anslutna fältet där den nya portföljen visas. Detta är ett obligatoriskt fält.
      * **Anpassat formulär att koppla till den nya portföljen**: Välj ett anpassat formulär att koppla till den nya portföljen. Du måste skapa ett anpassat portföljformulär innan du kan markera det.
   * **Skapa program**:
      * **Anslutet fält där programmet skapas**: Det här är det anslutna fältet som det nya programmet visas i. Detta är ett obligatoriskt fält.
      * **Programportfölj**: Välj en portfölj där det nya programmet ska läggas till. Detta är ett obligatoriskt fält.
      * **Anpassat formulär att koppla till det nya programmet**: Välj ett anpassat formulär att koppla till det nya programmet. Du måste skapa ett anpassat programformulär innan du kan markera det.
   * **Skapa grupp**:
      * **Anslutet fält där gruppen skapas**: Det här är det anslutna fältet där den nya gruppen visas. Detta är ett obligatoriskt fält.
      * **Anpassat formulär att koppla till den nya gruppen**: Välj ett anpassat formulär att koppla till det nya programmet. Du måste skapa ett anpassat programformulär innan du kan markera det.
   * **Skapa post**:
      * **Posttyp**: Välj den posttyp som du vill skapa.

        Underavsnittet **Inställningar** visas. Uppdatera följande fält i underavsnittet **Inställningar**:

         * **Fält på den anslutna posttypen där den aktuella posten visas**: Det här är det anslutna fältet på den posttyp som valts för åtgärden där den aktuella posten visas.

        Om du till exempel skapar en automatisering för kampanjer att koppla ihop produktposter från, är det här det anslutna fältet på produktposttypen där kampanjerna visas, efter att produkterna har skapats med automatiseringen.

        Detta är ett obligatoriskt fält.

        <!--submitted a change in functionality and UI text for this - revise??-->
Uppdatera följande information i området **Kartfält**:

         * **Överför från**: Välj fält från den posttyp som automatiseringen skapas för för att mappa dem till fälten för den anslutna posttypen.
         * **Överför till**: Välj fält från den nyligen skapade posten som ska innehålla information från den post som du kör automatiseringen från.

        >[!TIP]
        >
        >* Fälttyperna från den ursprungliga posttypen måste matcha fälttyperna från den nyligen skapade posttypen.
        >* Om du inte väljer några fält blir namnen på de nya posterna **Namnlös post**.

1. (Valfritt och villkorligt) Om du har valt att skapa en post klickar du på **Lägg till fält** för att mappa ytterligare uppslagsfält från en post till en annan.
1. (Villkorligt) Om det inte finns några anslutningsfält mellan den ursprungliga posttypen och den posttyp som har valts i fältet **Posttyp** klickar du på **Lägg till anslutet fält**.

   ![Automatisering för att skapa en post](assets/automation-setup-create-record.png)

   Följande två fält skapas:

   * Ett nytt anslutningsfält med namnet **Ansluten post** skapas för den posttyp som du angav i fältet **Posttyp**.
   * Ett nytt anslutningsfält med samma namn som det som anges i fältet **Posttyp** skapas för den posttyp som du konfigurerar automatiseringen för.

     Om du till exempel konfigurerar en automatisering för kampanjer att automatiskt skapa en annan posttyp som heter Varumärke och du klickar på **Lägg till anslutet fält** skapas följande fält:

      * Anslutningsfältet **Ansluten post** skapas för posttypen **Varumärken**.
      * Anslutningsfältet **Varumärken** skapas för posttypen **Kampanjer**.

1. (Valfritt) Om det inte finns några anslutningsfält mellan den ursprungliga posttypen och det Workfront-objekt som är markerat i åtgärdsområdet klickar du på **Lägg till anslutet fält**.

   ![Automatisering för att skapa flera projekt](assets/automation-setup-create-multiple-projects.png)

   Följande skapas:

   * Ett nytt anslutningsfält med namnet **Ansluten &lt; namnet på Workfront-objektet >** skapas för den posttyp som du bygger automatiseringen för. Ett **anslutet projekt**-fält skapas till exempel för den posttyp som du bygger automatiseringen för när du väljer att skapa projekt automatiskt.
   * Ett nytt posttypskort läggs till i Planning-delen av ett Workfront-projekt i Workfront med namnet på den posttyp som du konfigurerar automatiseringen för.

1. Klicka på **Spara** i det övre högra hörnet på sidan med automatiseringsinformation.

   Automatiseringen visas i listan över automatiseringar och finns tillgänglig för arkivering.

## Hantera befintliga automatiseringar

{{step1-to-planning}}

1. Klicka på ett posttypskort och klicka sedan på namnet på en post.

   Posttypssidan öppnas.
1. Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Hantera automatisering**.

   En lista över tillgängliga automatiseringar för den valda posttypen öppnas.

1. (Valfritt) Gör något av följande om du vill redigera, inaktivera eller ta bort en automatisering:

   1. Håll markören över namnet på en sparad automatisering i listan över automatiseringar och klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png).

   1. Klicka på **Redigera** för att uppdatera följande information:

      * Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om automatiseringsnamnet och klicka sedan på **Redigera** för att ändra namnet på automatiseringen.
      * Alla fält i automatiseringen, förutom fältet **Åtgärder**.

        >[!TIP]
        >
        >Du kan inte ändra åtgärden som du ursprungligen valde för en automatisering.


   1. Klicka på **Inaktivera** om du vill ta bort automatiseringen från postens tabellvy och hindra användare från att använda den för att skapa poster eller objekt.

      Poster som har skapats med en inaktiverad automatisering är fortfarande kopplade till den post som ursprungligen valdes.

      Om du vill göra den tillgänglig igen klickar du på menyn **Mer** ![Mer](assets/more-menu.png) igen och sedan på **Aktivera**.
   1. Klicka på **Ta bort** om du vill ta bort automatiseringen. En borttagen automatisering kan inte återställas.

      Poster som har skapats med en borttagen automatisering är fortfarande kopplade till den post som ursprungligen valdes.

## Skapa ett objekt eller en post med en Workfront Planning Automation

1. I Workfront Planning öppnar du den posttypssida som innehåller den automatisering som du vill använda för att automatiskt skapa och koppla poster eller objekt.
1. Öppna tabellvyn.
1. Markera en eller flera poster.

   Ett blått fält visas längst ned i tabellen med ytterligare knappar, inklusive automatiseringsknappar.
1. Klicka på knappen för automatisering i skärmens nedre högra hörn.

   ![Automatiseringsknappen](assets/automation-custom-button.png)

   Följande saker händer:

   * Ett bekräftelsemeddelande visas längst ned på skärmen om automatiseringen lyckades skapa ett objekt eller en post.

   * Det nya objektet visas i det anslutna fältet som anges i inställningarna för knappen för automatisering. Du kan behöva uppdatera sidan innan du kan visa det nya objektet. Det nya objektet har samma namn som den ursprungliga posten.

   <div class="preview">

   * Om flera projekt har skapats baserat på val av flera- eller enkelvalsfält får projekten automatiskt ett namn enligt följande mönster:

     `[ Name of the record ] Name of the field choice`

     Om en kampanj med namnet `Summer breeze` genererade ett projekt från ett fältval av `EMEA` får projektet namnet `[ Summer breeze ] EMEA`.

   </div>

   * Den post som du utlöser automatiseringen från läggs till i det anslutna fältet för den nya posten.

   >[!NOTE]
   >
   >Vi rekommenderar att du kontrollerar att objekten eller posterna har skapats och anslutits som förväntat.

1. (Valfritt) Klicka på det nya objektet i det anslutna fältet. Objektsidan öppnas och du kan göra ytterligare ändringar i det nya objektet.

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

