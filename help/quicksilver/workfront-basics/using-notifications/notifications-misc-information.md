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
source-wordcount: '884'
ht-degree: 0%

---

# Meddelanden: Övrig information

Följande meddelanden informerar dig om aktiviteter som utförs i ett projekt som du sponsrar.

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Se även [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Du kan inte aktivera eller inaktivera dagliga meddelanden och du får inte dagliga sammandrag via e-post för händelserna i den här kategorin. Du kan aktivera eller inaktivera enskilda snabbmeddelanden för kategorin [!UICONTROL Miscellaneous].

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
   <td> <p><strong>Ett meddelande skickas till [!UICONTROL Announcement Center]</strong> </p> <p>Du får ett e-postmeddelande när ett nytt meddelande har skickats till [!UICONTROL Announcement Center]. </p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL [!DNL Adobe Workfront] Meddelande]: &lt;Ämne för meddelandet&gt;</em></p> </td> 
   <td> Ämne för meddelandet<br>Texten i meddelandet finns i meddelandet<br>Bifogade dokument<br>Namnet på användaren som skickade meddelandet<br>Datum och tid när meddelandet skickades </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En ändring i aktivitetstilldelningen påverkar någon av mina personer</strong> </p> <p>När en av de direkta rapporterna för en användare som har utsetts till chef tilldelas en ny uppgift får chefen ett e-postmeddelande om uppdraget. </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Task Resource Assignment]: &lt;Aktivitetsnamn&gt;</em></p> </td> 
   <td>Projektnamn<br>Aktivitetsnamn<br>Datum och tid när aktiviteten skapades<br>Namn på den användare som skapade aktiviteten<br>Tilldelningsnamn<br>Förfallodatum (planerat slutförandedatum)<br>Aktivitetsstatus<br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Efter att ha tagit emot en begäran om dokumentöverföring avbryts begäran</strong> </p> <p>Dokumentbegäran får ett e-postmeddelande när en dokumentbegäran avbryts.</p> <p>Ämnet för e-postmeddelandet med snabbmeddelanden är: <em>&lt;Namnet på den användare som avbröt begäran&gt; avbröt dokumentbegäran. </em></p> <p>Följande text finns i e-postmeddelandets brödtext:</p> <p><em>[!UICONTROL Hi] &lt;Ditt namn&gt;, <br><br>&lt;Namnet på den användare som avbröt begäran&gt;[!UICONTROL no longer needs you to upload anything regarding the request you got earlier. We just wanted to let you know.]</em> </p> </td> 
   <td>Namnet på den användare som avbröt begäran<br>Texten i den ursprungliga dokumentöverföringsbegäran<br>En [!UICONTROL CANCELED]-banderoll över den ursprungliga dokumentbegäran<br>Datum och tid för den ursprungliga dokumentbegäran<br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett fel som kräver min uppmärksamhet hittades</strong> </p> <p>Användaren som svarar på en kommentar via e-post får ett e-postmeddelande när svaret inte kan levereras.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Failed to Process on] &lt;ämnet i det ursprungliga meddelandet&gt;</em></p> <p>Mer information om hur du använder e-post för att svara på kommentarer finns i <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Svara på e-postmeddelanden</a>.</p> </td>
   <td> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En ändring i en problemtilldelning påverkar en av mina medarbetare</strong> </p> <p>Hanteraren för en användare som tilldelats ett problem får ett e-postmeddelande när användaren tas bort från eller tilldelas till ett problem. </p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> <p>Ämnet för e-postmeddelandet med snabbmeddelanden är: <em>Utgåva: &lt;Utgivningsnamn&gt;</em></p> </td> 
   <td> <p>Utfärdningsnamn<br>Projektnamn<br>Utfärdningsreferensnummer<br>Namnet på den användare som tilldelades <br>Utgivningstypen<br>Namnet på den användare som tilldelats utgåvan<br>Angivet den <br>Utfärdandeprioritet<br>Primär kontakt<br>Utgåva [!UICONTROL Planned Completion Date]<br>Utgivningsstatus<br><strong>[!UICONTROL See More Details]</strong></p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En av mina medarbetare läggs till i ett projekt</strong> </p> <p>En projektledare får ett e-postmeddelande när någon av användarna läggs till i ett projekt. Det här meddelandet skickas oavsett projektets status. </p> <p>Användare med en [!UICONTROL Review]-licens får inget meddelande.</p> <p>E-postmeddelandets ämne är: <em>Projekttilldelning: &lt;Användarnamn&gt;[&lt;Project GUID&gt;_ &lt;Användarens GUID&gt;]</em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio <br>Projektreferensnummer<br>Namn på den användare som lade till personen i projektet<br>Namn på den användare som lades till i projektet<br>Projekt [!UICONTROL Planned Start Date]<br>Projektprocent [!UICONTROL Planned Completion Date]<br>Projektprocent slutfört<br>Namn på andra i projekt<br>Projektstatus<br>Projektägare<br><strong>[!UICONTROL See More Details]</strong><br><br><br></p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon lägger till ett projekt i en portfölj eller ett program som jag äger</strong> </p> <p>Portföljen och/eller programägaren får ett meddelande när ett nytt projekt läggs till i en portfölj eller ett program.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project added to] &lt;Portfolio-namn&gt;[Projekt-GUID]</em></p> </td> 
   <td> Portfolio-namn<br>Projektreferensnummer<br>Namnet på den användare som lade till projektet i portföljen/programmet<br><br></td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon delar ett objekt med mig</strong> </p> <p>Du får ett e-postmeddelande när någon lägger till dig i listan [!UICONTROL Sharing] med behörigheter för ett objekt.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Access Granted]: </em></p> <p>Ett meddelande skickas bara om projektet har statusen [!UICONTROL Current].</p> </td> 
   <td> Objektnamn<br>Namn på överordnat objekt<br>Objektreferensnummer<br>Ursprunglig åtkomst till objektet<br>Ny åtkomst beviljad till objektet<br>Datum och tid när åtkomst beviljades <br>Namn på användaren som beviljade åtkomst </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Någon delar ett objekt med mitt team</strong> </p> <p>Du får ett e-postmeddelande när någon lägger till ditt team i listan Delning av behörigheter för ett objekt.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Access Granted]: &lt;Objektnamn&gt; [GUID för åtkomstregel]</em></p> </td> 
   <td> Objektnamn<br>Namn på överordnat objekt<br>Objektreferensnummer<br>Gammal åtkomst<br>Ny åtkomst<br>Datum och tid när åtkomst beviljades<br>Namn på ditt team<br>Namn på den användare som beviljade åtkomst </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En uppdatering görs av en aktivitet, ett problem eller ett projekt som jag prenumererar på</strong> </p> <p>Du får ett e-postmeddelande när någon kommenterar ett objekt som du prenumererar på.</p> <p>Ämnet för prenumerationens e-postmeddelande är: <em>[!UICONTROL An update was made to the] &lt;Objekttyp&gt; som du prenumererar på: &lt;Objektnamn&gt;</em></p> </td> 
   <td> Objektnamn <br> Objektreferensnummer <br> Namnet på den användare som gjorde en kommentar på det prenumererade objektet <br> Datumkommentaren gjordes <br> till det prenumererade objektet  </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
 </tbody> 
</table>
