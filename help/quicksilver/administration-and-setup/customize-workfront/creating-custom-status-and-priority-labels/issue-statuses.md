---
title: Få åtkomst till listan över status för systemproblem
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Du kan använda status för en utgåva för att visa användare i systemet i vilket utvecklingsstadium ett problem befinner sig vid en given tidpunkt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 0%

---

# Åtkomst till listan över status för systemproblem

Du kan använda status för en utgåva för att visa användare i systemet i vilket utvecklingsstadium ett problem befinner sig vid en given tidpunkt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Åtkomst till utleveransstatus

Du kan komma åt och ändra status för problem på systemnivå. Du kan redigera viss information om standardsystemstatus eller skapa nya anpassade statusvärden. Mer information om hur du skapar anpassade statusar eller redigerar systemstatus finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Så här får du åtkomst till utgivningsstatus på systemnivå:

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Status**.

1. Klicka på fliken **Problem** om du vill visa status för utgåvor som är tillgängliga i Workfront.

   ![](assets/issue-status.png)

## Status för systemutleverans

Workfront levereras med 10 ursprungliga utgivningsstatusar. De första 4 i tabellen nedan är obligatoriska, vilket betyder att du kan låsa upp, byta namn på och ändra ordning på dem, men du kan inte dölja eller ta bort dem.

Du kan lägga till anpassade utgivningsstatusar för att passa behoven i din organisation. Mer information finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

För användare är det oftast en manuell process att ändra status på ett problem. Det finns emellertid situationer som beskrivs i följande lista när en utgåvas status ändras automatiskt, beroende på andra faktorer som inträffar i systemet.

