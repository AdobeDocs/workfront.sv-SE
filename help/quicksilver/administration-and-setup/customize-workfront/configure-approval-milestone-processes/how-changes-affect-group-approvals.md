---
title: Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: I den här artikeln förklaras vad som händer när en godkännandeprocess redan används när en Workfront-administratör (eller en användare med administrativ åtkomst till godkännandeprocesser) ändrar sin koppling till en grupp.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: 7f719c903ad4079470a6dbd046dce445ba227a5b
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 0%

---

# Hur ändringar i gruppering och godkännandeprocess påverkar tilldelade godkännandeprocesser

I den här artikeln beskrivs vad som händer när en godkännandeprocess redan är kopplad till uppgifter, ärenden, projekt, mallar eller malluppgifter och en Workfront-administratör (eller en användare med administrativ åtkomst till godkännandeprocesser) gör något av följande:

* Ändrar godkännandeprocessen (på gruppnivå) från en grupp till en annan
* Ändrar gruppen som är associerad med projektet
* Ändrar godkännandeprocessen från gruppnivå till systemnivå
* Ändrar godkännandeprocessen från systemnivå till gruppnivå

I artikeln beskrivs också vad som händer när du flyttar eller kopierar uppgifter eller problem som är kopplade till en godkännandeprocess på gruppnivå mellan två projekt från olika grupper.

