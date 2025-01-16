---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gör smarta uppdrag
description: Du kan använda smarta tilldelningar för att identifiera vem som är bäst på att slutföra arbetet. Smarta tilldelningar är förslag för användare, roller eller team som Adobe Workfront presenterar för dig när du tilldelar arbetsobjekt till resurser baserat på en algoritm som avgör vilken resurs som passar bäst för jobbet. Mer information om smarta uppdrag finns i Översikt över smarta uppdrag.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Gör smarta uppdrag

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Den markerade informationen på den här sidan refererar till funktioner som bara är tillgängliga i förhandsvisningsmiljön.</span>

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> This functionality will be removed from the Production environment for customers who enabled fast release with the 25.1 release in January 2025. For information about the 25.1 release, see [First Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md). -->

Du kan använda smarta tilldelningar för att identifiera vem som är bäst på att slutföra arbetet.

Smarta uppdrag är förslag för användare, roller eller team som Adobe Workfront presenterar för dig när du tilldelar resurser till arbetsobjekt. Workfront baserar sina förslag på en algoritm som avgör vilken resurs som passar bäst för jobbet.

<!--<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues.</span> -->

Mer information om villkoren som används för att fastställa smarta tilldelningar finns i [Översikt över smarta tilldelningar](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard</p>
      eller
      <p>Aktuell: Arbete eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och ärenden</p> <p>Visa eller ge högre åtkomst till projekt</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter med möjlighet att utföra uppgifter och ärenden</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gör smarta uppdrag

Smarta uppdrag är tillgängliga på de flesta platser där du kan göra uppdrag i Workfront.

1. Gå till följande områden och klicka på fältet **Tilldelningar** eller **Tilldela detta till**:

   * En uppgiftslista eller utgivningslista eller rapport
   * En aktivitets- eller utgivningsrubrik
   * Åtgärds- eller ärendesammanfattningspanelen
   * En uppgift eller ett problem i arbetsbelastningsutjämnaren
     <!--* <span class="preview">A New Task</span> or New Issue box, as you add <span class="preview">a new task</span> or issue to a project-->

1. Placera markören i uppdragsfältet och vänta i två sekunder.

   <!--For issues, the smart assignments display in the following sections: 
      * **Users and teams**
      * **Job roles**
        ![](assets/smart-assignments-issue-header.png)-->

   Smarta tilldelningar visas i följande avsnitt:<!--, depending on which phase of the algorithm's calculation identified the assignments-->:

   <!--* <span class="preview">**Suggested assignments**: Displays assignments identified in the first phase of the task smart assignment algorithm.</span> -->
   * **Användare och team**, **Jobbroller** eller <span class="preview">**Betygsätt jobbroller**</span>: <!--Assignments identified in the second phase of the task smart assignment's algorithm calculation.-->

   ![](assets/smart-assignments-task-list.png)

   Mer information finns i [Översikt över smarta uppdrag](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Välj resursen i listan med rekommendationer genom att klicka på deras namn.

1. (Valfritt) Klicka på **Tilldela mig** för att tilldela arbetsobjektet till dig själv.

   >[!TIP]
   >
   >Om det inte finns några förslag öppnas inte förslagslistan.

1. (Valfritt) Om du inte vill använda någon av de rekommenderade användarna i listan med smarta tilldelningar börjar du skriva namnet på den önskade resursen och väljer namnet när den visas i listan.
1. Klicka på **Enter** för att göra tilldelningen.

   Den valda användaren tilldelas uppgiften eller utgåvan.
