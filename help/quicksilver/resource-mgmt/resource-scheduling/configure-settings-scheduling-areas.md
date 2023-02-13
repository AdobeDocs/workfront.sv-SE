---
product-area: resource-management;setup
navigation-topic: resource-scheduling
title: Konfigurera inställningar i schemaläggningsområdena
description: Du kan konfigurera olika inställningar för att anpassa hur och vilken information som ska visas på tidslinjen för schemaläggning.
author: Alina
feature: Resource Management
exl-id: d76b59c0-d0fd-4698-8017-fa0778f61dc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2280'
ht-degree: 0%

---

# Konfigurera inställningar i schemaläggningsområdena

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.</span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Du kan konfigurera olika inställningar för att anpassa hur och vilken information som ska visas på tidslinjen för schemaläggning.

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa åtkomst eller senare till projekt, uppgifter och ärenden</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre för projekt, uppgifter och ärenden</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konfigurera problem som ska visas på tidslinjen för schemaläggning

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALL THE SECTIONS BELOW ARE LINKED TO PRODUCT. DO NOT CHANGE TITLES) </p>
-->

Du kan konfigurera problem som ska visas utöver aktiviteter på tidslinjen för schemaläggning.\
När resurser schemaläggs i schemaläggningsavsnittet för ett team visas problem som standard förutom aktiviteter. När resurser för projekt schemaläggs visas endast uppgifter som standard.

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. Aktivera dialogrutan Inställningar för resursschemaläggning **Visa problem** alternativ.\
   ![RS_eduling_tab_all_settings__1_.png](assets/rs-scheduling-tab-all-settings--1--350x417.png)

1. Klicka **Återgå till schemaläggning**. 

## Konfigurera slutfört arbete som ska visas på tidslinjen för schemaläggning

Du kan konfigurera tidslinjen för schemaläggning så att arbete som redan har markerats som slutfört visas. Som standard visas inte slutfört arbete på tidslinjen för schemaläggning. 

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. Aktivera dialogrutan Inställningar för resursschemaläggning **Visa slutfört arbete** alternativ.\
   ![RSS_show_completed_work_disabled__1_.png](assets/rss-show-completed-work-disabled--1--350x336.png)

1. Klicka **Återgå till schemaläggning**.\
   Färdigt arbete visas med en bockmarkering i det övre högra hörnet av arbetsuppgiften.

## Konfigurera projektnamn som ska visas på tidslinjen i schemat 

Du kan konfigurera projektnamnet som ska visas för varje aktivitet och utgåva på tidslinjen för schemaläggningen. På så sätt kan användare som visar tidslinjen snabbt se namnet på det projekt där uppgiften eller utgåvan finns.

När du aktiverar projektnamn som ska visas förbrukar varje aktivitet och problem mer lodrätt utrymme på tidslinjen, vilket resulterar i att färre uppgifter och problem visas i en enda vy.

Som standard visas inte projektnamn för aktiviteter och ärenden på tidslinjen för schemaläggning.

Så här visar du projektnamn för aktiviteter och ärenden på tidslinjen i schemat:

1. Gå till tidslinjen för schemaläggning för flera projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. Aktivera alternativet **Visa projektnamn**.\
   ![RS_eduling_tab_all_settings__2_.png](assets/rs-scheduling-tab-all-settings--2--350x348.png)

1. Klicka **Återgå till schemaläggning**.\
   Varje aktivitet och problem på tidslinjen visar namnet på det projekt där uppgiften eller utgåvan finns.\
   ![resourcescheduling_projectnames.png](assets/resourcescheduling-projectnames-350x200.png)

## Konfigurera planerade datum som ska visas på tidslinjen i schemat

Som standard används planerade datum på tidslinjen för tidsplanering. Du kan också konfigurera tidslinjen för schemaläggning så att Projicerade datum används.

Tänk på följande information om planerade och planerade datum:

