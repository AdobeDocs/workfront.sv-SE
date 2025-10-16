---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Skicka en tidrapport för godkännande
description: Om du skickar in tidrapporten för godkännande får din chef insyn i arbetstiden. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att ett tillräckligt antal timmar har registrerats för tidsperioden.
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Skicka en tidrapport för godkännande

<!--Audited: 8/2024-->

Om du skickar in tidrapporten för godkännande får din chef insyn i arbetstiden. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att ett tillräckligt antal timmar har registrerats för tidsperioden.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td> <p>Ljus eller högre </p>
   <p>Granska eller högre </p>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomsten till uppgifter och problem </p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i tidrapporten</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skicka en tidrapport för godkännande

* [Skicka in en tidrapport för godkännande](#submit-a-timesheet-for-approval)
* [Visa status för en skickad tidrapport](#view-the-status-of-a-submitted-timesheet)

### Skicka en tidrapport för godkännande

När en tidrapportgodkännare har angetts (enligt beskrivningen i avsnittet [Ange godkännare för tidrapport](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) i artikeln [Godkänn en tidrapport](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)) ändras knappen **Stäng** längst ned i tidrapporten till knappen **Skicka för godkännande** .

Så här skickar du in en tidrapport för godkännande:

1. Gå till en tidrapport som har konfigurerats att ha en godkännare.
1. Loggtid, enligt beskrivningen i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Klicka på **Skicka för godkännande** för att starta godkännandeprocessen för tidrapporten.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Knappen **Skicka för godkännande** ersätts av knapparna **Godkänn**, **Avvisa** och **Återkalla**. Status för tidrapporten ändras till **Skickat**.

   När tidrapporten skickas för godkännande ser godkännaren tidrapporten som listas i widgeten **Mina godkännanden** i området **Hem**. Följande saker kan hända:

   * Om de godkänner det ändras knappen **Återkalla** till **Öppna igen** och tidrapportens status uppdateras till **Öppna**.
   * Om de avvisar det ersätter knappen **Skicka för godkännande** knappen **Återkalla** och tidrapportens statusuppdatering **Avvisad**.

1. (Valfritt) Klicka på **Återkalla** om du behöver öppna tidrapporten igen och uppdatera din tid. Mer information finns i avsnittet [Återkalla en tidrapport](#recall-a-timesheet) i den här artikeln.

### Visa status för en skickad tidrapport {#view-the-status-of-a-submitted-timesheet}

Du kan visa status för en tidrapport när du har skickat in den.

Om Workfront-administratören har aktiverat händelsehanterarna Godkännande av tidrapport för användare och Avvisning av tidrapport för användare, meddelas du när tidrapporten har godkänts eller avvisats. Mer information om hur du aktiverar händelsemeddelanden finns i [Händelsemeddelandetyper](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Utan dessa meddelanden kan du lära dig mer om status för dina skickade tidrapporter i tidrapportområdet i Workfront.

Så här visar du status för en tidrapport:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.
1. Klicka på **Tidrapporter**. Filtret **Alla** är markerat som standard.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Uppdatera filtret i listan över tidrapporter genom att göra något av följande:

   * Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du godkänner

     eller

     Välj **Mina tidrapporter** om du bara vill visa dina tidrapporter.

     Detta tillämpar filtren Mina tidrapportgodkännanden eller Min tidrapport på listan med tidrapporter.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicka på Filterikonen ![](assets/filter-nwepng.png) om du vill använda ett annat filter eller skapa ett nytt. Mer information om hur du skapar eller uppdaterar filter finns i [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Alternativen Mina tidrapportgodkännanden och Mina tidrapporter visas inte högst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtren Mina tidrapportgodkännanden och Mina tidrapporter från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   >
   >   
   >   
   >   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Villkorligt) Om du valde **Mina tidrapporter** kontrollerar du att vyn **Standard** används och noterar kolumnen **Status**.

   Tidrapporter kan ha följande status:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öppna</td> 
      <td> <p>Din tidrapport är öppen och du kan logga tid. </p> <p>En återkallad tidrapport visas med statusen Öppna. Mer information finns i avsnittet <a href="#recall-a-timesheet" class="MCXref xref">Återkalla en tidrapport</a> i den här artikeln. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skickat</td> 
      <td>Du har skickat in din tidrapport för godkännande, men den har inte godkänts än. Du kan återkalla en inskickad tidrapport om du vill fortsätta redigera den. Mer information finns i avsnittet <a href="#recall-a-timesheet" class="MCXref xref">Återkalla en tidrapport</a> i den här artikeln. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stängd</td> 
      <td> <p>Följande scenarier finns:</p> 
       <ul> 
        <li> <p>Om tidrapporten inte har någon godkännare sparade du din tid och stängde den.</p> </li> 
        <li> <p>Om tidrapporten har en godkännare har du skickat in den för godkännande och den har godkänts.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avvisad</td> 
      <td>Du skickade tidrapporten för godkännande och godkännaren avvisade den.</td> 
     </tr> 
    </tbody> 
   </table>

## Återkalla en tidrapport {#recall-a-timesheet}

Du kan återkalla en tidrapport som redan har skickats in för godkännande. Endast tidrapporter som inte har godkänts kan återkallas.

Så här återkallar du en tidrapport:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Tidrapporter**.
1. Klicka på **Mina tidrapporter** i skärmens övre högra hörn eller välj **Mina tidrapporter** i listrutan **Filter** ![](assets/filter-nwepng.png).
1. Klicka på tidsramen för en tidrapport med statusen **Skickat**.
1. Klicka på **Återkalla**.

   Tidrapporten kan redigeras igen och dess status ändras till **Öppna**.
