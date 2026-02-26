---
title: Konfigurera Adobe Workfront Planning Automation
description: Du kan konfigurera automatisering i Adobe Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller poster i Workfront Planning. Objekten och posterna som skapas kopplas automatiskt till befintliga planeringsposter. I den här artikeln beskrivs hur du kan hantera automatiseringar, inklusive hur du redigerar, inaktiverar eller tar bort dem.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: cde20e5a-15a2-413a-8de4-ccf6eeb4395f
source-git-commit: f28d2eef57f63cede3a08b06053e8dc6431f21d4
workflow-type: tm+mt
source-wordcount: '1777'
ht-degree: 0%

---

# Konfigurera automatisering av Adobe Workfront Planning

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Du kan konfigurera automatisering i Adobe Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller poster i Workfront Planning när de aktiveras från en Planning-post. De skapade objekten eller posterna ansluts automatiskt till de poster som du aktiverar automatiseringen från.

Du kan konfigurera och aktivera automatiseringen på posttypens sida i Workfront Planning.

Du kan till exempel skapa en automatisering som tar en Workfront Planning-kampanj och skapar ett projekt i Workfront för att spåra kampanjens utveckling.

I den här artikeln beskrivs hur du kan hantera automatiseringar, inklusive hur du redigerar, inaktiverar, tar bort och utlöser dem för att skapa objekt och poster.

Mer information om hur du skapar poster eller objekt med hjälp av en befintlig automatisering finns i [Skapa objekt med hjälp av postautomatisering för Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla Workfront- och Planning-paket</p> <p>Alla arbetsflöden och alla planeringsdokument</p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter till arbetsytan och till den posttyp där du vill skapa automatiseringar. </p>
   <p>Systemadministratörer har behörigheten Hantera för alla arbetsytor, inklusive de som de inte skapade</p>
   </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
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
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and to the record type where you want to create automations. </p>
   <p>System Administrators have Manage permissions to all workspaces, including the ones they did not create</p>
   </td> 
  </tr> 
</tbody> 
</table> -->

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

1. Välj bland följande alternativ i avsnittet **Utlösare** på informationssidan för automatiseringen:

   * **Utlösare**: Välj en åtgärd som ska utlösa automatiseringen:

      * Knappklicka
      * <span class="preview">Fältvärdeändring</span>

   1. (Villkorligt) Om du valde **Knappklicka** går du till steget nedan som beskriver **åtgärdsområdet**.

   1. <span class="preview">(Villkorligt) Om du valde **Ändra fältvärde** gör du följande i avsnittet **Inställningar**: </span>

      1. <span class="preview">Välj ett fält i listrutan. Detta är fält som är associerade med den posttyp du valde.</span>
      1. <span class="preview">Fortsätt att definiera villkor för det markerade fältet.</span>
      1. <span class="preview">Klicka på **Lägg till villkor** om du vill lägga till upp till 5 fält och definiera deras villkor.</span>

         <span class="preview">Du kan lägga till följande typer av fält:</span>

         <div class="preview">

         * Enkelval
         * Flera val
         * Enkelradig text
         * Stycke
         * Nummer
         * Kryssruta
         * Datum

         </div>

         <span class="preview">Workfront Planning skapar objekt automatiskt när villkoren uppfylls. </span>

         ![Utlösaren för ändring av fältvärde har valts](assets/field-value-change-trigger-selected.png)

         >[!TIP]
         >
         ><span class="preview">Modifieraren i varje villkor ändras med den typ av fält som du väljer.</span>

1. Uppdatera följande fält i avsnittet **Åtgärder**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Åtgärder**: Välj den åtgärd som du vill att Workfront ska utföra när automatiseringen aktiveras. Detta är ett obligatoriskt fält.
Välj någon av följande åtgärder:

      * Skapa flera projekt
      * Skapa ett projekt
      * Skapa projekt
      * Skapa post
      * Skapa program
      * Skapa portfölj
      * Skapa grupp

     >[!TIP]
     >
     >När du har sparat automatiseringen kan du inte längre ändra åtgärden som är vald i det här fältet.

1. (Villkorligt) Beroende på vilken åtgärd du valde kan du uppdatera följande fält:

   * **Skapa ett enskilt projekt**: <!--replace to the left: Create a single project-->
      * **Anslutet fält där projektet skapas**: Det här är det anslutna fältet som det nya projektet ska visas i. Detta är ett obligatoriskt fält.
      * **Projektmall**: Välj en projektmall som Workfront ska använda för att skapa projektet.

   * Skapa flera projekt:
      * **Anslutet fält där projektet skapas**: Det här är det anslutna fältet som det nya projektet ska visas i. Detta är ett obligatoriskt fält.
      * **Fält vars val skapar posterna**: Välj ett fält med flera eller enstaka val från den valda posttypen. Workfront skapar ett projekt för varje fältval som är markerat på den post från vilken du utlöser automatiseringen.

     >[!TIP]
     >
     >Ett projekt skapas bara för de alternativ som är markerade i flervalsfältet eller envalsfältet i den post som du kör automatiseringen från, och inte för alla möjliga val för det fältet.
     >

      * **Använd samma mall**: Välj det här alternativet om du vill använda samma mall för varje nytt projekt. Om alternativet är avmarkerat väljer du en **projektmall** för varje fältval.
      * **Projektmall**: Om du valde alternativet **Använd samma mall** väljer du en projektmall som Workfront ska använda för att skapa projekten.

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