Mer information om de tre typerna av godkännandeprocesser som du kan använda i Workfront finns i [Översikt över godkännandeprocessen](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Om projektet, eller dess uppgifter eller problem redan är kopplade till en godkännandeprocess på gruppnivå med anpassade statusvärden på gruppnivå, kan en ändring av gruppen skapa en konflikt mellan den föregående gruppens godkännandestatus och de som finns på systemnivån.
>
>Om en godkännandeprocess till exempel innehåller två sökvägar, en för systemstatus och en andra för en gruppnivåstatus som motsvarar samma systemnivåstatus, kommer en ändring av gruppen för det ursprungliga projektet att leda till att Workfront får problem med att förstå den gruppspecifika statusen som kanske inte finns i den andra gruppen. I så fall kommer du att stöta på ett fel.
>
>Överväg att ta bort godkännandeprocesserna på gruppnivå för projektet eller dess uppgifter eller problem innan du uppdaterar projektgruppen.
>
>Mer information om hur du skapar godkännandeprocesser på gruppnivå finns i [Godkännandeprocesser på gruppnivå](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Mer information om hur du skapar en anpassad status på gruppnivå finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)

## Ändra en gruppspecifik godkännandeprocess från en grupp till en annan

Följande scenarier inträffar när en gruppspecifik godkännandeprocess redan används för ett objekt och någon tilldelar den till en annan grupp:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Område eller objekt där godkännandeprocessen bifogades</th> 
   <th>Godkännandeobjekt</th> 
   <th>Ändring i godkännandeprocessen för objektet eller området</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Godkännande av projekt eller mall </td> 
   <td>Projekt</td> 
   <td>Bli en godkännandeprocess för enstaka användning</td> 
  </tr> 
  <tr> 
   <td>Godkännande av uppgift eller malluppgift </td> 
   <td>Uppgift</td> 
   <td>Bli en godkännandeprocess för enstaka användning </td> 
  </tr> 
  <tr> 
   <td>Godkännande av utfärdande</td> 
   <td>Problem</td> 
   <td>Bli en godkännandeprocess för enstaka användning</td> 
  </tr> 
  <tr> 
   <td>Området Åtgärder i rutan Redigera projekt eller Redigera mall</td> 
   <td>Uppgift</td> 
   <td> <p>Fältet Standardprocess för godkännande av aktivitet återställs till Ej tillämpligt.</p> <p>Som standard är inga godkännandeprocesser kopplade till nya uppgifter i projektet.</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köinformation för ett projekt eller en mall</td> 
   <td>Problem</td> 
   <td> <p>Standardgodkännandefältet återställs till Ej tillämpligt.</p> <p>Som standard är inga godkännandeprocesser kopplade till nya problem eller förfrågningar i projektet.</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köämne i ett projekt eller en mall</td> 
   <td>Problem</td> 
   <td> <p>Standardgodkännandefältet återställs till Ej tillämpligt.</p> <p>Inga godkännandeprocesser är som standard kopplade till nya problem eller förfrågningar i projektet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändra gruppen som är associerad med ett projekt

När någon ändrar gruppen som är kopplad till ett projekt till en annan grupp händer följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Område eller objekt som redan har en godkännandeprocess</th> 
   <th>Godkännandeobjekt</th> 
   <th>Ändring i godkännandeprocessen för objektet eller området</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Godkännande av projekt eller mall </td> 
   <td>Projekt</td> 
   <td>Bli en godkännandeprocess för enstaka användning och statusen som är kopplad till den uppdateras för att matcha en liknande status för den nya gruppen.</td> 
  </tr> 
  <tr> 
   <td>Godkännande av uppgift eller malluppgift </td> 
   <td>Uppgift</td> 
   <td>Bli en godkännandeprocess för enstaka användning och statusen som är kopplad till den uppdateras för att matcha en liknande status för den nya gruppen.</td> 
  </tr> 
  <tr> 
   <td>Godkännande av utfärdande</td> 
   <td>Problem</td> 
   <td>Bli en godkännandeprocess för enstaka användning och statusen som är kopplad till den uppdateras för att matcha en liknande status för den nya gruppen.</td> 
  </tr> 
  <tr> 
   <td>Området Åtgärder i rutan Redigera projekt eller Redigera mall</td> 
   <td>Uppgift</td> 
   <td> <p>Fältet Standardprocess för godkännande av aktivitet har återställts till Ej tillämpligt</p> <p>Som standard är inga godkännandeprocesser kopplade till nya uppgifter i projektet</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köinformation för ett projekt eller en mall</td> 
   <td>Problem</td> 
   <td> <p>Fältet Standardgodkännandeprocess återställs till Ej tillämpligt</p> <p>Som standard är inga godkännandeprocesser kopplade till nya problem eller förfrågningar i projektet</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köämne i ett projekt eller en mall</td> 
   <td>Problem</td> 
   <td> <p>Fältet Standardgodkännandeprocess återställs till Ej tillämpligt</p> <p>Som standard är inga godkännandeprocesser kopplade till nya problem eller förfrågningar i projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändra en godkännandeprocess från gruppnivå till systemnivå

När någon ändrar gruppalternativet i en gruppspecifik godkännandeprocess till&quot;Alla grupper&quot; blir godkännandeprocessen systemomfattande och följande inträffar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Område eller objekt där godkännandeprocessen bifogades</th> 
   <th>Godkännandeobjekt</th> 
   <th>Ändring i godkännandeprocessen för objektet eller området</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Godkännande av projekt eller mall </td> 
   <td>Projekt</td> 
   <td>Ingen ändring</td> 
  </tr> 
  <tr> 
   <td>Godkännande av uppgift eller malluppgift </td> 
   <td>Uppgift</td> 
   <td>Ingen ändring</td> 
  </tr> 
  <tr> 
   <td>Godkännande av utfärdande</td> 
   <td>Problem</td> 
   <td>Ingen ändring</td> 
  </tr> 
  <tr> 
   <td>Området Åtgärder i rutan Redigera projekt eller Redigera mall</td> 
   <td>Uppgift</td> 
   <td> <p>Ingen ändring av godkännandeprocessen, men som standard är den kopplad till nya uppgifter i projektet</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köinformation för ett projekt eller en mall</td> 
   <td>Problem</td> 
   <td> <p>Ingen ändring av godkännandeprocessen, men som standard är den kopplad till nya utgåvor eller förfrågningar i projektet</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köämne i ett projekt eller en mall</td> 
   <td>Problem</td> 
   <td> <p>Ingen ändring av godkännandeprocessen, men som standard är den kopplad till nya utgåvor eller förfrågningar i projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändra en godkännandeprocess från systemnivå till gruppnivå

När någon ändrar tillgängligheten för en systemomfattande godkännandeprocess från&quot;Alla grupper&quot; till en viss grupp, blir godkännandeprocessen gruppspecifik och följande inträffar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Område eller objekt där godkännandeprocessen bifogades</th> 
   <th>Godkännandeobjekt</th> 
   <th>Ändring i godkännandeprocessen för objektet eller området</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt-, uppgifts-, utgåva-, mall- eller malluppgift som tillhör gruppen för godkännandeprocessen</td> 
   <td> <p>Projekt, uppgift eller utleverans</p> </td> 
   <td>Ingen ändring</td> 
  </tr> 
  <tr> 
   <td>Området Åtgärder i rutan Redigera projekt eller Redigera mall för ett projekt eller en mall som tillhör gruppen för godkännandeprocessen</td> 
   <td>Uppgift</td> 
   <td> <p>Ingen ändring av godkännandeprocessen, men som standard är den kopplad till nya uppgifter i projektet</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köinformation för ett projekt eller en mall som tillhör gruppen för godkännandeprocessen</td> 
   <td>Problem</td> 
   <td> <p>Ingen ändring av godkännandeprocessen, men som standard är den kopplad till nya utgåvor eller förfrågningar i projektet</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köämne för ett projekt eller en mall som tillhör gruppen för godkännandeprocessen</td> 
   <td>Problem</td> 
   <td> <p>Ingen ändring av godkännandeprocessen, men som standard är den kopplad till nya utgåvor eller förfrågningar i projektet</p> </td> 
  </tr> 
  <tr> 
   <td>Projekt-, uppgifts-, utgåva-, mall- eller malluppgift som tillhör en annan grupp än gruppen för godkännandeprocessen</td> 
   <td> <p>Projekt</p> <p>Uppgifter</p> <p>Problem</p> </td> 
   <td>Bli en godkännandeprocess för enstaka användning</td> 
  </tr> 
  <tr> 
   <td>Området Åtgärder i rutan Redigera projekt eller Redigera mall för ett projekt eller en mall som tillhör en annan grupp än gruppen för godkännandeprocessen</td> 
   <td>Uppgifter</td> 
   <td> <p>Fältet Standardprocess för godkännande av aktivitet återställs till Ej tillämpligt.</p> <p>Som standard är inga godkännandeprocesser kopplade till nya uppgifter i projektet.</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köinformation för ett projekt eller en mall som tillhör en annan grupp än gruppen för godkännandeprocessen</td> 
   <td>Problem</td> 
   <td> <p>Standardgodkännandefältet återställs till Ej tillämpligt.</p> <p>Som standard är inga godkännandeprocesser kopplade till nya problem eller förfrågningar i projektet.</p> </td> 
  </tr> 
  <tr> 
   <td>Avsnittet Köämne för ett projekt eller en mall som tillhör en annan grupp än gruppen för godkännandeprocessen</td> 
   <td>Problem</td> 
   <td> <p>Standardgodkännandefältet återställs till Ej tillämpligt.</p> <p>Som standard är inga godkännandeprocesser kopplade till nya problem eller förfrågningar i projektet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Flytta eller kopiera en uppgift eller ett problem till ett projekt med en annan grupp än godkännandeprocessen

Om du flyttar eller kopierar en uppgift eller ett problem från ett projekt till ett annat kan det påverka befintliga godkännandeprocesser för uppgiften eller problemet beroende på vilka grupper av de två projekten som är aktuella. Följande tabell visar vilka scenarier som kan finnas:

| Ursprunglig aktivitet eller godkännandeprocess för utfärdande | Grupper av de två projekten | Ändringar i godkännandeprocessen efter att uppgiften eller utgåvan har flyttats till ett annat projekt |
|---|---|---|
| Godkännandeprocess för engångsbruk som är kopplad till en systemomfattande status | Projekten finns i samma eller olika grupper | Ingen ändring |
| Godkännandeprocess för engångsbruk som är kopplad till en gruppspecifik status | Projekt finns i olika grupper | Godkännandet är fortfarande en enstaka godkännandeprocess och statusen som är kopplad till godkännandeuppdateringarna för att matcha en liknande status för den nya gruppen. |
| Godkännandeprocess för hela systemet | Projekten finns i samma eller olika grupper | Ingen ändring |
| Gruppspecifik godkännandeprocess | Projekt ingår i samma grupp | Ingen ändring |
| Gruppspecifik godkännandeprocess | Projekten finns i olika grupper och grupperna har olika gruppspecifika statusar | Godkännandet blir en engångsprocess för godkännande och statusen som är kopplad till godkännandeuppdateringarna för att matcha en liknande status för den nya gruppen. |
| Gruppspecifik godkännandeprocess | Projekt finns i olika grupper och det finns en status med samma nyckel i den nya gruppen som den status som är associerad med godkännandeprocessen från den första gruppen | Ingen ändring |
