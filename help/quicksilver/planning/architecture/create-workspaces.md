---
title: Skapa arbetsytor
description: En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning. Posttyperna är ordnade efter avsnitt på en arbetsyta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 10d2bcf3f2d349418a8a04e96873bc5c2d3af4a1
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 0%

---


# Skapa arbetsytor

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

I Adobe Workfront Planning är arbetsytorna centraliserade platser där team kan planera arbetet.

En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning.

Allmän information om arbetsytor finns i [Översikt över arbetsytor](/help/quicksilver/planning/architecture/workspaces-overview.md).

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
<p>Alla Workfront- eller Workflow-paket</p> 
<p>Alla Workfront Planning-paket</p>
<p>Ett Workfront Planning Prime-paket eller ett högre paket <span class="preview"> som kan användas för att skapa flera arbetsytor samtidigt</span></p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   <p><span class="preview">Systemadministratör kan skapa flera arbetsytor samtidigt med mallpaketet med bästa praxis</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta</p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:

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
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Skapa en arbetsyta

Du kan skapa en arbetsyta och lägga till posttyper för att ordna dina objekt i Workfront Planning.

Mer information om hur du redigerar en arbetsyta finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).

Du kan skapa arbetsytor på följande sätt:

* Skapa en arbetsyta från grunden eller från en mall

  Mer information finns i avsnittet [Skapa en arbetsyta från grunden eller från en mall](#create-a-workspace-from-scratch-or-from-a-template) i den här artikeln.
* Skapa en arbetsyta med AI-driven Planning Designer. Den här funktionen är för närvarande endast tillgänglig för ett begränsat antal kunder i ett Beta-program.

  Mer information finns i [Kom igång med Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

<div class="preview">

* Skapa flera arbetsytor med ett standardpaket med flera arbetsytor

  Mer information finns i avsnittet [Skapa flera arbetsytor med ett mallpaket för flera arbetsytor ](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) i den här artikeln

</div>

### Skapa en arbetsyta från grunden eller från en mall

{{step1-to-planning}}

1. Klicka på **Skapa arbetsyta**

   Rutan Skapa arbetsyta visas. Du kan skapa en arbetsyta från grunden eller skapa den med någon av de tillgängliga mallarna.

1. (Valfritt och villkorligt) Klicka på **Förhandsgranska** i någon av följande fördefinierade arbetsytemallar:

   * Grundläggande: Marknadsföringshantering
   * Avancerat: Marknadsföringshantering
   * Enterprise: Marketing Management
   * Försäljningshantering
   * Produkthantering

   Förhandsvisningsrutan för mallen öppnas.

   Det finns en indikation på vilka operativa posttyper, taxonomier och hur många fält som är associerade med varje mall.

   ![Förhandsgranska en arbetsytemall](assets/previewing-a-workspace-template.png)

   Mer information om mallar för arbetsytan i Workfront Planning finns i [Lista över arbetsytemallar](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Klicka på **Använd mall** i förhandsgranskningsrutan för mallen för att börja skapa arbetsytan från den valda mallen

   eller

   Klicka på **Bakåt** och sedan på **Ny arbetsyta** för att skapa en helt ny arbetsyta.

   En av följande typer av arbetsytor skapas:

   * En tom arbetsyta med namnet **Namnlös Workspace** där du kan börja lägga till posttyper manuellt när du skapar en arbetsyta från grunden.
   * En arbetsyta som namnges efter mallen som du valde och som fylls med exempelposttyper. Du kan anpassa posttyperna och arbetsytan ytterligare.

   För Workfront-administratörer visas den nya arbetsytan på fliken **Arbetsytor som jag är på**.

   För alla andra användare som kan skapa arbetsytor visas den nya arbetsytan i området **Arbetsytor**.

1. Klicka i namnet på arbetsytan i sidhuvudet på den nya arbetsytan för att byta namn på den och tryck sedan på Retur.

1. (Valfritt och villkorligt) Om du har skapat arbetsytan från en mall klickar du inuti namnet på **driftposttyperna** eller **taxonomierna** .

   eller

   Håll namnet på ett avsnitt, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Byt namn** för att byta namn på avsnittet.

   >[!TIP]
   >
   >Du kan byta namn på alla avsnitt på en arbetsyta, även om du inte har skapat avsnittet.

   Mer information om hur du redigerar arbetsytor, inklusive redigering av arbetsytor, finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Valfritt) Klicka på **Lägg till posttyp** om du vill lägga till posttyper på arbetsytan i valfritt avsnitt.

   Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Mer information om hur du redigerar och tar bort posttyper på en arbetsyta finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Valfritt) Klicka på bakåtpilen till vänster om den nya arbetsytan för att öppna huvudsidan Planering. Ett nytt arbetsytekort skapas för den nya arbetsytan på fliken **Arbetsytor som jag arbetar med**.

   Namnet på den användare som skapade arbetsytan sparas på arbetsytans kort som ägare.

   >[!NOTE]
   >
   >För användare som för närvarande går över till Adobe Identity Management System (IMS) visas arbetsytor som skapats av användare med endast Workfront som inte är IMS-användare som skapats av **System**.
   >
   >Mer information om IMS finns i [Adobe Unified Experience för Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

<div class="preview">

### Skapa flera arbetsytor med ett standardpaket med flera arbetsytor

>[!IMPORTANT]
>
>Att skapa flera arbetsytor samtidigt med mallpaketet för de bästa metoderna är bara tillgängligt när följande förutsättningar är uppfyllda:
>
>* Din organisation har köpt ett Workfront Planning Prime- eller Ultimate-paket.
>* Du är systemadministratör

Du kan använda ett mallpaket för flera arbetsytor för att skapa sex arbetsytor med ett enda klick.

Mallarna som ingår i paketet innehåller arbetsytor, posttyper, poster, vyer och fält som hjälper dig att komma igång med din planeringsimplementering.

>[!IMPORTANT]
>
>Alla namn på arbetsytor, posttyper, fält och poster som ingår i paketet är exempel och är inte en spegling av din egen miljö.
>
>Vi rekommenderar att du använder det här mallpaketet som exempel på en planeringsstruktur och fortsätter med att skapa objekt som återspeglar organisationens arbetsflöde.

{{step1-to-planning}}

1. Klicka på **Skapa arbetsyta**

   Rutan Skapa arbetsyta visas. Du kan skapa en arbetsyta från grunden eller skapa den med någon av de tillgängliga mallarna.

1. Klicka på **Konfiguration av arbetsyta för granskning** i området **Börja här (rekommenderas)**.
1. (Valfritt) Klicka på **Förhandsgranska** i någon av följande fördefinierade arbetsytemallar för att öppna rutan Förhandsgranska för varje mall:

   * &#x200B;1. Globala klassificeringar och taxonomier

     Mallen Globala klassificeringar och taxonomier innehåller alla posttyper och fält som vi rekommenderar att du skapar i din miljö för en lyckad implementering av Workfront Planning.

     Du kan senare länka eller importera posttyperna i den här mallen i andra arbetsytor som du skapar.
   * 2.Fréscopa Global Marketing
   * 3.Fréscopa Social Marketing
   * 4.Fréscopa Media och PR
   * 5.Fréscopa Global Events
   * 6.Fréscopa Executive Company Leadership

1. När du har öppnat rutan **Förhandsgranska** för varje arbetsytemall klickar du på Tillbaka för att gå tillbaka till rutan **Skapa arbetsyta** eller på Använd mallar för att använda mallarna inklusive i paketet och skapa arbetsytor.

   Arbetsytorna skapas och visas på flikarna **Arbetsytor som jag är** på och **Alla arbetsytor** för systemadministratörer. Alla användare med standardlicens kan se arbetsytorna i sin arbetsyta efter att en systemadministratör har skapat dem och delat de nya arbetsytorna med dem.

1. Börja redigera arbetsytorna som du har skapat och lägg till posttyper, poster, vyer och fält som är relevanta för din organisation.

   Mer information om de bästa sätten att implementera Workfront finns i artiklarna i avsnittet [Bästa praxis för Adobe Workfront-planering: artikelindex](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).

   Mer information om hur du redigerar arbetsytor finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).

</div>



