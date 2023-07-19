---
product-area: projects
navigation-topic: create-tasks
title: Skapa återkommande uppgifter
description: Du kan skapa återkommande uppgifter för uppgifter som du måste upprepa som en del av ett enda projekt.
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f8d596121f90d4f0c57e65cc415d1df87c14730c
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Skapa återkommande uppgifter

Du kan skapa återkommande uppgifter för uppgifter som du måste upprepa som en del av ett enda projekt.

Allmän information om återkommande uppgifter, inklusive effekten av att redigera en befintlig återkommande uppgift, finns i [Översikt över återkommande uppgifter](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till uppgifter finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Bevilja åtkomst till uppgifter</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter till projektet med möjlighet att lägga till uppgifter eller högre</p> <p>När du skapar en uppgift får du automatiskt behörigheten Hantera för uppgiften</p> <p> Mer information om aktivitetsbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Dela en uppgift </a>. </p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en återkommande uppgift

>[!NOTE]
>
>Du kan inte skapa en återkommande uppgift genom att ändra en befintlig uppgift. Du måste skapa en ny uppgift.

1. Gå till projektet där du vill skapa en återkommande uppgift och klicka sedan på **Uppgifter** i den vänstra panelen.
1. Klicka **Ny uppgift**.

   Dialogrutan Ny uppgift visas.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Klicka **Fler alternativ** anger du ett namn för uppgiften i dialogrutan **Aktivitetsnamn** fält.
1. Fortsätt uppdatera aktiviteten på samma sätt som om du lade till en ny uppgift. Mer information om hur du lägger till en ny uppgift finns i [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   Varaktighet och Planerade timmar som anges för en ny återkommande aktivitet är Varaktighet och Planerade timmar för varje upprepning. Den överordnade aktivitetens varaktighet är tiden mellan det planerade startdatumet för den första aktiviteten och det planerade slutförandedatumet för den senaste aktiviteten. Den överordnade uppgiftens planerade timmar är det totala antalet planerade timmar från alla återkommande aktiviteter.

1. Klicka **Översikt** i den vänstra panelen.
1. Bläddra nedåt till **Återkommande schema** väljer du **Gör detta till en återkommande uppgift** alternativ.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. I **Frekvens** väljer du antalet tidsenheter när du vill att uppgiften ska utföras och typ av tidsenheter. Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Upprepningstyp</th> 
      <th>Beskrivning</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Dag</strong> </td> 
      <td> <p>Uppgiften upprepas varannan dag, varannan dag, var tredje dag och så vidare, beroende på vilken gräns du väljer. Du kan konfigurera aktiviteter så att de upprepas upp till var sjätte dag. Standardinställningen är 1 dag. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Arbetsdag</strong> </td> 
      <td> <p> Uppgiften upprepas varannan arbetsdag, varannan arbetsdag, var tredje arbetsdag och så vidare, beroende på vilken gräns du väljer. Du kan konfigurera aktiviteter så att de upprepas upp till var sjätte arbetsdag.</p> <p>Det här alternativet använder det standardschema som definieras av systemadministratören, vilket beskrivs i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Vecka</strong> </td> 
      <td> <p> Uppgiften upprepas varje vecka, varannan vecka, var tredje vecka och så vidare, beroende på vilken frekvens du väljer.</p> <p>I <strong>Upprepningar</strong> väljer du den dag i veckan då du vill att varje uppgift ska utföras. Du kan välja flera dagar. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Månad</strong> </td> 
      <td> <p>Uppgiften upprepas varje månad, varannan månad, var tredje månad och så vidare, beroende på vilken frekvens du väljer. Du kan välja mellan 1 och 12 månader. </p> <p>I <strong>Upprepningar</strong> väljer du bland följande alternativ när du vill att uppgiften ska utföras:</p> 
       <ul> 
        <li> <p><strong>varje månad &lt;month date=""&gt;</strong> </p> <p>Du kan välja dagar mellan 1 och 30 eller välja <strong>sista</strong>. Du kan t.ex. välja "varje månad den 30:e". </p> </li> 
        <li> <p><strong>varje månad &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>I den första listrutan kan du välja ett tal mellan 1 och 4 för veckonumret i månaden eller så kan du välja "senaste". </p> <p>I den andra listrutan kan du välja vilken veckodag som helst. </p> <p>Du kan t.ex. välja "varje månad den andra tisdagen". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Om du har ett schemaundantag associerat med projektets schema kan återkommande aktiviteter inte starta under undantaget. Återkommande aktiviteter som inträffar under schemaundantaget är schemalagda att starta den första arbetsdagen efter undantaget. Mer information om schemaundantag finns i artikeln [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. I **Börjar** markerar du det datum och den tidpunkt då du vill att de återkommande uppgifterna ska börja.
1. I **Slutar** markerar du det datum och den tidpunkt då du vill att de återkommande uppgifterna ska slutföras

   eller

   Välj **efter `<number>` förekomster** för att ange hur många gånger den återkommande uppgiften ska utföras. Workfront skapar samma antal återkommande aktiviteter för uppgifterna som det antal du anger i det här fältet.

1. Klicka **Skapa uppgift.**

   Uppgiftslistan visas. Den återkommande uppgiften skapas som en överordnad uppgift och alla återkommande aktiviteter är dess underordnade. Workfront genererade automatiskt namnen på de underordnade uppgifterna med det namn du angav för den överordnade uppgiften följt av ett nummer. Mer information om vilka fält som fylls i automatiskt från den överordnade återkommande uppgiften finns i [Översikt över återkommande uppgifter](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Valfritt) Ändra varje återkommande uppgift på samma sätt som andra uppgifter i projektet.

   Du kan till exempel lägga till uppdrag, föregående aktiviteter, varaktigheter och ändra annan information om uppgiften, inklusive anpassade fält.

   >[!IMPORTANT]
   >
   >Om du ändrar den överordnade upprepningen efter att de underordnade objekten har ändrats individuellt kan det leda till att informationen skiljer sig mellan de underordnade och den överordnade. Mer information finns i [Översikt över återkommande uppgifter](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
