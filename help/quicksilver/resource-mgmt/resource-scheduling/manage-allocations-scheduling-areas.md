---
product-area: resource-management
navigation-topic: resource-scheduling
title: Hantera användarallokeringar i schemaläggningsområdena
description: I den här artikeln beskrivs hur du uppdaterar dagliga timtilldelningar för användare som har tilldelats aktiviteter eller problem med hjälp av området Resursschemaläggning.
author: Alina
feature: Resource Management
exl-id: c8ddb250-145e-4321-8747-4f4967fcce41
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2944'
ht-degree: 0%

---

# Hantera användarallokeringar i schemaläggningsområdena

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

Användartilldelningar är timtals som anger hur mycket en användare ska tillbringa en viss dag för att slutföra en arbetsuppgift. De ingår i arbetsuppgiftens planerade timmar.

I den här artikeln beskrivs hur du uppdaterar dagliga timtilldelningar för användare som har tilldelats aktiviteter eller problem med hjälp av området Resursschemaläggning. Information om hur du hanterar övergripande allokeringar för användare och jobbroller till uppgifter finns i [Hantera användar- och rolltilldelningstimmar för uppgifter](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md). Du kan inte uppdatera övergripande allokeringar för användare och jobbroller för utgåvor.

Du kan visa användartilldelningar inom följande områden i Adobe Workfront:

* I avsnittet Schemaläggning i resursområdet.
* I avsnittet Schemaläggning för ett projekt (vid schemaläggning av resurser för ett enskilt projekt).
* I schemaavsnittet för ett team (vid schemaläggning av resurser för ett team).

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

## Användarallokeringar i schemaläggningsområdena

