---
title: Skapa och anpassa prioriteringar
description: Du kan styra prioriteter för projekt, uppgifter och utgåvor under Konfigurera i Workfront. Prioriteringarna lägger stor vikt vid projekt, uppgifter och problem i Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 7db80f5bacf52b7bbe540f4e38e88853af86a5e2
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Skapa och anpassa prioriteringar

{{highlighted-preview}}

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Du kan styra prioriteter för projekt, uppgifter och utgåvor under Konfigurera i Workfront. Prioriteringarna lägger stor vikt vid projekt, uppgifter och problem i Adobe Workfront.

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
     <p>Nytt: Standard</p>
     <p>eller</p>
     <p>Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassa befintliga prioriteringar

Som Workfront-administratör kan du göra följande ändringar av standardprioriteterna i Workfront:

* Byt namn på prioriteter.
* Ändra ordningen på prioriteterna.

  Mer information om hur du ändrar ordning på prioriteter finns i [Skapa en prioritet för ett projekt, en aktivitet eller ett problem](#create-a-priority-for-a-project-task-or-issue).

* Ändra standardprioritet.

  Mer information om hur du ändrar standardprioritet finns i [Skapa en prioritet för ett projekt, en uppgift eller ett problem](#create-a-priority-for-a-project-task-or-issue).

* Redigera beskrivningen för prioriteterna.
* Ange en färg för varje prioritet.

  Färgen på prioriteten används i diagramrapporter när du grupperar dina resultat efter **Prioritet**.

  Mer information om diagramrapporter finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Ta bort prioriteter.

  När du tar bort en befintlig prioritet måste du välja en annan.

* Dölj prioriteter.

  Mer information om hur du döljer prioriteter finns i [Skapa en prioritet för ett projekt, en uppgift eller ett problem](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Du måste ha minst en prioritet i ditt Workfront-konto för varje objekt.

Prioriteringarna som anges som standard för varje objekttyp (projekt, uppgift och utgåva) är identiska:

* Ingen
* Låg
* Normal
* Hög
* Urgent

## Skapa en prioritet för ett projekt, en uppgift eller ett ärende {#create-a-priority-for-a-project-task-or-issue}

Förutom standardprioriteringarna i Workfront kan du lägga till egna prioriteringar som speglar organisationens behov.

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Prioriteter** i den vänstra panelen.

1. Klicka på fliken för den objekttyp som du vill skapa en prioritet för (**Projekt**, **Aktivitet** eller **Problem**).
1. Klicka på <span class="preview">**Ny rad** längst ned i tabellen</span> eller **Lägg till ny prioritet**.
1. Konfigurera följande alternativ för prioriteten:

   * **Prioritetsnamn**: Ange ett namn för prioriteten.
   * **Viktighet**: När du lägger till en ny prioritet tilldelas den ett nummer som standard. Redigera det här numret om det inte passar dina behov.

     Importnumret för varje prioritet måste vara unikt. Antalet prioriteter återspeglar projektets, uppgiftens eller frågans betydelse: det högsta antalet motsvarar den högsta prioriteten.

     Du kan inte redigera det här numret när du har sparat prioriteten.

   * **Färg**: Välj en färg för prioriteten.

     Färgen på prioriteten används i diagramrapporter och Agile Team Settings. Mer information om diagramrapporter finns i [Lägga till ett diagram i en rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md). Mer information om Agile Team-inställningar finns i [Skapa ett smidigt team](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * **Standardprioritet**: Välj den prioritet du vill att Workfront ska tillämpa automatiskt på alla nyskapade projekt, aktiviteter eller utgåvor.

     **Normal** är standardprioritet för alla objekt i Workfront.

     Du kan inte göra en dold prioritet till standard.

     <div class="preview">

     Standardprioriteten anges med ikonen ![Standardprioritet](assets/default-icon.png). Gör något av följande om du vill välja en ny standard:

      * Markera kryssrutan bredvid prioritetsnamnet och välj **Gör standard** i åtgärdsfältet längst ned på skärmen.
      * Håll muspekaren över prioritetsnamnet och klicka på menyn **Mer** som visas. Välj sedan **Använd som standard**.

        Den nya standardprioriteten anges med ikonen .

     </div>

   * **Beskrivning**: Ange en beskrivning av prioriteten för att förklara dess funktion.
   * <span class="preview">**Dölj alternativ**</span> eller **Dölj**: <span class="preview">Välj **Ja**</span> eller markera kryssrutan om du vill dölja en prioritet som inte längre behövs.

     En dold prioritet visas inte någonstans i Workfront, så användarna kan inte välja den för sina projekt, uppgifter eller ärenden.

     >[!IMPORTANT]
     >
     >Istället för att ta bort prioriteringar som du inte längre vill använda föreslår vi att du döljer dem. På så sätt behåller du alla historiska data om objekt som redan har slutförts med prioritet samtidigt som du förhindrar att andra använder prioriteten i framtiden.

1. (Valfritt) Ändra listordningen för dina prioriteringar genom att dra och släppa dem i önskad ordning.

   Detta ändrar visningsordningen för projekt, uppgifter eller utgåvor. Det ändrar inte **Importance**-numret.

1. Klicka på **Spara**.

Instruktioner om hur du prioriterar projekt, uppgifter och problem finns i följande artiklar:

* [Förstå och uppdatera projektprioriteringar](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Uppdatera aktivitetsprioritet](../../../manage-work/tasks/task-information/task-priority.md)
* [Uppdatera prioritet för utgåva](../../../manage-work/issues/issue-information/update-issue-priority.md)
