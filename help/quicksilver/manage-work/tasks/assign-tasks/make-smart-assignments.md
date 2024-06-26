---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gör smarta uppdrag
description: Du kan använda smarta tilldelningar för att identifiera vem som är bäst på att slutföra arbetet. Smarta tilldelningar är förslag för användare, roller eller team som Adobe Workfront presenterar för dig när du tilldelar arbetsobjekt till resurser baserat på en algoritm som avgör vilken resurs som passar bäst för jobbet. Mer information om smarta uppdrag finns i Översikt över smarta uppdrag.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Gör smarta uppdrag

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder eller i produktionsmiljön för kunder som aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba versioner finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Mer information om den aktuella versionen finns i [Översikt över utgåvan för tredje kvartalet 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Du kan använda smarta tilldelningar för att identifiera vem som är bäst på att slutföra arbetet.

Smarta uppdrag är förslag för användare, roller eller team som Adobe Workfront presenterar för dig när du tilldelar resurser till arbetsobjekt. Workfront baserar sina förslag på en algoritm som avgör vilken resurs som passar bäst för jobbet.

<span class="preview">Det finns två separata algoritmer i Workfront som beräknar smarta tilldelningar som fungerar på olika sätt för olika uppgifter och för olika utgåvor. </span>

Mer information om villkoren som används för att bestämma smarta tilldelningar finns i [Översikt över smarta uppdrag](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Gör smarta uppdrag

Smarta uppdrag är tillgängliga på de flesta platser där du kan göra uppdrag i Workfront.

1. Gå till följande områden genom att klicka på **Uppdrag** eller **Tilldela detta till** fält:

   * En uppgiftslista eller utgivningslista eller rapport
   * En aktivitets- eller utgivningsrubrik
   * Åtgärds- eller ärendesammanfattningspanelen
   * <span class="preview">En ny aktivitet eller nytt problem när du lägger till en ny uppgift eller ett nytt problem i ett projekt</span>
   * Uppdragsfältet för ett objekt som visas i hemområdet
   * En uppgift eller ett problem i arbetsbelastningsutjämnaren

1. Placera markören i uppdragsfältet och vänta i två sekunder.

   <div class="preview">
   Ett eller flera av följande avsnitt med förslag på smarta uppdrag visas:

   * **Föreslagna tilldelningar**: Visar för uppgifter. <!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   Listrubriken visas **Här är några rekommendationer** i stället för **Föreslagna tilldelningar** i produktionsmiljön.
     >
   * **Användare och team**: Visar uppgifter och problem.
   * **Jobbroller**: Visar för uppgifter och problem.
   * **Betygsätt jobbroller för kort**: Visar för uppgifter. Mer information finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   För uppgifter visas de smarta tilldelningarna i följande avsnitt, beroende på vilken fas av algoritmens beräkning som identifierar tilldelningarna:

   * **Föreslagna tilldelningar**: Tilldelningar som identifieras i den första fasen i den smarta uppgiftens algoritmberäkning. <span class="preview">Det här avsnittet är inte tillgängligt för problem.</span>
   * <span class="preview">**Användare och team**, **Jobbroller**, eller **Betygsätt jobbroller för kort**: Tilldelningar som identifieras i den andra fasen av den smarta uppgiftens algoritmberäkning. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Mer information finns i [Översikt över smarta uppdrag](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Markera användaren i listan med rekommendationer genom att klicka på namnet på användaren.

1. (Valfritt) Klicka på **Tilldela mig** om du vill tilldela arbetsuppgiften till dig själv.

   >[!TIP]
   >
   >Om det inte finns några förslag öppnas inte förslagslistan.

1. (Valfritt) Om du inte vill använda någon av de rekommenderade användarna i listan med smarta tilldelningar börjar du skriva namnet på den önskade resursen och väljer namnet när den visas i listan.
1. Klicka **Retur** för att göra uppdraget.

   Den valda användaren tilldelas uppgiften eller utgåvan.
