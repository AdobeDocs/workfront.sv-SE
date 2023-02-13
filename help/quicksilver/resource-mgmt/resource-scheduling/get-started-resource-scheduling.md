---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Kom igång med resursschemaläggning
description: När du använder funktionerna för resursplanering i Adobe Workfront kan du enklare tilldela uppgifter och ärenden till rätt användare.
author: Alina
feature: Resource Management
exl-id: 1858f6af-92e7-4d32-a401-40004eeb0cef
source-git-commit: f2297deed0640bbdad93cf2980e33afd7d1f23a0
workflow-type: tm+mt
source-wordcount: '2370'
ht-degree: 0%

---

# Kom igång med resursschemaläggning

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

<!--
<p>(NOTE: LINKED TO THE PRODUCT FROM: ALL SCHEDULING TOOLS: GLOBAL, TEAM, PROJECT STAFFING *** LINKED TO LOTS OF ARTICLES, AS WELL!) </p>
<p>(NOTE: Alina: this article should be divided in multiple articles, but CAREFULLY because some sections are linked to the UI)</p>
</div>
-->

När du använder funktionerna för resursplanering i Adobe Workfront kan du enklare tilldela uppgifter och ärenden till rätt användare. Du kan avgöra vilka användare som kan slutföra uppgiften eller problemet, med hänsyn tagen både till jobbrollen och användarens tillgänglighet.

I följande avsnitt finns mer information om hur du använder Scheduling-områdena i Workfront.

## Krav för att använda schemaläggningsverktygen i Workfront

>[!IMPORTANT]
>
>De krav som beskrivs i den här artikeln gäller endast Workfront schemaläggningsområden. Information om de bästa sätten att använda belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

För att du ska kunna använda funktionerna för resursplanering i Workfront måste du först se till att du, dina projekt och dina aktiviteter och problem uppfyller följande krav:

