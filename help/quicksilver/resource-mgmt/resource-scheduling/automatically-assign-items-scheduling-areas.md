---
product-area: resource-management
navigation-topic: resource-scheduling
title: Tilldela automatiskt ej tilldelade uppgifter och ärenden i schemaläggningsområdena
description: När du använder schemaläggningsverktygen kan du låta Adobe Workfront analysera aktuella arbetstilldelningar för alla dina tillgängliga användare och föreslå intelligenta, logiska tilldelningar för uppgifter eller ärenden som ännu inte har tilldelats. Du kan ändra alla föreslagna uppdrag innan du slutför dem.
author: Alina
feature: Resource Management
exl-id: 087fe3ef-9b85-491b-9fdc-436a01822ede
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 0%

---

# Tilldela automatiskt ej tilldelade uppgifter och ärenden i schemaläggningsområdena

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

När du använder schemaläggningsverktygen kan du låta Adobe Workfront analysera aktuella arbetstilldelningar för alla dina tillgängliga användare och föreslå intelligenta, logiska tilldelningar för uppgifter eller ärenden som ännu inte har tilldelats. Du kan ändra alla föreslagna uppdrag innan du slutför dem.

Workfront tittar på de uppgifter och utgåvor som är tillgängliga i området Ej tilldelade inom det valda datumintervallet och föreslår tilldelningar för varje objekt på en gång. Du kan skapa ett filter som begränsar antalet tillgängliga objekt i området Ej tilldelade.

