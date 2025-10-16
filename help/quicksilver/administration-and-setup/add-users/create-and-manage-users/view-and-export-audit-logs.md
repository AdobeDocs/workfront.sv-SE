---
title: Visa och exportera granskningsloggar
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Du kan visa alla granskningsloggar i systemet eller de som uppfyller vissa filtervillkor. Du kan också exportera granskningsloggar. Granskningsloggar visar användarändringar som har utlösts i systemet under de senaste 90 dagarna.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Visa och exportera granskningsloggar

<!--Audited: 08/2025-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Du kan visa alla granskningsloggar i systemet eller de som uppfyller vissa filtervillkor. Du kan också exportera granskningsloggar till en CSV-fil.

Granskningsloggar visar användarändringar som har utlösts i systemet under de senaste 90 dagarna.

Mer information om alla granskningsloggtyper och vad som genererar dem finns i [Översikt över granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td><p>Systemadministratör</p></td>
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
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>System Administrator</p></td>
  </tr> 
 </tbody> 
</table>-->

## Visa granskningsloggar

{{step-1-to-setup}}

1. Klicka på **System > Granskningsloggar** i den vänstra panelen.
1. I listrutan **Åtgärdstyp** väljer du vilken typ av granskning du vill visa.

   >[!NOTE]
   >
   >Alternativen i listrutan Åtgärdstyp varierar beroende på vilken granskningslogg som har valts.

1. I listrutan **Loggtyp** väljer du vilken typ av granskningslogg du vill visa.

   **Alla loggtyper** är markerade som standard.

   En lista över alla granskningsloggtyper som du kan visa och vilken information de innehåller finns i [Översikt över granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Valfritt) Ange något av de tillgängliga filtren för följande fält:

   * **Användare**: Ange namnet på den användare som gjorde en ändring.
   * **Från**: Startdatum för tidsramen när ändringen gjordes.
   * **Till**: Slutdatum för tidsramen när ändringen gjordes.

   ![Granskningsloggar](assets/audit-logs.png)

1. Klicka på **Använd**.
1. (Valfritt) Klicka på **Rensa** om du vill återställa ändringar som gjorts i filtren.

## Exportera granskningsloggar

{{step-1-to-setup}}

1. Klicka på **System** > **Granskningsloggar** i den vänstra panelen.

1. Välj en granskningslogg på den nedrullningsbara menyn **Loggtyp**.

   **Alla loggtyper** är markerade som standard.

1. Ange något av de tillgängliga filtren och klicka sedan på **Använd**.

   >[!IMPORTANT]
   >
   >Du kan inte exportera mer än 50 000 loggar samtidigt. Workfront exporterar loggar baserat på de filter du anger, inte på antalet loggar som visas på sidan. Du kan visa det totala antalet filtrerade loggar längst ned till höger på sidan.

1. Klicka på **Exportera**.

   Rutan Spara fil öppnas och du kan spara den exporterade filen på datorn.

   Du kan bara spara granskningsloggarna i CSV-format.

   Spara den exporterade filen. Nu kan du hitta den på datorn och dela den med andra.
