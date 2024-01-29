---
product-area: projects
navigation-topic: create-tasks
title: Skapa underaktiviteter
description: I Workfront kan uppgifter ha överordnade och underordnade relationer. Underordnade uppgifter kallas underaktiviteter. Du kan skapa underuppgifter i uppgiftslistan genom att göra en huvuduppgift till en underuppgift. Du kan också göra en underuppgift till en huvuduppgift.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Skapa underaktiviteter

<!-- Audited: 1/2024 -->

I Workfront kan uppgifter ha överordnade och underordnade relationer. Underordnade uppgifter kallas underaktiviteter. Du kan skapa underuppgifter i uppgiftslistan genom att göra en huvuduppgift till en underuppgift. Du kan också göra en underuppgift till en huvuduppgift.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Nytt: Standard</p>
   <p>Aktuell: Arbete eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter för projektet och den överordnade aktiviteten med möjlighet att lägga till uppgifter eller högre</p> <p>Du får automatiskt behörigheten Hantera för uppgiften när du har skapat den.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Skapa underaktiviteter

Du kan skapa underaktiviteter från uppgiftslistan eller underaktivitetsavsnittet.

### Skapa underaktiviteter från uppgiftslistan {#create-subtasks-from-the-task-list}

1. Gå till det projekt där du vill skapa underaktiviteter.
1. Klicka på **Uppgifter** i den vänstra panelen.
1. (Villkorligt) Om den uppgift som du vill göra till den underordnade uppgiften inte redan finns direkt under den uppgift som du vill göra till överordnad drar du den till lämplig plats i uppgiftslistan.
1. Markera den uppgift som du vill göra en underuppgift och gör något av följande:

   * Klicka på **Indrag** icon ![](assets/indent-icon-nwe-33x29.png) om du vill göra den markerade uppgiften till en underuppgift till uppgiften direkt ovanför den.
   * När du använder ett vanligt engelskt QWERTY-tangentbord trycker du på Alt + > (Mac) eller Alt + > (Windows) på tangentbordet. Andra språk kan använda kommandona Alt + , (Mac) eller Alt + , (Windows) för att dra in.

     >[!TIP]
     >
     >Kortkommandon fungerar inte när du redigerar uppgifter i en infogad redigering. I det här fallet använder du ikonen Indrag ![](assets/cs1.png) för att skapa underaktiviteter.

   * Dra och släpp uppgiften över den uppgift som du vill ange som överordnad uppgift.

     >[!NOTE]
     >
     >Du kan bara dra in uppgifter när listan med uppgifter sorteras efter Uppgiftsnummer och när inga grupper används i uppgiftslistan.

### Skapa underaktiviteter från aktivitetsavsnittet Underaktiviteter {#create-subtasks-from-the-task-subtasks-section}

1. Gå till det projekt där du vill skapa underaktiviteter.
1. Klicka på **Uppgifter** i den vänstra panelen.
1. Klicka på namnet på den uppgift där du vill skapa en underuppgift.
1. Klicka på **Underaktiviteter** i den vänstra panelen.
1. Klicka **Ny uppgift.**

   Följ stegen i följande artikel för att fortsätta skapa underuppgiften: [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Klicka **Spara uppgift.**

## Göra en underaktivitet till en huvuduppgift

1. Gå till det projekt där du vill göra en underaktivitet till en huvuduppgift.
1. Klicka på **Uppgifter** i den vänstra panelen.
1. Markera den underaktivitet som du vill göra till huvuduppgift.
1. Klicka på **Minska indrag** icon ![](assets/outdent-icon-nwe-31x29.png) för att göra underaktiviteten till en huvuduppgift.

   eller

   Tryck på Option + &lt; (Mac) eller Alt + &lt; (Windows) på ett vanligt engelskt QWERTY-tangentbord. Andra språk kan använda kommandona Alt + . (Mac) eller Alt + . (Windows) till Minska indrag.

   >[!NOTE]
   >
   >Du kan bara dra ut uppgifter när listan med uppgifter sorteras efter Uppgiftsnummer och när inga grupperingar används i uppgiftslistan.
