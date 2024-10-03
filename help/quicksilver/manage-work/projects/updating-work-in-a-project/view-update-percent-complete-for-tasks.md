---
product-area: projects
navigation-topic: update-work-in-a-project
title: Visa och uppdatera procent färdigt för aktiviteter
description: Du kan uppdatera procentandelen färdigt för en uppgift för att ange förloppet som du har gjort för uppgiften att slutföra den.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Visa och uppdatera Procent färdigt för uppgifter

<!--Audited:01/2024-->

Du kan uppdatera procentandelen färdigt för en uppgift för att ange förloppet som du har gjort för uppgiften att slutföra den.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna uppdatera uppgifter manuellt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Ny licens: Standard</p> 
   eller
   <p>Aktuell licens: Arbeta eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för uppgiften</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Områden där du kan uppdatera procentandelen färdigt för en uppgift

Du kan uppdatera procentandelen färdigt för en aktivitet i följande områden:

* **I en uppgiftslista**: Du kan uppdatera procentandelen färdigt för en aktivitet när kolumnen Procent färdigt visas.\
  Mer information om infogad redigering finns i [Redigera objekt i en lista i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **I milstolpevyn**: Du kan uppdatera procentandelen färdigt för en aktivitet när du använder milstolpevyn i en projektlista eller en projektrapport. Mer information finns i [Använd vyn Milstolpe](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **I uppgiftshuvudet**: Du kan uppdatera procentandelen färdigt för en aktivitet i uppgiftshuvudet. Mer information finns i [Redigera uppgifter](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **På sammanfattningspanelen för en uppgift**: Du kan uppdatera procentandelen färdigt för en uppgift högst upp på sammanfattningspanelen när du visar uppgiften i följande områden:

   * Uppgiftslista eller rapport
   * Tidrapport
   * Utjämning av arbetsbelastning

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Mer information finns i [Sammanfattning](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Hem**: Du kan uppdatera procentandelen färdigt för en uppgift eller ett problem från panelen Sammanfattning i Hem eller från widgeten Mitt arbete.

Mer information finns i [Komma igång med nya Hem](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

## Att tänka på när du uppdaterar procentandelen färdigt för en uppgift

* När du har markerat en uppgift som 100 % slutförd uppdateras aktivitetens status till Fullständig.
* Följande scenarier finns för överordnade uppgifter:
   * Du kan inte uppdatera procentandelen färdigt för en överordnad aktivitet till 100 % när projektets slutföringsläge för sammanfattning är inställt på Automatisk och underaktiviteterna inte är slutförda.
   * Du kan uppdatera procentandelen färdigt för en överordnad aktivitet till 100 % när projektets slutföringsläge för sammanfattning är inställt på Manuellt och underaktiviteterna är slutförda eller ofullständiga.

  Mer information finns i [Redigera projekt](../manage-projects/edit-projects.md).

## Uppdatera procentandelen slutfört för en uppgift

1. Gå till något av följande i Workfront:

   * En uppgiftslista
   * En lista över projekt och använd vyn Milstolpe
   * En uppgift genom att gå till uppgiftssidan
1. Leta reda på fältet **Procent färdigt** för den uppgift vars procent du vill uppdatera.

   >[!TIP]
   >
   >  Fältet Procent färdigt visas alltid högst upp på panelen Sammanfattning.


1. Klicka i fältet **Procent färdigt** och skriv ett tal mellan 0 och 100

   eller

   Klicka och dra fältet **Procent färdigt** till det nummer som behövs för att ange hur mycket av uppgiften du slutförde när den är tillgänglig.

   >[!NOTE]
   >
   >När du anger att 100 % av aktiviteten är slutförd uppdateras även aktivitetens status till Fullständig.


1. Tryck på Retur på tangentbordet för att spara procentandelen färdig.

Procent färdigt i projektet uppdateras också automatiskt.