Innan du börjar tilldela tid till användare enligt beskrivningen i den här artikeln bör du känna till hur resursplanering fungerar i Workfront, enligt beskrivningen i [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Du kan schemalägga resurser att arbeta med uppgifter och ärenden för ett enskilt team som du är medlem i, för ett enskilt projekt där du är medlem i projektteamet eller för flera projekt som du är resurshanterare för.

I följande avsnitt beskrivs hur du aktiverar och hanterar användartilldelningar i Workfront:

* [Använd schemaläggningsområdena för att tilldela arbete](#use-the-scheduling-areas-to-assign-work)
* [Tilldelningar som har angetts i rutorna Redigera aktivitet eller Redigera problem jämfört med i tidsplaneringsområdena](#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas)
* [Fördelningsindikatorer](#allocation-indicators)
* [Standardallokering för planerade timmar](#default-allocation-for-planned-hours)
* [Vem kan visa och ändra allokeringar?](#who-can-view-and-modify-allocations)
* [Tidszonshändelser i schemaläggningsområdena](#time-zone-considerations-in-the-scheduling-areas)

### Använd schemaläggningsområdena för att tilldela arbete {#use-the-scheduling-areas-to-assign-work}

När du tilldelar nya arbeten till användare på tidslinjen för schemaläggning kan du bestämma hur de planerade timmarna för en aktivitet eller utgåva ska fördelas mellan användarna.\
Mer information om planerade timmar finns i [Översikt över planerade timmar](../../manage-work/tasks/task-information/planned-hours.md).

Planerade timmar kan delas upp på följande sätt:

* Bland användare som har tilldelats uppgiften eller utgåvan
* Över tiden för aktiviteten eller utgåvan\
   En försäljningsrelaterad uppgift kan till exempel kräva mer arbete mot slutet av aktivitetens varaktighet. Du kan planera den här ojämna fördelningen av timmar i din uppgift.

>[!TIP]
>
>När du schemalägger resurser för flera projekt från schemaläggningsområdena visas inte alla användare och arbetsobjekt på tidslinjen för schemaläggning. Mer information om vilken information som visas på tidslinjen i tidslinjen finns i [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

### Tilldelningar som har angetts i rutorna Redigera aktivitet eller Redigera problem jämfört med i tidsplaneringsområdena {#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas}

Du kan ändra användarallokeringarna för en uppgift eller utgåva från följande platser i Workfront:

* Tidslinjen för schemaläggning\
   Tidslinjen för schemaläggning finns i följande områden:

   * I avsnittet Schemaläggning i resursområdet.
   * I avsnittet Schemaläggning för ett projekt (vid schemaläggning av resurser för ett enskilt projekt).
   * I schemaavsnittet för ett team (vid schemaläggning av resurser för ett team).

   När du ändrar användarallokeringar från tidslinjen för schemaläggning (enligt beskrivningen i [Ändra användarallokeringar](#modify-user-allocations) i den här artikeln) kan du definiera allokeringar för varje användare för uppgiften eller utgåvan, samt för varje dag under den tid som aktiviteten eller utgåvan varar.\
   ![schemaläggning_konturer.png](assets/scheduling-contours-350x139.png)

* Dialogrutan Redigera uppgift eller Redigera problem.\
   När du ändrar användartilldelningar från en dialogruta för att redigera uppgift eller Problem (enligt beskrivningen i [Hantera användar- eller rollallokeringsprocent för uppgifter](../../manage-work/tasks/assign-tasks/manage-allocation-percentage-on-tasks.md)) kan du definiera allokeringar för uppgiften eller utgåvan enbart som helhet för varje användare. Om du vill hantera dessa allokeringar per dag måste du ändra allokeringarna på tidslinjen för schemaläggning enligt beskrivningen i [Ändra användarallokeringar](#modify-user-allocations) i den här artikeln.

   >[!IMPORTANT]
   >
   >När du ändrar användartilldelningar från en dialogruta för att redigera uppgift eller utfärda, skrivs tilldelningar som du tidigare konfigurerat på tidslinjen för schemaläggning över. Dessutom återspeglas inte eventuella ändringar du gör i allokeringar på tidslinjen i tidslinjen i dialogrutan Redigera aktivitet eller Problem.

Vi rekommenderar att du hanterar användartilldelningar från tidslinjen i tidslinjen i stället för från Redigera aktivitet eller Problem för att få tillgång till följande fördelar:

* Du ser tydligt när användare har övertilldelats med hjälp av tilldelningsindikatorer, vilket beskrivs i [Fördelningsindikatorer](#allocation-indicators) -avsnitt.
* Du kan tilldela mer tid till en användare jämfört med en annan användare.\
   Allokeringsindikatorer ger en visuell representation av hur en användare tilldelas jämfört med andra användare, vilket beskrivs i [Fördelningsindikatorer](#allocation-indicators) -avsnitt.

* Du kan tilldela mer tid för arbete en dag över en annan.\
   Allokeringsindikatorer ger en visuell representation av hur tilldelade användare är på en viss dag, vilket beskrivs i [Fördelningsindikatorer](#allocation-indicators).

* Du kan utföra alla resursuppgifter på ett och samma ställe på tidslinjen för schemaläggning.

### Fördelningsindikatorer {#allocation-indicators}

Det finns olika visuella indikatorer som ger snabb information om i vilken grad en användare ska arbeta en viss dag.

Din systemadministratör avgör hur Workfront beräknar användartillgänglighet på systemnivå (med hänsyn till timmar och FTE-tillgänglighet). Beroende på den här systemomfattande inställningen beräknas användartillgängligheten antingen med standardschemat eller användarens schema. Mer information finns i [Konfigurera hur Workfront beräknar resurstimme och FTE-tillgänglighet för schemaläggningsområdet](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

* **Allokeringsskuggning**
Allokering visas visuellt för uppgifter som tilldelats användare i form av skuggning. Mörkare skuggning anger de tilldelade timmarna som en procentandel av den tilldelade användarens FTE (heltidsekvivalent) på en given dag. (Mer information om hur du konfigurerar FTE i Workfront finns i [Konfigurera hur Workfront beräknar resurstimme och FTE-tillgänglighet för schemaläggningsområdet](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).)\
   En enskild användare tilldelas till exempel till en aktivitet som har ett antal 4 planerade timmar och ett värde på 1 dag. FTE för användaren definieras i systemet som 1 (vilket innebär att användaren är schemalagd att arbeta med heltidsstatus, eller snarare 40 timmar i veckan eller 8 timmar om dagen). Skuggningen för uppgiften en viss dag upptar hälften av det lodräta utrymmet för uppgiften, vilket innebär att användaren tilldelas hälften av sitt heltidsanställda (4 timmar) den dagen.\
   ![](assets/scheduling-shading-allocation.png)\
   Uppgiften eller utgåvan visar den kumulativa allokeringen för alla användare som har tilldelats arbetsuppgiften. Du kan expandera en arbetsuppgift om du vill visa mer information, inklusive vem som är tilldelad till arbetsuppgiften och hur många timmar varje användare är tilldelad.\
   Skuggning visas inte för uppgifter i **Ej tilldelad** området på tidslinjen för schemaläggning.\
   ![resource_allokering_expanderad.png](assets/resource-allocation-expanded-350x192.png)

* **Dagliga summor för varje dag för varje användare:** Du kan visa det totala antalet planerade timmar som tilldelats en viss användare varje dag. Den här informationen visas högst upp på varje användares rad på tidslinjen för schemaläggning. Den här informationen visas inte som standard. Du kan aktivera enligt beskrivningen i [Aktivera användarallokeringar](#enable-user-allocations). Uppgifter från projekt med någon av följande statusvärden inkluderas vid beräkning av daglig totalsumma: Aktuell, Planering eller Godkänd.\
   ![resource_day_totals.png](assets/resource-daily-totals-350x55.png)

* **Överallokeringsindikatorer**
När det totala antalet planerade timmar som tilldelats en användare på en viss dag överskrider antalet timmar som användaren arbetar på en dag (för alla aktiviteter), anses den användaren vara överbelagd den dagen.\
   När en användare är överbelagd visas ett rött fält som visar varje uppgift på dagen.\
   Uppgifter från projekt med någon av följande statusvärden inkluderas när en användares överallokering bestäms: Aktuell, Planering eller Godkänd.\
   Det antal timmar en användare arbetar på en dag definieras via FTE-fältet i varje användares profil, vilket beskrivs i avsnittet [Konfigurera hur Workfront beräknar resurstimme och FTE-tillgänglighet för schemaläggningsområdet](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).\
   ![resource_over_allokering.png](assets/resource-over-allocation-350x72.png)\
   När du aktiverar **Visa summor för planerade timmar per dag** och **Visa markering av resursallokering** i inställningarna visas det totala antalet planerade timmar per dag i rött när användaren är överallokerad. Timmar visas som standard till närmaste tionde (t.ex. 1.3).\
   ![RS_planning_hours_in_red_with_decimals__1_.png](assets/rs-planned-hours-in-red-with-decimals--1--350x56.png)

### Standardallokering för planerade timmar {#default-allocation-for-planned-hours}

Workfront försöker distribuera planerade timmar mellan tilldelade användare och dagar enligt följande:

* När flera användare tilldelas till en uppgift eller en utgåva delas timmarna jämnt mellan användarna.\
   Distributionen återspeglar alla avancerade tilldelningar som redan har gjorts för uppgiften.\
   Mer information om avancerade uppdrag finns i [Skapa avancerade uppdrag](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

* När varaktigheten för aktiviteten eller utgåvan sträcker sig över flera dagar, fördelas de planerade timmarna jämnt mellan dagarna och bland alla användare som är tilldelade till aktiviteten, baserat på användarens schema.
* När de planerade timmarna för en aktivitet sträcker sig över flera dagar kan en användare som visar uppgiften från en annan tidszon se en skillnad i aktivitetens varaktighet eller det planerade startdatumet eller det planerade slutförandedatumet.

Timmar visas som standard till närmaste hundradel (till exempel 1,33). Du kan bläddra till höger för att se mer.\
![RS_Planned_Hours_with_two_decimals_in_contour_screen_1__1__1_.png](assets/rs-planned-hours-with-two-decimals-in-contour-screen--1---1--350x252.png)

### Vem kan visa och ändra allokeringar? {#who-can-view-and-modify-allocations}

Följande typer av användare kan visa eller ändra användarallokeringar i Workfront:

* **Resurshanterare:** Du kan visa och ändra användartilldelningar för uppgifter och ärenden i projekt som du är resurshanteraren för. Det kan du göra antingen på tidslinjen i tidslinjen i området Personer eller på fliken Personal i ett projekt.\
   Mer information om hur Resurshanterare kan ändra uppgifter och problem mellan projekt finns i [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

* **Planera och arbeta:** Du kan visa tilldelningar för alla uppgifter och ärenden som du har tilldelats med hjälp av den nya Min arbetskalender eller Arbeta med kalender i ett team som du är medlem i.\
   Förutom att visa tilldelningar kan du ändra tilldelningarna om du har Contribute-åtkomst till uppgifter och ärenden.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Article is conditioned to classic.)
  </MadCap:conditionalText>
  -->

### Tidszonshändelser i schemaläggningsområdena  {#time-zone-considerations-in-the-scheduling-areas}

I sällsynta fall kan användare som visar tidslinjen för schemaläggning se inkonsekvenser där de planerade timmarna för en aktivitet inte motsvarar de totala tilldelade timmarna för enskilda dagar. Detta kan inträffa när operativsystemets tidszonsinställning för en användare är sådan att det planerade startdatumet eller det planerade slutförandedatumet skiljer sig från en annan användare.

Om till exempel Planerat slutförandedatum för en aktivitet anges till 11:00 den 11 mars 3/18, kommer en användare i Australien som visar aktiviteten att se planerat slutförandedatum som 1:00 den 11/4/18, följande dag. Om användaren i Australien tilldelar timmar den 11/4/18 är dessa tilldelade timmar inte synliga för användaren på MST. Dessa timmar beaktas dock alltid i projektets planerade timmar.

## Aktivera användarallokeringar {#enable-user-allocations}

Funktionen för användarallokering är inaktiverad som standard på tidslinjen för schemaläggning. Innan du kan använda funktionen för användartilldelning som beskrivs i det här avsnittet måste du först aktivera den.

>[!NOTE]
>
>Användarallokeringar kan bara aktiveras när tidslinjen för schemaläggning har konfigurerats att använda planerade datum. Om tidslinjen för schemaläggning är konfigurerad att använda Planerade datum kan användarallokeringar inte visas. Mer information om hur du konfigurerar tidslinjen för schemaläggning att använda planerade eller planerade datum finns i&quot;Konfigurera planerade datum för visning på tidslinjen för schemaläggning&quot; i [Konfigurera inställningar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md).

Så här aktiverar du användarallokeringar på tidslinjen för schemaläggning:

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på&#x200B;**Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

   ![](assets/scheduling-tab-global-resourcing-area-nwe-350x145.png)

1. Klicka på **Inställningar** på tidslinjen för schemaläggning.\
   ![scheming_settings_icon.png](assets/scheduling-settings-icon-350x169.png)\
   Dialogrutan Inställningar för resursplanering visas.\
   ![RS_eduling_tab_all_settings__4_.png](assets/rs-scheduling-tab-all-settings--4--350x348.png)

1. Aktivera ett eller båda av följande alternativ för att visa användarallokeringar på tidslinjen för schemaläggning:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visa markering av resursallokering</td> 
      <td> <p>Visa skuggning av användarallokering för aktiviteter och ärenden på tidslinjen för schemaläggning. </p> <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa summor för planerade timmar per dag</td> 
      <td>Visar det totala antalet planerade timmar som tilldelas varje användare för varje dag på tidslinjen för schemaläggning. Planerade timmar visas till närmaste tionde (t.ex. 1.3).<br>Det här alternativet är inaktiverat som standard.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) I dialogrutan **Inkludera problem** väljer du om du vill att utgåvorna ska visas på tidslinjen för schemaläggningen.\
   Det här alternativet är inaktiverat som standard.

1. Klicka **Återgå till schemaläggning**.\
   Användarallokeringar visas nu på tidslinjen för schemaläggning.\
   ![RS_day_planning_sums_and_allokering_highlighting_1_.png](assets/rs-daily-planned-totals-and-allocation-highlighting--1--350x123.png)

## Ändra användarallokeringar {#modify-user-allocations}

Du kan ändra användarallokeringarna för en aktivitet eller ett ärende på tidslinjen för schemaläggning (enligt beskrivningen i det här avsnittet) eller i dialogrutan Redigera aktivitet eller Problem. Mer information finns i [Tilldelningar som har angetts i rutorna Redigera aktivitet eller Redigera problem jämfört med i tidsplaneringsområdena](#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas).

Som standard tilldelas användare till en uppgift eller ett ärende jämnt mellan tilldelningar och mellan dagar i varaktigheten enligt beskrivningen i [Standardallokering för planerade timmar](#default-allocation-for-planned-hours).

Så här ändrar du användarallokeringar för en aktivitet eller ett ärende från tidslinjen för schemaläggning:

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på&#x200B;**Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

   ![schemaläggning_konturer.png](assets/scheduling-contours-350x139.png)

1. Se till att användarallokeringar är aktiverade på tidslinjen för schemaläggning, vilket beskrivs i [Aktivera användarallokeringar](#enable-user-allocations) i den här artikeln.
1. Expandera uppgiften där du vill hantera användartilldelningar.\
   Som standard fördelas Planerade timmar jämnt mellan tilldelade användare och dagar för uppgiftens varaktighet. Timmar läggs inte till på helger (lördagar och söndagar). Mer information finns i [Standardallokering för planerade timmar](#default-allocation-for-planned-hours) i den här artikeln.

1. Klicka på fältet för den användare vars timmar du vill justera en viss dag.

   >[!NOTE]
   >
   >Om du vill behålla den ursprungliga fördelningen när du har ändrat timmar klickar du på **Avbryt**.

1. Ange det justerade antalet timmar.
1. Klicka **Spara**.\
   Du kan bara spara ändringarna när det totala antalet timmar för aktiviteten är lika med antalet ursprungliga planerade timmar. Numret visas i dialogrutan **Planerade timmar** på uppgiften. Talet visas i rött när summan inte är lika med det totala antalet planerade timmar.\
   ![resource_allokering_expanded_modified.png](assets/resource-allocation-expanded-modified-350x226.png)

## Kriterier som återställer användartilldelningar

Workfront återställer de användartilldelningar som du redigerar manuellt på tidslinjen för schemaläggning när ett antal åtgärder inträffar för aktiviteterna eller projektet. I allmänhet återställer Workfront användartilldelningar när tidslinjen för projektet beräknas om om antalet planerade timmar för aktiviteterna och problemen har ändrats i den här processen.\
Mer information om hur du beräknar om tidslinjen för projekt finns i [Beräkna om projekttidslinjer](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Några av de vanligaste villkoren som kan återställa användartilldelningar på tidslinjen för schemaläggning är:

* Lägga till en uppgift i en iteration.\
   Eftersom iterationer har fasta datum beräknas datum för aktiviteterna och allokeringarna om.\
   Mer information om hur iterationer kan påverka aktivitetsdatum finns i [Lägga till artiklar i en befintlig upprepning](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

* Ändra varaktighetstypen för en uppgift till ansträngningsstyrd.
* Ändra varaktighetstypen för en aktivitet till Beräknat uppdrag när mer än en person har tilldelats.\
   Mer information om aktivitetsvaraktighet finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Ändrar projektets planerade start- och slutförandedatum.\
   Mer information om projektplanerade datum finns i [Översikt över projektets planerade startdatum](../../manage-work/projects/planning-a-project/project-planned-start-date.md) och [Ange projektplanerat slutförandedatum](../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

   Mer information om schemalagt slutförandedatum för aktiviteten finns i [Översikt över aktivitetens planerade slutförandedatum](../../manage-work/tasks/task-information/task-planned-completion-date.md).

* Ändra datum för en föregående aktivitet om aktivitetsbegränsningen är en flexibel begränsning.\
   Exempel: Så snart som möjligt eller Så sent som möjligt.\
   Mer information om uppgiftsbegränsning finns i [Översikt över uppgiftsbegränsning](../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Ändra antalet planerade timmar för uppgifter eller problem.

   Mer information om planerade timmar i Workfront finns i [Översikt över planerade timmar](../../manage-work/tasks/task-information/planned-hours.md).
