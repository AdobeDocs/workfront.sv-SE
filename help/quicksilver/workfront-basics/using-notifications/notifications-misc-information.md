---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Övrig information'
description: Följande meddelanden informerar dig om aktiviteter som utförs i ett projekt som du sponsrar.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Meddelanden: Övrig information

Följande meddelanden informerar dig om aktiviteter som utförs i ett projekt som du sponsrar.

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Se även [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Du kan inte aktivera eller inaktivera dagliga meddelanden och du får inte dagliga sammandrag via e-post för händelserna i den här kategorin. Du kan aktivera eller inaktivera enskilda snabbmeddelanden för [!UICONTROL Miscellaneous] kategori.

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
   <td> <p><strong>Ett meddelande skickas till [!UICONTROL Announcement Center]</strong> </p> <p>Du får ett e-postmeddelande när ett nytt meddelande har skickats till [!UICONTROL Announcement Center]. </p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL [!DNL Adobe Workfront] Meddelande]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Ämne för meddelandet<br>Texten i meddelandet som ingår i meddelandet<br>Bifogade dokument<br>Namnet på den användare som skickade meddelandet<br>Datum och tid då meddelandet skickades </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En ändring av en uppgiftstilldelning påverkar en av mina medarbetare</strong> </p> <p>När en av de direkta rapporterna för en användare som har utsetts till chef tilldelas en ny uppgift får chefen ett e-postmeddelande om uppdraget. </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Task Resource Assignment]: &lt;task name=""&gt;</em></p> </td> 
   <td>Projektnamn<br>Aktivitetsnamn<br>Datum och tid när uppgiften skapades<br>Namnet på den användare som skapade uppgiften<br>Uppdragsnamn<br>Förfallodatum (planerat slutförandedatum)<br>Aktivitetsstatus<br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Efter att ha tagit emot en begäran om dokumentöverföring avbryts begäran</strong> </p> <p>Dokumentbegäran får ett e-postmeddelande när en dokumentbegäran avbryts.</p> <p>Ämnet för e-postmeddelandet är: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; avbröt dokumentbegäran. </em></p> <p>Följande text finns i e-postmeddelandets brödtext:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL no longer needs you to upload anything regarding the request you got earlier. We just wanted to let you know.]</em> </p> </td> 
   <td>Namnet på den användare som avbröt begäran<br>Texten i den ursprungliga dokumentöverföringsbegäran<br>A "[!UICONTROL CANCELED]" banner over the original document request<br>Datum och tid för den ursprungliga dokumentbegäran<br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett fel som kräver min uppmärksamhet hittades</strong> </p> <p>Användaren som svarar på en kommentar via e-post får ett e-postmeddelande när svaret inte kan levereras.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Failed to Process on] &lt;subject of="" original="" message=""&gt;</em></p> <p>Mer information om hur du använder e-post för att svara på kommentarer finns i <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Svara på e-postmeddelanden</a>.</p> </td>
   <td> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En ändring av en problemtilldelning påverkar en av mina medarbetare</strong> </p> <p>Hanteraren för en användare som tilldelats ett problem får ett e-postmeddelande när användaren tas bort från eller tilldelas till ett problem. </p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> <p>Ämnet för e-postmeddelandet är: <em>Ärendetilldelning: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som tilldelades<br>Ärendetyp<br>Namn på den användare som är tilldelad utgåvan<br>Angivet utgivningsdatum<br>Ärendeprioritet<br>Primär kontakt<br>Problem [!UICONTROL Planned Completion Date]<br>Ärendestatus<br><strong>[!UICONTROL See More Details]</strong> knapp</p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En av mina medarbetare läggs till i ett projekt</strong> </p> <p>En projektledare får ett e-postmeddelande när någon av användarna läggs till i ett projekt. Det här meddelandet skickas oavsett projektets status. </p> <p>Användare med en [!UICONTROL Review] licensen får inget meddelande.</p> <p>E-postmeddelandet innehåller följande: <em>Projekttilldelning: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namnet på den användare som lade till personen i projektet<br>Namnet på den användare som lades till i projektet<br>Projekt [!UICONTROL Planned Start Date]<br>Projekt [!UICONTROL Planned Completion Date]<br>Procent färdigt projekt<br>Namn på andra i projektet<br>Projektstatus<br>Projektägare<br><strong>[!UICONTROL See More Details]</strong> knapp<br><br><br></p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon lägger till ett projekt i en portfölj eller ett program som jag äger</strong> </p> <p>Portföljen och/eller programägaren får ett meddelande när ett nytt projekt läggs till i en portfölj eller ett program.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project added to] &lt;portfolio name=""&gt;[Project GUID]</em></p> </td> 
   <td> Portfolio<br>Projektets referensnummer<br>Namnet på den användare som lade till projektet i portföljen/programmet<br><br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon delar objekt med mig</strong> </p> <p>Du får ett e-postmeddelande när någon lägger till dig i [!UICONTROL Sharing] lista med behörigheter för ett objekt.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Access Granted]: &lt;object name=""&gt;</em></p> <p>Ett meddelande skickas bara om projektet är i [!UICONTROL Current] status.</p> </td> 
   <td> Objektnamn<br>Namn på överordnat objekt<br>Objektreferensnummer<br>Ursprunglig åtkomst till objektet<br>Ny åtkomst tilldelad objektet<br>Datum och tid då åtkomsten beviljades <br>Namnet på den användare som beviljade åtkomsten </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon delar ett objekt med mitt team</strong> </p> <p>Du får ett e-postmeddelande när någon lägger till ditt team i listan Delning av behörigheter för ett objekt.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Access Granted]: &lt;object name=""&gt; [GUID för åtkomstregel]</em></p> </td> 
   <td> Objektnamn<br>Namn på överordnat objekt<br>Objektreferensnummer<br>Gammal åtkomst<br>Ny åtkomst<br>Datum och tid då åtkomsten beviljades<br>Namn på ditt team<br>Namnet på den användare som beviljade åtkomsten </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En uppdatering görs av en uppgift, ett problem eller ett projekt som jag prenumererar på</strong> </p> <p>Du får ett e-postmeddelande när någon kommenterar ett objekt som du prenumererar på.</p> <p>Ämnet för prenumerationens e-postmeddelande är: <em>[!UICONTROL An update was made to the] &lt;object type=""&gt; du prenumererar på: &lt;object name=""&gt;</em></p> </td> 
   <td> Objektnamn<br> Objektreferensnummer<br> Namnet på den användare som kommenterade det prenumererade objektet<br> Datumkommentar har gjorts<br> Kommentar har lagts till i det prenumererade objektet  </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
 </tbody> 
</table>
