---
product-area: resource-management
navigation-topic: resource-scheduling
title: Ändra flera användartilldelningar för aktiviteter i schemaläggningsområdena
description: Ändra flera användartilldelningar för aktiviteter i schemaläggningsområdena.
author: Alina
feature: Resource Management
exl-id: 545a5033-a09e-4019-a10e-c388cf977ae4
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---

# Ändra flera användartilldelningar för aktiviteter i schemaläggningsområdena


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

This article refers to modifying user assignments for multiple tasks using the Scheduling area of Adobe Workfront. Also see the following articles for modifying assignments on multiple tasks in other areas:

* For information about modifying assignments on multiple tasks in a task list, see [Modify multiple user assignments in a task list](../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md). 
* For information about scheduling resources using the new Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
-->
Du kan tilldela användare till flera aktiviteter samtidigt när du använder Resursplaneraren.

>[!NOTE]
>
>Den här artikeln gäller endast vid schemaläggning av resurser för flera projekt (från avsnittet Schemaläggning ) eller för ett enskilt projekt (från avsnittet Schemaläggning ). du kan inte hantera användartilldelningar för flera uppgifter enligt beskrivningen i det här avsnittet när du schemalägger resurser för ett team (från schemaavsnittet ).

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
   <td role="rowheader">Adobe Workfront licensöversikt*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt, uppgifter och ärenden</p> <p><b>ANMÄRKNING</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre för projekt, uppgifter och ärenden som du uppdaterar uppdrag för</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du gör flera tilldelningar i schemaläggningsområdena

Du kan snabbt hantera användartilldelningar för flera uppgifter och ärenden i ett eller flera projekt (ändringarna återspeglas sedan på tidslinjen i tidsplanen).

Du kan tilldela en användare till alla uppgifter som för närvarande är tilldelade till en jobbroll, byta användartilldelningar mellan användare eller ta bort användartilldelningar från alla uppgifter.

Exempel:

* En resurshanterare ansvarar för att göra användartilldelningar i ett nytt projekt. Projektet skapades ursprungligen som en mall och jobbroller är redan tilldelade till de olika aktiviteterna i projektet. Resurshanteraren vill tilldela en specifik användare till alla uppgifter som för närvarande är tilldelade till en jobbroll.
* 45 uppgifter i tre olika projekt tilldelas Jackie Simms. Jackie lämnar organisationen och nu måste resurshanteraren omfördela sina uppgifter till en annan användare.

