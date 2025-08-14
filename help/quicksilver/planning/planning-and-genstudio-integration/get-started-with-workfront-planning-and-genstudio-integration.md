---
title: Kom igång med Workfront Planning och GenStudio for Performance Marketing Integration
description: GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna. Lär dig grunderna om hur du kan effektivisera dina arbetsflöden med den här integreringen.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 0%

---

# Kom igång med integreringen mellan Adobe Workfront Planning och Adobe GenStudio for Performance Marketing

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

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

Organisationer som använder både Adobe Workfront Planning och Adobe GenStudio for Performance Marketing definierar ofta mer detaljerade marknadsföringskoncept som kampanjer, produkter och profiler än vad GenStudio stöder som standard.

Det finns en inbyggd integrering mellan GenStudio for Performance Marketing och Workfront Planning. Tack vare den här integreringen kan användare i Workfront Planning hantera de kampanjer, produkter, profiler, aktiveringar, kanaler och regioner som används i GenStudio. De kan också konfigurera GenStudio att referera till befintliga posttyper från Workfront Planning, vilket skapar ett mer uppkopplat och enhetligt marknadsföringsarbetsflöde.

Denna integrering hjälper er att undvika att data läggs in flera gånger, upprätthålla en jämn fördelning mellan planerings- och aktiveringssatsningarna och stöder ert marknadssystem.

GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna.

Tack vare integrationen mellan Workfront Planning och GenStudio for Performance Marketing kan du

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Visa arbetsytan i GenStudio i Workfront Planning.
* Ändra era kampanjer i GenStudio och få samma information i realtid i Workfront Planning.
* Ändra kampanjerna i Workfront Planning och få uppdateringar i realtid av samma information i GenStudio.

## Integrationskrav

* Workfront och GenStudio for Performance Marketing måste aktiveras för samma organisation.

  Mer information om GenStudio finns i [Adobe GenStudio for Performance Marketing användarhandbok](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).

* GenStudio kommer inte att vara tillgängligt i Workfront Planning när ditt företag har flera instanser av Workfront. <!--this will change-->

* Instansen Workfront ingår i Adobe Unified Experience, inklusive användning av Identity Management System (IMS).

  Mer information finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Användare som använder både Planning och GenStudio kan bara tillhöra en Workfront-instans inom IMS-organisationen.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Åtkomstkrav

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
   <li><p> Adobe GenStudio for Performance Marketing</p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla Workfront Workflow-paket</p>  
<p>Alla Workfront Planning-paket</p>
   </td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio package</p></td> 
   <td> 
<p>??</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p> Systemadministratör</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio-licens</p></td> 
   <td><p> ??</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>  
   <p>Konfiguration för GenStudio: ???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  
   <p>I Workfront Planning: </p>
   <ul>
   <li><p>Contribute eller högre behörighet för en arbetsyta och en posttyp  </p> </li> 
   <li><p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p></li>
   </ul>
   <p>I Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Alla behörigheter i Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Skapa behörigheter i Adobe GenStudio for Performance Marketing för att skapa objekt</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Mer information om Adobe GenStudio for Performance Marketing finns i [Adobe GenStudio for Performance Marketing användarhandbok](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).


## Översikt över integrationen mellan Workfront Planning och GenStudio

I följande avsnitt beskrivs följande:

* Funktioner för att uppdatera Workfront Planning-information från GenStudio
* Funktioner för att uppdatera GenStudio-information från Workfront Planning
* Begränsningar för vad du kan och inte kan hantera på en GenStudio-arbetsyta från Workfront Planning.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### GenStudio arbetsyta i Workfront Planning

