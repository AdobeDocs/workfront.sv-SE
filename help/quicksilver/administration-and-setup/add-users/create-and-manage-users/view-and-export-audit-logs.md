---
title: Visa och exportera granskningsloggar
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Du kan visa alla granskningsloggar i systemet eller de som uppfyller vissa filtervillkor. Du kan också exportera granskningsloggar. Granskningsloggar visar användarändringar som har utlösts i systemet under de senaste 90 dagarna.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Visa och exportera granskningsloggar

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Du kan visa alla granskningsloggar i systemet eller de som uppfyller vissa filtervillkor. Du kan också exportera granskningsloggar.

Granskningsloggar visar användarändringar som har utlösts i systemet under de senaste 90 dagarna.

Mer information om alla granskningsloggtyper och vad som genererar dem finns i [Granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa granskningsloggar

{{step-1-to-setup}}

1. Klicka på **System > Granskningsloggar** i den vänstra panelen.
1. I listrutan **Loggtyp** väljer du vilken typ av granskningslogg du vill visa.

   **Alla loggtyper** är markerade som standard.

   En lista över alla granskningsloggtyper som du kan visa och vilken information de innehåller finns i [Granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Valfritt) Ange något av de tillgängliga filtren.

   >[!NOTE]
   >
   >Alternativen i listrutan Åtgärdstyp varierar beroende på vilken granskningslogg som har valts.

   ![](assets/audit-logs.jpg)

1. Klicka på **Använd**.
1. (Valfritt) Klicka på **Rensa filter** om du vill återställa ändringar som gjorts i filtren.

## Exportera granskningsloggar

{{step-1-to-setup}}

1. Klicka på **System > Granskningsloggar** i den vänstra panelen.

1. Välj en granskningslogg på den nedrullningsbara menyn **Loggtyp**.

   **Alla loggtyper** är markerade som standard.

1. Ange något av de tillgängliga filtren och klicka sedan på **Använd**.

   >[!IMPORTANT]
   >
   >Du kan inte exportera mer än 50 000 loggar samtidigt. Workfront exporterar loggar baserat på de filter du anger, inte på antalet loggar som visas på sidan. Du kan visa det totala antalet filtrerade loggar längst ned till höger på sidan.

1. Klicka på **Exportera**.
