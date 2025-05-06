---
product-area: projects
navigation-topic: use-predecessors
title: Skapa en föregående relation med området Föregående
description: Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Skapa en föregående relation med området Föregående

<!-- Audited: 5/2025 -->

Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en grupp (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).

I den här artikeln visas hur du kan ställa in föregångare med hjälp av fliken Föregående för en uppgift.

Mer information om hur du ställer in föregående aktiviteter i en lista med uppgifter finns i [Skapa en föregående relation i uppgiftslistan](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Du kan visa föregående aktiviteter för uppgifter i följande områden i Adobe Workfront:

* I avsnittet Föregående aktiviteter för beroende uppgifter
* I Gantt-schemat
* I uppgiftslistan i kolumnen Föregående

Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <p>Nytt: Standard </p>
   <p>eller </p>
   <p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en föregångare för en uppgift

1. Navigera till uppgiften som du vill ange som en beroende uppgift.

1. Klicka på **Föregående** i den vänstra panelen.

1. Klicka på **+Lägg till föregående** i avsnittet **Föregående**. Dialogrutan **Lägg till föregående** öppnas.

1. (Valfritt) Om du vill lägga till en föregångare för flera projekt ersätter du namnet på projektet i fältet **Överordnat projekt** med ett annat projekt.

   Mer information finns i [Skapa föregående projekt mellan projekt](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. I fältet **Uppgifter** skriver du in namnet på den eller de uppgifter som du vill utse till föregående aktiviteter och markerar dem sedan när de visas i listrutan.

1. Välj en **beroendetyp**.

   Mer information finns i [Översikt över aktivitetsberoendetyper](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Ange ett **Lag**-belopp.

   Mer information finns i &#x200B;[Översikt över fördröjda typer](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Dialogrutan Lägg till föregående](assets/add-predecessor-dialog-box.png)

1. Markera kryssrutan **Kräv** om du vill framtvinga den föregående relationen mellan de två aktiviteterna.

   Mer information finns i [Tvinga föregående](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Klicka på **Spara**.
