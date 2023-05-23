---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: Aktivitetsgruppering på fyra nivåer för Portfolio-ägare, programägare, projektägare och projektstatus'
description: Den här grupperingen innehåller fyra nivåer av gruppering. I det här fallet grupperas uppgifter efter Portfolio-ägare, programägare, projektägare och projektstatus. Du kan bara ha upp till tre nivåer av gruppering med standardgränssnittet. Om du vill lägga till en fjärde nivå måste du använda textläge. Du kan inte gruppera rapporter med fler än fyra villkor samtidigt.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Gruppering: Aktivitetsgruppering på fyra nivåer för Portfolio-ägare, programägare, projektägare och projektstatus

Den här grupperingen innehåller fyra nivåer av gruppering. I det här fallet grupperas uppgifter efter Portfolio-ägare, programägare, projektägare och projektstatus. Du kan bara ha upp till tre nivåer av gruppering med standardgränssnittet. Om du vill lägga till en fjärde nivå måste du använda textläge. Du kan inte gruppera rapporter med fler än fyra villkor samtidigt.

![Four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td> <p>Begäran om att ändra en gruppering </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en gruppering</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en aktivitetsgruppering på fyra nivåer för Portfolio-ägare, programägare, projektägare och projektstatus

Så här använder du den här grupperingen:

1. Gå till en lista med uppgifter.
1. Från **Gruppering** nedrullningsbar meny, välja **Ny gruppering**.

1. Klicka **Växla till textläge**.
1. Ta bort texten i **Gruppera din rapport** område.
1. Ersätt texten med följande kod:

   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:ägare:namn<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Programägare<br>group.1.notime=false<br>group.1.valuefield=project:program:ägare:namn<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listGroupParsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Klicka **Spara gruppering**.
