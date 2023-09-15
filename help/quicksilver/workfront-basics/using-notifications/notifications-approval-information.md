---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Godkännandeinformation'
description: Följande meddelanden informerar dig om godkännandeaktiviteter för en arbetsuppgift som du är inblandad i. Mer information om hur du konfigurerar vilka meddelanden du får finns i Ändra dina egna e-postmeddelanden.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Meddelanden: Godkännandeinformation

Följande meddelanden informerar dig om godkännandeaktiviteter för en arbetsuppgift som du är inblandad i. Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>En begäran om delegerat godkännande av utfärdande har slutförts</strong> </p> <p>Ett utfärdandegodkännande som du delegerat till en annan användare godkändes eller avvisades av den användaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue Approval/ Rejection Made on Your Behalf by] &lt;user name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som godkände/avvisade problemet för din räkning<br>Godkännandebeslut<br>Ärendestatus<br>Namn på den användare som begärde godkännandet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektets referensnummer<br>*Projektnamn<br>*Totalt antal delegerade utgåvor<br>*Ärendenamn<br>*Godkännarens namn<br>*Datum för den dagliga sammandraget<br><br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En delegerad begäran om projektgodkännande har slutförts</strong> </p> <p>Ett projektgodkännande som du har delegerat till en annan användare godkändes eller avvisades av den användaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project Approval/ Rejection Made on Your Behalf by] &lt;user name=""&gt;</em></p> <p><em>Det dagliga sammandraget innehåller följande uppgifter: [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Projektnamn<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br>Namnet på den användare som godkände/avvisade projektet för din räkning<br>[!UICONTROL Approval Decision]<br>[!UICONTROL Project Status]<br>Namn på den användare som begärde godkännandet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektets referensnummer<br>*Projektnamn<br>*Godkännarens namn<br>[!UICONTROL *Date of the daily digest]<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om godkännande av delegerad uppgift har slutförts</strong> </p> <p>Ett aktivitetsgodkännande som du har delegerat till en annan användare godkändes eller avvisades av den användaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Task Approval/ Rejection Made on Your Behalf by] &lt;user name=""&gt;</em></p> <p>Det dagliga sammandraget innehåller följande uppgifter:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som godkände/avvisade uppgiften åt dig<br>Godkännandebeslut<br>Aktivitetsstatus<br>Namn på den användare som begärde godkännandet<br><strong>Mer information</strong> knapp<br>*Projektets referensnummer<br>*Projektnamn<br>*Totalt antal godkännanden av delegerade uppgifter<br>*Aktivitetsnamn<br>*Godkännarens namn<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om dokumentgodkännande har avbrutits</strong> </p> <p>Dokumentgodkännaren får ett e-postmeddelande när dokumentets godkännandebegäran avbryts.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;user name=""&gt; [!UICONTROL canceled the document approval request]</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> Namnet på den användare som avbröt godkännandebegäran<br>[!UICONTROL Document Name] </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag har utsetts till godkännare</strong> </p> <p>Om någon har delegerat ett godkännande till dig får du ett e-postmeddelande. </p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Delegated] &lt;object type=""&gt; [!UICONTROL Approval - Please Review] &lt;object name=""&gt;</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Namnet på den användare som skickade objektet för godkännande<br>Namnet på den användare för vilken du godkänner objektet<br>Objektstatus<br>Datum och tid när godkännandet begärdes<br>Objektprioritet<br>Namn på godkännandesteg<br>[!UICONTROL Planned Completion Date] för objektet<br><strong>[!UICONTROL Make Approval Decision]</strong> knapp</p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Min tidrapport har godkänts</strong> </p> <p>När tidrapporten har godkänts får du ett e-postmeddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Timesheet Approved]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> Namn på den användare som godkände din tidrapport<br>Datum och tid då tidrapporten godkändes<br>Status för tidrapport ([!UICONTROL Approved])<br>Startdatum och slutdatum för tidrapport<br>Totalt antal loggade timmar i tidrapporten<br>Övertidstimmar som loggats i tidrapporten </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
 </tbody> 
</table>
