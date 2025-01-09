---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Ta bort en extern sida från en kontrollpanel
description: Du kan ta bort en extern sida från en kontrollpanel om den inte längre behövs.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# Ta bort en extern sida från en kontrollpanel

<!-- Audited: 1/2025 -->

Du kan ta bort en extern sida från en kontrollpanel om den inte längre behövs.

Du kan dock inte ta bort en extern sida efter att den har skapats i Adobe Workfront. Du kan bara ta bort en extern sida med API:t. Mer information om Workfront API finns i [API-grunder](../../../wf-api/general/api-basics.md). Mer information om hur du skapar externa sidor finns i [Bädda in en extern webbsida i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter på kontrollpanelen</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort en extern sida från en instrumentpanel

1. Gå till kontrollpanelen som innehåller den externa sida som du vill ta bort.

1. Klicka på **Instrumentpanelsåtgärder** och sedan på **Redigera**.

   ![](assets/unshimmed-edit-dashboard.png)

1. På skärmens högra sida letar du reda på den externa sida som du vill ta bort och klickar på ikonen **Ta bort** ![](assets/delete.png) .

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Klicka på **Spara + stäng** i det nedre vänstra hörnet.

   Detta tar bort den externa sidan från den valda kontrollpanelen. Den externa sidan ligger kvar i Workfront och kan nås via en rapport. Mer information finns i avsnittet Visa externa sidor i en rapport i artikeln [Bädda in en extern webbsida i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
