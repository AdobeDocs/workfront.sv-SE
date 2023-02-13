---
product-area: projects
navigation-topic: use-predecessors
title: Skapa en föregående relation med området Föregående
description: Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Skapa en föregående relation med området Föregående

Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).

I den här artikeln visas hur du kan ställa in föregångare med hjälp av fliken Föregående för en uppgift.

Mer information om hur du ställer in föregående aktiviteter i en lista med uppgifter finns i [Skapa en föregående relation i uppgiftslistan](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Du kan visa föregående aktiviteter för följande områden i Adobe Workfront:

* I avsnittet Föregående aktiviteter för de beroende aktiviteterna
* I Gantt-schemat
* I uppgiftslistan i kolumnen Föregående

Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en föregångare för en uppgift

1. Gå till en uppgift som du vill ange som beroende uppgift och klicka sedan på **Föregående** i den vänstra panelen.

   Du kan behöva klicka **Visa fler** sedan **Föregående**.

1. Klicka **+Lägg till föregående**.
1. (Valfritt) Om du vill lägga till en föregångare för flera projekt ersätter du namnet på projektet i **Överordnat projekt** i ett annat projekt skriver du namnet på den eller de uppgifter som du vill ska vara föregående aktiviteter.

   Mer information om hur du lägger till föregångare för flera projekt finns i [Skapa föregångare mellan projekt](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Skriv namnet på den eller de uppgifter som du vill utse till föregående aktiviteter.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Välj en **Beroendetyp**.

   Mer information om aktivitetsberoendetyper finns i [Översikt över typer av uppgiftsberoenden](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Ange en **Lag** antal dagar.

   Mer information om Lag Types finns i &#x200B; [Översikt över lagertyper](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Välj **Krävs** om du vill framtvinga den föregående relationen mellan de två uppgifterna.

   Mer information om att framtvinga föregående aktiviteter finns i [Tvinga föregående](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Klicka **Spara**.
