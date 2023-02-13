---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Systemprojektstatus
description: Workfront har 9 inbyggda systemprojektstatusar. De första tre i tabellen nedan är obligatoriska, vilket betyder att du kan låsa upp, byta namn på och ändra ordning på dem, men du kan inte dölja eller ta bort dem. Att ändra en projektstatus är vanligtvis en manuell process. Men ibland ändras en projektstatus automatiskt beroende på andra faktorer som inträffar i systemet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Systemprojektstatus

Workfront har 9 inbyggda systemprojektstatusar.

De första tre i tabellen nedan är obligatoriska, vilket betyder att du kan låsa upp, byta namn på och ändra ordning på dem, men du kan inte dölja eller ta bort dem.

Att ändra en projektstatus är vanligtvis en manuell process. Det finns emellertid vissa scenarier som beskrivs i följande lista när en projektstatus ändras automatiskt, beroende på andra faktorer som inträffar i systemet.

Följande projektstatusar finns i din Workfront-instans:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Systemprojektstatus</th> 
   <th>Projektstatus inträffar när</th> 
   <th>Vad händer i den här statusen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering (obligatorisk status)</td> 
   <td> <p>Projektledaren planerar tidslinjen för projektet, tilldelning av uppgifter och godkännanden. Projektledaren ställer in den här statusen för ett projekt manuellt.</p> <p>Tips: Vi rekommenderar att du anger standardstatus för nya projekt i Workfront till Planning. Som Workfront-administratör kan du ändra standardstatus för alla nya projekt under Projekt i Projektinställningar.</p> </td> 
   <td> <p>Användare i projektteamet kan som standard se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som tilldelats dem i projektet fyller inte i sin arbetslista. Endast godkännanden och godkända arbetsobjekt visas i hemarbetslistan.</p> <p>Inga meddelanden skickas när ett projekt har den här statusen.</p> <p>Vi rekommenderar att alla ändringar som kan utlösa en uppdatering av tidslinjen i projektet, eller ändringar av aktiviteter och tilldelningar av utleveranser, görs medan projektet är i planeringsstatus. Detta minimerar antalet meddelanden som användare får.</p> <p>Projektets tidslinje beräknas inte automatiskt av systemet.</p> </td> 
  </tr> 
  <tr> 
   <td>Aktuell (obligatorisk status)</td> 
   <td> <p>Användarna arbetar på det. Projektledaren ska omvandla ett projekt till Aktuell för att signalera att det har startat.</p> <p>Det här är standardstatusen för nya projekt i Workfront.</p> <p>Tips: Som Workfront-administratör kan du ändra standardstatus för nya projekt under Projekt i Projektinställningar. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </td> 
   <td> <p>Användare i projektteamet kan som standard se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som tilldelats dem i projektet fyller i deras arbetslista. De kan börja acceptera arbete med uppgifter och ärenden och flytta dem till sin lista Arbeta med.</p> <p>I ett aktuellt projekt skickas dessutom alla meddelanden om tidslinjeändringar, tilldelningar, nödvändiga åtgärder och godkännanden till användarna i projektteamet.</p> <p>Projektets tidslinje beräknas automatiskt av systemet om projektets uppdateringstyp är inställd på Automatisk, Vid ändring, Automatisk och Vid ändring.</p> <p>Tips: Det är en bra idé att hålla justeringarna för projektplaner så få som möjligt när ett projekt har den här statusen så att användarna inte får för många meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td>Slutförd (obligatorisk status)</td> 
   <td> <p> Projektet är slutfört:</p> 
    <ul> 
     <li> <p>Om projektets slutföringsläge är inställt på Manuellt väljer projektledaren den här statusen manuellt för att informera användare i projektteamet om att sluta arbeta med projektet.</p> </li> 
    </ul> 
    <ul> 
     <li>Om du har valt Automatiskt för Slutförandeläge för projektet markeras ett projekt automatiskt som Fullständigt när alla uppgifter och ärenden i projektet har markerats som Fullständigt. </li> 
    </ul> <p><b>VIKTIGT</b>: Du kan bara markera ett projekt som färdigt när alla aktiviteter, utgåvor och godkännanden av projektet har lösts.</p> </td> 
   <td>
    <ul>
     <li>Användare i projektteamet kan som standard inte se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som tilldelats dem i projektet fyller inte i listorna Arbetsförfrågningar eller Arbeta med.</li>
     <li>Alla meddelanden som rör projektet, förutom ett meddelande om statusändring, skickas inte längre till användarna i projektteamet. </li>
     <li>Projektets tidslinje beräknas inte längre av systemet.</li>
     <li>Det går inte att kopiera projektet.</li>
    </ul><p>Du kan hindra användare från att utföra ytterligare åtgärder när ett projekt har markerats som fullständigt. </p><p>Mer information om hur du begränsar åtgärder för projekt som har markerats som fullständiga finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Död</td> 
   <td>Projektet har inte slutförts ännu, men på grund av hinder eller förändringar i omfattningen kan projektet inte fortsätta att bearbetas och har övergivits. Projektledaren ändrar statusen till Död för att informera användarna i projektteamet om att projektet aldrig kommer att slutföras och att de inte längre ska arbeta med det.</td> 
   <td> <p>Användare i projektteamet kan som standard inte se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som har tilldelats dem i projektet tas bort från deras arbetslista.</p> <p>Godkännandebeslut kan inte beviljas för uppgifter eller ärenden.</p> <p>Meddelanden om ändringar i tidslinjen, tilldelningar, nödvändiga åtgärder och godkännanden skickas inte till användare i projektteamet.</p> <p>Projektets tidslinje beräknas inte automatiskt av systemet eftersom projektet uppfattas som slutfört.</p> <p>Du kan hindra användare från att utföra vissa åtgärder när ett projekt har markerats som Dölj. Mer information om hur du begränsar åtgärder i Dead-projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Parkerad</td> 
   <td>Projektet har inte slutförts ännu, men på grund av vissa förseningar måste projektet tillfälligt avbrytas. Projektledaren väljer att använda den här statusen för att varna användare i projektteamet om att sluta arbeta med projektet vid den aktuella tidpunkten.</td> 
   <td> <p>Användare i projektteamet kan som standard inte se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som har tilldelats dem i projektet tas bort från deras arbetslista. </p> <p>Godkännandebeslut kan inte beviljas för uppgifter eller ärenden.</p> <p>Meddelanden om ändringar i tidslinjen, tilldelningar, nödvändiga åtgärder och godkännanden skickas inte till användare i projektteamet.</p> <p> <p><b>ANMÄRKNING</b>: När du placerar ett projekt som är parkerat stoppas inte tidslinjen i projektet. Projektet kan fortfarande visa sig vara i riskzonen eller i svårigheter även om ingen arbetar aktivt med projektet. Vissa manuella justeringar av datumen för de återstående öppna uppgifterna kan behövas när du återställer projektet till Aktuell igen, så att projektet kan visa uppdaterat förlopp.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Begärd</td> 
   <td>Projektstatusen markeras automatiskt som Begärt av systemet när affärsärendet på en projektförfrågan har slutförts och skickats in för godkännande. Mer information om hur du begär ett projekt med hjälp av ett affärsfall finns i <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Granska begärda projekt</a>.</td> 
   <td> <p>Användare i projektteamet kan som standard inte se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor i projektet som tilldelats dem fyller inte i sin arbetslista.</p> <p>Alla meddelanden som rör projektet, förutom ett meddelande om statusändring, skickas inte till någon användare.</p> <p>Projektets tidslinje beräknas inte automatiskt av systemet.</p> </td> 
  </tr> 
  <tr> 
   <td>Godkänd</td> 
   <td>Projektstatusen markeras automatiskt som Godkänd när affärsärendet på en projektförfrågan har godkänts. Mer information om hur du begär ett projekt med hjälp av ett affärsfall finns i <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Granska begärda projekt</a>.</td> 
   <td> <p>Användare i projektteamet kan som standard se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som tilldelats dem i projektet fyller inte i sin arbetslista.</p> <p>Alla meddelanden som rör projektet, förutom ett meddelande om statusändring, skickas inte till någon användare.</p> <p>Projektets tidslinje beräknas inte automatiskt av systemet. </p> </td> 
  </tr> 
  <tr> 
   <td>Avvisad</td> 
   <td>Projektstatusen markeras automatiskt som Avvisad när affärsärendet på en projektförfrågan har avvisats. Mer information om hur du begär ett projekt med hjälp av ett affärsfall finns i <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Granska begärda projekt</a>.</td> 
   <td> <p>Användare i projektteamet kan som standard inte se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som tilldelats dem i projektet fyller inte i sin arbetslista.</p> <p>Alla meddelanden som rör projektet, förutom ett meddelande om statusändring, skickas inte till någon användare.</p> <p>Projektets tidslinje beräknas inte automatiskt av systemet.</p> </td> 
  </tr> 
  <tr> 
   <td>Idea</td> 
   <td>Projektstatusen markeras automatiskt som Idea när du skickar en projektförfrågan. Mer information om hur du begär ett projekt med hjälp av ett affärsfall finns i <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Granska begärda projekt</a>.</td> 
   <td> <p>Användare i projektteamet kan som standard inte se projektet i sina projektlistor i området Projekt i Workfront. De uppgifter och utgåvor som tilldelats dem i projektet fyller inte i sin arbetslista.</p> <p>Alla meddelanden som rör projektet, förutom ett meddelande om statusändring, skickas inte till någon användare.</p> <p>Projektets tidslinje beräknas inte automatiskt av systemet.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Följande projektstatus kan inte ändras till statusen Inaktuell, Väntande eller Fullständig:
>
>* Begärd
>* Idea
>* Godkänd
>* Avvisad (eller motsvarande)
>

