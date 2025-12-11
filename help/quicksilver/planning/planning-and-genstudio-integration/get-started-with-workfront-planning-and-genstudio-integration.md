---
title: Kom igång med Workfront Planning och GenStudio for Performance Marketing Integration
description: GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna. Lär dig grunderna om hur du kan effektivisera dina arbetsflöden med den här integreringen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: ca16652aa06b4652d0d1b41156ed1ef96225c49a
workflow-type: tm+mt
source-wordcount: '2170'
ht-degree: 0%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Kom igång med integreringen mellan Adobe Workfront Planning och Adobe GenStudio for Performance Marketing

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Organisationer som använder både Adobe Workfront Planning och Adobe GenStudio for Performance Marketing definierar ofta mer detaljerade marknadsföringskoncept som kampanjer, produkter, aktiveringar och personligheter än vad GenStudio stöder som standard.

Det finns en inbyggd integrering mellan GenStudio for Performance Marketing och Workfront Planning. Tack vare den här integreringen kan användare i Workfront Planning hantera de kampanjer, produkter, profiler, aktiveringar, kanaler och regioner som används i GenStudio. De kan också konfigurera GenStudio att referera till befintliga posttyper från Workfront Planning, vilket skapar ett mer uppkopplat och enhetligt marknadsföringsarbetsflöde.

GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna.

## Integreringsfördelar

Tack vare integrationen mellan Workfront Planning och GenStudio for Performance Marketing kan du

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Visa arbetsytan i GenStudio i Workfront Planning.
* Modifiera kampanjer, produkter, profiler och aktiveringar i GenStudio for Performance Marketing och få uppdateringar i realtid av samma information i Workfront Planning.
* Modifiera kampanjer, produkter, profiler och aktiveringar i Workfront Planning och få uppdateringar i realtid av samma information i GenStudio for Performance Marketing.
* Undvik dubblettinmatning.
* Bibehåll enhetligheten i planeringen och aktiveringen.
* Koppla GenStudio Brands och deras information till Workfront Planning records.

## Integrationskrav

Din organisation måste uppfylla följande krav för att integreringen mellan Workfront Planning och GenStudio for Performance Marketing ska finnas:

* Workfront och GenStudio for Performance Marketing måste aktiveras för samma organisation.

  Mer information om GenStudio finns i [Adobe GenStudio for Performance Marketing användarhandbok](https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/home).

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Din Workfront-instans ingår i Adobe Unified Experience, inklusive användning av Identity Management System (IMS).

  Mer information finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Användare som använder både Workfront Planning och GenStudio for Performance Marketing får bara tillhöra en Workfront-instans inom IMS-organisationen.

  Användare som bara har Workfront kan visa arbetsytan i GenStudio, även om de inte är GenStudio for Performance Marketing-användare.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Åtkomstkrav

I följande tabell beskrivs behörighets- och behörighetskraven för att använda Adobe Workfront Planning med Adobe GenStudio for Performance Marketing:

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
<td> 
   <p> Ytterligare produkter</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing användarroller</p></td> 
   <td><p><ul><li>Alla GenStudio användarroller för att få tillgång till kampanjer, produkter och uppgifter</li>
   <li>GenSudio System Manager för att komma åt aktiveringar <!--and Events--></li></ul>
   Mer information finns i <a href="https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Användarroller och behörigheter</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  
   <p>I Workfront Planning: </p>
   <ul>
   <li><p>Hantera behörigheter på arbetsytan i GenStudio för att lägga till nya fält eller posttyper på arbetsytan i GenStudio</p></li>
   <li><p>Contribute-behörigheter på arbetsytan i GenStudio för att lägga till, uppdatera eller ta bort poster på arbetsytan i GenStudio</p> </li>  
   </ul>
   <p>Inga användare kan ta bort posttyper eller fält från GenStudio for Performance Marketing från GenStudio arbetsyta i Workfront Planning</p>
   <p>I Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Alla behörigheter i Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Skapa behörigheter i Adobe GenStudio for Performance Marketing för att skapa objekt</p></li></ul>
   </td>  