>[!NOTE]
>
>Tänk på följande begränsningar när du hanterar användartilldelningar för flera uppgifter:
>
>* När du schemalägger resurser för flera projekt måste de projekt som du hanterar ha någon av följande statusvärden (eller en status som motsvarar en av dessa statusvärden): Planering, Aktuell eller Godkänd. Mer information om projektstatus finns i [Skapa eller redigera en status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* När resurser för ett enskilt projekt schemaläggs påverkar inte projektstatusen tillgängligheten för den här funktionen.
>* Du kan göra resursändringar för användare med följande licenser: Planera, arbeta och granska. Du kan inte göra resursändringar för användare med en Request-licens.
>


## Hantera användartilldelningar för ett eller flera projekt

1. Gå till tidslinjen för schemaläggning för flera projekt eller för ett enskilt projekt:

   * **För flera projekt**: Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
   * **För ett enskilt projekt**: Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.

1. Klicka **Åtgärder**.\
   ![resource_eduling.png](assets/resource-scheduling.png)

1. I **Välj projekt** beroende på om du visar tidslinjen för schemaläggning för flera projekt (från fliken Schemaläggning) eller för ett enskilt projekt (från fliken Personal), gör du något av följande:

   * **För flera projekt:** Börja skriva namnet på det projekt där du vill ändra tilldelningen och klicka sedan på namnet när det visas i listrutan. Du kan också klicka på listrutepilen och välja från en lista med projekt. Upprepa den här processen om du vill göra uppdragsändringar i flera projekt.\
      Lämna det här fältet tomt om du vill göra tilldelningsändringar i alla projekt som du är resurshanterare för.

      >[!NOTE]
      >
      >Det går bara att välja projekt om:
      >
      >   
      >   
      >   * Du är utsedd som resurshanterare i projektet\
         >     Mer information finns i [Ange resurshanterare för ett projekt eller en mall](../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md).
      >   
      >   * Projektet har en av följande statusvärden (eller en status som motsvarar en av dessa statusvärden): Planering, aktuell eller godkänd\
         >     Mer information om projektstatus finns i [Skapa eller redigera en status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
      >   
      >   * Du är en användare med en planlicens.


   * **För ett enskilt projekt:** The **Välj projekt** kan inte ändras. The **Välj projekt** fältet innehåller alltid namnet på det projekt som du visar.

1. (Valfritt) Klicka på **Ange uppgifter** om du vill ändra uppdragsändringar för enskilda uppgifter. När du anger enskilda uppgifter kan du välja projekt i **Välj projekt** fält ignoreras.\
   I **Välj uppgifter** börjar du skriva namnet på den uppgift där du vill göra uppdragsändringar. Upprepa det här steget om du vill göra uppdragsändringar för ytterligare uppgifter.\
   Om du lämnar det här fältet tomt påverkas alla uppgifter i de projekt som du valde i steg 3.\
   När du gör uppdragsändringar för enskilda uppgifter tillämpas ändringarna på alla underaktiviteter för de uppgifter som du anger. Ändringarna tillämpas även på alla problem som är kopplade till uppgifterna om problemen har konfigurerats att visas på tidslinjen för schemaläggningen, vilket beskrivs i [Du kan konfigurera olika inställningar för att anpassa hur och vilken information som ska visas på tidslinjen för schemaläggning.](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md#configuring-issues-to-display-on-the-scheduling-timeline) in [Konfigurera inställningar i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md).

1. Fortsätt med något av följande avsnitt:

   * [Tilldela en användare](#assign-a-user)
   * [Byta ut en användare](#swap-a-user)
   * [Ta bort användartilldelning](#unassign-a-user)

### Tilldela en användare {#assign-a-user}

Du kan tilldela en användare till alla uppgifter som för närvarande är tilldelade till en viss roll i de valda projekten.

När du tilldelar en användare på det här sättet tilldelas användaren inte följande typer av uppgifter:

* Uppdrag för uppgifter som redan har tilldelats en användare
* Slutförda uppgifter

Så här tilldelar du en användare till uppgifter i de markerade projekten eller aktiviteterna:

1. Välj **Tilldela användare** i **Välj åtgärd** -avsnitt.\
   ![](assets/resource-scheduling-assign-350x678.png)

1. I **Välj roll** klickar du på listrutepilen för att välja från en lista med roller. Endast roller som för närvarande är tilldelade till aktiviteter i de angivna projekten visas.\
   När du tilldelar en användare ersätter användaren de roller du väljer här.

1. I **Välj användare att tilldela** klickar du på listrutepilen och väljer en användare i en lista.\
   Om **Begränsa tilldelningar till användare med en matchande roll** är aktiverat i området Inställningar. Användarna kan bara välja om de har tilldelats den valda rollen i sina användarinställningar (antingen som primär roll eller en annan roll). Om det här alternativet är inaktiverat kan du börja skriva namnet på en annan användare som du vill tilldela, även om användaren inte har någon matchande roll definierad i systemet. Alternativet är aktiverat som standard.\
   Mer information om det här alternativet finns i [Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md). Som standard kan tilldelningar endast göras till användare som har en definierad roll i användarprofilen som matchar rolltilldelningen för uppgiften eller utgåvan som tilldelas dem.

1. Klicka **Tilldela**.\
   Du kan göra högst 1 000 tilldelningar i en enda åtgärd. Om de markeringar du gör kommer att göra fler än 1 000 uppdragsändringar måste du justera om markeringarna och försöka igen.

### Byta ut en användare {#swap-a-user}

Du kan byta ut en användares uppgiftstilldelningar mot en annan användares uppgiftstilldelningar i de valda projekten eller för de valda uppgifterna.

När du byter ut en användares uppgiftstilldelningar enligt beskrivningen i det här avsnittet, byts inte tilldelningar som redan är markerade Fullständigt ut.

Så här byter du ut en användares uppgiftstilldelningar mot en annan användares uppgiftstilldelningar:

1. Välj **Växla användare** i **Välj åtgärd** -avsnitt.\
   ![](assets/resource-scheduling-swap-350x674.png)

1. I **Välj användare** klickar du på listrutepilen för att välja från en lista med användare (eller börjar skriva namnet på den användare som du vill byta ut och klickar sedan på namnet när det visas i listrutan).\
   Användare visas bara när de har tilldelats en eller flera ofullständiga uppgifter inom de angivna projekten.

1. (Villkorligt) **Välj en roll** -fältet visas bara när användaren du har valt tilldelas flera uppgifter med olika roller. (Om du vill visa den jobbroll som har angetts för uppgiften för en användare går du till **Uppdragarens roll** i dialogrutan Avancerat uppdrag för uppgiften, enligt beskrivningen i [Skapa avancerade uppdrag](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)).\
   I **Välj en roll** väljer du rollen för att avgöra vilken typ av uppgifter du vill byta ut. Endast de uppgifter som användaren har tilldelats med den här rollen tilldelas den nya användaren.\
   Hanna Marin tilldelas till exempel 5 uppgifter i projektet. På två av arbetsuppgifterna definieras hennes roll som&quot;ingenjör&quot;. På de återstående tre uppgifterna definieras hennes jobbroll som&quot;Designer&quot;. Om du väljer Designer i fältet Välj roll innebär det att du vill ändra tilldelningarna för alla tre av Hannas uppgifter där hennes jobbroll definieras som&quot;Designer&quot;. De två uppgifter där hennes jobbroll definieras som en&quot;ingenjör&quot; förblir oförändrade.\
   ![](assets/resource-scheduling-swap-role.png)

1. I **Välj användare att tilldela** klickar du på listrutepilen och väljer en användare i en lista. Användarna är bara tillgängliga att tilldela om deras roller (enligt deras användarinställningar) matchar rollerna för det arbete som tilldelats användaren som du ersätter.\
   Om **Begränsa tilldelningar till användare med en matchande roll** är aktiverat i området Inställningar, är användare bara tillgängliga att tilldela om deras roller (enligt definition i deras användarinställningar) matchar rollerna i det arbete som tilldelats användaren som du ersätter. Om det här alternativet är inaktiverat kan du börja skriva namnet på en annan användare som du vill tilldela, även om användaren inte har någon matchande roll definierad i systemet. Alternativet är aktiverat som standard.\
   Mer information om det här alternativet finns i [Tillåt användartilldelningar oavsett roll- och gruppmedlemskap i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md). Som standard kan tilldelningar endast göras till användare som har en definierad roll i användarprofilen som matchar rolltilldelningen för uppgiften eller utgåvan som tilldelas dem.\
   Om användaren som du ersätter har tilldelats flera roller för uppgifter i de markerade projekten och du väljer mer än en roll i **Välj en roll** fält, **Välj användare att tilldela** visas endast användare som har alla angivna roller.

1. Klicka **Växla**.\
   Du kan göra högst 1 000 tilldelningar i en enda åtgärd. Om de markeringar du gör kommer att göra fler än 1 000 uppdragsändringar måste du justera om markeringarna och försöka igen.

### Ta bort användartilldelning {#unassign-a-user}

Du kan ta bort tilldelningen för en användare från alla uppgifter som användaren har tilldelats i de valda projekten eller för de valda aktiviteterna. När du tar bort tilldelningen för en användare återställs alla uppgifter som tilldelats användaren till tilldelningsläget innan användaren tilldelades.

Om en användare har en primär roll definierad i systemet och du tar bort användartilldelningen, tilldelas uppgiften automatiskt till användarens primära roll när du tar bort användartilldelningen. Eller så tilldelas den rollen den tilldelades innan användaren tilldelades.

Om en användare inte har någon primär roll definierad i systemet och du tar bort användartilldelningen, försätts uppgiften i ett icke tilldelat läge när du tar bort användartilldelningen.

Aktiviteter som har markerats som Slutförd kan inte tas bort.

Så här frigör du en användare från uppgifter i de markerade projekten eller för de valda uppgifterna:

1. Välj **Ta bort användartilldelning** i **Välj åtgärd** -avsnitt.\
   ![](assets/resource-scheduling-unassign-350x618.png)

1. I **Välj användare** klickar du på listrutepilen för att välja från en lista med användare (eller börjar skriva namnet på den användare som du vill ta bort och klickar sedan på namnet när det visas i listrutan). Du kan bara ta bort tilldelningen för en användare åt gången.
1. (Villkorligt) **Välj en roll** -fältet visas bara när användaren du har valt tilldelas flera uppgifter med olika roller. (Om du vill visa vilken jobbroll som är inställd för en användare kan du gå till **Uppdragarens roll** i dialogrutan Avancerat uppdrag för uppgiften, enligt beskrivningen i [Skapa avancerade uppdrag](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)).\
   I **Välj en roll** väljer du rollen för att bestämma vilken typ av uppgifter du vill ta bort tilldelningen för. Endast de uppgifter som användaren har tilldelats med den här rollen kommer att tas bort.\
   Hanna Marin tilldelas till exempel 5 uppgifter i ett projekt. I två arbetsuppgifter definieras hennes roll som ingenjör. På de återstående tre uppgifterna definieras hennes jobbroll som en designer. Om du väljer Designer i fältet Välj roll innebär det att du vill ta bort tilldelningen av Hanna för alla tre av hennes uppgifter där hennes jobbroll definieras som Designer. De två uppgifterna där hennes jobbroll definieras som en tekniker förblir oförändrade.\
   ![](assets/resource-scheduling-unassign-role.png)

1. Klicka **Ta bort tilldelning**.\
   Du kan göra högst 1 000 tilldelningar i en enda åtgärd. Om de markeringar du gör kommer att göra fler än 1 000 uppdragsändringar måste du justera om markeringarna och försöka igen.
