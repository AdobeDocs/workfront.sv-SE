---
product-area: projects
navigation-topic: update-work-in-a-project
title: Visa och uppdatera procent färdigt för aktiviteter
description: Du kan uppdatera procentandelen färdigt för en uppgift för att ange förloppet som du har gjort för uppgiften att slutföra den. Att uppdatera procentandelen slutförd för problem liknar att uppdatera den för en aktivitet. I den här artikeln beskrivs hur du uppdaterar procentandelen färdigt för en uppgift.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Visa och uppdatera Procent färdigt för uppgifter

<!--Audited: 05/2025-->

Du kan uppdatera procentandelen färdigt för en uppgift för att ange förloppet som du har gjort för uppgiften att slutföra den.

Att uppdatera procentandelen slutförd för problem liknar att uppdatera den för en aktivitet. I den här artikeln beskrivs hur du uppdaterar procentandelen färdigt för en uppgift.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Arbeta eller högre</p>
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

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Områden där du kan uppdatera procentandelen färdigt för en uppgift

Du kan uppdatera procentandelen färdigt för en aktivitet i följande områden:

* **I en uppgiftslista**: Du kan uppdatera procentandelen färdigt för en aktivitet när kolumnen Procent färdigt visas.

  Mer information om infogad redigering finns i [Redigera objekt i en lista i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **I milstolpevyn**: Du kan uppdatera procentandelen färdigt för en aktivitet när du använder milstolpevyn i en projektlista eller en projektrapport.

  >[!TIP]
  >
  >  Du kan inte uppdatera procentandelen färdiga problem i vyn Milstolpe.


  Mer information finns i [Använd vyn Milstolpe](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **I uppgiftshuvudet**: Du kan uppdatera procentandelen färdigt för en aktivitet i uppgiftshuvudet.

  ![Uppdatera procent i huvudet](assets/nwe-updatetaskpercentinheader-350x54.png)

* **På sammanfattningspanelen för en uppgift**: Du kan uppdatera procentandelen färdigt för en uppgift högst upp på sammanfattningspanelen när du visar uppgiften i följande områden:

   * Uppgiftslista eller rapport
   * Tidrapport
   * Utjämning av arbetsbelastning

  ![Uppdateringsprocent i aktivitetssammanfattning är markerat](assets/update-percent-complete-in-task-summary-highlighted.png)

  Mer information finns i [Sammanfattning](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Hem**: Du kan uppdatera procentandelen färdigt för en uppgift eller ett problem från panelen Sammanfattning i Hem eller från widgeten Mitt arbete.

  Mer information finns i [Komma igång med Hem](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Att tänka på när du uppdaterar procentandelen färdigt för en uppgift

* När du har markerat en uppgift som 100 % slutförd uppdateras aktivitetens status till Fullständig. Status för ett problem uppdateras till Stängt.
* När du slutför en uppgift uppdateras även procentandelen slutfört för det överordnade projektet och för projektet.
* Följande scenarier finns för överordnade uppgifter och projekt:
   * Du kan inte uppdatera procentandelen färdigt för en överordnad aktivitet till 100 % när projektets slutföringsläge för sammanfattning är inställt på Automatisk och underaktiviteterna inte är slutförda.
   * Du kan uppdatera procentandelen färdigt för en överordnad aktivitet eller ett projekt till 100 % när projektets slutföringsläge är inställt på Manuellt och underaktiviteterna är slutförda eller ofullständiga.

  Mer information finns i [Redigera projekt](../manage-projects/edit-projects.md).

## Uppdatera procentandelen slutfört för en uppgift

1. Gå till något av de områden där du vill uppdatera procentandelen färdigt för en uppgift.

   Mer information finns i avsnittet [Områden där du kan uppdatera procentandelen färdigt för en uppgift](#areas-where-you-can-update-the-percent-complete-of-a-task) i den här artikeln.

1. Leta reda på fältet **Procent färdigt** för den uppgift vars procent du vill uppdatera.

   >[!TIP]
   >
   >Fältet Procent färdigt visas alltid högst upp på panelen Sammanfattning.

1. Klicka i fältet **Procent färdigt** och skriv ett tal mellan 0 och 100

   eller

   Klicka och dra den blå bubblan **Procent färdigt** till det nummer som behövs för att ange hur mycket av uppgiften du slutförde när den är tillgänglig.

   >[!NOTE]
   >
   >    * Du kan inte ange ett decimaltal när du klickar i bubblan Procent färdigt.
   >    * När du drar och släpper den blå bubblan på panelen Sammanfattning uppdateras Procent färdigt i steg om en punkt.
   >
   >    * När du drar och släpper den blå bubblan i uppgiftshuvudet uppdateras Procent färdigt i steg om 5 punkter.

1. Tryck på Retur på tangentbordet för att spara procentandelen färdig.

   Procent färdigt för projektet eller andra överordnade uppgifter kan också uppdateras automatiskt.

   Uppgiftens eller problemets status uppdateras också.

