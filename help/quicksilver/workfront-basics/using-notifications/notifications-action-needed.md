---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Åtgärd krävs'
description: Följande meddelanden talar om för dig om du behöver utföra en åtgärd på en arbetsuppgift. Mer information om hur du konfigurerar vilka meddelanden du får finns i Ändra dina egna e-postmeddelanden.
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 0%

---

# Meddelanden: [!UICONTROL Action needed]

Följande meddelanden talar om för dig om du behöver utföra en åtgärd på en arbetsuppgift. Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Jag får en ny arbetsförfrågan</strong> </p> <p>Den som har tilldelats arbetsuppgiften får ett e-postmeddelande, såvida inte den som har gjort begäran också är tilldelad. </p> <p>Ett meddelande skickas inte om aktivitetsstatusen är [!UICONTROL Complete] eller utgivningsstatusen är [!UICONTROL Closed].</p> <p>Användare med en [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL New Work Request]: &lt;request name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter: <em>[!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Aktivitetsnamn</p> <p>[!UICONTROL Planned Completion Date]</p> <p>Överordnade</p> <p>Tilldelad av</p> <p>Tilldelad till</p> <p>[!UICONTROL Status]</p> <p>[!UICONTROL Description]</p> <p>[!UICONTROL View] knapp<br>Alternativ för att lägga till i den dagliga sammanfattningen</p> <br> </td> 
   <td><strong>Direkt och</strong> <strong>Dagligen</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste godkänna ett dokument</strong> </p> <p>Godkännaren av ett dokument får ett meddelande när de listas som godkännare.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;name of="" the="" user="" who="" submitted="" the="" approval=""&gt; [!UICONTROL asked you to approve a document in [!DNL Adobe Workfront].]</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Namn på den användare som skickade godkännandet<br>Dokumentnamn<br>Dokumentets referensnummer<br>Datum och tid för begärd godkännande<br>Dokumentinformation (format, storlek, versionsnummer)<br><strong>[!UICONTROL Make Approval Decision]</strong> knapp<br>*Totalt antal väntande dokumentgodkännanden<br>*Länk till <strong>[!UICONTROL Document Approvals</strong>*<strong>See All Approvals]</strong> knapp<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste godkänna ett projekt</strong> </p> <p>Vid godkännande av jobbroller, vilka användare som får ett e-postmeddelande för den här händelsen, beror på om '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]inställningen är aktiverad (enligt beskrivningen i <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurera globala inställningar för godkännande</a>). </p> <p><strong>Om det här alternativet är aktiverat</strong>, skickas ett e-postmeddelande till alla användare i systemet med den jobbroll som är associerad med godkännandet. </p> <p><strong>Om det här alternativet är inaktiverat</strong>, får endast projektgruppsmedlemmar med den jobbroll som är associerad med godkännandeprocessen ett e-postmeddelande.</p> <p>Om godkännandet är kopplat till en användare får användaren meddelandet.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project Pending Approval]: &lt;project name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namn på den användare som skickade godkännandet<br>Väntande godkännandestatus<br>Datum och tid för begärd godkännande<br>Projektprioritet<br>Godkännandesteg väntar på godkännande<br>Antal beslut som väntar på godkännande<br>Namn på godkännare (endast användare)<br>[!UICONTROL Project Planned Completion Date] <br><strong>[!UICONTROL Make Approval Decision]</strong> knapp<br>*Totalt antal väntande projektgodkännanden <br>*Länk till <strong>[!UICONTROL Project Approvals]</strong><br>*<strong>[!UICONTROL See All Approvals]</strong> knapp<br>*Datum för den dagliga sammandraget</p> </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste godkänna en uppgift</strong> </p> <p>Vid godkännande av jobbroller, vilka användare som får ett e-postmeddelande för den här händelsen, beror på om '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]inställningen är aktiverad (enligt beskrivningen i <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurera globala inställningar för godkännande</a>). </p> <p><strong>Om det här alternativet är aktiverat</strong>, skickas ett e-postmeddelande till alla användare i systemet med den jobbroll som är associerad med godkännandet. </p> <p><strong>Om det här alternativet är inaktiverat</strong>, får endast projektgruppsmedlemmar med den jobbroll som är associerad med godkännandeprocessen ett e-postmeddelande.</p> <p>Om godkännandet är kopplat till en användare får användaren meddelandet. </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Task Pending Approval]: &lt;task name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Aktivitetsnamn<br>Projektnamn<br>Namn på den användare som skickade godkännandet<br>Väntande godkännandestatus<br>Datum och tid för begärd godkännande<br>Aktivitetsprioritet<br>Namn på godkännandefas<br>Namn på godkännare<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knapp<br>*Totalt antal väntande aktivitetsgodkännanden<br>*Länk till<strong>[!UICONTROL Task Approvals *See All Approvals]</strong> knapp<strong></strong>*Datum för den dagliga sammandraget<br></p> </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste godkänna en tidrapport</strong> </p> <p>Godkännaren av tidrapporten får ett e-postmeddelande när en tidrapport som de måste godkänna skickas, såvida inte användaren som skickade tidrapporten också är godkännare av tidrapporten.</p> <p>Ett meddelande skickas bara om tidrapportens status är [!UICONTROL Submitted].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Timesheet Submitted]: &lt;timesheet owner=""&gt;, &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> Namn på den användare som skickade tidrapporten för godkännande<br>Datum och tid då tidrapporten skickades<br>Status för tidrapporten<br>Start- och slutdatum för tidrapporten<br>Antal timmar som är inloggade på tidrapporten<br>Antal övertidstimmar som är loggade på tidrapporten<br><strong>[!UICONTROL Review]</strong> och <strong>[!UICONTROL Approve]</strong> knappar<br>*Totalt antal väntande tidrapportgodkännanden<br>*Länk till <strong>[!UICONTROL Timesheet Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knapp<br>*Datum för den dagliga sammandraget </td> 
   <td><strong>Direkt och</strong> <strong>Dagligen</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste godkänna ett problem</strong> </p> <p>Vid godkännande av jobbroller, vilka användare som får ett e-postmeddelande för den här händelsen, beror på om '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]inställningen är aktiverad (enligt beskrivningen i <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL Configure global approval] inställningar</a>). </p> <p><strong>Om det här alternativet är aktiverat</strong>, skickas ett e-postmeddelande till alla användare i systemet med den jobbroll som är associerad med godkännandet. </p> <p><strong>Om det här alternativet är inaktiverat</strong>, får endast projektgruppsmedlemmar med den jobbroll som är associerad med godkännandeprocessen ett e-postmeddelande.</p> <p>Om godkännandet är kopplat till en användare får användaren meddelandet. </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue Pending Approval]: &lt;issue name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namn på den användare som skickade utgåvan för godkännande<br>Väntande godkännandestatus<br>Datum och tid för begärd godkännande<br>Ärendeprioritet<br>Godkännandefas<br>Namn på godkännare<br>[!UICONTROL Issue Planned Completion Date]<br>[!UICONTROL Primary Contact]<br><strong>[!UICONTROL Make Approval Decision]</strong> knapp<br>*Det totala antalet väntande utleveranser<br>*Länk till <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knapp<br>*Datum för den dagliga sammandraget </td> 
   <td><strong>Direkt och</strong> <strong>Dagligen</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste granska ett projektgodkännande som jag har delegerats</strong> </p> <p>Ett projektgodkännande har delegerats till dig och du måste granska det.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Delegated Project Approval - Please Review] &lt;project name=""&gt;</em></p> <p><em>Det dagliga sammandraget innehåller följande uppgifter: [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namnet på den användare som bad om godkännande<br>Namnet på den användare för vars räkning du godkänner projektet<br>Väntande godkännandestatus<br>Datum och tid för begärd godkännande<br>Projektprioritet<br>Godkännandesteg<br>Namn på godkännare<br>[!UICONTROL Project Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knapp<br>*Totalt antal väntande projektgodkännanden<br>*Länk till <strong>[!UICONTROL Project Approvals *See All Approvals]</strong> knapp <br>*Datum för den dagliga sammandraget </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste granska ett uppgiftsgodkännande som jag har delegerats</strong> </p> <p>Ett godkännande av en uppgift har delegerats till dig och du måste granska det.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Delegated Task Approval - Please Review ]&lt;task name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som bad om godkännande<br>Namnet på den användare för vars räkning du godkänner uppgiften<br>Väntande godkännandestatus<br>Datum och tid för begärd godkännande<br>Aktivitetsprioritet<br>Godkännandefas<br>Namn på godkännare<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> knapp <br>*Totalt antal väntande aktivitetsgodkännanden<br>*Länk till <strong>[!UICONTROL Task Approvals *See All Approvals]</strong> knapp<br>*Datum för den dagliga sammandraget </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag måste granska ett godkännande av ett ärende som jag har delegerats</strong> </p> <p>Du har fått ett godkännande av ett ärende och du måste granska det.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Delegated Issue Approval - Please Review] &lt;issue name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som bad om godkännande<br>Namnet på den användare för vars räkning du godkänner problemet<br>Väntande godkännandestatus<br>Datum och tid för begärd godkännande<br>Ärendeprioritet<br>Godkännandefas<br>Namn på godkännare<br>Planerat slutdatum för problem<br>Primär kontakt<br><strong>[!UICONTROL Make Approval Decision]</strong> knapp<br>*Totalt antal väntande utfärdandegodkännanden<br>*Länk till <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> knapp<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag har tilldelats ett ärende</strong> </p> <p>Den som tilldelats utgåvan får ett e-postmeddelande. Den som tilldelat utgåvan får inget e-postmeddelande om status för utgåvan är eller är lika med [!UICONTROL Closed].</p> <p>Användare med en [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL New Work Request]: &lt;issue name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Ärendenamn<br>Projektnamn<br>[!UICONTROL Issue Reference Number]<br>Ditt namn<br>Utgivningens förfallodatum ([!UICONTROL Planned Completion Date])<br>Namnet på den användare som tilldelade utgåvan till dig<br><strong>[!UICONTROL Work On It]</strong> knapp<br>*Totalt antal tilldelningar<br>*Totalt antal uppgifter och ärenden som tilldelats dig<br>*Länk till <strong>[!UICONTROL Work Requests]</strong><br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag är angiven som primär tilldelare för en uppgift</strong> </p> <p>Uppgiftstilldelaren får ett e-postmeddelande om han eller hon är den primära tilldelaren för uppgiften, såvida inte den som tilldelat uppgiften är den användare som tilldelat uppgiften.</p> <p>Ett meddelande skickas om projektstatusen är [!UICONTROL Current] och aktiviteten är inte markerad [!UICONTROL Complete].</p> <p>Användare med en [!UICONTROL Review] eller [!UICONTROL Requestor] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL New Work Request]: &lt;task name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Ditt namn<br>Aktivitetens förfallodatum ([!UICONTROL Planned Completion Date])<br>Namnet på den användare som tilldelade uppgiften till dig<br><strong>[!UICONTROL Work On It]</strong> knapp<br>*Totalt antal uppgifter och ärenden som tilldelats dig<br>*Länk till <strong>[!UICONTROL Work Requests]</strong>*Datum för den dagliga sammandraget </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mitt team får en ny arbetsförfrågan</strong> </p> <p>Teammedlemmar får ett e-postmeddelande när teamet får en ny arbetsförfrågan. (Användaren som skickade begäran får inget meddelande om han eller hon är medlem i gruppen.)</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och arbetsförfrågans status är [!UICONTROL New].</p> <p>Användare med en [!UICONTROL Review] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL New Work Request]: &lt;request name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter: <em>[!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p> Ärendenamn<br>Projektnamn (namn på begärandekö)<br>Ärendereferensnummer<br>Teamnamn<br>Förfallodatum för utfärdande (planerat slutförandedatum)<br>Namn på den användare som skickade begäran<br><strong>[!UICONTROL Work On It]</strong> knapp<br>*Totalt antal förfrågningar som tilldelats ditt team</p> <p>*Namn på arbetsbegäran</p> <p>[!UICONTROL *Planned Completion Date]</p> <p>*Namn på den användare som skickade begäran<br>*Länk till <strong>[!UICONTROL Team Requests]</strong><br>*Datum för den dagliga sammandraget </p> <p><span class="preview">*Teamtilldelningar</span> </p> </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Min tidrapport öppnas igen</strong> </p> <p>Ägaren av tidrapporten får ett e-postmeddelande när tidrapporten öppnas igen, såvida inte användaren som öppnat tidrapporten också är ägare till tidrapporten.</p> <p>Ett e-postmeddelande skickas bara om tidrapportens status är [!UICONTROL Open].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Timesheet Re-opened]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </td> 
   <td> Namnet på den användare som öppnade tidrapporten igen<br>Datum och tid när tidrapporten öppnades igen<br>Status för tidrapporten ([!UICONTROL Re-opened])<br>Antal loggade totalt antal timmar i tidrapporten<br>Antal övertidstimmar som är loggade på tidrapporten<br><strong>[!UICONTROL Review]</strong> knapp </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Min tidrapport har avvisats</strong> </p> <p>Ägaren av tidrapporten får ett e-postmeddelande när tidrapporten avvisas, såvida inte användaren som avvisade tidrapporten också är ägare.</p> <p>Ett e-postmeddelande skickas bara om tidrapportens status är [!UICONTROL Rejected].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Timesheet Rejected]:&lt;start date="" of="" the="" timesheet=""&gt; - &lt;end date="" of="" the="" timesheet=""&gt;</em></p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </td> 
   <td> Namnet på den användare som avvisade tidrapporten<br>Status för tidrapporten ([!UICONTROL Rejected])<br>Datum och tid då tidrapporten avvisades<br><strong>[!UICONTROL Review]</strong> knapp </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon begär åtkomst från mig</strong> </p> <p>Be mig göra något, så sätt på den.</p> <p>Den person som skapar projektet får åtkomst till det.</p> <p>Detta gör att användaren får ett meddelande när någon begär åtkomst.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;name of="" user="" who="" requested="" the="" access=""&gt; [!UICONTROL needs access to] &lt;object name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Action Needed] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Objektnamn<br>Namn på överordnat objekt<br>Objektreferensnummer<br>Namnet på den användare som begärde åtkomst<br>Den typ av åtkomst som användaren begär<br><strong>[!UICONTROL Grant] &lt;name of="" the="" access="" requested=""&gt; Åtkomst</strong> och <strong>[!UICONTROL Grant different access]</strong> knappar<br>*Totalt antal väntande åtkomstförfrågningar<br>*Länk till <strong>[!UICONTROL Access Request]</strong> Godkännanden<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Direkt och dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon ber mig ladda upp ett dokument</strong> </p> <p>Dokumentbegäran får ett e-postmeddelande när en användare tar emot en begäran om att överföra ett dokument.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;name of="" the="" user="" requesting="" the="" document=""&gt; [!UICONTROL needs a document from you in [!DNL Workfront].]</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> Namnet på den användare som begär dokumentet<br>Namnet på objektet som dokumentet ska överföras till<br><strong>[!UICONTROL Attach it here]</strong> link </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
 </tbody> 
</table>
