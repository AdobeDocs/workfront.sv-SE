---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Kommunikation'
description: Följande meddelanden informerar dig om kommunikation, t.ex. en uppdateringskommentar, som händer med ett arbetsobjekt som du är inblandad i. Mer information om hur du konfigurerar vilka meddelanden du får finns i Ändra dina egna e-postmeddelanden.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 0%

---

# Meddelanden: Meddelande

Följande meddelanden informerar dig om kommunikation, t.ex. en uppdateringskommentar, som händer med ett arbetsobjekt som du är inblandad i. Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>De här meddelandena varnar dig om alla kommentarer som har bokförts för en viss artikel. Därför måste du markera eller avmarkera alla meddelanden på samma gång för att kunna levereras i ett dagligt meddelande. Om du bara vill få meddelanden om vissa kommentarer när de inträffar, kan du ange att de enskilda meddelandena ska skickas direkt.

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
   <td> <p><strong>Någon inkluderar mig i en riktad uppdatering</strong> </p> <p>En riktad uppdatering är när en användare specifikt inkluderar en annan användare i en uppdatering, vilket beskrivs i <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] uppdateringar</a>.</p> <p>I det här fallet får den användare som ingår i den riktade uppdateringen ett e-postmeddelande om uppdateringen.</p> <p>E-postmeddelandet skickas endast om användaren har åtkomstbehörighet till objektet.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;Namnet på den användare som inkluderade dig i uppdateringen&gt; [!UICONTROL wanted you to know]</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är: <em>[!UICONTROL Digest of Communication] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Objektnamn där uppdateringen gjordes<br>Överordnat objektnamn<br>Objektreferensnummer<br>Namn på alla användare och team som ingår i den riktade uppdateringen<br>Datum och tid när uppdateringen gjordes<br>Text för riktad uppdatering<br><strong>[!UICONTROL Comment]</strong> button<br>*Totalt antal kommentarer som tagits emot<br>*Antal kommentarer som tagits emot för varje objekt<br>*<strong>[!UICONTROL See All Notifications]</strong> button<br>*Datum för daglig sammandrag<br></td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon svarar på min förfrågan</strong> </p> <p>När en användare har skickat in en arbetsförfrågan och en annan användare har svarat på den, får användaren som skickade begäran ett e-postmeddelande.</p> <p>Ett e-postmeddelande skickas inte om:</p> 
    <ul> 
     <li> <p>Användaren som svarar är samma användare som gjorde begäran</p> </li> 
     <li> <p>Användaren har inte åtkomst för att se anteckningen</p> </li> 
    </ul><strong>Ämnet i e-postmeddelandet är: <em>[!UICONTROL Comment on] &lt;Namn på begäran&gt; på &lt;Projektnamn&gt; (ref# &lt;Referensnummer för begäran&gt;)</em></strong> Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Communication] &lt;Datum för daglig sammandrag&gt;</em></td> 
   <td> Begärannamn<br>Projektnamn<br>Referensnummer<br>Namn på den användare som besvarade din begäran<br>Datum och tid när kommentaren gjordes<br>Text som gjorts på din begäran<br>*Totalt antal kommentarer som tagits emot<br>*Antal kommentarer som tagits emot för varje begäran<br>*<strong>[!UICONTROL See All Notifications]</strong> knapp<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En kommentar har publicerats på min begäran</strong> </p> <p>Den primära kontakten för en utgåva får ett e-postmeddelande när en kommentar publiceras på en [!UICONTROL Help Desk]-begäran, såvida inte den användare som publicerade kommentaren också är den primära kontakten för utgåvan.</p> <p>Alla användare som är direkt inkluderade i kommentaren får också ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet med snabbmeddelanden är: <em>[!UICONTROL Comment on] &lt;Namn på begäran&gt; på &lt;Projektnamn&gt; (ref# &lt;Referensnummer för begäran&gt;)</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Communication] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Begärannamn<br>Projektnamn<br>Referensnummer<br>Namn på den användare som besvarade din begäran<br>Datum och tid när kommentaren gjordes<br>Text som gjorts på din begäran<br>*Totalt antal kommentarer som tagits emot<br>*Antal kommentarer som tagits emot för varje begäran<br>*Projektnamn<br>*<strong>[!UICONTROL See All Notifications]</strong> knapp<br>*Datum för den dagliga sammandraget<br></td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En kommentar läggs till i mitt dokument</strong> </p> <p>Ägaren till ett dokument i [!DNL Adobe Workfront] får ett e-postmeddelande när en kommentar publiceras i dokumentet, såvida inte den användare som publicerade kommentaren också är dokumentägaren.</p> <p>Alla användare som är direkt inkluderade i kommentaren får också ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current]. </p> <p>Ämnet för e-postmeddelandet med snabbmeddelanden är: <em>[!UICONTROL Comment on] &lt;Namn på begäran&gt; på &lt;Projektnamn&gt; (ref# &lt;Referensnummer för begäran&gt;)</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Communication] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td>Dokumentnamn<br>Projekt-, aktivitets- eller problemnamn<br>Referensnummer<br>Namnet på den användare som besvarade din förfrågan<br>Datum och tid när kommentaren gjordes<br>Text som kommentaren gjordes i dokumentet</td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon kommenterar en tråd som jag är i</strong> </p> <p>Deltagare i tråden och användare som är inkluderade i ett direktmeddelande får ett e-postmeddelande när en användare gör en kommentar i tråden.</p> <p>Användarna måste ha [!UICONTROL View]-åtkomst för att kunna ta emot ett meddelande.</p> <p>Följande användare får inget meddelande:</p> 
    <ul> 
     <li>Team som ingår i ett direktmeddelande</li> 
     <li>Anteckningens ägare</li> 
     <li>Den primära kontakten</li> 
    </ul> <p><strong>Ämnet i e-postmeddelandet är: <em>[!UICONTROL RE: Comment on] &lt;Objektnamn&gt;&lt;Objekttyp&gt; på &lt;Projektnamn&gt;(ref# &lt;Objektreferensnummer&gt;</em>)</strong> </p> <p><strong> Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Communication] &lt;Datum för den dagliga sammandraget&gt;</em></strong> </p> </td> 
   <td> Objektnamn<br>Överordnat objektnamn<br>Namnet på den användare som kommenterade tråden<br>Text som kommenterats i tråden<br>Datum och tid när kommentaren gjordes<br>*Totalt antal kommentarer som tagits emot<br>*Antal kommentarer som tagits emot för varje objekt<br>*Projektnamn<br>*<strong>[!UICONTROL See All Notifications]</strong> knapp<br>*Datum för daglig sammandrag </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon kommenterar något av mina arbetsobjekt</strong> </p> <p>Den som har tilldelats arbetsuppgiften får ett e-postmeddelande när som helst när en användare lägger till en uppdatering av en arbetsuppgift, såvida inte den användare som lägger till uppdateringen också är den som har tilldelats uppgiften. </p> <p>När en kommentar har publicerats på en förfrågan skickar du den primära kontakten via e-post.</p> <p>Den primära kontakten för en utgåva får ett e-postmeddelande när en kommentar publiceras på en förfrågan, såvida inte den användare som publicerade kommentaren också är den primära kontakten för utgåvan.</p> <p>Alla användare som är direkt inkluderade i kommentaren får också ett e-postmeddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Comment on] &lt;Namn på arbetsobjekt&gt; på &lt;Projektnamn (ref# &lt;Referensnummer för arbetsobjekt&gt;)</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Communication] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Arbetsobjektnamn<br>Projektnamn<br>Arbetsobjektets referensnummer<br>Namnet på den användare som kommenterade arbetsobjektet<br>Text för kommentaren som gjorts på arbetsobjektet<br>Datum och tid när kommentaren gjordes<br>*Totalt antal kommentarer som tagits emot<br>*Antal kommentarer som tagits emot för varje objekt<br>*Projektnamn<br>*<strong>[!UICONTROL See All Notifications]</strong> knapp<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon inkluderar mitt team i en dirigerad uppdatering</strong> </p> <p>En riktad uppdatering är när en användare specifikt inkluderar en annan användare i en uppdatering, vilket beskrivs i <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a>.</p> <p>I det här fallet får alla medlemmar i teamet som ingår i den riktade uppdateringen ett e-postmeddelande om uppdateringen.</p> <p>E-postmeddelandet skickas endast till användare som har åtkomstbehörighet till objektet.</p> <p>Om användaren som skickar den dirigerade uppdateringen är medlem i det team som inkluderas får användaren som skickar uppdateringen inget e-postmeddelande.</p> <p>Ämnet för e-postmeddelandet med snabbmeddelanden är: [!UICONTROL Comment on] &lt;objektnamn&gt; på &lt;överordnat objektnamn&gt; (ref# &lt;objektreferensnummer&gt;)</p> <p> Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Communication] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> <p>Objektnamn<br>Överordnat objektnamn<br>Objektreferensnummer<br>Namnet på den användare som gjorde den riktade uppdateringen<br>Namnet på alla team och användare som ingår i den riktade uppdateringen<br>Datum och tid när den riktade uppdateringen gjordes<br>Text för den riktade uppdateringen<br><strong>[!UICONTROL Comment]</strong> knapp<br>*Totalt antal kommentarer som tagits emot <br>*Antal kommentarer som tagits emot för varje objekt<br>*Projektnamn<br>*{1 <strong>[!UICONTROL See All Notifications]</strong> button <br>*Datum för daglig sammandrag </p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>När en kommentar läggs till för användaren</strong> </p> <p>Du kan kommentera en användare på fliken [!UICONTROL Updates] i användarobjektet. Du kan också kommentera en användare när du redigerar användarens inställningar. Användaren som kommentaren görs mot får ett e-postmeddelande om kommentaren. </p> <p>Du måste ha behörighet till minst [!UICONTROL View] användaren för att kunna ange en uppdatering på fliken [!UICONTROL Updates] för användaren. Du måste ha [!UICONTROL Edit] behörigheter för användaren för att kunna redigera användarens inställningar. </p> <p>Mer information om hur du gör kommentarer om användare på fliken Uppdateringar finns i <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Uppdatera arbete</a>.</p> <p>Mer information om hur du anger en kommentar för en användare när du redigerar användarens inställningar finns i <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Konfigurera mina inställningar</a>.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;Användarnamn&gt; [!UICONTROL wanted you to know]</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Communication] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Ditt användarnamn<br>Namnet på den användare som lade till kommentaren<br>Kommentarens text<br>Datum och tid när kommentaren gjordes<br>*Totalt antal kommentarer som togs emot<br>*Antal kommentarer som tagits emot för varje objekt<br>*<strong>[!UICONTROL See All Notifications]</strong> knapp<br>*Datum för daglig sammandrag </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
