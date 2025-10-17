---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Information om projekt som jag är på'
description: Följande meddelanden informerar dig om aktiviteter som utförs i projekt som du arbetar med.
author: Courtney
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Meddelanden: Information om projekt som jag är på

Följande meddelanden informerar dig om aktiviteter som utförs i projekt som du arbetar med.

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
   <td> <p><strong>Ett dokument läggs till i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett dokument läggs till i projektet, med undantag för den användare som lade till dokumentet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och dokumentet inte är privat.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Document added to] &lt;Project Name&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är <em>[!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Projektnamn<br>Portfolio-namn<br>Dokumentreferensnummer<br>Namnet på den användare som lade till dokumentet<br>Dokumentnamn<br>lades till den <br>Dokumentinformation (format, storlek, versionsnummer)<br>Dokumentminiatyrbild<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal dokument som lagts till<br>*Dokumentnamn<br> *Namn på den användare som överförde dokumentet <br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En milstolpeaktivitet har slutförts för ett projekt som jag är på </strong> </p> <p>Medlemmar i ett projektteam får ett meddelande när en milstolpe-uppgift i projektet har slutförts. Meddelanden skickas inte när en personlig uppgift har slutförts.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnesraden är <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt; på &lt;Projektnamn&gt;</em></p> <p>Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt;</em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på användaren som slutförde aktiviteten<br>Aktivitetsstatus<br>Datum och tid när aktiviteten slutfördes<br>Tidigare aktivitetsstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på användaren som slutförde aktiviteten<br>}*Datum för den dagliga sammandraget<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett projekt som jag är på blir aktivt</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när projektstatusen är inställd på [!UICONTROL Current].</p> <p>Obs! Användare måste vara listade på fliken Personal i ett projekt för att få meddelanden när en projektstatus är inställd på [!UICONTROL Current]. Mer information om hur du lägger till användare i ett projektteam finns i <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Hantera projektteamet</a>.</p> <p>Ämnet för e-postmeddelandet är <em>&lt;Projektnamn&gt; [!UICONTROL is Current - Go to your project and see your tasks!]</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio-namn<br>Projektreferensnummer<br>Projektstatus<br>Projekt [!UICONTROL Planned Completion Date]<br>Projektägare<br>En lista över aktiviteter som tilldelats dig, en av dina jobbroller eller en av dina team<br><strong>[!UICONTROL See More Details]</strong>-knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Projektstatus<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Ett projekt som mitt team är på blir aktivt</strong> <p>Medlemmar i ett team får ett e-postmeddelande när ett projekt blir aktivt. Teamet måste tilldelas minst en uppgift för att kunna ta emot meddelandet.</p><p>Om både en enskild användare och ett team har tilldelats en uppgift i projektet. teamet kommer inte att få något meddelande.</p><p>Ämnet för e-postmeddelandet är <i>&lt;Projektnamn&gt; [!UICONTROL is Active - Go to your project and see your tasks!]</i></p><p>Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p></td> 
   <td>Projektnamn<br>Portfolio-namn<br>Projektreferensnummer<br>Projektstatus<br>Projekt [!UICONTROL Planned Completion Date]<br>Projektägare<br>En lista över aktiviteter som har tilldelats ditt team<br><strong>[!UICONTROL See More Details]</strong>-knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Projektstatus<br>*Datum för daglig sammandrag</td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett projekt som jag är i har slutförts</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när projektstatusen är [!UICONTROL Complete].</p> <p>Tips! Om projekten slutförs regelbundet kan du aktivera det här alternativet för att skapa många e-postmeddelanden för användare som har ett begränsat antal uppgifter i många projekt.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Project Status Change]: &lt;Project Name&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio-namn<br>Projektreferensnummer<br>Namnet på den användare som slutförde projektet<br>Projektstatus<br>Datum och tid när projektet slutfördes<br>Tidigare projektstatus<br><strong>[!UICONTROL See More Details]</strong>-knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Projektstatus<br>*Datum för daglig sammandrag<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En aktivitet har slutförts i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när en uppgift har slutförts i projektet. <br>Mer information om projektteamet finns i <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Projektteamöversikt</a>.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt; på &lt;Projektnamn&gt;</em></p> <p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete] visas fortfarande [!UICONTROL Complete] som ämne i e-postmeddelandet.</p> </p> <p><em> Ämnet för det dagliga sammandragsmeddelandet är: [!UICONTROL Digest of Projects You're On] &lt;Datum för det dagliga sammandraget&gt; </em> </p> </td> 
   <td> <p>Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på den användare som slutförde aktiviteten<br>Aktivitetsstatus<br>Datum och tid när aktivitetens status ändrades<br>Tidigare aktivitetsstatus<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namn för användaren som slutförde uppgiften <br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har lagts till i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Issue added to] &lt;Project Name&gt;</em></p> <p> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio-namn<br>Referensnummer<br>Namn på den användare som lade till problemet<br>Utgivningstyp<br>Utgivningsnamn<br>Angivet<br>Utgivningsprioritet<br>Tilldelad till namn <br>Utgivningsstatus<br>Primär kontakt<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal utleveranser som lagts till projektet <br>*Ärendenamn <br>*Namnet på användaren som tilldelats utgåvan <br>*Datum för daglig sammandrag </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har slutförts i ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett problem har slutförts i projektet.<br>Mer information om projektteamet finns i <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Projektteamöversikt</a>.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Complete]: &lt;Issue Name&gt; på &lt;Project name&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p> </td> 
   <td> Utgivningsnamn<br>Projektnamn<br>Namnet på den användare som slutförde utleveransen<br>Utgivningsstatus<br>Datum och tid då utleveransen slutfördes<br>Tidigare utgivningsstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda utleveranser<br>*Utgivningsnamn<br>*Namn på den användare som tilldelats utleveransen<br>*Datum sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett otilldelat problem har lagts till i ett projekt som jag är på </strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när ett ej tilldelat problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Who should be assigned to this new issue on] &lt;Project Name&gt;?</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio-namn<br>Utfärdningsreferensnummer<br>Namn på den användare som lade till problemet<br>Utgivningsnamn<br>Utgivningstyp<br>Angivet den<br>Utgivningsprioritet<br>Tilldelad till namn (tom) <br>Utgivningsstatus<br>Primär kontakt<br>*Projektreferensnummer<br>*Totalt antal tillagda ärenden <br>*Ärendenamn <br>*Namnet på den användare som lade till problemet <br>*Datum för den dagliga sammandraget<br><br></td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag har lagts till i ett projekt</strong> </p> <p>Användaren som lades till i projektet får ett e-postmeddelande när han eller hon läggs till, såvida inte användaren själv har lagt till sig själv i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL You've been added to the project] &lt;Project Name&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio-namn<br>Projektreferensnummer<br>Namnet på den användare som lade till dig i projektet<br>Projekt [!UICONTROL Planned Start Date]<br>Projekt [!UICONTROL Planned Completion Date]<br>Procent färdigt<br>Namn på andra i projekt <br>Projektägare<br><strong>Mer information</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Status ändras för ett projekt som jag är på</strong> </p> <p>Medlemmar i ett projektteam får ett e-postmeddelande när statusen för projektet ändras. <br>Mer information om projektteamet finns i <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Projektteamöversikt</a>.</p> <p>Ämnet för e-postmeddelandet är <em>[!UICONTROL Project Status Change]: &lt;Project Name&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är <em> [!UICONTROL Digest of Projects You're On] &lt;Datum för den dagliga sammandraget&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio-namn<br>Projektreferensnummer<br>Namnet på den användare som ändrade status för projektet<br>Ny projektstatus<br>Datum och tid när projektets status ändrades<br>Tidigare projektstatus<br><strong>[!UICONTROL See More Details]</strong>, knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Projektstatus<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
 </tbody> 
</table>
