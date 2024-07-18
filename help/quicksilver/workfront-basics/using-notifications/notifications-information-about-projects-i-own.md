---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Information om projekt som jag äger'
description: Följande meddelanden informerar dig om aktiviteter som utförs i ett projekt som du äger. Mer information om hur du konfigurerar vilka meddelanden du får finns i Ändra dina egna e-postmeddelanden.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Meddelanden: Information om projekt som jag äger

Följande meddelanden informerar dig om aktiviteter som utförs i ett projekt som du äger. Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Ett dokument läggs till i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett dokument läggs till i projektet, såvida inte den användare som lade till dokumentet också är projektägare.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] och dokumentet inte är privat.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Document added to] &lt;Projektnamn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Projektnamn<br>Portfolio <br>Projektreferensnummer<br>Namnet på den användare som lade till dokumentet<br>Dokumentnamn<br>lades till den <br>Dokumentinformation (format, storlek, versionsnummer)<br><strong>[!UICONTROL Preview]</strong> och <strong>[!UICONTROL Download]</strong> knappar<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal dokument som lagts till<br>*Dokumentnamn<br>*Användarens namn som lade till dokumentet <br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En milstolpeaktivitet har slutförts för ett projekt som jag äger</strong> </p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt; på &lt;Projektnamn&gt;</em></p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete] visas fortfarande [!UICONTROL Complete] som ämne i e-postmeddelandet.</p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på användaren som slutförde aktiviteten<br>Ny aktivitetsstatus<br>Datum och tid när aktiviteten slutfördes<br>Tidigare aktivitetsstatus<br><strong>[!UICONTROL See More Details]</strong> knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda uppgifter<br>*Aktivitetsnamn<br>*Namnet på användaren som slutförde aktiviteten<br> 2}*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett projekt som jag äger ligger efter</strong> </p> <p>Projektägaren får ett e-postmeddelande när projektet är försenat. Ett projekt ligger efter när förloppsstatusen är [!UICONTROL At Risk], [!UICONTROL Behind] eller [!UICONTROL Late].</p> <p>Det bästa sättet är att se till att detta meddelande är aktivt. </p> <p>Användare med en [!UICONTROL Review]-licens får inget meddelande.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Project Progress Change]: &lt;Projektnamn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio <br>Projektreferensnummer<br>Projektförloppsstatus<br>Projekt [!UICONTROL Planned Start Date]<br>Projekt [!UICONTROL Planned Completion Date]<br>Projekt [!UICONTROL Projected Start Date]<br>Projekt [!UICONTROL Projected Completion Date]<br>Projektprocent slutfört<br>Projektstatus<br>Projektägare<br>*Projektnamn<br>*Projektreferensnummer<br>*Projektförloppsstatus<br>*Datum för daglig sammandrag<br></p> </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har lagts till i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Issue added to] &lt;Projektnamn&gt;</em></p> <p> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio-namn<br>Ärendereferensnummer<br>Namn på den användare som lade till problemet<br>Utgivningsnamn<br>Utgivningstyp<br>Angivet den<br>Utgivningsprioritet<br>Tilldelad till namn <br>Utgivningsstatus<br>Primär kontakt<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal utleveranser som lagts till project<br>*Issue Name<br>*Name of the user who added the issue<br>*Date of day digest</p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En aktivitet har slutförts i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett meddelande när en uppgift har slutförts i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;Aktivitetsnamn&gt; på &lt;Projektnamn&gt;</em></p> <p> <p>Obs! Om aktiviteten ändras till en status som är lika med [!UICONTROL Complete] visas fortfarande [!UICONTROL Complete] som ämne i e-postmeddelandet.</p> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på användaren som slutförde aktiviteten <br>Aktivitetsstatus<br>Datum och tid när aktiviteten slutfördes<br>Tidigare aktivitetsstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda uppgifter <br>*Aktivitetsnamn<br>*Namnet på användaren som slutförde aktiviteten<br> * Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En aktivitet i ett projekt som jag äger ligger bakom</strong> </p> <p>Projektägaren får ett e-postmeddelande när en aktivitet i projektet försenas. En aktivitet ligger efter när förloppsstatusen är [!UICONTROL At Risk], [!UICONTROL Behind] eller [!UICONTROL Late].</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Task Progress Change]: &lt;Aktivitetsnamn&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Aktivitetsnamn<br>Projektnamn<br>Referensnummer för aktivitet<br>Status för ny aktivitetsstatus<br>Aktivitet [!UICONTROL Planned Start Date]<br>Aktivitet [!UICONTROL Planned Completion Date]<br>Aktivitet [!UICONTROL Projected Start Date]<br>Aktivitet [!UICONTROL Projected Completion Date]<br>Procent färdigt<br>Aktivitetsstatus<br>Tilldelad till namn<br>Anges av namn<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal aktiviteter som ligger bakom schema<br>*Uppgiftsnamn<br>*Tilldelat till namn<br>*Datum för daglig sammandrag </td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett problem har slutförts i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett ärende har slutförts i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Användare med en [!UICONTROL Review]-licens får inget meddelande. </p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Complete]: &lt;Issue Name&gt; på &lt;Project Name&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> Utgivningsnamn<br>Projektnamn<br>Utgivningsreferensnummer<br>Namn på den användare som slutförde utleveransen<br>Utgivningsstatus<br>Datum och tid då utleveransen slutfördes<br>Tidigare utgivningsstatus<br><strong>[!UICONTROL See More Details]</strong> <br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal slutförda utleveranser<br>*Utgivningsnamn<br>*Namn på den användare som tilldelats utleveransen <br>*Datum för den dagliga sammandraget<br></td> 
   <td><strong>Dagligen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ett otilldelat problem har lagts till i ett projekt som jag äger</strong> </p> <p>Projektägaren får ett e-postmeddelande när ett ej tilldelat problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är [!UICONTROL Current] eller [!UICONTROL Planning].</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Who should be assigned to this new issue on] &lt;Projektnamn&gt;?</em></p> <p> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> Digest of Projects You Own &lt;Date of day digest&gt; </em></p> </td> 
   <td> <p>Projektnamn<br>Portfolio-namn<br>Ärendereferensnummer<br>Namn på den användare som lade till problemet<br>Utgivningsnamn<br>Utgivningstyp<br>Angivet den<br>Utgivningsprioritet<br>Tilldelad till namn (tom)<br>Utgivningsstatus<br>Primär kontakt<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal utgåvor lade till <br>*Ärendenamn<br>*Namnet på den användare som lade till problemet<br>*Datum för den dagliga sammandraget<br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och Dagligen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jag är inställd som ägare av ett nytt projekt</strong> </p> <p>När en användare tilldelas som projektägare får användaren ett e-postmeddelande.</p> <p>Om projektägaren är samma användare som tilldelades skickas inget e-postmeddelande.</p> <p>Användare med en [!UICONTROL Review]-licens får inget meddelande.</p> <p>Aktivera det här eftersom de tilldelas något. </p> <p> Tilldela något, dela något, få åtkomst till något.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL You're now the project owner of] &lt;Projektnamn&gt;</em></p> <p>Följande text finns i e-postmeddelandets brödtext:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;ditt namn&gt;,<br></em><em>&lt;Namnet på den användare som tilldelade dig som projektägare&gt; [!UICONTROL made you the owner of] &lt;Projektnamn&gt;. [!UICONTROL As the Project Owner, you might receive additional email notifications about project activity, be required to approve hours for the project, or be involved in approving work related to the project. It's all yours.]</em> </p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> <p> </p> </td> 
   <td> <p>Projektnamn<br>Portfolio <br>Projektreferensnummer<br>Projektslutförandedatum<br>*Projektnamn<br>*Projektreferensnummer<br>*Datum för daglig sammandrag</p> </td> 
   <td><strong>Direkt</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Bekräftelsedatumet ändras för en aktivitet i ett av mina projekt</strong> </p> <p>Projektägaren får ett e-postmeddelande när implementeringsdatumet ändras för en aktivitet i projektet, såvida inte användaren som ändrade implementeringsdatumet också är projektägaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Commit date for] &lt;Aktivitetsnamn&gt; [!UICONTROL is now] &lt;Nytt implementeringsdatum&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> Digest of Projects You Own &lt;Date of day digest&gt; </em></p> </td> 
   <td> <p>Aktivitetsnamn<br>Projektnamn<br>Aktivitetsreferensnummer<br>Namnet på den användare som ändrade implementeringsdatumet<br>Nytt implementeringsdatum<br>Aktivitet [!UICONTROL Planned Completion Date]<br>Information om hur projekttidslinjen påverkas av den här ändringen<br>Tilldelad till namn<br>Anges av namn<br>Projektägare<br><strong>[!UICONTROL See More Details]</strong>, knapp<br>*Projektreferensnummer<br>*Totalt antal uppgifter vars implementeringsdatum har ändrats <br>*Aktivitetsnamn <br>*Datum för den dagliga sammandraget<br><br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Bekräftelsedatumet ändras för ett problem i ett av mina projekt</strong> </p> <p>Projektägaren får ett e-postmeddelande när implementeringsdatumet ändras för en utgåva i projektet, såvida inte användaren som ändrar implementeringsdatumet är samma användare som projektägaren.</p> <p>Ämnet för e-postmeddelandet är: <em>[!UICONTROL Commit date for] &lt;Utfärdsnamn&gt; [!UICONTROL is now] &lt;Nytt implementeringsdatum&gt;</em></p> <p> Ämnet för det dagliga sammandragsmeddelandet är: <em> [!UICONTROL Digest of Projects You Own] &lt;Datum för det dagliga sammandraget&gt; </em></p> </td> 
   <td> <p>Utleveransnamn<br>Projektnamn<br>Utgivningsreferensnummer<br>Namnet på den användare som ändrade implementeringsdatumet<br>Nytt implementeringsdatum<br>Utgivningsdatum<br>Tilldelad till namn<br>Anges av namn<br>Projektägare<br><strong>[!UICONTROL See More Details]</strong>, knapp<br>*Projektnamn<br>*Projektreferensnummer<br>*Totalt antal ärenden vars implementeringsdatum har ändrats <br>*Ärendenamn <br>*Datum för daglig sammandrag<br></p> </td> 
   <td> <p><strong>Direkt</strong> </p> <p><strong>och [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