* Om din organisation har flera Workfront-instanser visas inte GenStudio-arbetsytan från någon av dina Workfront-instanser. <!-- this might change-->
* På arbetsytan i GenStudio visas en visuell indikator som tydligt anger att den importeras från GenStudio. Mer information finns i [Hantera GenStudio-arbetsytan i Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Alla användare som har tillgång till både GenStudio och Workfront Planning kan även se arbetsytan GenStudio i Workfront Planning.
* Workfront Planning-användare måste hanteras via Adobe Identity Management System (IMS) för att kunna visa och använda GenStudio arbetsyta från Workfront.

  Användare som bara har Workfront kan inte se arbetsytan i GenStudio, även när den är tillgänglig i Workfront.

  Mer information finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


### Posttyper

* Du kan redigera posttypsinformation (till exempel deras utseende) från GenStudio i Workfront Planning.
* Du kan dela posttyper från GenStudio med andra i Planning.
* Du kan skapa posttyper från Planering på arbetsytan i GenStudio. De här posttyperna finns bara kvar i Planning. De visas inte i GenStudio.
* Posttyper som synkroniseras med GenStudio visar en visuell indikator i Workfront Planning som visar att posttyperna importeras från GenStudio.

### Poster

* Du kan lägga till eller ta bort poster i GenStudio och de blir synliga i (eller tas bort från) Workfront Planning.
* Du kan lägga till eller ta bort poster i Workfront Planning och de blir synliga i (eller tas bort från) GenStudio.
* När du tar bort poster från antingen Workfront Planning eller GenStudio placeras de i behållaren Senast borttagna i 30 dagar. GenStudio har ingen nyligen borttagen behållare.
* När du återställer en post från den nyligen borttagna behållaren återställs den i Workfront Planning och GenStudio.
* Du kan lägga till poster från Workfront Planning på följande sätt:

   * Manuellt, från scratch, från alla vyer med knappen Ny post
   * Importera dem med en CSV- eller Excel-fil
   * Manuellt, textbundet, i tabellvyn
   * Manuellt, direkt i tidslinjevyn

  Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* Du kan inte skapa eller ta bort aktiveringsposter från Workfront Planning.
* Du kan redigera postinformation på alla poster i GenStudio arbetsyta i Planning i något av de synliga fälten i Workfront Planning.

  Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Fält

* Postfält importeras från GenStudio. Du kan redigera fältinställningarna i Workfront Planning.
* Du kan skapa fält för posttyper i GenStudio i Workfront Planning om du har behörigheten Hantera i Gen Studio.
* När du skapar fält för GenStudio-posttyper i Planning visas de i följande områden:
   * Planeringsvyer
   * Sidor med information om planeringsposter
   * GenStudio postinformationssidor

  >[!TIP]
  >
  >Fält som skapas i Workfront Planning visas inte i listvyn i GenStudio.

* Du kan dölja fält i tabellvyn för en GenStudio-posttyp i Planning.
* Du kan inte ta bort fält som importerats från GenStudio från Workfront Planning.
* Du kan ta bort fält som har skapats i Workfront Planning för GenStudio-posttyper från Workfront Planning.


### Fälten Skapad av och Godkänd av

* Du kan lägga till fälten Skapad av och Godkänd av för posttyperna GenStudio i Workfront Planning från Workfront Planning.
* Posterna som visas i posttyperna Kanal och Region visar &quot;System&quot; som Skapat av användaren. Posterna skapas automatiskt när arbetsytan i GenStudio skapas i Workfront Planning.
* Poster som skapas i GenStudio efter att arbetsytan gjorts tillgänglig i Workfront Planning visar namnet på den IMS-användare som skapade posten i fältet Skapad av, även om användaren skapade posterna i GenStudio och inte är en Workfront-användare.
* Fältet Godkänd av visar namnet på godkännaren när ett begärandeformulär skickas för att skapa en post.

### Vyer

* Du kan skapa vyer för posttyper i GenStudio.

  Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

* Du kan dela vyn av en posttyp i GenStudio när du delar en vy för posttypen Planning.
* Du kan inte skapa flera vyer i GenStudio.

### Anslutningar

* Du kan göra följande anslutningar mellan posttyperna i GenStudio och andra post- eller objekttyper i Workfront Planning:

   * Två GenStudio-posttyper
   * En posttyp för GenStudio och en posttyp för Planning från samma arbetsyta
   * En posttyp i GenStudio och en posttyp för planering från en annan arbetsyta, om posttyperna har konfigurerats för att ansluta från en annan arbetsyta.
   * En posttyp i GenStudio och en objekttyp i Workfront (projekt, portföljer, program, företag, grupper)
   * En posttyp för GenStudio och en objekttyp för AEM Assets.

### Begär blanketter och automatisering

* Du kan lägga till förfrågningsformulär och automatiseringar till en GenStudio-posttyp i Workfront Planning.

### Förhandsvisningsmiljön

* Den GenStudio-arbetsyta som du kommer åt från din produktionsmiljö visas också i förhandsvisningsmiljön.
* Du kan utföra alla aktiviteter som beskrivs i den här artikeln på GenStudio-arbetsytan i Workfront Planning i förhandsvisningsmiljön, men dessa ändringar överförs inte till GenStudio.
Endast ändringar du gör i objekt i produktionsmiljön synkroniseras mellan Workfront Planning och GenStudio.
GenStudio har ingen förhandsvisningsmiljö.

