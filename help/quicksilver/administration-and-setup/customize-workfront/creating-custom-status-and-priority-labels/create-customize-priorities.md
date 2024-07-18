---
title: Skapa och anpassa prioriteringar
description: Du kan styra prioriteter för projekt, uppgifter och utgåvor under Konfigurera i Workfront. Prioriteringarna lägger stor vikt vid projekt, uppgifter och problem i Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Skapa och anpassa prioriteringar

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Du kan styra prioriteter för projekt, uppgifter och utgåvor under Konfigurera i Workfront. Prioriteringarna lägger stor vikt vid projekt, uppgifter och problem i Adobe Workfront.

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa befintliga prioriteringar

Som Workfront-administratör kan du göra följande ändringar av standardprioriteterna i Workfront:

* Byt namn på prioriteter.
* Ändra ordningen på prioriteterna.

  Mer information om hur du ändrar ordning på prioriteter finns i [Skapa en prioritet för en projektuppgift eller Problem](#create-a-priority-for-a-project-task-or-issue).

* Ändra standardprioritet.

  Mer information om hur du ändrar standardprioritet finns i [Skapa en prioritet för en projektuppgift eller ett problem](#create-a-priority-for-a-project-task-or-issue).

* Redigera beskrivningen för prioriteterna.
* Ange en färg för varje prioritet.

  Färgen på prioriteten används i diagramrapporter när du grupperar dina resultat efter **Prioritet**.

  Mer information om diagramrapporter finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Ta bort prioriteter.

  När du tar bort en befintlig prioritet måste du välja en annan.

* Dölj prioriteter.

  Mer information om hur du döljer prioriteter finns i [Skapa en prioritet för en projektuppgift eller ett problem](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Du måste ha minst en prioritet i ditt Workfront-konto för varje objekt.

Prioriteringarna som anges som standard för varje objekttyp (projekt, uppgift och utgåva) är identiska:

* Ingen
* Låg
* Normal
* Hög
* Urgent

## Skapa en prioritet för en projektuppgift eller ett ärende {#create-a-priority-for-a-project-task-or-issue}

Förutom standardprioriteringarna i Workfront kan du lägga till egna prioriteringar som speglar organisationens behov.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Projektinställningar** > **Prioriteter** i den vänstra panelen.

1. Klicka på fliken för den objekttyp som du vill skapa en prioritet för (**Projekt**, **Aktivitet** eller **Problem**).
1. Klicka på **Lägg till en ny prioritet**.
1. Ange följande information för den nya prioriteten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prioritetsnamn</td> 
      <td>Ange ett namn för prioriteten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioritet</td> 
      <td> <p>När du lägger till en ny prioritet tilldelas den som standard ett nummer. Redigera det här numret om det inte passar dina behov.</p> <p><strong>Importance</strong>-numret för varje prioritet måste vara unikt för det valda objektet.<br>Antalet prioriteter återspeglar vikten av projektet, aktiviteten eller utgåvan: det högsta antalet motsvarar den högsta prioriteten.</p> <p><b>Obs!</b> Du kan inte redigera prioritetsnumret när du har sparat prioriteten. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Färg</td> 
      <td> <p>Välj en färg som du vill prioritera.</p> <p>Färgen på prioriteten används i diagramrapporter och Agile Team Settings. Mer information om diagramrapporter finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Lägga till ett diagram i en rapport</a>.</p> <p>Mer information om Agile Team-inställningar finns i .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardprioritet</td> 
      <td> <p>Bestäm om detta ska vara standardprioritet eller inte genom att markera alternativknappen.</p> <p>Om en prioritet har angetts som <strong>standardprioritet</strong> väljs den automatiskt för alla projekt, aktiviteter eller utgåvor i Workfront. <strong>Normal</strong> är standardprioritet för alla objekt i Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Lägg till en beskrivning av prioriteten för att förklara dess funktion.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dölj</td> 
      <td> <p>Markera den här rutan om du vill dölja prioriteten.</p><p>När du väljer alternativet <b>Dölj</b> visas inte prioriteten någonstans i Workfront och användarna kan inte välja den för sina projekt, uppgifter och ärenden.</p> 
      <p><b>VIKTIGT</b>: Vi rekommenderar att du döljer de prioriteringar som du inte längre vill använda, i stället för att ta bort dem. Genom att dölja dem sparar du fortfarande alla historiska data om objekt som har slutförts med den här prioriteten, samtidigt som du förhindrar att andra väljer den här prioriteten i framtiden. </p>
      <p>Om du vill kan du ändra ordningen på prioriteterna genom att dra och släppa dem i önskad ordning. Detta ändrar visningsordningen för projekt, uppgifter och ärenden. Detta ändrar inte <b>Importance</b>-numret. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

Instruktioner om hur du prioriterar projekt, uppgifter och problem finns i följande artiklar:

* [Förstå och uppdatera projektprioriteringar](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Uppdatera aktivitetsprioritet](../../../manage-work/tasks/task-information/task-priority.md)
* [Uppdatera prioritet för utgåva](../../../manage-work/issues/issue-information/update-issue-priority.md)
