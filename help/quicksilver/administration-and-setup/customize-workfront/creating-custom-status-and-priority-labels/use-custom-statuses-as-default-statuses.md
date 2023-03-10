---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Använd anpassade statusvärden som standardstatusvärden
description: När en anpassad status anges som standardstatus används den nya standardstatusen i hela systemet på olika sätt. Hur det används beror på om det är inställt som standardstatus på systemnivå eller standardstatus på gruppnivå.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Använd anpassade statusvärden som standardstatusvärden

När en anpassad status anges som standardstatus används den nya standardstatusen i hela systemet på olika sätt. Hur det används beror på om det är inställt som standardstatus på systemnivå eller standardstatus på gruppnivå.

## Åtkomstkrav

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassade standardstatusvärden på systemnivå

När du anger en anpassad status som standardsystemstatus ärver alla nya grupper som skapas i systemet den statusen.

Grupper som redan fanns när du angav den nya standardsystemstatusen ärver inte automatiskt den.

Anta till exempel att det redan finns två grupper i din Adobe Workfront-miljö (Marknadsföring och Försäljning). Du skapar en ny anpassad status som motsvarar aktuell och anropar statusen Pågår. Nu skapar du en ny grupp som kallas Engineering. I detta scenario ärver konstruktörsgruppen den nya standardstatusen. marknadsförings- och säljgrupperna inte gör det.

## Anpassade standardstatusvärden på gruppnivå

En anpassad status som du anger som standardgruppstatus används i följande fall:

* **När Workfront-systemet automatiskt väljer en status används standardgruppstatusen:** Den anpassade status som du anger som standardgruppstatus används när Workfront automatiskt tilldelar ett objekt en status.

   En uppgift kan till exempel konfigureras så att den automatiskt ändras till Fullständig status när procentandelen är 100 %. Om du skapar en anpassad status som är lika med Fullständig och du anger den anpassade statusen som standardstatus, ändrar Workfront aktivitetens status till den nya standardstatusen.

   Anpassade statusvärden används bara på det här sättet med gruppstatusvärden som är kopplade till en aktivitet eller ett problem. Anpassade statusvärden kan inte användas på det här sättet för statusvärden som är kopplade till ett projekt.

* The **statusen för ett projekt bestäms av den grupp som är associerad med projektet**: Om gruppen som är associerad med ett visst projekt ändras, ändras projektets status beroende på standardstatusvärdena som har definierats för gruppen. (En grupp kan kopplas till ett projekt via fältet Grupper när du redigerar projektet.)

   Om den gruppen ändras ändras, ändras projektets status om den nya gruppen har en annan definierad standardstatus som motsvarar projektets aktuella status.

   Ett projekt kan t.ex. associeras med marknadsföringsgruppen och projektets status anges till Planering. Projektet redigeras så att det nu associeras med försäljningsgruppen. Försäljningsgruppen har en anpassad standardgruppstatus som heter Thinking (och den här statusen motsvarar Planning). Eftersom gruppen i projektet ändrades ändras projektstatusen till Tänkning.

Om du är gruppadministratör kan du läsa [Ange en status som standardstatus för en grupp](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Utfärdandestatus

Om den anpassade statusen är Problem, måste alla fyra problemtyperna aktiveras för den (Felrapport, Ändra ordning, Problem och Begäran). I den utgivningsstatus som visas nedan kan statusen Återöppnad inte användas som standardstatus eftersom typen Ändra ordning inte har valts:

![](assets/all-4-issue-types-enabled.png)

## Ange en anpassad status som standardstatus

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).
1. Klicka på i den vänstra panelen **Projektinställningar** > **Status**.
1. (Villkorligt) Om du anger en standardstatus för en grupp börjar du med att skriva namnet på gruppen på menyn i det övre högra hörnet och markerar den när den visas.
1. Öppna **Projekt**, **Uppgifter**, eller **Problem** beroende på vilken typ av status du vill ange som standardstatus.
1. Klicka på **Ange standardstatus** nedrullningsbar meny.
1. I listrutan som visas väljer du den standardstatus som du vill använda bredvid den status där du vill ange standardstatus.
1. Klicka **Spara**.
1. Associera projektet med gruppen där statusen finns.

   >[!NOTE]
   >
   >Om du anger anpassad status för en grupp och sedan tilldelar projektet till en annan grupp, läses projektstatusen in igen och kan ändras.

   1. Gå till det projekt där du vill använda den anpassade statusen.
   1. Klicka på Mer-menyn ![](assets/more-icon.png)och sedan klicka **Redigera**.
   1. I **Redigera projekt** som visas i **Grupp** fält under **Projektassociation** väljer du den grupp där statusen finns.
   1. Klicka **Spara ändringar**.
