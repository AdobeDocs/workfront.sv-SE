---
content-type: reference
navigation-topic: notifications
title: "Meddelanden: Information om projekt jag är på"
description: Följande meddelanden informerar dig om aktiviteter som utförs i projekt som du arbetar med.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1389'
ht-degree: 0%

---

# Meddelanden: Information om projekt som jag är på

Följande meddelanden informerar dig om aktiviteter som utförs i projekt som du arbetar med.

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
   <td> <p><strong>Ett dokument läggs till i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett dokument läggs till i projektet, med undantag för den användare som lade till dokumentet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och dokumentet är inte privat.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Document added to] &lt;project name=""&gt;</em></p> <p>Ämnet för den dagliga sammandragsanmälan är <em>[!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Dokumentets referensnummer<br>Namnet på den användare som lade till dokumentet<br>Dokumentnamn<br>Tillagd den<br>Dokumentinformation (format, storlek, versionsnummer)<br>Dokumentminiatyr<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal tillagda dokument<br>*Dokumentnamn<br>*Namnet på den användare som överförde dokumentet<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En milstolpe-uppgift har slutförts i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett meddelande när en milstolpe-uppgift i projektet har slutförts. Meddelanden skickas inte när en personlig uppgift har slutförts.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnesraden är <em>[!UICONTROL Complete]: &lt;task name=""&gt; på &lt;project name=""&gt;</em></p> <p>Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som slutförde uppgiften<br>Aktivitetsstatus<br>Datum och tid när uppgiften slutfördes<br>Status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp <br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett projekt som jag håller på att bli aktivt</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när projektstatusen är inställd på [!UICONTROL Current].</p> <p>Obs! Användarna måste listas på fliken Anställda i ett projekt för att få meddelanden när en projektstatus är inställd på [!UICONTROL Current]. Information om hur du lägger till användare i ett projektteam finns i <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Hantera projektgruppen</a>.</p> <p>Ämnet för e-postmeddelandet är <em>&lt;project name=""&gt; [!UICONTROL is Current - Go to your project and see your tasks!]</em></p> <p> Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Projektstatus<br>Projekt [!UICONTROL Planned Completion Date]<br>Projektägare<br>En lista över uppgifter som tilldelats dig, någon av dina jobbroller eller något av dina team<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Projektstatus<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Ett projekt som mitt team är på blir aktivt</strong> <p>Medlemmar i ett team får ett e-postmeddelande när ett projekt blir aktivt. Teamet måste tilldelas minst en uppgift för att kunna ta emot meddelandet.</p><p>Om både en enskild användare och ett team har tilldelats en uppgift i projektet. teamet kommer inte att få något meddelande.</p><p>Ämnet för e-postmeddelandet är <i>&lt;project name=""&gt; [!UICONTROL is Active - Go to your project and see your tasks!]</i></p><p>Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Projektstatus<br>Projekt [!UICONTROL Planned Completion Date]<br>Projektägare<br>En lista över uppgifter som tilldelats ditt team<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Projektstatus<br>*Datum för daglig sammandrag</td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett projekt jag håller på med är slutfört</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när projektstatusen är [!UICONTROL Complete].</p> <p>Tips: Om projekten slutförs regelbundet kan du aktivera det här alternativet för att skapa många e-postmeddelanden för användare som har ett begränsat antal uppgifter i många projekt.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Project Status Change]: &lt;project name=""&gt;</em></p> <p> Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namnet på den användare som slutförde projektet<br>Projektstatus<br>Datum och tid då projektet slutfördes<br>Status för föregående projekt<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Projektstatus<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En uppgift har slutförts i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när en uppgift har slutförts i projektet. <br>Mer information om projektteamet finns i <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Översikt över projektteamet</a>.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Complete]: &lt;task name=""&gt; på &lt;project name=""&gt;</em></p> <p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete]visas fortfarande "[!UICONTROL Complete]".</p> </p> <p><em> Det dagliga sammandraget innehåller följande uppgifter: [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som slutförde uppgiften<br>Aktivitetsstatus<br>Datum och tid när aktivitetens status ändrades<br>Status för föregående aktivitet<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har lagts till i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Issue added to] &lt;project name=""&gt;</em></p> <p> </p> <p> Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Ärendereferensnummer<br>Namnet på den användare som lade till utgåvan<br>Ärendetyp<br>Ärendenamn<br>Angivet den<br>Ärendeprioritet<br>Tilldelad till namn <br>Ärendestatus<br>Primär kontakt<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal ärenden som lagts till i projektet<br>*Ärendenamn<br>*Namnet på den användare som är tilldelad utgåvan<br>*Datum för daglig sammandrag </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har slutförts i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett problem har slutförts i projektet.<br>Mer information om projektteamet finns i <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Översikt över projektteamet</a>.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Complete]: &lt;issue name=""&gt; på &lt;project name=""&gt;</em></p> <p> Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Namnet på den användare som slutförde problemet<br>Ärendestatus<br>Datum och tid då utgåvan slutfördes<br>Status för föregående problem<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda ärenden<br>*Ärendenamn<br>*Namnet på den användare som är tilldelad utgåvan<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett ej tilldelat problem läggs till i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett ej tilldelat problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Who should be assigned to this new issue on] &lt;project name=""&gt;?</em></p> <p> Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Ärendereferensnummer<br>Namnet på den användare som lade till utgåvan<br>Ärendenamn<br>Ärendetyp<br>Angivet den<br>Ärendeprioritet<br>Tilldelad till namn (tom) <br>Ärendestatus<br>Primär kontakt<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal tillagda utgåvor<br>*Ärendenamn<br>*Namnet på den användare som lade till problemet<br>*Datum för den dagliga sammandraget<br></td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag har lagts till i ett projekt</strong> </p> <p>Användaren som lades till i projektet får ett e-postmeddelande när han eller hon läggs till, såvida inte användaren själv har lagt till sig själv i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL You've been added to the project] &lt;project name=""&gt;</em></p> <p> Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namnet på den användare som lade till dig i projektet<br>Projekt [!UICONTROL Planned Start Date]<br>Projekt [!UICONTROL Planned Completion Date]<br>Procent färdigt projekt<br>Namn på andra i projektet <br>Projektägare<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Status ändras för ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när statusen för projektet ändras. <br>Mer information om projektteamet finns i <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Översikt över projektteamet</a>.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Project Status Change]: &lt;project name=""&gt;</em></p> <p> Ämnet för den dagliga sammandragsanmälan är <em> [!UICONTROL Digest of Projects You're On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namnet på den användare som ändrade status för projektet<br>Ny projektstatus<br>Datum och tid när projektets status ändrades<br>Status för föregående projekt<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Projektstatus<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
 </tbody> 
</table>