* [Krav för användare](#user-prerequisites)
* [Projektkrav](#project-prerequisites)
* [Krav för aktivitet och problem](#task-and-issue-prerequisites)

### Krav för användare {#user-prerequisites}

Du kan använda verktygen för resursplanering som är tillgängliga på fliken Schemaläggning, på fliken Personal eller på fliken Arbeta på när vart och ett av följande villkor är uppfyllt:

**När resurser schemaläggs som resurshanterare (från fliken Schemaläggning):**

* Du är utsedd som resurshanterare för de projekt som du vill hantera resurser för.

   Mer information om hur du anger resurshanterare för ett projekt finns i artikeln [Ange resurshanterare för ett projekt eller en mall](../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md).

* Du är en användare med en planlicens.

Som standard visas användare endast på tidslinjen för schemaläggning när en jobbroll har definierats i systemet (antingen den primära jobbrollen eller en sekundär jobbroll) och den jobbrollen matchar den jobbroll som tilldelats en aktivitet eller ett problem som är synligt i **Ej tilldelad** området på tidslinjen för tidsplanering. Du kan inaktivera den här funktionen så att uppgifter och utgåvor kan tilldelas alla användare, oavsett om användaren har en roll definierad i användarprofilen som matchar rolltilldelningen för den uppgift eller det problem som tilldelas dem. Mer information finns i artikeln [Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).

Som standard kan tilldelningar endast göras till användare som har en definierad roll i användarprofilen som matchar rolltilldelningen för uppgiften eller utgåvan som tilldelas dem.

**När du schemalägger resurser som medlem i projektteamet (från fliken Personal i ett projekt):**

* Du har behörighet att visa, Contribute eller hantera projektet
* Du har en plan- eller arbetslicens

<!--
<note type="note">  If Workfront has not removed the Use New Scheduling Area option from your Scheduling settings, users must have a Plan license and Manage permissions to the project to view the Scheduling timeline. For more information about the removal of the Use New Scheduling Area option, see the article
<a href="../../product-announcements/announcements/announcement-archive/replace-flash-tools.md" class="MCXref xref">Replacement of Flash-based tools in Adobe Workfront</a>.
</note>
-->

**När resurser schemaläggs som en teammedlem (från fliken Arbeta på):**

* Du är medlem i teamet\
   Alla medlemmar i teamet visas på tidslinjen för tidsplanering. Uppgifter och ärenden som tilldelats teamet och inte tilldelats någon användare visas i området Ej tilldelade. Uppgiften och utgåvor som tilldelats teamet och en användare i teamet visas på raden för den användare som de är tilldelade till.

### Projektkrav {#project-prerequisites}

Projektkraven som beskrivs i det här avsnittet gäller endast när resurser schemaläggs som resurshanterare från tidslinjen för schemaläggning.

De projekt som du hanterar måste vara i någon av följande statusar (eller ha en status som motsvarar en av dessa statusvärden) för att arbetsobjekt från de projekten ska kunna visas på tidslinjen i tidsplanen: Planering, Aktuell eller Godkänd. Som standard visas bara projekt med statusen Aktuell.

Mer information om projektstatus finns i artikeln [Skapa eller redigera en status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! I assume this doesn't apply when using the Staffing tab on a single project? The project can be in whatever status?]) </p>
-->

### Krav för aktivitet och problem {#task-and-issue-prerequisites}

För att vara effektivast när du använder verktygen för resursplanering i Workfront måste du se till att uppgifter och problem i ditt system har följande kriterier definierade:

* Varaktighet
* Planerade startdatum
* Planerade timmar\
   Planerade timmar krävs för att ändra användarallokeringar, vilket beskrivs i artikeln [Hantera användarallokeringar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

   >[!NOTE]
   >
   >Fältet Planerade timmar i resursplaneringskortet visar faktiskt summan av alla workPerDay-värden, inte planerade timmar för aktiviteten. workPerDay-värden beräknas genom att dividera värdet för Planerade timmar med aktivitetsvaraktighet. För varaktigheter som inte är noll matchar värdena vanligtvis aktivitetens planerade timmar, även om vissa små avvikelser på grund av avrundning kan inträffa. När en varaktighet är 0 dagar visas 0 timmar under Planerade timmar.

* Rolltilldelningar

## Visa information i schemaläggningsområdena

* [Hitta och visa information i schemaläggningsområdena](#locate-and-view-information-in-the-scheduling-areas)
* [Visa resurstilldelningar och detaljer](#view-resource-assignments-and-details)
* [Minimera aktiviteter och problem i schemaläggningsområdena](#minimize-tasks-and-issues-on-the-scheduling-areas)
* [Justera datumintervallet för schemaläggningsområdena](#adjust-the-date-range-of-the-scheduling-areas)

### Hitta och visa information i schemaläggningsområdena {#locate-and-view-information-in-the-scheduling-areas}

Beroende på var du vill schemalägga resurser kan du komma åt tidslinjen för schemaläggning i följande områden av Workfront:

* För flera projekt, i området Schemaläggning
* För ett projekt i avsnittet Schemaläggning
* För ett team, i avsnittet Schema

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. (Valfritt) Klicka på **Helskärm** -ikonen i det övre högra hörnet av tidslinjen för schemaläggning.\
   ![scheming_fullscreen_enter.png](assets/scheduling-fullscreen-enter.png)\
   Tidslinjen för schemaläggning visas i helskärmsläge. När tidslinjen för schemaläggning visas i helskärmsläge upptar tidslinjen hela skärmen. all annan information är dold (inklusive eventuell teaminformation eller projektinformation, det globala navigeringsfältet och webbläsarinformation).

1. (Valfritt) Gör något av följande om du vill avsluta helskärmsläget:

   * Klicka på **Helskärm** ikon.
   * Tryck på Esc.

### Visa resurstilldelningar och detaljer {#view-resource-assignments-and-details}

Du kan visa aktuella resurstilldelningar och annan information om enskilda uppgifter och ärenden på tidslinjen för tidsplanen.

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. (Valfritt) Om du vill anpassa vilket innehåll som ska visas på tidslinjen skapar du ett filter enligt beskrivningen i [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
1. Expandera en uppgift eller ett problem om du vill visa följande information:

   * **Projekt:** Namnet och länken till det projekt där aktiviteten finns.

   * **Datum:** Datumen Starta på och Förfaller den som är associerade med uppgiften.

   * **Planerade timmar:** Antalet planerade timmar som är associerade med uppgiften.\
      Planerade timmar visas bara om uppgiften har tilldelats en användare eller jobbroll.

   * **Föregående ikon:** Föregångare som är associerade med uppgiften. Föregående-ikonen visas bara om det finns föregångare associerade med uppgiften. Föregående-ikonen är grön när föregångaren är klar och uppgiften är klar att bearbetas.

   * **Uppdrag:** Alla användar- eller jobbrolltilldelningar som är associerade med uppgiften. Jobbrolltilldelningar visas inom parentes bredvid användartilldelningen.\
      Teamtilldelningar visas inte.\
      Om du har Contribute-åtkomst till uppgiften eller utgåvan kan du ändra de tider som användarna tilldelas för varje dag i uppgiften eller ärendets varaktighet. Mer information om hur du ändrar användartilldelningar finns i artikeln [Hantera användarallokeringar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

### Minimera aktiviteter och problem i schemaläggningsområdena {#minimize-tasks-and-issues-on-the-scheduling-areas}

Genom att minimera åtgärder och problem kan du visa användartilldelningar för ett stort antal användare på en enda skärm.\
Alla aktiviteter och ärenden på tidslinjen minimeras som standard.

När uppgifter och problem minimeras kan du:

* Visa aktivitetens varaktighet
* Visa projektfärg
* Tilldela uppgifter från området Ej tilldelade till användare på tidslinjen för schemaläggning

När uppgifter och ärenden minimeras kan du inte:

* Visa uppgiftsnamn
* Dra uppgifter som redan har tilldelats en användare och tilldela om dem
* Expandera uppgifter för att visa detaljer

Om du aktiverar inställningen Visa summor för planerade timmar per dag kan du bara göra följande när uppgifter och ärenden minimeras:

* Visa det totala antalet planerade timmar per dag för varje användare.

När du minimerar uppgifter och problem enligt beskrivningen i det här avsnittet visas dessa ändringar endast åt dig. Uppgifter och problem minimeras tills du expanderar dem eller tills du avslutar webbläsarsessionen. (När du uppdaterar sidan återställs inte minimerade uppgifter och utleveranser till ett utökat läge.)

På tidslinjen kan du minimera uppgifter och problem som visas för enskilda användare, för jobbroller eller för alla användare.

* [Minimera arbetsuppgifter och problem för enskilda användare](#minimize-tasks-and-issues-for-individual-users)
* [Minimera uppgifter och ärenden för en jobbroll](#minimize-tasks-and-issues-for-a-job-role)
* [Minimera uppgifter och problem för alla användare](#minimize-tasks-and-issues-for-all-users)

#### Minimera arbetsuppgifter och problem för enskilda användare {#minimize-tasks-and-issues-for-individual-users}

1. Klicka på cirkumflexet bredvid användaren på tidslinjen vars uppgifter och ärenden du vill minimera.\
   ![scheming_minimize_user.png](assets/scheduling-minimize-user-350x137.png)\
   Hur uppgifter och problem visas beror på följande inställningar:

   * Om du aktiverar **Visa summor för planerade timmar per dag** följande villkor gäller:

      * Endast planerade timmar för användarvisningen
      * Uppgifter och problem döljs
   * Om du aktiverar **Visa summor för planerade timmar per dag** uppgifter och problem för användaren minimeras.\
      ![RS_user_collapsed_1_.png](assets/rs-user-collapsed--1--350x152.png)


#### Minimera uppgifter och ärenden för en jobbroll {#minimize-tasks-and-issues-for-a-job-role}

Du kan minimera uppgifter och problem för alla användare som är kopplade till en specifik jobbroll.

1. Klicka på cirkumflexet bredvid jobbrollen på tidslinjen för schemaläggning som innehåller de användare vars uppgifter och ärenden du vill minimera.\
   ![scheming_minimize_group.png](assets/scheduling-minimize-group-350x137.png)\
   Aktiviteter och problem för alla användare som är kopplade till den rollen minimeras om du inaktiverar **Visa summor för planerade timmar per dag** inställning.\
   Aktiviteter och problem döljs och endast Planerade timmar för användarna visas om du aktiverar den här inställningen.\
   ![RS_role_collapsed_1_.png](assets/rs-role-collapsed--1--350x125.png)

#### Minimera uppgifter och problem för alla användare {#minimize-tasks-and-issues-for-all-users}

1. Klicka **Komprimera alla** överst i området Användare och roller.\
   ![resurserSchemaläggning_komprimering.png](assets/resourcescheduling-collapseall-350x261.png)\
   eller\
   Klicka på cirkumflexet bredvid en användare eller jobbroll på tidslinjen i tidslinjen i tidslinjen samtidigt som du håller ned Skift.\
   ![](assets/scheduling-minimize-user-350x137.png)\
   Uppgifter och problem för alla användare och roller minimeras om du inaktiverar **Visa summor för planerade timmar per dag** och uppgifter och ärenden döljs om du aktiverar dem.\
   Om **Visa summor för planerade timmar per dag** är bara aktiverat för de planerade timmarna för användarna. Aktiviteter och problem förblir minimerade för området Ej tilldelade.\
   ![RS_all_collapsed__1_.png](assets/rs-all-collapsed---1--350x102.png)

### Justera datumintervallet för schemaläggningsområdena {#adjust-the-date-range-of-the-scheduling-areas}

Som standard visas 14 dagar i följd (inklusive helger) på tidslinjen i tidsplanen, med början på den aktuella dagen.

Använd något av följande alternativ för att ändra det datumintervall som data visas för på tidslinjen i tidsplanen:

* **Alternativ för datumintervall:** Klicka på det aktuella datumintervallet och välj sedan det antal veckor som ska visas på tidslinjen. Du kan visa Dag (en dag), 1 vecka (7 dagar), 2 veckor (14 dagar), 3 veckor (21 dagar), 4 veckor (28 dagar) eller 6 veckor (42 dagar).\
   Tänk på följande när du justerar tidslinjens datumintervall:

   * Alternativen för datumintervall som du väljer bevaras nästa gång du besöker tidslinjen för schemaläggning.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! Not sure if this is going to apply to all 3 scheduling areas...]) </p>   
     -->

   * När du visar tidslinjen för schemaläggning i dagsvyn visas inte användartilldelningar.\
      ![resource_daterange_zoom.png](assets/resource-daterange-zoom-350x227.png)

* **Kalender:** Klicka på det aktuella datumintervallet och klicka sedan på dagen före eller efter den aktuella dagen. Tiden mellan den aktuella dagen och den valda dagen är det nya intervallet.\
   ![resource_daterange.png](assets/resource-daterange-350x227.png)

* **Idag:** Klicka på det här alternativet om du vill visa den aktuella dagen. Den aktuella dagen visas sedan längst till vänster i datumintervallet.\
   Klicka på vänster- och högerpilarna för att visa tidigare eller framtida datum.

   >[!NOTE]
   >
   >Den tidsram du väljer bevaras när du uppdaterar sidan.

   ![resource_daterange_today.png](assets/resource-daterange-today-350x227.png)

* **Dra och släpp datumintervallet:** Dra datumintervallet högst upp på tidslinjen för tidsplanering.\
   ![resourcescheduling_daterange.png](assets/resourcescheduling-daterange-350x141.png)

## Konfigurera inställningar i schemaläggningsområdena

Viss information visas som standard på tidslinjen för schemaläggning. Du kan också konfigurera inställningarna så att ytterligare information visas.

Mer information om hur du konfigurerar inställningarna på tidslinjen för schemaläggning finns i följande artiklar:

[Konfigurera inställningar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md)

[Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

[Tilldela automatiskt ej tilldelade uppgifter och ärenden i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/automatically-assign-items-scheduling-areas.md)

## Filtrera information i schemaläggningsområdena

Du kan definiera vad som ska visas på tidslinjen genom att skapa ett filter.

Mer information finns i artikeln [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

## Ändra användartilldelningar och allokeringar

* [Ändra användartilldelningar](#modify-user-assignments)
* [Ändra användarallokeringar](#modify-user-allocations)

### Ändra användartilldelningar {#modify-user-assignments}

Du kan ändra användartilldelningar på fliken Schemaläggning (när du schemalägger resurser för projekt) antingen med växlingsverktyget eller genom att ändra aktiviteter och ärenden direkt på tidslinjen i schemaläggningen. Du kan ändra användartilldelningar från fliken Arbeta med (när resurser för team schemaläggs) genom att ändra uppgifter och ärenden direkt från tidslinjen i schemaläggningen.

Mer information finns i artikeln [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Ändra användarallokeringar {#modify-user-allocations}

Du kan bestämma hur Planerade timmar för en uppgift eller utgåva ska tilldelas användare. Planerade timmar kan delas upp på följande sätt:

* Bland användare som är tilldelade till uppgiften eller utgåvan.
* Över aktivitetens eller problemets varaktighet.

Mer information finns i artikeln [Hantera användarallokeringar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
