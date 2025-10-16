---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Exportera en lista med tidrapporter
description: Som personansvarig eller tidrapportgodkännare kan du behöva ladda ned en lista med tidrapporter för att snabbt kunna visa information om tidrapporterna för de personer du ansvarar för. Du kan göra detta genom att exportera en lista med tidrapporter.
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Exportera en lista med tidrapporter

<!--Audited: 8/2024-->

Som personansvarig eller tidrapportgodkännare kan du behöva ladda ned en lista med tidrapporter för att snabbt kunna visa information om tidrapporterna för de personer du ansvarar för. Du kan göra detta genom att exportera en lista med tidrapporter.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td> <p>Ljus eller högre </p>
   <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Åtkomstnivåkonfiguration</td> 
   <td> <p>Visa eller ge högre åtkomst till uppgifter och ärenden</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för uppgifter och problem</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old permissions:

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
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to Tasks and Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the timesheets</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan or license type you have, contact your Workfront administrator.-->

## Exportera en lista med tidrapporter

{{step1-to-timesheets}}

Området **Tidrapporter** öppnas.


![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Klicka på ikonen **sök** ![](assets/search-icon.png) och skriv ett nyckelord och sök efter en viss tidrapport. Du kan till exempel söka efter en tidsbestämd tidsram eller ägarnamn.

1. (Valfritt) Uppdatera filtret i listan över tidrapporter genom att göra något av följande:

   * Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du godkänner

     eller

     Välj **Mina tidrapporter** om du bara vill visa dina tidrapporter.

     Detta tillämpar filtren Mina tidrapportgodkännanden eller Min tidrapport på listan med tidrapporter.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicka på Filterikonen ![](assets/filter-nwepng.png) om du vill använda ett annat filter eller skapa ett nytt. Mer information om hur du skapar eller uppdaterar filter finns i [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Alternativen Mina tidrapportgodkännanden och Mina tidrapporter visas inte högst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtren Mina tidrapportgodkännanden och Mina tidrapporter från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   >
   >   
   >   
   >   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Valfritt) Klicka på ikonerna **Visa** ![](assets/view-icon.png) eller **Gruppera** ![](assets/grouping.png) om du vill använda en annan vy eller gruppering eller skapa en ny.

   Mer information om hur du skapar filter, vyer och grupperingar finns i följande artiklar:

   * [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Skapa eller redigera vyer i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Skapa grupperingar i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Markera de tidrapporter som du vill exportera och klicka sedan på ikonen **Exportera** ![](assets/export-38x15.png) .

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. Välj den typ av fil som du vill exportera listan med tidrapporter till bland följande alternativ:

   * PDF Ladscape
   * PDF stående
   * PDF, andra storlekar
   * Excel
   * Excel (xlsx)
   * Tabbavgränsad

   En lista över tidrapporter hämtas till datorn i det valda formatet och innehåller följande tidrapportinformation:

   * Datumintervall
   * Ägarens namn
   * Totalt antal timmar
   * Övertidsbelopp
   * Namn på godkännare
   * Status