* Planerade datum för uppgifter kan anges manuellt eller automatiskt, beroende på aktivitetsbegränsning och varaktighetstyp. Mer information finns i artiklarna [Översikt över uppgiftsbegränsning](../../manage-work/tasks/task-constraints/task-constraint-overview.md) och  [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

   Planerade datum för problem anges manuellt av användare. Systemadministratören kan dock hindra användare från att justera planerade datum för problem.

* Planerade datum för både uppgifter och ärenden anges automatiskt. Mer information om planerade datum finns i artiklarna [Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden](../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

>[!NOTE]
>
>När Projicerade datum används på tidslinjen för tidsplanering kan information om användarallokering inte visas. Mer information om användartilldelningar finns i artikeln [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

Så här konfigurerar du tidslinjen för schemaläggning så att aktiviteter och ärenden visas enligt Planerade datum: 

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. I dialogrutan Inställningar för resursplanering inaktiverar du **Använd planerade i stället för planerade datum** alternativ.
1. Klicka **Återgå till schemaläggning**.

## Konfigurera hur användare visas på tidslinjen för schemaläggning

>[!NOTE]
>
>Det här avsnittet gäller endast när resurser för team schemaläggs (från schemaläggningsavsnittet för ett team). Vid schemaläggning av resurser för flera projekt (från fliken Schemaläggning) eller för ett enskilt projekt (från fliken Tillstånd) kan användarna inte visas i bokstavsordning. de är alltid ordnade efter roll.

När du schemalägger resurser för ett team kan du konfigurera användare så att de visas på tidslinjen för schemaläggningen i alfabetisk ordning eller efter roll. Som standard visas användare i bokstavsordning (roller visas inte).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på Teams. Ett team väljs som standard.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. I dialogrutan Inställningar väljer du om du vill aktivera **Gruppera efter roll** alternativ.\
   När det här alternativet är inaktiverat visas användarna i alfabetisk ordning och roller visas inte på tidslinjen för schemaläggningen.\
   När det här alternativet är aktiverat visas roller på tidslinjen för tidsplanering och användarna grupperas inom sina respektive roller. Om en viss användare har flera roller definierade i systemet, visas den användaren flera gånger på tidslinjen för schemaläggningen, under varje lämplig roll.\
   ![RS_working_on_team_eduling_full_settings__1_.png](assets/rs-working-on-team-scheduling-full-settings--1--350x348.png)

1. Klicka **Återgå till schemaläggning**.

## Konfigurera om överordnade uppgifter ska visas på tidslinjen för schemaläggningen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!! - Resource Scheduling (People> Scheduling>Settings>Show Parent Tasks tooltip)</p>
-->

Överordnade uppgifter visas på olika sätt beroende på vilken tidslinje du använder. 

* [Visa överordnade uppgifter för flera projekt](#display-parent-tasks-for-multiple-projects)
* [Visa överordnade uppgifter för ett projekt eller ett team](#display-parent-tasks-for-a-project-or-a-team)

### Visa överordnade uppgifter för flera projekt {#display-parent-tasks-for-multiple-projects}

Om överordnade aktiviteter visas eller inte beror på följande inställningar när resurser för flera projekt schemaläggs i avsnittet Schemaläggning:

* Projektets slutföringsläge.
* Projektets slutförandeläge för sammanfattning.
* Inställningen Visa överordnade aktiviteter på fliken Schemaläggning.

Följande tabell visar när de överordnade aktiviteterna visas på fliken Schemaläggning och endast när underaktiviteterna visas. 

| **Visa inställning för överordnade aktiviteter** | **Projektets slutförandeläge** | **Projektets slutförandeläge för sammanfattning** | **Typ av uppgifter som visas på tidslinjen för schemaläggning** |
|---|---|---|---|
| Handikappade | Manuell | Automatisk | Endast underaktiviteter |
| Handikappade | Manuell | Manuell | Endast underaktiviteter |
| Handikappade | Automatisk | Automatisk | Endast underaktiviteter |
| Handikappade | Automatisk | Manuell | Endast underaktiviteter |
| Aktiverad | Automatisk | Manuell | Underaktiviteter och överordnade uppgifter |
| Aktiverad | Automatisk | Automatisk | Endast underaktiviteter |
| Aktiverad | Manuell | Manuell | Underaktiviteter och överordnade uppgifter |
| Aktiverad | Manuell | Automatisk | Endast underaktiviteter |

Mer information om hur du konfigurerar **Slutförandeläge** och **Läge för slutförande av sammanfattning** fält för varje projekt, se avsnittet Inställningar i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

Du kan konfigurera inställningen Visa överordnade uppgifter manuellt i avsnittet Schemaläggning för flera projekt. 

Så här konfigurerar du inställningen Visa överordnade uppgifter: 

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. I dialogrutan Inställningar för resursplanering väljer du om du vill aktivera alternativet, **Visa överordnade uppgifter.**
När det här alternativet är aktiverat visas överordnade uppgifter från alla projekt i enlighet med inställningarna för sammanfattande slutföringsläge och slutföringsläge för projekten, enligt tabellen ovan. Det här alternativet är aktiverat som standard.
\
   ![RS_eduling_tab_all_settings__3_.png](assets/rs-scheduling-tab-all-settings--3--350x348.png)

1. Klicka **Återgå till schemaläggning** i det nedre vänstra hörnet.

### Visa överordnade uppgifter för ett projekt eller ett team {#display-parent-tasks-for-a-project-or-a-team}

När du schemalägger resurser i personalavsnittet i ett projekt eller i schemaavsnittet beror det på om överordnade uppgifter visas eller inte på följande inställningar:

* Projektets slutföringsläge.
* Projektets slutförandeläge för sammanfattning.

Mer information om hur du konfigurerar **Slutförandeläge** och **Läge för slutförande av sammanfattning** fält för varje projekt, se avsnittet Inställningar i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

Följande tabell visar när de överordnade uppgifterna visas i personalavsnittet i ett projekt eller i schemaavsnittet och endast när underuppgifterna visas. 

| Projektets slutförandeläge | Projektets slutförandeläge för sammanfattning | Typ av aktiviteter som visas i avsnittet Schemaläggning | Typ av aktiviteter som visas i teamschemaläggningsavsnittet |
|---|---|---|---|
| Manuell | Automatisk | Endast underaktiviteter | Endast underaktiviteter |
| Manuell | Manuell | Underaktiviteter och överordnade uppgifter | Endast underaktiviteter |
| Automatisk | Automatisk | Endast underaktiviteter | Endast underaktiviteter |
| Automatisk | Manuell | Underaktiviteter och överordnade uppgifter | Endast underaktiviteter |
| Automatisk | Manuell | Underaktiviteter och överordnade uppgifter | Endast underaktiviteter |
| Automatisk | Automatisk | Endast underaktiviteter | Endast underaktiviteter |
| Manuell | Manuell | Underaktiviteter och överordnade uppgifter | Endast underaktiviteter |
| Manuell | Automatisk | Endast underaktiviteter | Endast underaktiviteter |

## Konfigurera om dagliga planerade timmar ska visas på tidslinjen för tidsplanen

Så här konfigurerar du tidslinjen för schemaläggning så att de dagliga summorna för de planerade timmarna för varje användare visas: 

1. Gå till tidslinjen för schemaläggning av flera projekt, för ett enskilt projekt eller för ett team:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
   * **För ett team**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. Aktivera följande alternativ i dialogrutan Inställningar:

   *  **Visa summor för planerade timmar per dag**: Visar det totala antalet planerade timmar per dag för varje användare.
   * **Visa markering av resursallokering**: Markerar användarens allokering för uppgifter och ärenden, och visar även vilka dagar användarna är överallokerade.\
      Dessa alternativ är inaktiverade som standard.\
      ![RS_all_settings__1_.png](assets/rs-all-settings--1--350x358.png)

1. Klicka **Återgå till schemaläggning**.\
   Det totala antalet planerade timmar som tilldelats användarvisningen för varje dag.\
   De planerade timmarna för de dagar då användaren överfördelas markeras med rött.\
   Mer information om användartilldelningar finns i artikeln [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## Konfigurera om alla användaruppgifter ska visas på tidslinjen för schemaläggningen

>[!NOTE]
>
>Det här alternativet gäller endast vid schemaläggning av resurser för enskilda projekt (från avsnittet Schemaläggning i projektet). Det här alternativet är inte tillgängligt vid schemaläggning av resurser för flera projekt (från schemaläggningsavsnittet ) eller för team (från schemaläggningsavsnittet för ett team).

Så här konfigurerar du om alla uppgifter som tilldelas varje användare (inte bara de uppgifter som är kopplade till det projekt som du visar) ska visas på tidslinjen för schemaläggningen:

1. Gå till det projekt där du vill konfigurera tidslinjen för schemaläggning för att visa alla uppgifter som tilldelats varje användare.
1. Klicka på **Utjämning av arbetsbelastning** i den vänstra panelen (den kan finnas under **Visa fler**) och sedan väljer **Schemaläggning** i den övre vänstra listrutan.
1. Klicka på **Inställningar** -ikonen på tidslinjen för schemaläggning.

1. I området Inställningar väljer du om du vill aktivera alternativet, **Visa alla användaruppgifter**.\
   När det här alternativet är aktiverat visas alla uppgifter som tilldelats varje användare på tidslinjen för schemaläggningen, oavsett vilket projekt som uppgifterna finns i.\
   Det här alternativet är inaktiverat som standard.\
   ![RS_project_eduling_area__1_.png](assets/rs-project-scheduling-area--1--350x340.png)

1. Klicka **Återgå till schemaläggning**.