Systemadministratören bestämmer hur Workfront beräknar resurstillgängligheten på systemnivå (med hänsyn till timmar och FTE-tillgänglighet). Beroende på den här systemomfattande inställningen beräknas resurstillgängligheten antingen enligt standardschemat eller användarens schema. Mer information finns i [Konfigurera hur Workfront beräknar resurstimme och FTE-tillgänglighet för schemaläggningsområdet](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

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

## Förutsättningar {#prerequisites}

Workfront använder en egen algoritm för att fastställa uppdragsförslag. För att få bästa möjliga resultat bör du se till att följande information är korrekt i Workfront:

* Uppgifts- och utgivningsinformation, inklusive:

   * Rolltilldelningar\
      Inget förslag har gjorts för uppgifter och ärenden som inte har tilldelats en roll.
   * Planerade timmar\
      Om en uppgift eller utgåva för närvarande inte har några planerade timmar antar Workfront 4 planerade timmar per arbetsdag när arbete tilldelas automatiskt. Dessa timmar tilldelas inte automatiskt till arbetsuppgiften. används endast för att säkerställa mer realistiska tilldelningar.
   * Planerade startdatum och planerade slutförandedatum

* Användarinformation, inklusive:

   * Primära och sekundära rolltilldelningar i användarprofilen
   * Information om projektteam

## Konfigurera rollbegränsningar

Rollbegränsningar styr antalet användare, med en viss roll, som kan tilldelas arbete automatiskt. Rollbegränsningar fungerar per projekt för att säkerställa att rollbaserade uppgifter inte sprids ut bland ett stort antal användare.

I följande scenarier beskrivs hur rollbegränsningar gäller för projekt:

* **Scenario 1**: Om inga användare har tilldelats projektteamet använder systemet rollgränsen för att tilldela uppgifter.\
   Du har till exempel ett projekt utan användare tilldelade till projektteamet. Det här projektet innehåller 10 projekthanteringsaktiviteter som behöver tilldelas, och du har angett en rollgräns på 1 för rollen Projektledare. I systemet tilldelas 1 projektledare alla 10 uppgifter eftersom rollgränsen är 1.

* **Scenario 2**: Om rollgränsen är större än antalet användare som tilldelats projektteamet tilldelas ytterligare användare uppgifter.\
   Du har till exempel ett projekt med en skrivare tilldelad till projektteamet. Det här projektet har 12 skrivaruppgifter som måste tilldelas och du har en rollgräns på 2 för rollen Författare. Systemet tilldelar alla 12 uppgifter mellan projektgruppens skrivare och ytterligare en författare eftersom rollgränsen är 2.

* **Scenario 3**: Om rollgränsen är mindre än antalet användare som tilldelats projektteamet, åsidosätts rollgränsen.\
   Du har till exempel ett projekt med fyra designers tilldelade till projektteamet. Det här projektet har åtta designeruppgifter som behöver tilldelas och du har angett en rollgräns på 2 för Designer-rollen. Systemet tilldelar alla åtta uppgifterna mellan var och en av de fyra projektteamdesignerna trots att rollgränsen är 2.

Så här anger du gränser för jobbrolltilldelningar:

1. Gå till tidslinjen för schemaläggning för flera projekt eller för ett enskilt projekt:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.

1. Klicka på **Inställningar** ikon.\
   ![Automode_settings.png](assets/automode-settings.png)

1. I avsnittet Automatiserad resursschemaläggning klickar du på **Gräns** kolumn textbunden med objektet i **Roll** och ange ett positivt tal.\
   Workfront sparar automatiskt ändringarna.

   >[!NOTE]
   >
   >Alla aktuella projektgruppsmedlemmar är automatiskt berättigade till allt rekommenderat arbete oavsett rollbegränsningen som angetts.

   ![Set_Role_Limits.png](assets/set-role-limits-350x341.png)

1. (Valfritt) Klicka på **Visar** längst upp i kolumnen Gräns och välj önskade visningsalternativ.
1. Om du vill gå tillbaka till resursplaneringsområdet klickar du på **Återgå till schemaläggning**.

## Tilldela uppgifter och ärenden automatiskt

Du kan tilldela användare uppgifter och utgåvor på tidslinjen, oavsett om du är på fliken Schemaläggning (när resurser för flera projekt schemaläggs) eller på fliken Personal (när resurser för ett enskilt projekt schemaläggs).

Så här kan Workfront automatiskt föreslå tilldelningar för aktiviteter och ärenden i området Ej tilldelade:

1. Gå till tidslinjen för schemaläggning för flera projekt eller för ett enskilt projekt:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.

1. (Valfritt) Skapa ett filter för att anpassa vilket innehåll som visas i området Ej tilldelat på tidslinjen i schemaläggningen.\
   Mer information om hur du skapar ett filter finns i [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) in [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) [Filterinformation i området Schemaläggning](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

   >[!TIP]
   >
   >För att säkerställa att Workfront tilldelar de mest berättigade användarna arbete:
   >
   >* Filtrera bara information som påverkar vilka uppgifter som visas i området Ej tilldelade (till exempel Portfolio, Program och Projekt).
   >* Vi rekommenderar att du inte filtrerar information som påverkar vilka användare som är tillgängliga för tilldelning på tidslinjen i tidsplanen. På så sätt begränsas Workfront från att visa alla möjliga tilldelningar, vilket kan leda till mindre tillfredsställande tilldelningar.


1. (Valfritt) Ändra datumintervallet som visas på tidslinjen i schemat enligt beskrivningen i [Justera datumintervallet för schemaläggningsområdena](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). Workfront gör tilldelningar endast för uppgifter och utgåvor inom det synliga datumintervallet på tidslinjen för tidsplanen.

1. Klicka på **Auto** i tidslinjens övre högra hörn.\
   ![scheming_auto.png](assets/scheduling-auto-350x221.png)\
   Workfront föreslår uppdrag för varje uppgift eller utgåva i **Ej tilldelad** område.

   >[!TIP]
   >
   >Aktiviteter och ärenden måste redan ha tilldelats en roll för att ett uppdrag ska kunna föreslås. För att få bästa möjliga resultat bör uppgifter och ärenden innehålla den information som beskrivs i [Förutsättningar](#prerequisites).

   Föreslagna tilldelningar skiljs åt med en prickad kontur runt varje uppgift eller utgåva enligt följande:\
   **Föreslagen uppgiftstilldelning:**

   **Befintlig aktivitetstilldelning:**

1. (Valfritt) Du kan ändra alla föreslagna eller befintliga tilldelningar innan du slutför tilldelningarna:

   >[!NOTE]
   >
   >Om du ändrar ett befintligt uppdrag ändras det till ett föreslaget läge.

   * Så här tilldelar du ett objekt till en annan användare:

      * Dra uppgiften eller utgåvan från den föreslagna användaren till raden för en annan användare som du vill tilldela.

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE: lists in this article need to be reformatted and maybe split - too many levels in)      
        </MadCap:conditionalText>      
        -->

         Högst 10 uppgifter per dag visas för en viss användare. Du kan expandera listan om du vill visa alla uppgifter som för närvarande är tilldelade den användaren. (När du har gjort tilldelningar på tidslinjen kan fler än 10 uppgifter visas tillfälligt.)\
         När du drar ett objekt visas följande information innan du släpper uppgiften eller utgåvan och slutför uppdraget:

         * En släppindikator visas på användarens rad. På så sätt kan du se var ett objekt tilldelas innan du gör tilldelningen.
         * Om användartilldelningar är aktiverade på tidslinjen för tidsplanering visas de röda överallokeringsindikatorerna om tilldelningen slutförs, vilket resulterar i att användaren överfördelas.\
            Mer information om överallokeringsindikatorer finns i [Fördelningsindikatorer](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators).

         * Användare som inte är berättigade att ta emot uppdraget är nedtonade.
      * Utöka uppgiften eller problemet som du vill tilldela genom att klicka på den nedrullningsbara pilen i dialogrutan **Uppdrag** börjar du skriva namnet på den användare som du vill tilldela och klickar sedan på användarens namn i listrutan.\
         ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)
   * Om du vill skjuta upp ett uppdrag drar du en uppgift eller ett problem som du inte är redo att tilldela tillbaka till **Ej tilldelad** område.



1. Klicka på **Skapa uppdrag** längst upp på tidslinjen för att slutföra föreslagna tilldelningar.\
   eller\
   Klicka **Avbryt** för att returnera alla föreslagna tilldelningar till sina tidigare positioner.
