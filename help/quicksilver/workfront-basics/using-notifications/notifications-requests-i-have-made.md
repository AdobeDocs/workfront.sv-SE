---
content-type: reference
navigation-topic: notifications
title: '''Meddelanden: Begäranden jag har gjort'
description: I följande meddelanden får du information om begäranden som du har gjort i Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# Meddelanden: Begäranden som jag har gjort

Följande meddelanden informerar dig om de förfrågningar du har gjort i [!DNL Adobe Workfront].

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Se även [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Förfrågningar jag gjort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om dokumentgodkännande har slutförts</strong> </p> <p>Användaren som begärde godkännande av ett dokument får ett e-postmeddelande när begäran om godkännande av dokumentet har slutförts.</p> <p>Ämnet för e-postmeddelandet är:<em> &lt;approver name=""&gt; har &lt;approval decision="" span="" id="1" translate="no" /&gt;, [!UICONTROL Approved with Changes], [!UICONTROL Rejected])&gt; det här dokumentet.</em>[!UICONTROL Approved]</p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt e-postmeddelande med sammandrag.</p> </td> 
   <td> Dokumentnamn<br>Godkännarens namn </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett dokument ändras eller överförs vid ett problem som jag är primär kontakt för</strong> </p> <p>Den primära kontakten får ett e-postmeddelande när ett dokument överförs eller ändras i frågan, såvida inte den användare som överförde eller ändrade dokumentet också är den primära kontakten.</p> <p>Ett meddelande skickas bara om projektet har konfigurerats som en [!UICONTROL Help Request Queue] (enligt beskrivning i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>Dokumentet har lagts till i &lt;issue name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter: <em>Sammandrag av dina begäranden &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Objektnamn som dokumentet överfördes till<br>Namn på överordnat objekt<br>Dokumentets referensnummer<br>Namnet på den användare som överförde dokumentet<br>Dokumentnamn<br>Tillagd den<br>Dokumentinformation (format, storlek, versionsnummer)<br>Dokumentminiatyr<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal överförda dokument<br>*Dokumentets namn<br>*Namn på överordnat objekt<br>*Namnet på den användare som lade till dokumentet<br>*Datum för den dagliga sammandraget </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om dokumentöverföring har uppfyllts</strong> </p> <p>Dokumentbegäraren får ett e-postmeddelande när en begäran om dokumentöverföring har slutförts.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Your document request from] &lt;user name=""&gt; uppfylldes</em></p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt e-postmeddelande med sammandrag.</p> </td> 
   <td> <p>Namnet på den användare som överförde dokumentet<br>Objektnamn som dokumentet överfördes till<br>Dokumentnamn<br><br></p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En personlig uppgift som jag har tilldelat någon annan har slutförts</strong> </p> <p>Ett meddelande skickas till den användare som tilldelade en ad hoc-uppgift till någon annan när uppgiften är slutförd. </p> <p>Mer information om ad hoc-åtgärder finns i <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Skapa arbetsobjekt från [!UICONTROL Home] area</a>.</p> <p>Ämnet för e-postmeddelandet är: <em>Slutförd uppgift: &lt;task name=""&gt;</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt e-postmeddelande med sammandrag.</p> </p> </td> 
   <td> Aktivitetsnamn<br>Standardprojektnamn (personligt projekt för den användare som tog emot den personliga uppgiften)<br>Referensnummer för uppgift<br>Namn på aktivitetsägare<br>Ny aktivitetsstatus<br>Datum och tid när uppgiften slutfördes<br>Status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br><br><br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem som jag är primär kontakt för har åtgärdats</strong> </p> <p>Den primära kontakten i ett problem får ett meddelande när problemet är slutfört.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue Completion]: &lt;issue name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> Sammandrag av dina förfrågningar &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som slutförde problemet<br>Ny status<br>Datum och tid då utgåvan slutfördes<br>Status för föregående problem<br><strong>[!UICONTROL See More Details]</strong> knapp <br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda ärenden<br>*Ärendenamn<br>*Namnet på den användare som slutförde problemet<br>*Datum för daglig sammandrag </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag lägger till ett problem i ett projekt</strong> </p> <p>Den primära kontakten i ett problem får ett meddelande när han eller hon lägger till ett problem i ett projekt.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue submitted]: &lt;issue name=""&gt; på &lt;project name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> Sammandrag av dina förfrågningar &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Ärendereferensnummer<br>Ditt namn<br>Ärendenamn<br>Angivet den<br>Ärendeprioritet<br>Ärendestatus<br>Tilldelad till namn<br>Primär kontakt<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal tillagda utgåvor<br>*Ärendenamn<br>*Datum för daglig sammandrag </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag skickar en begäran (bekräftelse)</strong> </p> <p>Den primära kontakten får ett e-postmeddelande när han eller hon skickar ett problem.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och om projektet har konfigurerats som en [!UICONTROL Help Request Queue] (enligt beskrivning i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Request Submitted]: &lt;request name=""&gt; på &lt;project request="" queue="" name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> Sammandrag av dina förfrågningar &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Projektnamn (namn på begärandekö)<br>Portfolio<br>Ärendereferensnummer<br>Ärendenamn<br>Angivet den<br>Ärendeprioritet<br>Ärendestatus<br>Tilldelad till namn<br>Primär kontakt<br>*Projektets referensnummer<br>*Projektnamn<br>*Totalt antal inlämnade ansökningar<br>*Namn på förfrågan<br>*Prioritet för förfrågan<br>*Datum för daglig sammandrag</p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Min förfrågan är stängd (bekräftelse)</strong> </p> <p>Den primära kontakten får ett e-postmeddelande när begäran stängs.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet har konfigurerats som en [!UICONTROL Help Request Queue] (enligt beskrivning i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Your request has been closed]:"&lt;request name=""&gt;"</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Namn på begäran<br>Projektnamn<br>Referensnummer för begäran<br>Namnet på den användare som stängde begäran<br>Ärendestatus<br>Datum och tid då begäran stängdes<br>Status för föregående begäran<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektets referensnummer<br>*Projektnamn<br>*Totalt antal stängda begäranden<br>*Namn på förfrågan<br>*Namnet på den användare som stängde begäran<br>*Datum för daglig sammandrag </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon har tilldelats min begäran</strong> </p> <p>Den primära kontakten för utgåvan får ett e-postmeddelande när en användare tilldelas utgåvan, såvida inte den primära kontakten och den tilldelade användaren är samma användare.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet har konfigurerats som en [!UICONTROL Help Request Queue] (enligt beskrivning i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL has been assigned to your request]: "&lt;request name=""&gt;"</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namn på begäran<br>Typ av begäran<br>Angivet den<br>Ärendeprioritet<br>Primär kontakt<br>Planerat slutförandedatum<br>Ärendestatus<br><strong>Mer information</strong> knapp <br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal tilldelade begäranden<br>*Namn på förfrågan<br>*Namn tilldelat<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Statusändringarna för ett projekt som jag har skapat</strong> </p> <p>Användaren som skapade projektet får ett e-postmeddelande när projektstatusen ändras.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project Status Change]: &lt;project name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namnet på den användare som ändrade statusen<br>Ny status<br>Datum och tid när projektstatus ändrades<br>Status för föregående projekt<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Ny projektstatus<br>*Namnet på den användare som ändrade projektstatus<br>*Datum för daglig sammandrag</p> </td> 
   <td> <p><strong>Direkt</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Statusen ändras på min begäran</strong> </p> <p>Den primära kontakten för problemet får ett e-postmeddelande när utgivningsstatusen ändras, såvida inte den användare som ändrade statusen också är den primära kontakten.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och projektet har konfigurerats som en [!UICONTROL Help Request Queue] (enligt beskrivning i <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;request name=""&gt; är &lt;new status=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> Sammandrag av dina förfrågningar &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Namn på begäran<br>Projektnamn<br>Referensnummer för begäran<br>Namnet på den användare som ändrade status för begäran<br>Ny status<br>Datum och tid när status för begäran ändrades<br>Status för föregående begäran<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal begäranden vars status har ändrats<br>*Namn på förfrågan<br>*Status för föregående begäran<br>*Status för ny begäran<br>*Namnet på den användare som ändrade statusen<br>*Datum för den dagliga sammandraget<br></td> 
   <td> <p><strong>Dagligen</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
