---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Information om arbete som tilldelats mig'
description: Följande meddelanden informerar dig om aktiviteter som utförs på en arbetsuppgift som du har tilldelats.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1870'
ht-degree: 0%

---

# Meddelanden: Information om arbete som tilldelats mig

Följande meddelanden informerar dig om aktiviteter som utförs på en arbetsuppgift som du har tilldelats.

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>En föregångare till en uppgift som har tilldelats mitt team har slutförts</strong> </p> <p>Det tilldelade teamet får ett e-postmeddelande när en föregångare till en av sina uppgifter är klar. </p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Fullständigt: &lt;Aktivitetsnamn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Föregående aktivitetsnamn<br>Föregående aktivitetsprojekt<br>Referensnummer för föregående aktivitet<br>Namn på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid när föregående aktivitet slutfördes<br>Tidigare status för föregående aktivitet<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda föregångare <br>*Aktivitetsnamn<br>*Namn på den användare som slutförde aktiviteten<br>*Datum för daglig sammandrag </p> </td> 
   <td><strong>Dagligen</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>En föregångare till en av mina uppgifter har slutförts</strong> </p> <p>Den tilldelade uppgiften får ett e-postmeddelande när en föregångare till en av sina uppgifter är klar. </p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Föregående aktivitetsnamn<br>Föregående aktivitetsprojekt<br>Referensnummer för föregående aktivitet<br>Namn på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid när föregående aktivitet slutfördes<br>Tidigare status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal föregående aktiviteter slutfördes <br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde aktiviteten<br>*Datum för daglig sammandrag </p> </td> 
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
   <td> <p><strong>En åtgärd som jag har slutfört har godkänts eller avvisats</strong> </p> <p>Uppgiftstilldelande får ett e-postmeddelande när uppgiften har godkänts eller avvisats.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt; på &lt;Projektnamn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på den användare som beviljade godkännandet<br>Ny aktivitetsstatus<br>Datum och tid när aktiviteten godkändes eller avvisades<br>Tidigare aktivitetsstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal godkända eller avvisade uppgifter<br>*Aktivitetsnamn<br>*Namn på den användare som godkänts eller avslagits avvisade aktiviteten <br>*Godkännandebeslut ([!UICONTROL Approved]/ [!UICONTROL Rejected])<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>En uppgift som jag har tilldelats är slutförd</strong> </p> <p>Uppgiftstilldelaren får ett e-postmeddelande när uppgiften har slutförts.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt; på &lt;Projektnamn&gt;</em></p> <p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete] visas fortfarande"Fullständigt" som ämne i e-postmeddelandet.</p> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på den användare som slutförde aktiviteten<br>Datum och tid när aktiviteten slutfördes<br>Föregående aktivitetsstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namn på den användare som slutförde uppgiften<br>*Datum för den dagliga sammandraget test<br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Alla föregående aktiviteter för en uppgift som har tilldelats mitt team är slutförda</strong> </p> <p>Det tilldelade teamet får ett e-postmeddelande när en föregångare till någon av deras uppgifter har markerats som slutförd.</p> <p>Användare med en Granska eller Begärande licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Uppgiften slutförd: &lt;Namn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> Sammandrag av arbete som tilldelats dig &lt;Datum för dagligt sammandrag&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Aktivitetsprojekt<br>Referensnummer för aktivitet<br>Namn på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid när föregående aktivitet slutfördes<br>Tidigare status för föregående aktivitet<br><strong>Se Mer information</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda uppgifter&lbrace;11 <br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde aktiviteten<br>*Datum för daglig sammandrag </td>
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
   <td> <p><strong>Alla föregående aktiviteter för mina uppgifter är slutförda</strong> </p> <p>Uppgiftstilldelande får ett e-postmeddelande för varje föregående som har slutförts.</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt;</em><br></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Aktivitetsprojekt<br>Referensnummer för aktivitet<br>Namn på den användare som slutförde föregående aktivitet<br>Status för föregående aktivitet<br>Datum och tid när föregående aktivitet slutfördes<br>Tidigare status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br> *Namn på den användare som slutförde uppgiften <br>*Datum för daglig sammandrag </td> 
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
   <td> <p><strong>Ett problem som jag löser har godkänts eller avvisats</strong> </p> <p>Den som är tilldelad en utgåva får ett e-postmeddelande när ett godkännandebeslut fattas (godkänt eller avvisat).</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Utfärdande väntar på godkännande: &lt;Planerat startdatum&gt; &lt;Utfärdningsreferensnummer&gt; - &lt;Utfärdningsnamn&gt; i &lt;Projektnamn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> Sammandrag av arbete som tilldelats dig &lt;Datum för dagligt sammandrag&gt; </em></p> </td> 
   <td> Utleveransnamn<br>Projektnamn<br>Utgivningsreferensnummer<br>Namn på den användare som godkände eller avvisade felet<br>Godkännandebeslut (godkänt eller avvisat)<br>Utgivningsstatus<br>Namn på den användare som begärde godkännandet<br><strong>[!UICONTROL See More Details]</strong>-knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal godkända eller avvisade<br>*Utgivningsnamn<br> Namn på den användare som godkände eller avvisade frågan <br>*Godkännandebeslut (godkänt eller avvisat) <br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Ett problem som jag har tilldelats är slutfört</strong> </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>Fullständigt: &lt;Issue Name&gt; på &lt;Project Name&gt;</em></p> <p><em> Ämnet för det dagliga sammandragsmeddelandet är: Sammandrag av arbete som tilldelats dig &lt;Datum för dagligt sammandrag&gt; </em> </p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Utfärdningsreferensnummer<br>Namnet på den användare som slutförde problemet<br>Nytt ärende-status<br>Datum och tid när utgåvan slutfördes<br>Föregående aktivitetsstatus<br><strong>[!UICONTROL See More Details]</strong>-knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda problem<br>*Utfärdningsnamn<br>*Namn på den användare som slutförde utgåvan <br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dokument överförs eller ändras vid begäranden som jag har tilldelats till</strong> </p> <p>Den som tilldelats utgåvan får ett e-postmeddelande när dokument överförs eller när dokumentinformationen ändras i ett ärende som han eller hon har lagt till.</p> <p>Ett e-postmeddelande skickas inte om den användare som utlöste problemet är den som tilldelades problemet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och projektet har konfigurerats som en kö för hjälpbegäran (enligt beskrivningen i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Document added to] &lt;Namn på begäran&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Begäransnamn<br>Projektnamn (begärandekönamn)<br>Dokumentreferensnummer <br>Namnet på den användare som överförde dokumentet<br>Dokumentnamn <br>lades till den <br>Dokumentinformationen (format, storlek, versionsnummer)<br>Dokumentminiatyrbild<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal överförda eller ändrade dokument <br>*Dokumentnamn<br>*Objektnamn<br>*Namn på den användare som överförde dokumentet <br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Förfallodatumet ändras för en aktivitet som jag har tilldelats till</strong> </p> <p>Uppgiftstilldelaren får ett e-postmeddelande när [!UICONTROL Planned Completion Date] för uppgiften ändras, såvida inte den användare som ändrade det planerade slutförandedatumet också är Uppgiftstilldelad.</p> <p>Ett meddelande skickas bara om projektstatusen är något annat än [!UICONTROL Planning].</p> <p>Inget meddelande skickas om personliga uppgifter.</p> <p> Användare med en Granska eller Begärande licens får inget meddelande. </p> <p> Ämnet för e-postmeddelandet är: <em>[!UICONTROL Due Date has been changed.]</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Nytt förfallodatum ([!UICONTROL Planned Completion Date])<br>Datum och tid när förfallodatumet ändrades<br>Namnet på den användare som ändrade förfallodatumet<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal aktiviteter där förfallodatumet (planerat slutförandedatum) ändrades<br>*Aktivitetsnamn<br>*Nytt planerat slutförandedatum <br>*Namnet på den användare som ändrade förfallodatumet <br>*Datum för den dagliga sammandraget </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Förfallodatumet ändras för ett ärende som jag har tilldelats till</strong> </p> <p>Den som tilldelat utgåvan får ett e-postmeddelande när [!UICONTROL Planned Completion Date] ändras, såvida inte användaren som ändrade [!UICONTROL Planned Completion Date] också är tilldelad.</p> <p>Ett meddelande skickas bara om projektstatusen är något annat än [!UICONTROL Planning].</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Due Date has been changed]</em></p> <p> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt;</em></p> </td> 
   <td> <p>Utgivningsnamn<br>Projektnamn<br>Utgivningsreferensnummer<br>Nytt förfallodatum ([!UICONTROL Planned Completion Date])<br>Datum och tid när förfallodatumet ändrades<br>Namnet på den användare som ändrade förfallodatumet<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal ärenden där förfallodatumet ([!UICONTROL Planned Completion Date]) ändrades<br>*Utgivningsnamn<br>*Nytt [!UICONTROL Planned Completion Date]<br> *Namnet på den användare som ändrade förfallodatumet <br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Status ändras för en aktivitet som jag har tilldelats till </strong> <p>Uppgiftstilldelaren får ett e-postmeddelande när uppgiftsstatus ändras, såvida inte den användare som ändrade statusen också är tilldelad.</p> <p>Obs! Det här meddelandet skickas inte när aktivitetsstatusen ändras till slutförd. Ett separat meddelande används för slutförda uppgifter. Se <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">En uppgift som jag har tilldelats är slutförd</a> ovan.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;Aktivitetsnamn&gt; från &lt;Projektnamn&gt; är &lt;Ny status&gt;</em></p> <p> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på den användare som ändrade status<br>Ny status<br>Datum och tid när statusen ändrades<br>Förhandsgranskningsstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal aktiviteter där statusen ändrades<br>*Aktivitetsnamn<br>*Tidigare aktivitetsstatus<br> Ny aktivitetsstatus <br>*Namnet på den användare som ändrade status <br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Statusen ändras för ett av mina arbetsobjekt</strong> </p> <p>Du får ett e-postmeddelande när statusen ändras för ett ärende som du har tilldelats, såvida du inte själv ändrar statusen. </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Användare med en [!UICONTROL Review]- eller [!UICONTROL Requestor]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;Issue Name&gt; från &lt;Project Name&gt; är &lt;New Status&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Utfärdningsreferensnummer<br>Namnet på den användare som ändrade status<br>Ny status<br>Datum och tid när statusen ändrades<br>Tidigare utgåvstatus<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal problem där statusen ändrades<br>*Aktivitetsnamn<br>&rbrace;*Status för föregående problem <br>*Status för nytt problem<br>*Namn på den användare som ändrade status<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
 </tbody> 
</table>