</tbody> 
</table>

Mer information om åtkomst till Adobe Workfront Planning finns i [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Mer information om Adobe GenStudio for Performance Marketing finns i [Adobe GenStudio for Performance Marketing användarhandbok](https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/home).

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****and Events****</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Översikt över integrationsfunktionerna i Workfront Planning och GenStudio for Performance Marketing

Beroende på hur många Workfront-instanser din organisation har, har du automatiskt följande behörigheter till arbetsytan i GenStudio under Planning:

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>En instans av Workfront</p></td> 
   <td> 
<p>Arbetsytan i GenStudio visas i din instans av Workfront Planning</p>
<p>Alla användare, inklusive Workfront-administratörer, har som standard Contribute-åtkomst till GenStudio arbetsyta i Planning</p>
<p>Workfront-administratörer kan ändra och bevilja behörigheten Hantera på arbetsytan i GenStudio till vem som helst</p>
</td> </tr>
   <tr> 
<td> 
   <p> Flera instanser av Workfront</p> </td> 
   <td> 
   <p>Här följer exempel på när din organisation har mer än en instans av Workfront med Workfront Planning:</p>
   <ul><li>Om ditt företag har flera instanser av Workfront samtidigt som de köper Adobe GenStudio for Performance Marketing visas GenStudio-arbetsytan från alla Workfront-instanser.</li>
   <li>Om ditt företag lägger till fler Workfront-instanser efter att deras ursprungliga instans redan har integrerats med Adobe GenStudio for Performance Marketing, visas arbetsytan i GenStudio endast från den ursprungliga Workfront-instansen. Kontakta din kontorepresentant om du vill ha information om hur du ansluter ytterligare instanser av Workfront till Adobe GenStudio. </li></ul>    
</td> 
  </tr>
   </tbody> 
</table>

<!--Old for the second row in the table:

<p>The GenStudio workspace is visible from all Workfront instances</p>
<p>All users with access to GenStudio for Performance Marketing and Workfront Planning have Contribute permissions on the GenStudio in Planning by default</p> 
<p>Workfront administrators cannot grant Manage permissions to the GenStudio workspace to anyone</p>-->

Mer information om Workfront Planning-behörigheter finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Avsnitten nedan beskriver följande:

* Funktioner för att uppdatera Workfront Planning-information från GenStudio for Performance Marketing
* Funktioner för att uppdatera GenStudio for Performance Marketing-information från Workfront Planning
* Begränsningar för vad du kan och inte kan hantera på en GenStudio-arbetsyta från Workfront Planning.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### GenStudio arbetsyta i Workfront Planning

* På arbetsytan i GenStudio visas en visuell indikator i Workfront Planning som anger att den representerar arbetsytan i GenStudio for Performance Marketing.

  ![GenStudio-kort i Planning](assets/genstudio-card-with-tag-highlighted.png)

  Mer information finns i [Hantera GenStudio-arbetsytan i Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* GenStudio-arbetsytan delas automatiskt med alla GenStudio-användare som också har tillgång till Workfront när den skapas i Workfront Planning.
* Som arbetsytehanterare för GenStudio arbetsyta i Planning kan du:

   * Uppdatera GenStudio-arbetsytan i Planning (namn, beskrivning, ikon)
   * Skapa avsnitt
   * Lägg till posttyper
   * Dela det med andra

     >[!NOTE]
     >
     >* Du kan dela arbetsytan i GenStudio med andra som inte har något GenStudio-konto. Du kan bara dela den med användare som är tillgängliga i Identity Management System (IMS) i din organisation.
     >* Du kan inte ta bort GenStudio-användare från GenStudio arbetsyta eller dela med dess posttyper.

  <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Om du har Contribute-behörighet till arbetsytan i GenStudio under Planning kan du inte ändra arbetsytan i Workfront Planning.

### Posttyper på arbetsytan i GenStudio

* Posttyper som visas både i GenStudio for Performance Marketing och Planning har en GenStudio-indikator i Workfront Planning.

  ![GenStudio-posttypkort i Workfront Planning](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Posttyper på arbetsytan i GenStudio delas automatiskt med alla GenStudio-användare som också har tillgång till Workfront när arbetsytan skapas i Planning.
* När du har behörighet att hantera arbetsytan i GenStudio i Planning kan du göra följande från Workfront Planning:
   * Redigera information om posttyper i GenStudio (deras utseende, avancerade inställningar).
   * Dela GenStudio-posttyper med andra. Du kan inte ta bort GenStudio-användare från delning av GenStudio posttyper.
   * Skapa posttyper. Dessa posttyper finns bara kvar i Workfront Planning. De visas inte i GenStudio.
   * Aktivera posttyper från GenStudio-arbetsytan för att ansluta från andra arbetsytor.
   * Aktivera att posttyper från GenStudio-arbetsytan läggs till i andra arbetsytor.
* När du har Contribute-behörighet till GenStudio arbetsyta i Planning går det inte att ändra posttyperna i GenStudio från Planning.

### Poster på arbetsytan i GenStudio

* Alla GenStudio-poster delas automatiskt med alla GenStudio-användare som också har tillgång till Workfront när arbetsytan skapas i Planning.
* När du redigerar GenStudio-poster från GenStudio for Performance Marketing visas ändringarna på arbetsytan i GenStudio i alla instanser av Workfront.
* Du kan inte skapa eller ta bort aktiveringsposter från GenStudio-arbetsytan i Workfront Planning.
* När du har behörigheten Hantera eller Contribute för GenStudio arbetsyta i Planning kan du göra följande från Workfront Planning:
   * Lägg till eller ta bort poster så visas de i (eller tas bort från) GenStudio for Performance Marketing.

     Borttagna poster från antingen Workfront Planning eller GenStudio for Performance Marketing placeras i Workfront Planning Recent deleted-behållaren i 30 dagar. GenStudio for Performance Marketing har ingen nyligen borttagen behållare.
   * Återställ en post från papperskorgen som tagits bort nyligen. När du återställer borttagna poster återställs de i Workfront Planning och GenStudio for Performance Marketing.
   * Lägg till poster på följande sätt:

      * Manuellt, från scratch, från alla vyer med knappen Ny post
      * Genom att importera dem via en CSV- eller Excel-fil i tabellvyn
      * Manuellt, i valfri vy i Workfront Planning
      * Genom att skicka en begäran till ett formulär för posttypsbegäran i Workfront.

  Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* Du kan redigera postinformation för alla poster på arbetsytan i GenStudio från Workfront Planning.

  Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

### Posttypsfält på arbetsytan i GenStudio

Posttypsfält importeras som standard från GenStudio for Performance Marketing till Workfront Planning.

Tänk på följande när det gäller posttypsfält i GenStudio:

* När du har behörighet att hantera arbetsytan i GenStudio i Planning kan du göra följande från Workfront Planning:

   * Redigera fältinställningar för GenStudio.
   * Skapa fält för posttyper i GenStudio.

     När du skapar fält för GenStudio-posttyper i Planning visas de i följande områden:

      * Workfront Planeringsvyer
      * Workfront Planering - postinformationssidor
      * GenStudio postinformationssidor

     >[!TIP]
     >
     >Fält som skapas i Workfront Planning visas inte i GenStudio-listor.

   * Dölj fält i tabellvyn för en GenStudio-posttyp i Workfront Planning.
   * Du kan inte ta bort fält som har skapats i GenStudio från Workfront Planning.

* När du har Contribute-behörighet till arbetsytan i GenStudio under Planning:

   * Du kan inte redigera fältinställningar, ta bort eller lägga till fält från GenStudio-arbetsytan i Workfront Planning.
   * Du kan dölja fält från tabellvyn i Workfront Planning.

#### Fälten Skapad av och Godkänd av

* Du kan lägga till fälten Skapad av och Godkänd av för posttyperna GenStudio i Workfront Planning från Workfront Planning.
* Posterna som visas i posttyperna Kanal och Region visar &quot;System&quot; som Skapat av användaren. Posterna skapas automatiskt när arbetsytan i GenStudio skapas i Workfront Planning.
* Poster som skapas i GenStudio efter att arbetsytan gjorts tillgänglig i Workfront Planning visar namnet på den IMS-användare som skapade posten i fältet Skapad av, även om användaren skapade posterna i GenStudio och inte är en Workfront-användare.
* Fältet Godkänd av visar namnet på godkännaren när ett begärandeformulär skickas för att skapa en post i posttypen GenStudio i Workfront Planning.
* Fälten Skapad av och Godkänd av visas i postens information i GenStudio for Performance Marketing. De visas inte i listvyn.

### Spela in vyer på arbetsytan i GenStudio

>[!NOTE]
>
>Posttyperna i GenStudio visas i standardtabellvyn som importeras från listvyn i GenStudio for Performance Marketing.
>
>Du kan inte ta bort den ursprungliga tabellvyn som importerades som standard från GenStudio for Performance Marketing.

* Du kan inte skapa flera vyer i GenStudio for Performance Marketing.

* När du har behörighet att hantera arbetsytan i GenStudio i Planning kan du göra följande från Workfront Planning:

   * Skapa vyer för posttyper i GenStudio.

     Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   * Byt namn på, dela, exportera, duplicera eller ta bort anpassade vyer från posttyperna i GenStudio.

* När du har Contribute-behörighet till GenStudio arbetsyta i Planning kan du göra följande från Workfront Planning:

   * Skapa vyer för posttyper i GenStudio.

     Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   * Byt namn på, exportera, duplicera eller ta bort anpassade vyer från posttyperna i GenStudio.

     Du kan inte dela vyer från GenStudio-arbetsytan i Workfront Planning

### Spela in anslutningar på arbetsytan i GenStudio

Du kan skapa anslutningar mellan posttyper i GenStudio arbetsytor där du har behörigheten Hantera.

Du kan göra följande anslutningar mellan posttyperna i GenStudio och andra post- eller objekttyper i Workfront Planning:

* Två GenStudio-posttyper
* En posttyp för GenStudio och en posttyp för Planning från samma arbetsyta
* En posttyp i GenStudio och en posttyp för planering från en annan arbetsyta, om posttyperna har konfigurerats för att ansluta från en annan arbetsyta.
* En posttyp i GenStudio och en objekttyp i Workfront (projekt, portföljer, program, företag, grupper)
* En posttyp för GenStudio och en objekttyp för AEM Assets.
* GenStudio posttyper och GenStudio Brands. Varumärkesanslutningen läggs till som standard i posttyperna Produkter och Personas.

### Begär blanketter och automatisering i GenStudio posttyp

* Du kan lägga till förfrågningsformulär till en GenStudio-posttyp i Workfront Planning.

  Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Du kan konfigurera automatisering för en posttyp i GenStudio i Workfront Planning.

  Mer information finns i [Konfigurera Adobe Workfront Planning Automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Connection to GenStudio Brands from Workfront Planning workspaces

När organisationen har en integrering mellan Workfront Planning och Adobe GenStudio kan du koppla posttyperna Planning till GenStudio Brands från vilken posttyp som helst på arbetsytan i Workfront Planning.

Varumärken är som standard anslutna till följande posttyper för arbetsytan i GenStudio:

* Produkter
* Personas

Varumärkena är tillgängliga för manuell anslutning till alla andra posttyper för arbetsytan i GenStudio, eller posttyper från alla andra arbetsytor som du har behörighet att hantera.

## Förhandsvisningsmiljön

* Den GenStudio-arbetsyta som du kommer åt från din produktionsmiljö visas också i förhandsvisningsmiljön för samma Workfront-instans.
* Du kan utföra alla aktiviteter som beskrivs i den här artikeln på GenStudio-arbetsytan i Workfront Planning i förhandsvisningsmiljön, men dessa ändringar visas inte i GenStudio.

  Endast ändringar du gör i objekt i produktionsmiljön synkroniseras mellan Workfront Planning och GenStudio.

  GenStudio har ingen förhandsvisningsmiljö.