Följande problemstatus finns i din Workfront-instans:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status för systemproblem</th> 
   <th>Så här kan du använda statusen</th> 
   <th>Vad händer i statusen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ny (obligatorisk status)</td> 
   <td>Det här är standardstatus för alla nya utgåvor.</td> 
   <td>Om problemet gäller ett projekt med statusen Aktuell visas det på fliken Arbetsbegäran för de användare som är tilldelade till problemet. Nu kan användare börja arbeta med problemet.</td> 
  </tr> 
  <tr> 
   <td>Pågår (obligatorisk status)</td> 
   <td> <p>Du kan placera ett problem i den här statusen för att ange att arbetet med det problemet har startat.</p> <p>Om problemlösningen är kopplad till ett annat objekt (en aktivitet, ett projekt eller något annat problem) ändras problemstatusen automatiskt till Pågår när du ändrar statusen för det matchande objektet till Pågår. </p> <p>Mer information om hur du löser objekt finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över objekt som kan lösas och lösas </a>.</p> </td> 
   <td> <p>Om problemet gäller ett projekt med statusen Aktuell visas det på fliken Arbeta med för de användare som är tilldelade till problemet.</p> <p>När en utgåva pågår visas ett värde för Faktiskt startdatum.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Stängd (obligatorisk status)</td> 
   <td> <p>Du kan manuellt markera ett problem som stängt när arbetet är slutfört. </p> <p>Om problemlösningen är kopplad till ett annat objekt (en uppgift, ett projekt eller ett annat problem) ändras problemstatusen automatiskt till Stängd när du ändrar statusen för det matchande objektet till Stängd.</p> <p>Mer information om hur du löser objekt finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över objekt som kan lösas och lösas </a>.</p> </td> 
   <td> <p>När en utgåva stängs tas den bort från listan Arbeta på. I det här fallet visas ett värde för Faktiskt slutförandedatum. </p> <p>När alla uppgifter är slutförda och problemen stängs i ett projekt kan projektet slutföras.</p> </td> 
  </tr> 
  <tr> 
   <td>Spärrad (obligatoriskt läge)</td> 
   <td> <p>Du kan markera ett problem som Spärrat manuellt för att ange att det har uppstått en fördröjning när problemet är färdigt. </p> </td> 
   <td> <p>Om problemet gäller ett projekt med statusen Aktuell visas det på fliken Arbeta med för de användare som är tilldelade till problemet. </p> <p>När alla uppgifter har slutförts i ett projekt, men det finns minst ett spärrat problem i projektet, kan projektet inte slutföras. </p> </td> 
  </tr> 
  <tr> 
   <td>Återöppnad (motsvarar med pågående)</td> 
   <td> <p>Du kan ställa in en fråga i denna status för att indikera att arbetet med den frågan inte var helt slutfört när den tidigare var stängd och att den behövde öppnas igen för att slutföra arbetet.</p> </td> 
   <td> <p>Om problemet gäller ett projekt med statusen Aktuell visas det på fliken Arbetsbegäran för de användare som är tilldelade till problemet. Nu kan användare börja arbeta med problemet.</p> <p>Den här statusen är viktig vid rapportering för att skilja mellan problem som är öppna för första gången (vanligtvis med statusen Nytt) och problem som öppnas efter att ha stängts tidigare (vanligtvis med statusen Återöppnad). </p> </td> 
  </tr> 
  <tr> 
   <td>Väntar på återkoppling (motsvarar med Väntande)</td> 
   <td>Du kan placera ett problem i den här statusen som indikerar att du väntar på feedback (vanligtvis från den primära kontakten) innan du kan fortsätta arbeta med problemet. </td> 
   <td> <p>Om problemet gäller ett projekt med statusen Aktuell visas det på fliken Arbeta med för de användare som är tilldelade till problemet.</p> <p>Om ett problem väntar på feedback kan ett projekt inte slutföras.</p> <p>Den här statusen är viktig vid rapportering för att skilja mellan problem som är öppna men som bearbetas (vanligtvis med statusen Pågår) och problem som är öppna men som inte bearbetas eftersom mer feedback behövs för att slutföra dem (vanligtvis med statusen Väntar på feedback).</p> </td> 
  </tr> 
  <tr> 
   <td>Det går inte att duplicera (motsvarar med stängd)</td> 
   <td>Du kan placera ett problem i den här statusen som indikerar att du stänger utgåvan, men du kunde inte se problemet som utlöste att utgåvan öppnades. Problemet kan finnas kvar, men kan inte replikeras vid en given tidpunkt. </td> 
   <td> <p>Den här statusen är viktig vid rapportering, för att skilja mellan problem som har slutförts och vars problem har åtgärdats (vanligtvis i statusen Stängt) och problem vars problem inte är synligt vid en viss tidpunkt (vanligtvis i statusen Kan inte dupliceras).</p> <p>När en utgåva är markerad som Kan inte dupliceras tas den bort från listan Arbeta på för den som tilldelats. I det här fallet visas ett värde för Faktiskt CompletionDate.</p> <p>Om alla uppgifter i ett projekt har slutförts och vissa problem har statusen Kan inte duplicera, kan projektet slutföras.</p> </td> 
  </tr> 
  <tr> 
   <td>Löst (motsvarar med stängd)</td> 
   <td>Du kan placera ett problem i den här statusen som indikerar att du stänger problemet och att problemet som skapade det faktiskt har lösts.</td> 
   <td> <p>Den här statusen är viktig vid rapportering för att skilja mellan problem som stängs med eller utan en lösning (vanligtvis med statusen Stängd) och problem som stängs med en faktisk lösning (vanligtvis med statusen Löst).</p> <p>När en utgåva markeras som löst tas den bort från listan Arbeta på. I det här fallet visas ett värde för Faktiskt slutförandedatum.</p> <p>Om alla uppgifter i ett projekt har slutförts och minst ett problem har statusen Löst kan projektet slutföras. </p> </td> 
  </tr> 
  <tr> 
   <td>Verifierad slutförd (motsvarar stängd)</td> 
   <td>Du kan placera ett problem i den här statusen för att ange att du stänger problemet och att du har verifierat att det problem som genererade problemet har åtgärdats.</td> 
   <td> <p>När en utgåva har markerats som Verifierad fullständig tas den bort från listan Arbeta på för den som tilldelats problemet. I det här fallet visas ett värde för Faktiskt slutförandedatum.</p> <p>Om alla uppgifter i ett projekt har slutförts och vissa problem har statusen Verifierat slutfört, kan projektet slutföras.</p> </td> 
  </tr> 
  <tr> 
   <td>Matcha inte (motsvarar med stängd)</td> 
   <td>Du kan placera ett problem i den här statusen som indikerar att du stänger problemet, men problemet som genererade det kan inte lösas.</td> 
   <td> <p>Den här statusen är viktig vid rapportering för att skilja mellan problem som stängs med eller utan en lösning (vanligtvis med statusen Stängt) och problem som stängs utan en faktisk lösning (vanligtvis med statusen Lösning).</p> <p>När en utgåva har markerats som Won't Resolve tas den bort från listan Arbeta på för den som tilldelats. I det här fallet visas ett värde för Faktiskt slutförandedatum.</p> <p>Om alla uppgifter i ett projekt är slutförda och minst ett problem har statusen Inte löst kan projektet slutföras.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa utgivningsstatus

En Workfront-administratör kan lägga till utgivningsstatus på system- och gruppnivå i Workfront och ändra ordningen som användarna ser dem i. Mer information finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

En gruppadministratör kan lägga till en anpassad status som är specifik för en grupp. Mer information finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
