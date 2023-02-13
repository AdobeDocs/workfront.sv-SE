---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Översikt över schemaläggningsområden
description: I följande avsnitt beskrivs var du kan komma åt schemaläggningsområdet i Adobe Workfront samt vilka funktioner som är tillgängliga i schemaläggningsområdet.
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# Översikt över schemaläggningsområden

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
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->


I följande avsnitt beskrivs var du kan komma åt schemaläggningsområdet i Adobe Workfront samt vilka funktioner som är tillgängliga i schemaläggningsområdet.

## Workfront-områden där du kan schemalägga resurser

Du kan schemalägga resurser inom följande områden i Workfront:

* **För projekt som du är resurshanterare för** (från **Schemaläggning** området) Med Scheduling-området i Workfront kan resurshanterare göra resurstilldelningar i flera projekt.

* **För ett enskilt projekt när du är medlem i projektteamet** (från **Schemaläggning** projektområde):

   Med schemaläggningsområdet i ett projekt kan medlemmar i projektteamet tilldela arbete från projektet till användare i projektteamet.

* **För ett enskilt team är du medlem i** (från **Schema** -delen av teamet) Med schemaläggningssektionen i ett team kan teammedlemmar tilldela arbete som redan har tilldelats teamet från flera projekt till enskilda teammedlemmar.

## Tillgängliga funktioner i området Schemaläggning

I schemaläggningsområdet visas uppgifter och ärenden samt aktuella resurstilldelningar.\
![resource_eduling_overview.png](assets/resource-scheduling-overview-350x237.png)

