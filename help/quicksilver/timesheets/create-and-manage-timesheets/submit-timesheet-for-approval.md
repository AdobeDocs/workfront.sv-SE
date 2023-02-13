---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Skicka en tidrapport för godkännande
description: Om du skickar in tidrapporten för godkännande får din chef insyn i arbetstiden. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att ett tillräckligt antal timmar har registrerats för tidsperioden.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Skicka en tidrapport för godkännande

Om du skickar in tidrapporten för godkännande får din chef insyn i arbetstiden. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att ett tillräckligt antal timmar har registrerats för tidsperioden.

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
   <td> <p>Visa åtkomst eller senare till uppgifter och ärenden</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för uppgifter och problem</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skicka en tidrapport för godkännande

* [Skicka en tidrapport för godkännande](#submit-a-timesheet-for-approval)
* [Visa status för en skickad tidrapport](#view-the-status-of-a-submitted-timesheet)

### Skicka en tidrapport för godkännande

När en tidrapportgodkännare har angetts (enligt beskrivningen i avsnittet) [Utse godkännare av tidrapporter](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) i artikeln [Godkänn en tidrapport](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), **Stäng** längst ned i tidrapporten ändras till **Skicka för godkännande** -knappen.

Så här skickar du in en tidrapport för godkännande:

1. Gå till en tidrapport som har konfigurerats att ha en godkännare.
1. Loggtid enligt beskrivningen i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Klicka **Skicka för godkännande** för att starta godkännandeprocessen för tidrapporten.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   The **Skicka för godkännande** knappen ersätts av **Godkänn**, **Avvisa** och **Återkalla** knappar. Tidrapportens status ändras till **Skickat**.

   När tidrapporten skickas in för godkännande ser godkännaren tidrapporten som listas i **Godkännanden** området på **Startsida** sida. Följande saker kan hända:

   * Om de godkänner det **Återkalla** knappen ändras till **Öppna igen** och tidrapportens status uppdateras till **Öppna**.
   * Om de avvisar det **Skicka för godkännande** knappen ersätter **Återkalla** och tidrapportens status uppdateras till **Avvisad**.

1. (Valfritt) Klicka på **Återkalla** om du behöver öppna tidrapporten igen och uppdatera din tid. Mer information finns i [Återkalla en tidrapport](#recall-a-timesheet) i den här artikeln.

### Visa status för en skickad tidrapport {#view-the-status-of-a-submitted-timesheet}

Du kan visa status för en tidrapport när du har skickat in den.

Om Workfront-administratören har aktiverat händelsehanterarna Godkännande av tidrapport för användare och Avvisning av tidrapport för användare, meddelas du när tidrapporten har godkänts eller avvisats. Information om hur du aktiverar händelsemeddelanden finns i [Händelsemeddelanden är tillgängliga i Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Utan dessa meddelanden kan du lära dig mer om status för dina skickade tidrapporter i tidrapportområdet i Workfront.

Så här visar du status för en tidrapport:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.
1. Klicka **Tidrapporter**. The **Alla** filtret är markerat som standard.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Uppdatera filtret i listan över tidrapporter genom att göra något av följande:

   * Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du har godkänt

      eller

      Välj **Mina tidrapporter** om du bara vill visa dina tidrapporter.

      Detta tillämpar filtren Mina tidrapportgodkännanden eller Min tidrapport på listan med tidrapporter.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicka på ikonen Filter ![](assets/filter-nwepng.png) om du vill använda ett annat filter eller skapa ett nytt. Mer information om hur du skapar eller uppdaterar filter finns i [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Alternativen Mina tidrapportgodkännanden och Mina tidrapporter visas inte högst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtren Mina tidrapportgodkännanden och Mina tidrapporter från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   >
   >   
   >   
   >   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Villkorligt) Om du har valt **Mina tidrapporter**, se till att **Standard** vyn används och du ser **Status** kolumn.

   Tidrapporter kan ha följande status:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öppna</td> 
      <td> <p>Din tidrapport är öppen och du kan logga tid. </p> <p>En återkallad tidrapport visas med statusen Öppna. Mer information finns i <a href="#recall-a-timesheet" class="MCXref xref">Återkalla en tidrapport</a> i den här artikeln. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skickat</td> 
      <td>Du har skickat in din tidrapport för godkännande, men den har inte godkänts än. Du kan återkalla en inskickad tidrapport om du vill fortsätta redigera den. Mer information finns i <a href="#recall-a-timesheet" class="MCXref xref">Återkalla en tidrapport</a> i den här artikeln. </td> 
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

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Tidrapporter**.
1. Klicka **Mina tidrapporter** i skärmens övre högra hörn eller välj **Mina tidrapporter** från **Filter** ![](assets/filter-nwepng.png) nedrullningsbar meny.
1. Klicka på tidsramen för en tidrapport med statusen **Skickat**.
1. Klicka **Återkalla**.

   Tidrapporten kan redigeras igen och dess status ändras till **Öppna**.
