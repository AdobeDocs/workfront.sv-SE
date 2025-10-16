---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: Aktivitetsgruppering på fyra nivåer för Portfolio-ägare, programägare, projektägare och projektstatus'
description: Den här grupperingen innehåller fyra nivåer av gruppering. I det här fallet grupperas uppgifterna efter Portfolio-ägare, programägare, projektägare och projektstatus. Du kan bara ha upp till tre nivåer av gruppering med standardgränssnittet. Om du vill lägga till en fjärde nivå måste du använda textläge. Du kan inte gruppera rapporter med fler än fyra villkor samtidigt.
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Gruppering: Aktivitetsgruppering på fyra nivåer för Portfolio-ägare, programägare, projektägare och projektstatus

<!--Audited: 10/2024-->

Den här grupperingen innehåller fyra nivåer av gruppering. I det här fallet grupperas uppgifterna efter Portfolio-ägare, programägare, projektägare och projektstatus. Du kan bara ha upp till tre nivåer av gruppering med standardgränssnittet. Om du vill lägga till en fjärde nivå måste du använda textläge. Du kan inte gruppera rapporter med fler än fyra villkor samtidigt.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td> 
   <p>Medarbetare eller begäran om att ändra ett filter </p>
   <p>Standard eller Plan för att ändra en rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en aktivitetsgruppering på fyra nivåer för Portfolio-ägare, programägare, projektägare och projektstatus

Så här använder du den här grupperingen:

1. Gå till en lista med uppgifter.
1. Välj **Ny gruppering** i listrutan **Gruppering**.

1. Klicka på **Växla till textläge**.
1. Ta bort texten i området **Gruppera din rapport**.
1. Ersätt texten i rutan som visas med följande kod:
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>}group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectNmm{2 14}group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.3 namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueFormat=val<br></pre>

1. Klicka på **Klar** och sedan på **Spara gruppering**.
1. (Valfritt) Uppdatera grupperingens namn och klicka sedan på **Spara gruppering**.
