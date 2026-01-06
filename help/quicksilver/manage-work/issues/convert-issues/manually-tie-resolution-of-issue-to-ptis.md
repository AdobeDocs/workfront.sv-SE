---
product-area: projects
navigation-topic: convert-issues
title: Koppla en problemlösning till andra problem, uppgifter eller projekt manuellt
description: Du kan koppla en problemlösning manuellt till en lösning på ett projekt, en uppgift eller ett problem utan att konvertera problemet. Problemet blir ett av de objekt som kan lösas i projektet, uppgiften eller problemet som du väljer. När du gör detta ändras statusen för projektet, aktiviteten eller utgåvan av statusen för den ursprungliga utgåvan.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Koppla lösningen av ett problem manuellt till andra problem, uppgifter eller projekt

<!--Audited: 08/2025-->

Du kan koppla en problemlösning manuellt till en lösning på ett projekt, en uppgift eller ett problem utan att konvertera problemet. Problemet blir ett av de objekt som kan lösas i projektet, uppgiften eller problemet som du väljer. När du gör detta ändras statusen för projektet, aktiviteten eller utgåvan av statusen för den ursprungliga utgåvan.

>[!TIP]
>
>När du kopplar en problemlösning till ett annat objekts upplösning kan du inte längre manuellt redigera status för det ursprungliga problemet.

Mer information om hur du löser och löser problem finns i [Översikt över objekt som kan lösas och lösas](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

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
   <td><p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem, uppgifter, projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för det problem som du länkar till ett annat problem, en annan uppgift eller ett annat projekt</p> <p>Visa eller högre behörigheter för det problem, den uppgift eller det projekt som du lägger till i det befintliga problemet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

Innan du börjar måste du:

* Har ett problem vars lösning du vill koppla till en lösning av ett annat problem, en annan uppgift eller ett annat projekt

* Har ytterligare ett problem, en uppgift eller ett projekt

## Bind lösningen av ett problem till en lösning av ett annat problem, en annan uppgift eller ett annat projekt

1. Navigera till ett problem vars lösning du vill koppla till en lösning på ett annat problem eller till lösningen av en uppgift eller ett projekt.
1. Klicka på **Utleveransinformation** i den vänstra panelen och utöka området **Översikt**.

   ![Ikon för probleminformation](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Klicka på fältet **Löst av** och välj bland följande typer av matchande objekt:

   * **Projekt**
   * **Aktivitet**
   * **Utgåva**

   Beroende på vilket objekt du har markerat visas följande fält:

   * **Åtgärdar projekt**
   * **Åtgärdar aktivitet**
   * **Löser problem**

1. Börja skriva namnet på ett visst projekt, en viss aktivitet eller ett specifikt problem i fältet **Lösa projekt**, **aktivitet** eller **Problem** och klicka sedan på det när det visas i listan.

   >[!NOTE]
   >
   >Du kan inte koppla en problemlösning till den uppgift eller det projekt där problemet finns. Aktiviteten eller projektet för problemet visas inte i fälten Lös uppgift eller Lös uppgift.


1. Klicka på **Spara ändringar**.

   Det ursprungliga problemet blir ett löstagbart objekt för det projekt, den uppgift eller det problem som du valde i steg 4 och 5. Detta innebär att det ursprungliga problemet slutförs när det matchande objektet (projektet, aktiviteten eller problemet som du länkade det till) har slutförts.

   >[!NOTE]
   >
   >Ett projekt, en aktivitet eller ett problem kan ha flera problem som upplösbara objekt.
