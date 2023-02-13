---
content-type: reference
navigation-topic: notifications
title: '''Meddelanden: Information om arbete som tilldelats mig'
description: Följande meddelanden informerar dig om aktiviteter som utförs på en arbetsuppgift som du har tilldelats.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 39ba9e93a8597d4354472a19b1ac1c5f530f4398
workflow-type: tm+mt
source-wordcount: '1874'
ht-degree: 0%

---

# Meddelanden: Information om arbete som tilldelats mig

Följande meddelanden informerar dig om aktiviteter som utförs på en arbetsuppgift som du har tilldelats.

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Se även [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Meddelande</th> 
   <th> <p>Inkluderade fält </p> <p> *Endast dagliga sammanfattningsfält</p> </th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>En föregångare till en uppgift som har tilldelats mitt team har slutförts</strong> </p> <p>Det tilldelade teamet får ett e-postmeddelande när en föregångare till en av sina uppgifter är klar. </p> <p>Användare med [!UICONTROL Review] eller Re[!UICONTROL Requestor]frågelicensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Fullständigt: &lt;task name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Föregående aktivitetsnamn<br>Föregående aktivitetsprojekt<br>Referensnummer för föregående aktivitet<br>Namnet på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid då föregående var slutfört<br>Föregående status för föregående aktivitet<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda föregångare<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för daglig sammandrag </p> </td> 
   <td><strong>Dagligen</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>En föregångare till en av mina uppgifter har slutförts</strong> </p> <p>Den tilldelade uppgiften får ett e-postmeddelande när en föregångare till en av sina uppgifter är klar. </p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Föregående aktivitetsnamn<br>Föregående aktivitetsprojekt<br>Referensnummer för föregående aktivitet<br>Namnet på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid då föregående var slutfört<br>Föregående status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda föregångare<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för daglig sammandrag </p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>En uppgift som jag har slutfört har godkänts eller avvisats</strong> </p> <p>Uppgiftstilldelande får ett e-postmeddelande när uppgiften har godkänts eller avvisats.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;task name=""&gt; på &lt;project name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namn på den användare som beviljade godkännandet<br>Ny aktivitetsstatus<br>Datum och tid när uppgiften godkändes eller avvisades<br>Status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal godkända eller avvisade uppgifter<br>*Aktivitetsnamn<br>*Namnet på den användare som godkände eller avvisade uppgiften<br>*Godkännandebeslut ([!UICONTROL Approved]/ [!UICONTROL Rejected])<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>En uppgift som jag har tilldelats är slutförd</strong> </p> <p>Uppgiftstilldelaren får ett e-postmeddelande när uppgiften har slutförts.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;task name=""&gt; på &lt;project name=""&gt;</em></p> <p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete]visas fortfarande"Fullständigt" som ämne i e-postmeddelandet.</p> </p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som slutförde uppgiften<br>Datum och tid när uppgiften slutfördes<br>Status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Alla föregångare till en uppgift som har tilldelats mitt team är slutförda</strong> </p> <p>Det tilldelade teamet får ett e-postmeddelande när en föregångare till någon av deras uppgifter har markerats som slutförd.</p> <p>Användare med en Granska eller Begärande licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Uppgiften har slutförts: &lt;name&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> Sammanfattning av arbete som tilldelats dig &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Uppgiftsprojekt<br>Referensnummer för uppgift<br>Namnet på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid då föregående var slutfört<br>Föregående status för föregående aktivitet<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för daglig sammandrag </td>
   <td><strong>Direkt</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Alla föregångare till mina uppgifter är slutförda</strong> </p> <p>Uppgiftstilldelande får ett e-postmeddelande för varje föregående som har slutförts.</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em><br></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Uppgiftsprojekt<br>Referensnummer för uppgift<br>Namnet på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid då föregående var slutfört<br>Föregående status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för daglig sammandrag </td> 
   <td><strong>Direkt</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Ett problem som jag löser har godkänts eller avvisats</strong> </p> <p>Den som är tilldelad en utgåva får ett e-postmeddelande när ett godkännandebeslut fattas (godkänt eller avvisat).</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Problem som väntar på godkännande: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> Sammanfattning av arbete som tilldelats dig &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som godkände eller avvisade problemet<br>Godkännandebeslut (godkänt eller avvisat)<br>Ärendestatus<br>Namn på den användare som begärde godkännandet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal godkända eller avvisade problem<br>*Ärendenamn<br>*Namnet på den användare som godkände eller avvisade problemet<br>*Godkännandebeslut (godkänt eller avvisat)<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Ett problem som jag har tilldelats är slutfört</strong> </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Fullständigt: &lt;issue name=""&gt; på &lt;project name=""&gt;</em></p> <p><em> Det dagliga sammandraget innehåller följande uppgifter: Sammanfattning av arbete som tilldelats dig &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som slutförde problemet<br>Status för nytt problem<br>Datum och tid då utgåvan slutfördes<br>Status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda ärenden<br>*Ärendenamn<br>*Namnet på den användare som slutförde problemet<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dokument överförs eller ändras vid begäranden som jag har tilldelats till</strong> </p> <p>Den som tilldelats utgåvan får ett e-postmeddelande när dokument överförs eller när dokumentinformationen ändras i ett ärende som han eller hon har lagt till.</p> <p>Ett e-postmeddelande skickas inte om den användare som utlöste problemet är den som tilldelades problemet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och om projektet har konfigurerats som en kö för hjälpbegäran (enligt beskrivningen i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Document added to] &lt;request name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Namn på begäran<br>Projektnamn (namn på begärandekö)<br>Dokumentets referensnummer <br>Namnet på den användare som överförde dokumentet<br>Dokumentnamn <br>Tillagd den<br>Dokumentinformation (format, storlek, versionsnummer)<br>Dokumentminiatyr<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal överförda eller ändrade dokument<br>*Dokumentnamn<br>*Objektnamn<br>*Namnet på den användare som överförde dokumentet<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Förfallodatumet ändras för en uppgift som jag har tilldelats till</strong> </p> <p>Uppgiftstilldelaren får ett e-postmeddelande när [!UICONTROL Planned Completion Date] om aktiviteten ändras, såvida inte den användare som ändrade det planerade slutförandedatumet också är Uppgiftstilldelningsmannen.</p> <p>Ett meddelande skickas bara om projektstatusen är något annat än [!UICONTROL Planning].</p> <p>Inget meddelande skickas om personliga uppgifter.</p> <p> Användare med en Granska eller Begärande licens får inget meddelande. </p> <p> Ämnet för e-postmeddelandet är: <em>[!UICONTROL Due Date has been changed.]</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Nytt förfallodatum ([!UICONTROL Planned Completion Date])<br>Datum och tid när förfallodatumet ändrades<br>Namnet på användaren som ändrade förfallodatumet<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal aktiviteter där förfallodatumet (planerat slutförandedatum) ändrades<br>*Aktivitetsnamn<br>*Nytt planerat slutförandedatum<br>*Namnet på den användare som ändrade förfallodatumet<br>*Datum för daglig sammandrag </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Förfallodatumet ändras för en utgåva som jag har tilldelats till</strong> </p> <p>Den som tilldelat utgåvan får ett e-postmeddelande när [!UICONTROL Planned Completion Date] ändras, såvida inte användaren som ändrade [!UICONTROL Planned Completion Date] är även den som har tilldelats.</p> <p>Ett meddelande skickas bara om projektstatusen är något annat än [!UICONTROL Planning].</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Due Date has been changed]</em></p> <p> </p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Nytt förfallodatum ([!UICONTROL Planned Completion Date])<br>Datum och tid när förfallodatumet ändrades<br>Namnet på den användare som ändrade förfallodatumet<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal utgåvor där förfallodatumet ([!UICONTROL Planned Completion Date]) ändrad<br>*Ärendenamn<br>*Nytt [!UICONTROL Planned Completion Date]<br>*Namnet på den användare som ändrade förfallodatumet<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Statusändringarna för en uppgift som jag har tilldelats till</strong> <p>Uppgiftstilldelaren får ett e-postmeddelande när uppgiftsstatus ändras, såvida inte den användare som ändrade statusen också är tilldelad.</p> <p>Obs! Det här meddelandet skickas inte när aktivitetsstatusen ändras till slutförd. Ett separat meddelande används för slutförda uppgifter. Se <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">En uppgift som jag har tilldelats är slutförd</a>, ovan.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;task name=""&gt; från &lt;project name=""&gt; är &lt;new status=""&gt;</em></p> <p> </p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som ändrade statusen<br>Ny status<br>Datum och tid när statusen ändrades<br>Förhandsgranskningsstatus<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal uppgifter där statusen ändrades<br>*Aktivitetsnamn<br>*Status för föregående aktivitet<br>*Ny aktivitetsstatus<br>*Namnet på den användare som ändrade statusen<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Statusen ändras för en av mina arbetsuppgifter</strong> </p> <p>Du får ett e-postmeddelande när statusen ändras för ett ärende som du har tilldelats, såvida du inte själv ändrar statusen. </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Användare med [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;issue name=""&gt; från &lt;project name=""&gt; är &lt;new status=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Work Assigned to You] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som ändrade statusen<br>Ny status<br>Datum och tid när statusen ändrades<br>Status för föregående problem<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal problem där statusen ändrades<br>*Aktivitetsnamn<br>*Status för föregående problem<br>*Status för nytt problem<br>*Namnet på den användare som ändrade statusen<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
 </tbody> 
</table>
