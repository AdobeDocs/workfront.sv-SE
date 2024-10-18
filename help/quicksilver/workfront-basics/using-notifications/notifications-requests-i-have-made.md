---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Jag har gjort förfrågningar'
description: I följande meddelanden får du information om begäranden som du har gjort i Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: 9f351a16c2a741b922e8ee51efb3ea3d7d2d18e1
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# Meddelanden: Begäranden jag gjort

I följande meddelanden får du information om begäranden som du har gjort i [!DNL Adobe Workfront].

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Se även [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Begäranden jag gjort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om dokumentgodkännande har slutförts</strong> </p> <p>Användaren som begärde godkännande av ett dokument får ett e-postmeddelande när begäran om godkännande av dokumentet har slutförts.</p> <p>Ämnet för e-postmeddelandet med snabbmeddelanden är:<em> &lt;Godkännarens namn&gt; har &lt;Godkännandebeslut ([!UICONTROL Approved], [!UICONTROL Approved with Changes], [!UICONTROL Rejected])&gt; det här dokumentet.</em></p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </td> 
   <td> Dokumentnamn<br>Godkännarens namn </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett dokument har ändrats eller överförts för ett problem som jag är primär kontakt för</strong> </p> <p>Den primära kontakten får ett e-postmeddelande när ett dokument överförs eller ändras i frågan, såvida inte den användare som överförde eller ändrade dokumentet också är den primära kontakten.</p> <p>Ett meddelande skickas bara om projektet har konfigurerats som [!UICONTROL Help Request Queue] (enligt beskrivningen i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>Dokumentet har lagts till i &lt;Issue Name&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är: <em>Sammandrag av dina begäranden &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Objektnamn där dokumentet överfördes<br>Överordnat objektnamn<br>Dokumentreferensnummer<br>Namnet på den användare som överförde dokumentet<br>Dokumentnamn<br>lades till den <br>Dokumentinformationen (format, storlek, versionsnummer)<br>Dokumentminiatyrbild<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal överförda dokument <br>*Namn på dokument <br>*Namn på överordnat objekt<br>*Namn på den användare som lade till dokumentet <br>*Datum för den dagliga sammanfattningen </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om dokumentöverföring har uppfyllts</strong> </p> <p>Dokumentbegäraren får ett e-postmeddelande när en begäran om dokumentöverföring har slutförts.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Your document request from] &lt;Användarnamn&gt; har uppfyllts</em></p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </td> 
   <td> <p>Namn på den användare som överförde dokumentet<br>Objektnamn där dokumentet överfördes<br>Dokumentnamn<br><br></p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En personlig uppgift som jag har tilldelat någon annan har slutförts</strong> </p> <p>Ett meddelande skickas till den användare som tilldelade en ad hoc-uppgift till någon annan när uppgiften är slutförd. </p> <p>Mer information om ad hoc-åtgärder finns i <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Skapa arbetsobjekt och projekt från [!UICONTROL Home] området </a>.</p> <p>Ämnet för e-postmeddelandet är: <em>Slutförd aktivitet: &lt;Aktivitetsnamn&gt;</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> Aktivitetsnamn<br>Standardprojektnamn (personligt projekt för den användare som tog emot den personliga aktiviteten)<br>Referensnummer för aktivitet<br>Namn på aktivitetsägare<br>Ny aktivitetsstatus<br>Datum och tid när aktiviteten slutfördes<br>Knappen Tidigare aktivitetsstatus<br><strong>[!UICONTROL See More Details]</strong><br><br><br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem som jag är primär kontakt för har slutförts</strong> </p> <p>Den primära kontakten i ett problem får ett meddelande när problemet är slutfört.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue Completion]: </em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> Sammandrag av dina begäranden &lt;Datum för den dagliga sammandraget&gt;</em></p> <p> </p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som slutförde problemet<br>Ny status<br>Datum och tid när problemet slutfördes<br>Tidigare utgåvstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda utgåvor<br>*Ärendenamn<br>*Namnet på den användare som slutförde utgåvan <br>*Datum för daglig sammandrag </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag lägger till ett problem i ett projekt</strong> </p> <p>Den primära kontakten i ett problem får ett meddelande när han eller hon lägger till ett problem i ett projekt.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue submitted]: &lt;Issue Name&gt; på &lt;Project Name&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> Sammandrag av dina begäranden &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Projektnamn<br>Portfolio-namn<br>Ärendereferensnummer<br>Ditt namn<br>Utgåva<br>Angivet datum<br>Utgivningsprioritet<br>Utgåva status<br>Tilldelad till namn<br>Primär kontakt<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal tillagda fel<br>*Utgångsnamn<br>*Datum dagens sammandrag </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag skickar en begäran (bekräftelse)</strong> </p> <p>Den primära kontakten får ett e-postmeddelande när han eller hon skickar ett problem.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och om projektet har konfigurerats som [!UICONTROL Help Request Queue] (enligt beskrivningen i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Request Submitted]: &lt;Namn på begäran&gt; på &lt;Namn på projekt (begärandekö)&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> Sammandrag av dina begäranden &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> <p>Projektnamn (namn på frågekö)<br>Portfolio-namn<br>Ärendereferensnummer<br>Utfärdsnamn<br>Angivet datum<br>Ärendeprioritet<br>Utfärdat till namn<br>Tilldelat till namn<br>Primär kontakt<br>*Projektreferensnummer<br>*Projektnamn<br>*Totalt antal förfrågningar som skickats<br>*Namn på förfrågan<br>*Prioritet <br>*Datum för daglig sammandrag</p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Min förfrågan är stängd (bekräftelse)</strong> </p> <p>Den primära kontakten får ett e-postmeddelande när begäran stängs.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet har konfigurerats som [!UICONTROL Help Request Queue] (enligt beskrivningen i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Your request has been closed]: </em> </p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of your Requests] &lt;Datum för det dagliga sammandraget&gt;</em></p> </td> 
   <td> Begäransnamn<br>Projektnamn<br>Referensnummer för begäran<br>Namn på den användare som stängde begäran<br>Utgivningsstatus<br>Datum och tid när begäran stängdes<br>Status för föregående begäran<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektreferensnummer<br>*Projektnamn<br>*Totalt antal stängda begäranden<br>*Namn på begäran<br>*Namn på den användare som stängde begäran<br> 2}*Datum för daglig sammandrag </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon har tilldelats min begäran</strong> </p> <p>Den primära kontakten för utgåvan får ett e-postmeddelande när en användare tilldelas utgåvan, såvida inte den primära kontakten och den tilldelade användaren är samma användare.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet har konfigurerats som [!UICONTROL Help Request Queue] (enligt beskrivningen i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet med snabbmeddelanden är: <em>&lt;Namnet på den användare som har tilldelats din begäran&gt; [!UICONTROL has been assigned to your request]: "&lt;Namn på begäran&gt;"</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of your Requests] &lt;Datum för det dagliga sammandraget&gt;</em></p> </td> 
   <td> <p>Utleveransnamn<br>Projektnamn<br>Utgivningsreferensnummer<br>Namn på förfrågan<br>Typ av förfrågan<br>Angivet den<br>Utgivningsprioritet<br>Primär kontakt<br>Planerat slutförandedatum<br>Utgivningsstatus<br><strong>Mer information</strong> knapp <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal tilldelade begäranden <br>*Namn på begäran<br>*Tilldelad till namn<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Status ändras för ett projekt som jag har skapat</strong> </p> <p>Användaren som skapade projektet får ett e-postmeddelande när projektstatusen ändras.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project Status Change]: &lt;Projektnamn&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of your Requests] &lt;Datum för det dagliga sammandraget&gt;</em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio <br>Projektreferensnummer<br>Namn på den användare som ändrade status<br>Ny status<br>Datum och tid när projektstatus ändrades<br>Föregående projektstatus<br><strong>[!UICONTROL See More Details]</strong>-knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Ny projektstatus<br>*Namn på den användare som ändrade projektstatus<br>*Datum för daglig sammandrag</p> </td> 
   <td> <p><strong>Direkt</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Statusen ändras på min begäran</strong> </p> <p>Den primära kontakten för problemet får ett e-postmeddelande när utgivningsstatusen ändras, såvida inte den användare som ändrade statusen också är den primära kontakten.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och projektet har konfigurerats som [!UICONTROL Help Request Queue] (enligt beskrivningen i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;Namn på begäran&gt; är &lt;Ny status&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> Sammandrag av dina begäranden &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Begäransnamn<br>Projektnamn<br>Referensnummer för begäran<br>Namnet på den användare som ändrade status för begäran<br>Ny status<br>Datum och tid när status för begäran ändrades<br>Status för föregående begäran<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal begäranden vars status ändrades<br>*Namn på begäran<br>*Föregående begäran Status <br>*Status för ny begäran <br>*Namn på den användare som ändrade status <br>*Datum för den dagliga sammandraget<br></td> 
   <td> <p><strong>Dagligen</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
