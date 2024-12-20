---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gör smarta uppdrag
description: Du kan använda smarta tilldelningar för att identifiera vem som är bäst på att slutföra arbetet. Smarta tilldelningar är förslag för användare, roller eller team som Adobe Workfront presenterar för dig när du tilldelar arbetsobjekt till resurser baserat på en algoritm som avgör vilken resurs som passar bäst för jobbet. Mer information om smarta uppdrag finns i Översikt över smarta uppdrag.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Gör smarta uppdrag

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som bara är tillgängliga i produktionsmiljön för kunder som har aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> Den här funktionen kommer att tas bort från produktionsmiljön för kunder som aktiverade en snabb version med version 25.1 i januari 2025. Mer information om version 25.1 finns i [Översikt över utgåvan för första kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

Du kan använda smarta tilldelningar för att identifiera vem som är bäst på att slutföra arbetet.

Smarta uppdrag är förslag för användare, roller eller team som Adobe Workfront presenterar för dig när du tilldelar resurser till arbetsobjekt. Workfront baserar sina förslag på en algoritm som avgör vilken resurs som passar bäst för jobbet.

<span class="preview">Det finns två separata algoritmer i Workfront som beräknar smarta tilldelningar som fungerar på olika sätt för uppgifter och för utgåvor.</span>

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
   * <span class="preview">En ny aktivitet</span> eller en ny utgåva när du lägger till <span class="preview">en ny aktivitet</span> eller ett problem i ett projekt
   * En uppgift eller ett problem i arbetsbelastningsutjämnaren

1. Placera markören i uppdragsfältet och vänta i två sekunder.

   För problem visas de smarta tilldelningarna i följande avsnitt:

   * **Användare och team**
   * **Jobbroller**

   ![](assets/smart-assignments-issue-header.png)

   För uppgifter visas de smarta tilldelningarna i följande avsnitt, beroende på vilken fas av algoritmens beräkning som identifierar tilldelningarna:

   * <span class="preview">**Föreslagna tilldelningar**: Visar tilldelningar som identifieras i den första fasen i den smarta tilldelningsalgoritmen för aktiviteten.</span>
   * **Användare och team**, **Jobbroller** eller <span class="preview">**Betygsätt jobbroller för kort**</span>: Tilldelningar som identifieras i den andra fasen av den smarta tilldelningens algoritmberäkning.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Mer information finns i [Översikt över smarta uppdrag](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Välj resursen i listan med rekommendationer genom att klicka på deras namn.

1. (Valfritt) Klicka på **Tilldela mig** för att tilldela arbetsobjektet till dig själv.

   >[!TIP]
   >
   >Om det inte finns några förslag öppnas inte förslagslistan.

1. (Valfritt) Om du inte vill använda någon av de rekommenderade användarna i listan med smarta tilldelningar börjar du skriva namnet på den önskade resursen och väljer namnet när den visas i listan.
1. Klicka på **Enter** för att göra tilldelningen.

   Den valda användaren tilldelas uppgiften eller utgåvan.
