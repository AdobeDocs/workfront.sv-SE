---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena
description: I Resursschemaläggning kan tilldelningar endast göras till användare som har en definierad roll i användarprofilen som matchar rolltilldelningen för den aktivitet eller det problem som tilldelas dem.
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena

>[!IMPORTANT]
>  
><span class="preview">Funktionen för schemaläggning som beskrivs i den här artikeln har tagits bort och ersatts från Adobe Workfront från och med version 23.1 i januari 2023.   </span>
>  
> <span class="preview"> Den här artikeln kommer också att tas bort kort efter version 23.1, i början av 2023. Nu rekommenderar vi att du uppdaterar bokmärkena i enlighet med detta. </span>
> 
><span class="preview"> Du kan nu använda belastningsutjämnaren för att schemalägga arbete för dina resurser. </span>
>  
> <span class="preview">Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i avsnittet [Utjämning av arbetsbelastning](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

Som standard kan tilldelningar endast göras till användare som har en definierad roll i användarprofilen som matchar rolltilldelningen för den uppgift eller det problem som tilldelas dem när de använder verktygen för resursplanering.

Du kan konfigurera Adobe Workfront så att uppgifter och utgåvor kan tilldelas alla användare, oavsett om användaren har en definierad roll i användarprofilen som matchar rolltilldelningen för uppgiften eller utgåvan som de tilldelas. När du tilldelar en användare till en uppgift eller ett problem och den användaren inte har någon roll som matchar rolltilldelningen för uppgiften eller utgåvan, tas den ursprungliga rolltilldelningen bort och rolltilldelningen ändras till rollen för den användare du tilldelar.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt, uppgifter och ärenden</p> <p><strong>ANMÄRKNING</strong>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre för projekt, uppgifter och ärenden som du uppdaterar uppdrag för</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Tillåt tilldelningar till användare oavsett roll

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.
1. Inaktivera alternativet **Begränsa tilldelningar till användare med matchande roll**.
1. Klicka **Återgå till schemaläggning**.

## Tillåt tilldelningar till användare oavsett gruppmedlemskap

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

Som standard kan uppdrag endast göras till användare som är medlemmar i gruppen som är kopplad till projektet (det här är gruppen som definieras när projektet redigeras).

>[!IMPORTANT]
>
>Den här inställningen tar endast hänsyn till medlemmarna i den grupp som är associerad med projektet, och inte till medlemmar i någon undergrupp i den gruppen.

Du kan konfigurera Workfront så att uppgifter och utgåvor kan tilldelas alla användare, oavsett om användaren är medlem i den grupp som är associerad med projektet där uppgiften eller utgåvan finns.

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.
1. Inaktivera alternativet **Begränsa tilldelningar till den grupp som är associerad med projektet**.
1. Klicka **Återgå till schemaläggning**.

 
