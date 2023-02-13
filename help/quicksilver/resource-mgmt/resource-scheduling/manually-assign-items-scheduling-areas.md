---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena
description: Med tidslinjen för schemaläggning kan du hantera användartilldelningar, förutom att ange hur mycket tid varje användare tilldelas för en arbetsuppgift.
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Med tidslinjen för schemaläggning kan du hantera användartilldelningar, förutom att ange hur mycket tid varje användare tilldelas för en arbetsuppgift.

## Åtkomstkrav

Du måste ha följande:

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt, uppgifter och ärenden</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Bidra med behörigheter till projekt, uppgifter och ärenden</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar innan aktiviteter och problem tilldelas på tidslinjen för schemaläggning

Innan du börjar hantera användartilldelningar enligt beskrivningen i det här avsnittet bör du känna till hur resursplanering fungerar i Workfront, enligt beskrivningen i [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Om du vill hantera användartilldelningar enligt beskrivningen i det här avsnittet måste du först se till att du, dina projekt och dina aktiviteter och problem uppfyller de krav som beskrivs i [Krav för att använda schemaläggningsverktygen i Workfront](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) i artikeln [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

I följande avsnitt beskrivs hur du ändrar användartilldelningar manuellt, automatiskt eller genom att byta tilldelningar efter användare eller roll.

## Tilldela användare ej tilldelade uppgifter eller ärenden manuellt

Tidslinjen för schemaläggning ger den synlighet som behövs för att användarna ska kunna slutföra uppgiften eller problemet.\
Mer information om tidslinjen i schemaläggningen finns i [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Du kan tilldela enskilda uppgifter och utgåvor till användare på tidslinjen i Workfront:

* Avsnittet Schemaläggning under Resurs (vid schemaläggning av resurser för flera projekt).
* Avsnittet Schemaläggning under ett projekt (vid planering av resurser för ett enskilt projekt).
* Avsnittet Schema under ett team (när resurser för ett team schemaläggs).

Den information som visas i området Ej tilldelat högst upp i tidslinjen för schemaläggning varierar beroende på det område i Workfront där du använder resursplanering (antingen från avsnittet Schemaläggning (när du schemalägger resurser för flera projekt), avsnittet Schemaläggning (när du schemalägger resurser för ett enskilt projekt) eller avsnittet Schemalägg (när resurser för ett team schemaläggs). Mer information finns i avsnittet [Tillgängliga funktioner i området Schemaläggning](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) i artikeln [Översikt över schemaläggningsområden](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Beroende på vilket område i Workfront som du visar tidslinjen kan endast vissa användare vara berättigade till arbete. Mer information finns i [Översikt över schemaläggningsområden](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Så här tilldelar du otilldelade uppgifter eller utleveranser till användare på tidslinjen för schemaläggning:

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

   ![schemaläggning_konturer.png](assets/scheduling-contours-350x139.png)

1. (Valfritt) Skapa ett filter för att anpassa vilket innehåll som visas på tidslinjen i schemaläggningen enligt beskrivningen i [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). Om du t.ex. vill att utgåvor ska visas på tidslinjen i tidslinjen måste du skapa ett filter.

1. (Valfritt) Ändra datumintervallet som visas på tidslinjen i schemat enligt beskrivningen i [Justera datumintervallet för schemaläggningsområdena](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. Så här tilldelar du en otilldelad uppgift eller ett otilldelat problem:

   * Dra uppgiften eller utgåvan till raden för den användare som du vill tilldela.\
      Högst 10 uppgifter per dag visas för en viss användare. Du kan expandera listan om du vill visa alla uppgifter som för närvarande är tilldelade den användaren. (När du har gjort tilldelningar på tidslinjen kan fler än 10 uppgifter visas tillfälligt.)\
      När du drar ett objekt visas följande information innan du släpper uppgiften eller utgåvan och slutför uppdraget:

   * Om användartilldelningar är aktiverade på tidslinjen för tidsplanering visas indikatorerna för röd överallokering om tilldelningen slutförs, vilket resulterar i att användaren överfördelas.\
      Mer information om överallokeringsindikatorer finns i avsnittet [Fördelningsindikatorer](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) i artikeln [Hantera användarallokeringar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      Om **Begränsa tilldelningar till användare med en matchande roll** är aktiverat i området Inställningar, och användare som inte är berättigade att ta emot uppdraget är nedtonade. Om det här alternativet är inaktiverat är alla användare tillgängliga för att ta emot uppdraget. Alternativet är aktiverat som standard.\
      Mer information om det här alternativet finns i [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) in [Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      En släppindikator visas på användarens rad. På så sätt kan du se var ett objekt tilldelas innan du gör tilldelningen.

      Utöka uppgiften eller problemet som du vill tilldela genom att klicka på den nedrullningsbara pilen i dialogrutan **Uppdrag** börjar du skriva namnet på den användare som du vill tilldela och klickar sedan på användarens namn i listrutan.\
      ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)

1. (Villkorligt) När du har tilldelat en otilldelad uppgift eller ett otilldelat problem till en användare, kanske du vill justera de befintliga tilldelningarna för aktiviteter och utgåvor bland användarna på tidslinjen för schemaläggningen. Vid schemaläggning av resurser för projekt (antingen på fliken Schemaläggning eller på fliken Tillstånd) kan endast användare som har samma jobbroll ta emot tilldelningen.\
   Om du vill återtilldela en uppgift eller ett problem till en annan användare drar du uppgiften från en användares rad till en annan användares rad.
1. (Valfritt) Konfigurera det antal timmar som varje tilldelad användare tilldelas till uppgiften eller utgåvan enligt beskrivningen i [Hantera användarallokeringar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
