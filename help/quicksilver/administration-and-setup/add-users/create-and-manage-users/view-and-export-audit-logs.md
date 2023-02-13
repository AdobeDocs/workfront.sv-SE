---
title: Visa och exportera granskningsloggar
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Du kan visa alla granskningsloggar i systemet eller de som uppfyller vissa filtervillkor. Du kan också exportera granskningsloggar. Granskningsloggar visar användarändringar som har utlösts i systemet under de senaste 90 dagarna.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Visa och exportera granskningsloggar

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Du kan visa alla granskningsloggar i systemet eller de som uppfyller vissa filtervillkor. Du kan också exportera granskningsloggar.

Granskningsloggar visar användarändringar som har utlösts i systemet under de senaste 90 dagarna.

Information om alla granskningsloggtyper och vad som genererar dem finns i [Granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Plan </p> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visa granskningsloggar

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **System > Granskningsloggar**.
1. I **Loggtyp** väljer du vilken typ av granskningslogg du vill visa.

   **Alla loggtyper** är markerat som standard.

   En lista över alla granskningsloggtyper som du kan visa och vilken information de innehåller finns i [Granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Valfritt) Ange något av de tillgängliga filtren.

   >[!NOTE]
   >
   >Alternativen i listrutan Åtgärdstyp varierar beroende på vilken granskningslogg som har valts.

   ![](assets/audit-logs.jpg)

1. Klicka **Använd**.
1. (Valfritt) Klicka på **Rensa filter** för att återställa ändringar som gjorts i filtren.

## Exportera granskningsloggar

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **System > Granskningsloggar**.

1. I **Loggtyp** väljer du en granskningslogg.

   **Alla loggtyper** är markerat som standard.

1. Ange något av de tillgängliga filtren och klicka sedan på **Använd**.

   >[!IMPORTANT]
   >
   >Du kan inte exportera mer än 50 000 loggar samtidigt. Workfront exporterar loggar baserat på de filter du anger, inte på antalet loggar som visas på sidan. Du kan visa det totala antalet filtrerade loggar längst ned till höger på sidan.

1. Klicka **Exportera**.
