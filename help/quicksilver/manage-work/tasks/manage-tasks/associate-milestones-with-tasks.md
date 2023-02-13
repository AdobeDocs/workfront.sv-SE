---
product-area: projects
navigation-topic: manage-tasks
title: Koppla milstolpar till uppgifter
description: Du kan associera milstolpar med uppgifter för att ange när du når viktiga steg i projektets livstid.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Koppla milstolpar till uppgifter

Du kan associera milstolpar med uppgifter för att ange när du når viktiga steg i projektets livstid.

## Åtkomstkrav

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>Redigera åtkomst till uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för uppgiften</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du kan associera en milstolpe med en uppgift måste följande finnas:

* Workfront-administratören måste skapa en milstolpe-sökväg enligt beskrivningen i [Skapa en milstolpbana](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Om du vill associera en milstolpe-sökväg med ett projekt måste projektet ha statusen Planering eller Aktuell.

>[!TIP]
>
>För att få bästa möjliga överblick över hur milstolparna i dina projekt utvecklas i vyn Milstolpe bör du skapa överordnade uppgifter och associera dem med varje större fas i projektet. Koppla sedan dessa överordnade uppgifter till var och en av milstolparna i milstolpen.

## Koppla en milstolpe till en uppgift

1. Gå till ett projekt och klicka sedan på **Mer** icon ![](assets/more-icon.png)sedan **Redigera**.
1. Använda **Inställningar** anger du den milstolpe-väg som ska användas i projektet.
1. Klicka **Spara**.

   När en milstolpe-sökväg har associerats med ett projekt kan uppgifter tilldelas en milstolpe.

1. Gå till en uppgift och klicka sedan på **Mer** icon ![](assets/more-icon.png)sedan **Redigera**.

   Aktiviteter och milstolpar har ett 1:1-förhållande. Du kan inte koppla samma milstolpe till flera uppgifter. Varje aktivitet kan länkas till en enskild milstolpe, eller varje milstolpe kan mappas till en aktivitet.

1. Klicka **Inställningar** väljer du sedan en milstolpe i **Milstolpe** för uppgiften.
1. Klicka **Spara**.
1. (Valfritt) Lägg till **Statusikoner** -kolumn för att identifiera vilka aktiviteter som har milstolpar.

   ![](assets/amwt3.png)

1. (Valfritt) I en lista med projekt väljer du **Milstolpe** för att identifiera förloppet för dina milstolpeuppgifter.

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
