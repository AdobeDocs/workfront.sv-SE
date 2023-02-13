---
content-type: reference
navigation-topic: notifications
title: '''Meddelanden: Information om projekt som jag äger'
description: Följande meddelanden informerar dig om aktiviteter som utförs i ett projekt som du äger. Mer information om hur du konfigurerar vilka meddelanden du får finns i Aktivera eller inaktivera egna händelsemeddelanden.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 0%

---

# Meddelanden: Information om projekt som jag äger

Följande meddelanden informerar dig om aktiviteter som utförs i ett projekt som du äger. Mer information om hur du konfigurerar vilka meddelanden du får finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Ett dokument läggs till i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett dokument läggs till i projektet, såvida inte den användare som lade till dokumentet också är projektägare.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och dokumentet är inte privat.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Document added to] &lt;project name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Namnet på den användare som lade till dokumentet<br>Dokumentnamn<br>Tillagd den<br>Dokumentinformation (format, storlek, versionsnummer)<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal tillagda dokument<br>*Dokumentnamn<br>*Namnet på den användare som lade till dokumentet<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En milstolpeuppgift slutförs i ett projekt som jag äger</strong> </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;task name=""&gt; på &lt;project name=""&gt;</em></p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete]visas fortfarande "[!UICONTROL Complete]".</p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som slutförde uppgiften<br>Ny aktivitetsstatus<br>Datum och tid när uppgiften slutfördes<br>Status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett projekt som jag äger kommer efter</strong> </p> <p>Projektägaren får ett e-postmeddelande när projektet är försenat. Ett projekt ligger efter när förloppsstatusen är[!UICONTROL At Risk]," "[!UICONTROL Behind]," eller "[!UICONTROL Late]."</p> <p>Det bästa sättet är att hålla det här meddelandet aktivt. </p> <p>Användare med [!UICONTROL Review] licensen får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project Progress Change]: &lt;project name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Status för projektförlopp<br>Projekt [!UICONTROL Planned Start Date]<br>Projekt [!UICONTROL Planned Completion Date]<br>Projekt [!UICONTROL Projected Start Date]<br>Projekt [!UICONTROL Projected Completion Date]<br>Procent färdigt projekt<br>Projektstatus<br>Projektägare<br>*Projektnamn<br>*Projektets referensnummer<br>*Projektförloppsstatus<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har lagts till i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue added to] &lt;project name=""&gt;</em></p> <p> </p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Ärendereferensnummer<br>Namnet på den användare som lade till utgåvan<br>Ärendenamn<br>Ärendetyp<br>Angivet den<br>Ärendeprioritet<br>Tilldelad till namn <br>Ärendestatus<br>Primär kontakt<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal ärenden som lagts till i projektet<br>*Ärendenamn<br>*Namnet på den användare som lade till problemet<br>*Datum för daglig sammandrag</p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En uppgift har slutförts i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett meddelande när en uppgift har slutförts i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;task name=""&gt; på &lt;project name=""&gt;</em></p> <p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete]visas fortfarande "[!UICONTROL Complete]".</p> </p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som slutförde uppgiften <br>Aktivitetsstatus<br>Datum och tid då uppgiften slutfördes<br>Status för föregående aktivitet<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda uppgifter <br>*Aktivitetsnamn<br>*Namnet på den användare som slutförde uppgiften<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En uppgift i ett projekt som jag själv har hamnat bakom</strong> </p> <p>Projektägaren får ett e-postmeddelande när en aktivitet i projektet ligger efter schemat. En aktivitet ligger efter när förloppsstatusen är[!UICONTROL At Risk]" eller "[!UICONTROL Behind]" eller "[!UICONTROL Late]."</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Task Progress Change]: &lt;task name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Ny status för aktivitetens förlopp<br>Uppgift [!UICONTROL Planned Start Date]<br>Uppgift [!UICONTROL Planned Completion Date]<br>Uppgift [!UICONTROL Projected Start Date]<br>Uppgift [!UICONTROL Projected Completion Date]<br>Procent färdigt för aktivitet<br>Aktivitetsstatus<br>Tilldelad till namn<br>Anges efter namn<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal aktiviteter som ligger efter schemat<br>*Aktivitetsnamn<br>*Namn tilldelat<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har uppstått i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett ärende har slutförts i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Användare med [!UICONTROL Review] licensen får inget meddelande. </p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;issue name=""&gt; på &lt;project name=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som slutförde problemet<br>Ärendestatus<br>Datum och tid då utgåvan slutfördes<br>Status för föregående problem<br><strong>[!UICONTROL See More Details]</strong> knapp <br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal slutförda ärenden<br>*Ärendenamn<br>*Namnet på den användare som är tilldelad utgåvan<br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett otilldelat problem läggs till i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett ej tilldelat problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Who should be assigned to this new issue on] &lt;project name=""&gt;?</em></p> <p> </p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> Sammanfattning av projekt som du äger &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Ärendereferensnummer<br>Namnet på den användare som lade till utgåvan<br>Ärendenamn<br>Ärendetyp<br>Angivet den<br>Ärendeprioritet<br>Tilldelad till namn (tom)<br>Ärendestatus<br>Primär kontakt<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal tillagda utgåvor<br>*Ärendenamn<br>*Namnet på den användare som lade till problemet<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag är nu ägare till ett nytt projekt</strong> </p> <p>När en användare tilldelas som projektägare får användaren ett e-postmeddelande.</p> <p>Om projektägaren är samma användare som tilldelades skickas inget e-postmeddelande.</p> <p>Användare med [!UICONTROL Review] licensen får inget meddelande.</p> <p>Aktivera det här eftersom de tilldelas något. </p> <p> Tilldela något, dela något, få åtkomst till något.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL You're now the project owner of] &lt;project name=""&gt;</em></p> <p>Följande text finns i e-postmeddelandets brödtext:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL made you the owner of] &lt;project name=""&gt;. [!UICONTROL As the Project Owner, you might receive additional email notifications about project activity, be required to approve hours for the project, or be involved in approving work related to the project. It's all yours.]</em> </p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Projektnamn<br>Portfolio<br>Projektets referensnummer<br>Slutförandedatum för projekt<br>*Projektnamn<br>*Projektets referensnummer<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Bekräftelsedatumet ändras för en aktivitet i ett av mina projekt</strong> </p> <p>Projektägaren får ett e-postmeddelande när implementeringsdatumet ändras för en aktivitet i projektet, såvida inte användaren som ändrade implementeringsdatumet också är projektägaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Commit date for] &lt;task name=""&gt; [!UICONTROL is now] &lt;new commit="" date=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> Sammanfattning av projekt som du äger &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Aktivitetsnamn<br>Projektnamn<br>Referensnummer för uppgift<br>Namnet på den användare som ändrade implementeringsdatumet<br>Nytt implementeringsdatum<br>Uppgift [!UICONTROL Planned Completion Date]<br>Information om hur projekttidslinjen påverkas av den här ändringen<br>Tilldelad till namn<br>Anges efter namn<br>Projektägare<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal uppgifter vars implementeringsdatum har ändrats<br>*Aktivitetsnamn<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Bekräftelsedatumet ändras för ett problem i ett av mina projekt</strong> </p> <p>Projektägaren får ett e-postmeddelande när implementeringsdatumet ändras för en utgåva i projektet, såvida inte användaren som ändrar implementeringsdatumet är samma användare som projektägaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Commit date for] &lt;issue name=""&gt; [!UICONTROL is now] &lt;new commit="" date=""&gt;</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter: <em> [!UICONTROL Digest of Projects You Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Ärendenamn<br>Projektnamn<br>Ärendereferensnummer<br>Namnet på den användare som ändrade implementeringsdatumet<br>Nytt implementeringsdatum<br>Planerat slutdatum för problem<br>Tilldelad till namn<br>Anges efter namn<br>Projektägare<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektets referensnummer<br>*Totalt antal ärenden vars implementeringsdatum har ändrats<br>*Ärendenamn<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