* [Filter- och växlingsverktyg](#filter-and-swap-tools)
* [Val av datum](#date-selection)
* [Ej tilldelat område](#unassigned-area)
* [Användare och roller](#users-and-roles)
* [Tidslinje för schemaläggning](#scheduling-timeline)

### Filter- och växlingsverktyg {#filter-and-swap-tools}

* **Filterverktyg:** Gör att du kan filtrera innehållet som visas på tidslinjen i schemaläggningen. Mer information om filterverktyget finns i [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **Växla:** (Endast tillgängligt när du schemalägger resurser för projekt från fliken Schemaläggning eller Ställning) Du kan snabbt tilldela, byta ut eller ta bort användartilldelningar för aktiviteter i flera projekt. Mer information finns i [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Val av datum {#date-selection}

Du kan justera det datumintervall för vilket data visas på tidslinjen i tidsplanen. Som standard är datumintervallet 2 veckor (14 dagar i följd, inklusive helger) med början på den aktuella dagen.

### Ej tilldelat område {#unassigned-area}

* [När resurser schemaläggs som resurshanterare (för flera projekt i schemaläggningsområdet)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [När resurser schemaläggs som medlem av projektteamet (från ett projekt)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [När resurser schemaläggs som en teammedlem (från ett team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### När resurser schemaläggs som resurshanterare (för flera projekt i schemaläggningsområdet) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

The **Ej tilldelad** i tidslinjen visas endast de uppgifter och ärenden som uppfyller följande kriterier:

* Inte tilldelad till en användare.
* Inte tilldelad ett team.\
   Om uppgiften eller utgåvan har tilldelats ett team visas den fortfarande i **Ej tilldelad** om uppgiften eller utgåvan även har tilldelats en roll utöver grupptilldelningen.\
   Om uppgifter eller ärenden har ytterligare jobbrolltilldelningar som inte utförs av en användare, visas de också.\
   En uppgift tilldelas till exempel tre jobbroller: Designer, Product Manager och Developer. Du tilldelar den här uppgiften till Användare A som har en Designer-jobbroll och till Användare B som har en Product Manager-jobbroll. I det här scenariot är uppgiften fortfarande synlig i området Ej tilldelad på tidslinjen för schemaläggning, eftersom utvecklarjobbrollen inte är tilldelad en användare.

#### När resurser schemaläggs som medlem av projektteamet (från ett projekt) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

The **Ej tilldelad** överst på tidslinjen visas uppgifter och problem som uppfyller följande kriterier:

* Associerat med projektet men inte tilldelats några användare i projektteamet.\
   Uppgifter som är kopplade till projektet och som är tilldelade till en användare i projektteamet visas på raden för den användare som uppgifterna är tilldelade till.
* Associerad med projektet men tilldelad till en medlem som inte ingår i projektteamet.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **När resurser schemaläggs som en teammedlem (från ett team)** {#when-scheduling-resources-as-a-team-member-from-a-team}

The **Ej tilldelad** överst på tidslinjen visas uppgifter och problem som uppfyller följande kriterier:

* Tilldelad teamet och inga andra användare i teamet.\
   Uppgifter som tilldelats både teamet och en användare i teamet visas på raden för användaren som uppgifterna tilldelas till.
* Tilldelad både till teamet och till en användare som inte är medlem i teamet.

### Användare och roller {#users-and-roles}

* [När resurser schemaläggs som resurshanterare (för flera projekt i schemaläggningsområdet)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [När resurser schemaläggs som medlem av projektteamet (från ett projekt)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [När resurser schemaläggs som en teammedlem (från ett team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### När resurser schemaläggs som resurshanterare (för flera projekt i schemaläggningsområdet) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

Alla användare som är berättigade att tilldelas en av de ej tilldelade uppgifterna finns under **Ej tilldelad** område. Användare är tillgängliga på tidslinjen för schemaläggning och kan tilldelas en aktivitet eller ett ärende under följande omständigheter:

* Som standard visas användare endast på tidslinjen för schemaläggning när en jobbroll har definierats i systemet (antingen den primära jobbrollen eller en sekundär jobbroll) och den jobbrollen matchar den jobbroll som tilldelats en aktivitet eller ett problem som är synligt i **Ej tilldelad** området på tidslinjen för tidsplanering. Du kan inaktivera den här funktionen så att uppgifter och utgåvor kan tilldelas alla användare, oavsett om användaren har en roll definierad i användarprofilen som matchar rolltilldelningen för den uppgift eller det problem som tilldelas dem. Mer information finns i [Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   En användare och användarens tilldelade uppgifter kan visas flera gånger på tidslinjen för schemaläggning om användaren har flera jobbroller angivna i Workfront-systemet.\
   Användarna finns kvar på tidslinjen när de har tilldelats en uppgift eller ett ärende, även om det inte finns några återstående uppgifter eller problem som har en matchande rolltilldelning. På så sätt kan du göra nödvändiga ändringar när de har tilldelats.\
   Om uppgiften inte har tilldelats en jobbroll visas alla användare som uppfyller filterkraven. Mer information om filtret finns i [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* De har utsetts i **Användare** i **Filter** -fliken.\
   Mer information om filtret finns i [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   När du schemalägger resurser för ett team (på fliken Arbeta med) visas även teamtilldelningen.

Alla andra uppgifter eller problem som tilldelats dessa användare visas också på tidslinjen.

Du kan se i vilken nivå användare tilldelas en viss dag enligt beskrivningen i [Hantera användarallokeringar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Uppgifter som du inte har minst Contribute-behörighet för visas som ett grått fält på tidslinjen i schemaläggningen.

#### När resurser schemaläggs som medlem av projektteamet (från ett projekt) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

Varje teammedlem visas alltid på tidslinjen för tidsplanering, oavsett användarnas jobbrolltilldelningar och rolltilldelningarna för aktiviteterna i området Ej tilldelade.

Om en användare har flera jobbroller definierade i systemet visas användaren flera gånger på tidslinjen för schemaläggning när något av följande villkor uppfylls:

* Det visas uppgifter eller problem i **Ej tilldelad** som är tilldelade till de jobbroller som är kopplade till användaren.
* Det finns uppgifter eller problem i projektet som har tilldelats jobbroller, och dessa uppgifter eller utgåvor tilldelas en användare som har den jobbrollen definierad i systemet.

#### När resurser schemaläggs som en teammedlem (från ett team) {#when-scheduling-resources-as-a-team-member-from-a-team-1}

Varje teammedlem visas alltid på tidslinjen för tidsplanering, oavsett användarnas jobbrolltilldelningar och rolltilldelningarna för aktiviteterna i området Ej tilldelade.

Du kan se i vilken nivå användare tilldelas en viss dag enligt beskrivningen i [Hantera användarallokeringar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Åtgärder som du inte har minst Contribute-behörighet att visa som ett grått fält på tidslinjen för schemaläggning.

### Tidslinje för schemaläggning {#scheduling-timeline}

* **Standardinnehåll:** Som standard alla uppgifter som uppfyller kraven i avsnittet [Krav för aktivitet och problem](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) i [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) artikel om alla projekt med statusen Aktuell visas på tidslinjen för schemaläggningen.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   Om du vill anpassa vad som visas på tidslinjen, inklusive visa problem och projekt med en annan status, använder du filtret enligt beskrivningen i [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   Högst 10 uppgifter per dag visas för en viss användare. Du kan expandera listan om du vill visa alla uppgifter som för närvarande är tilldelade den användaren.

* **Överordnade uppgifter:** Vilka överordnade uppgifter som visas på tidslinjen beror på flera inställningar. Mer information finns i avsnittet&quot;Konfigurera om överordnade uppgifter ska visas på tidslinjen i schemat&quot; i [Konfigurera inställningar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artikel.

* **Färgkodning:** Aktiviteter och problem på tidslinjen i schemaläggningen färgkodas beroende på vilket projekt de tillhör. Du kan inte anpassa färgen som är kopplad till ett visst projekt.

   Vid schemaläggning av arbete för team (från fliken Personal) används färger endast om **Visa alla användaruppgifter** är aktiverat. Mer information finns i avsnittet&quot;Konfigurera om överordnade uppgifter ska visas på tidslinjen för schemaläggning&quot; i [Konfigurera inställningar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artikel.

* **Aktivitetsvaraktigheter:** Uppgiftens varaktighet visas på tidslinjen för varje uppgift (uppgiften sträcker sig fysiskt över det antal dagar som motsvarar varaktigheten). Du kan inte justera aktivitetens varaktighet från tidslinjen för schemaläggning.

* **Ledig tid:** Avstängningstiden representeras på tidslinjen av en ljusgrå indikator i kolumnen på den dag som avstämningstiden schemaläggs för en viss användare.\
   Tidsgränsen för varje användare har konfigurerats baserat på följande information:

   Användarens egen kalender för tidsgräns. Mer information om den personliga tidskonverteringen finns i [Konfigurera ledig tid i Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   Det schema som är tilldelat användaren. Det här kan vara standardschemat eller ett anpassat schema. Mer information om scheman finns i [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Helger:** Veckoslut visas på tidslinjen som ljusgrå skuggning på lördagar och söndagar. Det går inte att konfigurera veckodagar som anges som helger på tidslinjen för tidsplanering. Du kan schemalägga användare att arbeta på helger.
