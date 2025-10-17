---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Godkännandeinformation'
description: Följande meddelanden informerar dig om godkännandeaktiviteter för en arbetsuppgift som du är inblandad i. Mer information om hur du konfigurerar vilka meddelanden du får finns i Ändra dina egna e-postmeddelanden.
author: Courtney
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
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
   <td> <p><strong>En delegerad godkännandebegäran för utfärdande har slutförts</strong> </p> <p>Ett utfärdandegodkännande som du delegerat till en annan användare godkändes eller avvisades av den användaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue Approval/ Rejection Made on Your Behalf by] &lt;Användarnamn&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Approval Information] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> <p>Utleveransnamn<br>Projektnamn<br>Utfärdarreferensnummer<br>Namn på den användare som godkände/avvisade utgåvan för din räkning<br>Godkännandebeslut<br>Utfärdandestatus<br>Namn på den användare som begärde godkännandet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektreferensnummer<br>*Projektnamn<br>*Totalt antal delegerade utgivningsgodkännanden<br>*Utfärdarnamn<br> <br>*Datum för den dagliga sammandraget<br><br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En delegerad begäran om projektgodkännande har slutförts</strong> </p> <p>Ett projektgodkännande som du har delegerat till en annan användare godkändes eller avvisades av den användaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project Approval/ Rejection Made on Your Behalf by] &lt;Användarnamn&gt;</em></p> <p><em>Ämnet för det dagliga sammandragsmeddelandet är: [!UICONTROL Digest of Approval Information] &lt;Datum för det dagliga sammandraget&gt;</em> </p> </td> 
   <td> Projektnamn<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br>Namnet på den användare som godkände/avvisade projektet åt dig<br>[!UICONTROL Approval Decision]<br>[!UICONTROL Project Status]<br>Namnet på den användare som begärde godkännandet<br><strong>[!UICONTROL See More Details]</strong>-knappen<br>*Projektreferensnummer<br>*Projektnamn<br>*Godkännarens namn<br>[!UICONTROL *Date of the daily digest]<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om godkännande av delegerad aktivitet har slutförts</strong> </p> <p>Ett aktivitetsgodkännande som du har delegerat till en annan användare godkändes eller avvisades av den användaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Task Approval/ Rejection Made on Your Behalf by] &lt;Användarnamn&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är:<em> [!UICONTROL Digest of Approval Information] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på den användare som godkände/avvisade aktiviteten åt dig<br>Godkännandebeslut<br>Aktivitetsstatus<br>Namnet på den användare som begärde godkännandet<br><strong>Se Mer information</strong> Knapp<br>*Projektreferensnummer<br>*Projektnamn<br>*Totalt antal delegerade aktivitetsgodkännanden<br>*Aktivitetsnamn<br>*Godkännanden ver Name<br>*Date of the day digest<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En begäran om dokumentgodkännande har avbrutits</strong> </p> <p>Dokumentgodkännaren får ett e-postmeddelande när dokumentets godkännandebegäran avbryts.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;Användarnamn&gt; [!UICONTROL canceled the document approval request]</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> Namnet på den användare som avbröt godkännandebegäran <br>[!UICONTROL Document Name] </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag har delegerats som godkännare</strong> </p> <p>Om någon har delegerat ett godkännande till dig får du ett e-postmeddelande. </p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Delegated] &lt;Objekttyp&gt; [!UICONTROL Approval - Please Review] &lt;Objektnamn&gt;</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Namn på den användare som skickade objektet för godkännande<br>Namn på den användare för vars räkning du godkänner objektet<br>Objektstatus<br>Datum och tid när godkännandet begärdes<br>Objektprioritet<br>Namn på godkännandesteg<br>[!UICONTROL Planned Completion Date] för knappen Objekt<br><strong>[!UICONTROL Make Approval Decision]</strong></p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Min tidrapport har godkänts</strong> </p> <p>När tidrapporten har godkänts får du ett e-postmeddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Timesheet Approved]: &lt;Startdatum för tidrapport&gt; - &lt;Slutdatum för tidrapport&gt;</em></p> <p> <p>Obs! Du kan inte konfigurera det här meddelandet för ett dagligt sammandrag-e-postmeddelande.</p> </p> </td> 
   <td> Namn på den användare som godkände tidrapporten<br>Datum och tid när tidrapporten godkändes<br>Status för tidrapporten ([!UICONTROL Approved])<br>Startdatum och slutdatum för tidrapporten<br>Totalt antal timmar som loggats i tidrapporten<br>Övertidstimmar som loggats i tidrapporten </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
 </tbody> 
</table>
