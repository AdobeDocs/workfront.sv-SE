---
product-area: projects
navigation-topic: create-tasks
title: Skapa underaktiviteter
description: I Adobe Workfront kan uppgifter ha överordnade och underordnade relationer. Underordnade uppgifter kallas underaktiviteter. Du kan skapa underuppgifter i uppgiftslistan genom att göra en huvuduppgift till en underuppgift. Du kan också göra en underuppgift till en huvuduppgift.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Skapa underaktiviteter

<!-- Audited: 01/2025 -->

I Adobe Workfront kan uppgifter ha överordnade och underordnade relationer. Underordnade uppgifter kallas underaktiviteter. Du kan skapa underuppgifter i uppgiftslistan genom att göra en huvuduppgift till en underuppgift. Du kan också göra en underuppgift till en huvuduppgift.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Contribute-behörigheter till projektet och den överordnade aktiviteten med möjlighet att lägga till uppgifter eller högre</p> <p>Du får automatiskt behörigheten Hantera för uppgiften när du har skapat den.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa underaktiviteter

Du kan skapa underaktiviteter från uppgiftslistan eller underaktivitetsavsnittet.

### Skapa underaktiviteter från uppgiftslistan {#create-subtasks-from-the-task-list}

1. Gå till det projekt där du vill skapa underaktiviteter.
1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.
1. (Villkorligt) Om den uppgift som du vill göra till den underordnade uppgiften inte redan finns direkt under den uppgift som du vill göra till överordnad, drar och släpper du den till rätt plats i uppgiftslistan.
1. Markera den uppgift som du vill göra en underuppgift och gör något av följande:

   * Klicka på ikonen **Indrag** ![](assets/indent-icon-nwe-33x29.png) för att göra den markerade aktiviteten till en underaktivitet för aktiviteten direkt ovanför den.
   * När du använder ett vanligt engelskt QWERTY-tangentbord trycker du på Alt + > (Mac) eller Alt + > (Windows) på tangentbordet. Andra språk kan använda kommandona Alt + , (Mac) eller Alt + , (Windows) för att dra in.

     >[!TIP]
     >
     >Kortkommandon fungerar inte när du redigerar uppgifter i en infogad redigering. I det här fallet använder du ikonen Indrag ![](assets/indent-icon-nwe-33x29.png) för att skapa underaktiviteter.

   * Dra och släpp uppgiften över den uppgift som du vill ange som överordnad uppgift.

     >[!NOTE]
     >
     >Du kan bara dra in uppgifter när listan med uppgifter sorteras efter Uppgiftsnummer och när inga grupper används i uppgiftslistan.

### Skapa underaktiviteter från aktivitetsavsnittet Underaktiviteter {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>Din Workfront- eller gruppadministratör kan ta bort underuppgiftsavsnittet i din miljö med hjälp av en layoutmall.

1. Gå till det projekt där du vill skapa underaktiviteter.
1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.
1. Klicka på namnet på den uppgift där du vill skapa en underuppgift.
1. Klicka på avsnittet **Underaktiviteter** i den vänstra panelen, om det finns några.
1. Klicka på **Ny aktivitet.**

   Följ stegen i följande artikel för att fortsätta skapa underaktiviteten: [Skapa aktiviteter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Klicka på **Skapa uppgift.**

## Göra en underaktivitet till en huvuduppgift

1. Gå till det projekt där du vill göra en underaktivitet till en huvuduppgift.
1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.
1. Markera den underaktivitet som du vill göra till huvuduppgift.
1. Klicka på ikonen **Minska indrag** ![](assets/outdent-icon-nwe-31x29.png) för att göra underaktiviteten till en huvuduppgift.

   eller

   Tryck på Option + &lt; (Mac) eller Alt + &lt; (Windows) på ett vanligt engelskt QWERTY-tangentbord. Andra språk kan använda kommandona Alt + . (Mac) eller Alt + . (Windows) till Minska indrag.

   >[!NOTE]
   >
   >Du kan bara dra ut uppgifter när listan med uppgifter sorteras efter Uppgiftsnummer och när inga grupperingar används i uppgiftslistan.
