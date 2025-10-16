---
product-area: projects
navigation-topic: approvals
title: Visa godkännanden
description: Godkännandeprocesser ger flexibilitet att skapa godkännanden i flera steg för projekt, uppgifter och ärenden. Adobe Workfront administratörer definierar godkännandeprocesser för att skapa enhetlighet i hela systemet.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 2503b6e628e4860a5652c620d8e4d0eea2414443
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Visa godkännanden

Godkännandeprocesser ger flexibilitet att skapa godkännanden i flera steg för projekt, uppgifter och ärenden. Adobe Workfront administratörer definierar godkännandeprocesser för att skapa enhetlighet i hela systemet.

Mer information om hur du skapar godkännandeprocesser finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Mer information om hur du associerar godkännanden med arbete i Workfront finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p></p>Contribute eller högre</p>
   <p>Granska eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td><p>Visa eller öka åtkomsten till objekt som är kopplade till godkännanden</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för objekt som är associerade med godkännanden</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hitta godkännanden i Adobe Workfront

Du kan visa eller hantera godkännanden från flera områden i Workfront. Mer information om hur du hanterar godkännanden inom olika områden finns i [Godkänna arbete](../../review-and-approve-work/manage-approvals/approving-work.md).

Du kan visa eller hantera godkännanden från följande områden:

* I hemområdet

   * Alla projekt, uppgifter, utgåvor, tidrapporter, dokument och åtkomst som väntar på ditt godkännande visas i widgeten Mina godkännanden i området Hem.
   * Godkännanden som du har skickat själv visas också i widgeten Mina godkännanden i hemområdet när du väljer alternativet Godkännanden som jag har skickat. Mer information finns i avsnittet [Granskningsarbete som du skickar in för godkännande i hemområdet](#review-work-you-submit-for-approval-in-the-home-area) i den här artikeln.
   * Godkännanden tas bort från widgeten Mina godkännanden i hemområdet när det associerade projektet, aktiviteten eller utgåvan har markerats som Löst, Spärrat, Stängt eller Avbrutet.

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

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Klicka på **Anpassa** för att lägga till widgeten **Mina godkännanden**.
1. (Villkorligt) Klicka på listrutan **Filter** och välj sedan **Godkännanden som jag har skickat** för att se de godkännanden som du har skickat in.


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
1. Klicka på **Godkännanden** i den vänstra panelen.

   På fliken Godkännanden visas fullständig information om alla tidigare godkännandesökvägar och steg. Du kan se exakt vem som har fattat ett beslut om godkännandet eller om godkännandet har ställts in för ett team, en jobbroll eller en användare.

   ![Fliken Godkännanden utökad](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Mer information om hur du skapar en godkännandeprocess finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
