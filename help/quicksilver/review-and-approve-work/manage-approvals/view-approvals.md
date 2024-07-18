---
product-area: projects
navigation-topic: approvals
title: Visa godkännanden
description: Godkännandeprocesser ger flexibilitet att skapa godkännanden i flera steg för projekt, uppgifter och ärenden. Adobe Workfront administratörer definierar godkännandeprocesser för att skapa enhetlighet i hela systemet.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Visa godkännanden

Godkännandeprocesser ger flexibilitet att skapa godkännanden i flera steg för projekt, uppgifter och ärenden. Adobe Workfront administratörer definierar godkännandeprocesser för att skapa enhetlighet i hela systemet.

Mer information om hur du skapar godkännandeprocesser finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Mer information om hur du associerar godkännanden med arbete i Workfront finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till objekt som är kopplade till godkännanden</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för objekt som är associerade med godkännanden</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Hitta godkännanden i Adobe Workfront

Du kan visa eller hantera godkännanden från flera områden i Workfront. Mer information om hur du hanterar godkännanden inom olika områden finns i [Godkänna arbete](../../review-and-approve-work/manage-approvals/approving-work.md).

Du kan visa eller hantera godkännanden från följande områden:

* I hemområdet

   * Alla projekt, uppgifter, utgåvor, tidrapporter, dokument och åtkomst som väntar på ditt godkännande visas i Hem-området när du väljer att visa alla eller godkännanden.
   * Godkännanden som du själv har skickat visas även i Hem, i avsnittet Godkännanden som jag har skickat i arbetslistan. Mer information finns i avsnittet [Granskningsarbete som du skickar in för godkännande i hemområdet](#review-work-you-submit-for-approval-in-the-home-area) i den här artikeln.
   * Godkännanden tas bort från Hem-området när det associerade projektet, aktiviteten eller utgåvan har markerats som Löst, Spärrat, Stängt eller Avbrutet.

  Mer information om att använda Hem finns i [Kom igång med Hem](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* I huvudet på ett projekt, en uppgift, en utgåva, ett dokument eller ett korrektur
* I avsnittet Godkännanden för ett projekt, en uppgift eller ett ärende
* I en rapport

  >[!NOTE]
  >
  >Du kan inte fatta ett beslut om ett godkännande från en rapport.

  Du kan skapa en rapport för projekt, uppgifter, utgåvor eller dokumentgodkännande som innehåller godkännandeinformation.

  Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Granska material som du skickar in för godkännande på Hem-sidan {#review-work-you-submit-for-approval-in-the-home-area}

1. Klicka på ikonen **Hem** ![](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmenyn** ![](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Välj **Arbetslista**, klicka på listrutan **Filter** och välj **Godkännanden**.
1. Expandera avsnittet **Godkännanden som jag har skickat** och hitta de godkännanden som du har skickat.

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## Visa godkännandestatus för ett objekt

Du kan visa godkännandestatusen för ett objekt i följande avsnitt av objektet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Uppdateringar </td> 
   <td> <p>Visar alla godkännandestatusar när de inträffar. Godkännandestatus visas i linje med andra statusvärden som visas i avsnittet <strong>Uppdateringar</strong> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Godkännanden</td> 
   <td> <p>Visar mer detaljerad information om godkännandeprocessen, t.ex. varje steg i godkännandeprocessen och om godkännarna har beviljat godkännandet.</p> </td> 
  </tr> 
 </tbody> 
</table>

* [Använd uppdateringsområdet för att visa godkännandestatus](#use-the-updates-area-to-view-an-approval-status)
* [Använd området Godkännanden för att visa godkännandestatus](#use-the-approvals-area-to-view-an-approval-status)

### Använd uppdateringsområdet för att visa godkännandestatus {#use-the-updates-area-to-view-an-approval-status}

När ett godkännande initieras för ett projekt, en aktivitet eller ett problem visas en status på fliken **Uppdateringar** för objektet, vilket anger godkännandestatusen. En ny status visas när objektet övergår genom godkännandeprocessen. Detta inkluderar följande händelser:

* En godkännandeprocess initieras för ett objekt. Godkännandeprocessen initieras när statusen ändras.
* Objektet har avvisats
* Objektet har godkänts 

>[!TIP]
>
>Om ett godkännande används för en uppgift visas godkännandeuppdateringarna på fliken Uppdateringar för uppgiften, inte på fliken Uppdateringar i projektet där uppgiften finns.

### Använd området Godkännanden för att visa godkännandestatus {#use-the-approvals-area-to-view-an-approval-status}

Du kan se var en uppgift eller ett problem som du arbetar med just nu befinner sig i godkännandeprocessen. Du kan se följande information:

* Godkännandeprocessens fas
* Vilka godkännare har redan godkänt det
* Vilka godkännare har ännu inte godkänt det

Så här ser du det aktuella läget för var en uppgift eller en utgåva befinner sig i godkännandeprocessen:

1. Gå till projektet, aktiviteten eller utgåvan som godkännandet är kopplat till.
1. Klicka på **Godkännanden** i den vänstra panelen. Du kan behöva klicka först på **Visa mer**.

   På fliken Godkännanden visas fullständig information om alla tidigare godkännandesökvägar och steg. Du kan se exakt vem som har fattat ett beslut om godkännandet eller om godkännandet har ställts in för ett team, en jobbroll eller en användare.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Mer information om hur du skapar en godkännandeprocess finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
