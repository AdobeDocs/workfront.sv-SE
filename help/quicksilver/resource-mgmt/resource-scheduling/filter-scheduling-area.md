---
product-area: resource-management
navigation-topic: resource-scheduling
title: Filterinformation i området Schemaläggning
description: Med hjälp av ett filter i området Resursschemaläggning kan du avgöra vilka arbetsobjekt som visas på tidslinjen i tidslinjen. Detta inkluderar vilka uppgifter och problem som visas i området Ej tilldelade samt vilka användare som visas.
author: Alina
feature: Resource Management
exl-id: 974b2515-ed10-459d-a317-36e62c52afc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2452'
ht-degree: 0%

---

# Filterinformation i området Schemaläggning

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
<p>(SEVERAL SECTIONS BELOW LINKED TO THE PRODUCT. SEE NOTES</p>
-->

Med hjälp av ett filter i området Resursschemaläggning kan du avgöra vilka arbetsobjekt som visas på tidslinjen i tidslinjen. Detta inkluderar vilka uppgifter och problem som visas i området Ej tilldelade samt vilka användare som visas.

Innan du börjar filtrera innehåll enligt beskrivningen i det här avsnittet bör du känna till hur resursplanering fungerar i Adobe Workfront.\
Mer information om resursplanering i Workfront finns i artikeln [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).\
Mer information om tidslinjen för schemaläggning finns i artikeln [Kom igång med resursschemaläggning](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Du kan schemalägga resurser för ett enskilt team som du är medlem i eller för projekt som du är resurshanterare för.

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
   <td> <p>Visa åtkomst eller senare till projekt, uppgifter och ärenden</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre till projekt, uppgifter och ärenden</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

<!--
<p>(NOTE: sections below - LINKED TO THE ui. DO NOT RENAME/ DELETE)</p>
-->

## Skapa ett filter i schemaavsnittet (för team)

Uppgifter och ärenden från projekt, användare och roller som du definierar i filtret visas på tidslinjen för schemaläggning på fliken Arbeta med. Använd alternativen i filtret för att bestämma vilka projekt, användare och roller som ska visas på tidslinjen i tidsplanen.

>[!NOTE]
>
>Du kan inte spara ett filter på fliken Arbeta på (för ett team). När du uppdaterar sidan eller navigerar bort från den, återställs filtret till standardinställningarna.

Så här skapar du ett filter för tidslinjen i schemat på fliken Arbeta på för team:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Team**, välj ett team, klicka på **Utjämning av arbetsbelastning** i den vänstra panelen väljer **Schemaläggning** i den övre vänstra listrutan.
1. Klicka **Filter**.
1. Bestäm vilka projekt som ska visas i området Ej tilldelade genom att ange följande information:

   <!--
   <p>(NOTE: Alina: there was a note that [This step is linked to from the context-sensitive help] but I could not find from where in the UI it is linked.)&nbsp;</p>
   -->

   * **Projektprioriteringar:** Välj prioriteten för de projekt som du vill ska representeras på tidslinjen i tidsplanen. Uppgifter och ärenden från projekt med de prioriteringar du väljer visas på tidslinjen för schemaläggning.\
      Det går bara att välja prioriteter från projekt som innehåller uppgifter eller ärenden som har tilldelats teamet på den här menyn.
   * **Projektstatus:** Välj status för de projekt som du vill ska visas på tidslinjen i tidsplanen. Uppgifter och ärenden från projekt med de statusvärden du väljer visas på tidslinjen för tidsplanering.\
      Det går bara att välja status från projekt som innehåller uppgifter eller ärenden som har tilldelats teamet på den här menyn.
   * **Projekt:** Välj de projekt som du vill ska visas på tidslinjen i tidsplanen. Uppgifter och ärenden från de projekt du väljer visas på tidslinjen för tidsplanering.\
      Dina val i de föregående fälten avgör vilka projekt som är tillgängliga att välja.\
      Det är bara projekt som innehåller uppgifter eller ärenden som har tilldelats teamet som kan väljas på den här menyn.

1. Bestäm vilka användare som ska visas på tidslinjen genom att ange följande information. Som standard visas alla teammedlemmar.

   <!--
   <p>(NOTE: this step is linked in the UI.)</p>
   -->

   * **Roller:** Välj de roller som du vill ska representeras på tidslinjen i tidsplanen.\
      Endast uppgifter som tilldelats den rollen visas i området Ej tilldelade. Endast användare med de roller du väljer som kan tilldelas dessa uppgifter visas.\
      Användare visas på tidslinjen för schemaläggning, ordnade efter jobbroll.
   * **Användare:** Markera de enskilda användare som du vill ska visas på tidslinjen i tidsplanen.\
      Endast de användare du väljer visas, oavsett om de har en rolltilldelning som matchar rolltilldelningen för uppgifter i området Ej tilldelade.\
      Det här alternativet påverkar inte vilka uppgifter och problem som visas i området Ej tilldelade.

      <!--   
     <p>(NOTE: Alina: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])</p>   
     -->

1. (Valfritt) Om du vill göra ytterligare ändringar i tidslinjen för tidsplanering (till exempel ändra datumintervallet) och om du vill göra ändringar i användartilldelningar kan du läsa artikeln [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p>(NOTE: below - LINKED TO THE UI, DO NOT RENAME/ DELETE/ CHANGE)</p>
-->

## Skapa och ändra filter i avsnittet Schemaläggning (för flera projekt)

Du kan skapa ett nytt filter, använda ett filter som du har skapat tidigare, ändra ett filter som du har skapat tidigare eller ta bort ett filter. Du kan inte dela filter som du skapar med andra användare.

* [Skapa ett filter i avsnittet Schemaläggning (för projekt)](#create-a-filter-in-the-scheduling-section-for-projects)
* [Använda ett sparat filter](#apply-a-saved-filter)
* [Ändra ett sparat filter](#modify-a-saved-filter)
* [Ta bort ett sparat filter](#delete-a-saved-filter)

### Skapa ett filter i avsnittet Schemaläggning (för projekt) {#create-a-filter-in-the-scheduling-section-for-projects}

<!--
<p>(NOTE: *****LINKED TO THE PRODUCT FROM THE GLOBAL SCHEDULER >> BOTH THE FIRST AND THE SECOND AREAS) </p>
-->

Uppgifter och ärenden från projekt, användare och roller som du definierar i filtret visas på tidslinjen för schemaläggning på fliken Schemaläggning. Använd alternativen i filtret för att bestämma vilka projekt, användare och roller som ska visas på tidslinjen i tidsplanen.

Så här skapar du ett filter för tidslinjen i schemaläggningen på fliken Schemaläggning för flera projekt:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
1. Klicka **Filter**.\
   ![](assets/scheduling-filter-350x351.png)

1. Lämna **Sparade filter** fältet är tomt.
1. Bestäm vilka projekt som ska visas i området Ej tilldelade genom att ange följande information:

   <!--
   <p>(NOTE: Alina: this step is linked in the UI.) </p>
   -->

   * **Portfolio:** Välj alla portföljer som innehåller program och projekt som du vill ska visas på tidslinjen i tidsplanen.

      Endast program i portföljerna du väljer är tillgängliga att välja i **Program** fält.

   * **Program:** Välj alla program som innehåller projekt som du vill ska visas på tidslinjen för schemaläggningen.\
      Dina val i **Portfolio** -fältet avgör vilka program som är tillgängliga att välja.\
      Endast projekt i de program du väljer är tillgängliga för val i **Projekt** fält.

   * **Projektprioriteringar:** Välj prioriteten för de projekt som du vill ska representeras på tidslinjen i tidsplanen.\
      Endast projekt med de prioriteringar du väljer visas.

   * **Projektstatus:** Välj status för de projekt som du vill ska visas på tidslinjen i tidsplanen.\
      Endast projekt med de statusvärden du väljer visas.

   * **Projektföretag:** Uppgifter och ärenden visas bara på tidslinjen i tidslinjen när de tillhör ett projekt som matchar ett företag som du väljer.

   * **Projektgrupper:** Uppgifter och ärenden visas bara på tidslinjen i tidslinjen när de tillhör ett projekt som matchar en grupp som du väljer.

   * **Projekt:** Välj de projekt som du vill ska visas på tidslinjen i tidsplanen. Uppgifter och ärenden från de projekt du väljer visas på tidslinjen för tidsplanering.\
      Dina val i de föregående fälten avgör vilka projekt som är tillgängliga att välja.\
      Uppgifter och ärenden från de projekt du väljer visas på tidslinjen för tidsplanering. Det är bara projekt som innehåller uppgifter eller ärenden som har tilldelats teamet som kan väljas på den här menyn.

1. Bestäm vilka användare som ska visas på tidslinjen för tidsplanering genom att ange följande information: (Som standard visas endast användare som är berättigade att tilldelas en uppgift eller ett problem i området Ej tilldelade. När du väljer enskilda användare visas användarna på tidslinjen för schemaläggning oavsett om de är berättigade att tilldelas en uppgift eller ett problem i området Ej tilldelade.) 

   <!--
   <p>(NOTE: Alina: this step had a note that it is linked in the UI but I could not find from where.) </p>
   -->

   * **Användarföretag:** I det här fältet kan du hindra användare från andra företag från att visas på tidslinjen för schemaläggningen.\
      Lämna det här fältet tomt om du vill att användare från ett företag ska läggas till. Om du anger enskilda företag kan bara användare från dessa företag läggas till på tidslinjen för schemaläggning. Om du anger ett företag läggs användare från det företaget inte automatiskt till på tidslinjen för schemaläggning. Använd i stället fälten nedan för att lägga till specifika användare.\
      Det här alternativet påverkar inte vilka uppgifter och problem som visas i området Ej tilldelade.****

   * **Användargrupper:** Alla användare från en användargrupp som du anger visas på tidslinjen för schemaläggning.

   * **Team:** Alla användare från det team du anger visas på tidslinjen för schemaläggningen.\
      Det här alternativet påverkar inte vilka uppgifter och problem som visas i området Ej tilldelade.

   * **Roller:** Välj de roller som du vill ska representeras på tidslinjen i tidsplanen.\
      Endast uppgifter som tilldelats den rollen visas i området Ej tilldelade. Endast användare med de roller du väljer som kan tilldelas dessa uppgifter visas.\
      Användare visas på tidslinjen för schemaläggning, ordnade efter jobbroll.

   * **Användare:** Markera de enskilda användare som du vill ska visas på tidslinjen i tidsplanen.\
      Endast de användare du väljer visas, oavsett om de har en rolltilldelning som matchar rolltilldelningen för uppgifter i området Ej tilldelade.\
      Det här alternativet påverkar inte vilka uppgifter och problem som visas i området Ej tilldelade.
   <!--
   <p>NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->

1. Klicka **Spara nytt filter**.\
   Dina data visas på tidslinjen för tidsplanering.

1. (Valfritt) Om du vill göra ytterligare ändringar i tidslinjen för tidsplanering (till exempel ändra datumintervallet) och om du vill göra ändringar i användartilldelningar kan du läsa artikeln [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Använda ett sparat filter {#apply-a-saved-filter}

>[!NOTE]
>
>Det här alternativet gäller endast vid schemaläggning av resurser för flera projekt (från fliken Schemaläggning). Du kan inte använda ett sparat filter när du schemalägger resurser för ett team (från fliken Arbeta med) eller när du schemalägger resurser för ett enskilt projekt (från fliken Personal).

Du kan använda ett filter som du har skapat tidigare.

Så här använder du ett sparat filter för flera projekt:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
1. Klicka **Filter**.
1. I **Sparade filter** markerar du det filter som du vill använda.\
   Dina data visas på tidslinjen för tidsplanering.

1. (Valfritt) Om du vill göra ytterligare ändringar i tidslinjen för tidsplanering (till exempel ändra datumintervallet) och om du vill göra ändringar i användartilldelningar kan du läsa artikeln [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Ändra ett sparat filter {#modify-a-saved-filter}

>[!NOTE]
>
>Det här alternativet gäller endast vid schemaläggning av resurser för flera projekt (från fliken Schemaläggning). Du kan inte ändra ett sparat filter när du schemalägger resurser för ett team (från fliken Arbeta med) eller när du schemalägger resurser för ett enskilt projekt (från fliken Personal).

Du kan ändra ett filter som du har skapat tidigare.

Så här ändrar du ett sparat filter för flera projekt:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
1. Klicka **Filter**.
1. I **Sparade filter** väljer du det filter som du vill ändra i listrutan.
1. Ange vilka data som ska visas på tidslinjen för tidsplanen.
1. Klicka **Spara**.\
   Dina data visas på tidslinjen för tidsplanering.

1. (Valfritt) Om du vill göra ytterligare ändringar i tidslinjen för tidsplanering (till exempel ändra datumintervallet) och om du vill göra ändringar i användartilldelningar kan du läsa artikeln [Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Ta bort ett sparat filter {#delete-a-saved-filter}

>[!NOTE]
Det här alternativet gäller endast vid schemaläggning av resurser för flera projekt (från fliken Schemaläggning). Du kan inte ta bort ett sparat filter när du schemalägger resurser för ett team (på fliken Arbeta med) eller när du schemalägger resurser för ett enskilt projekt (på fliken Personal).

Du kan ta bort ett filter som du har skapat tidigare.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront klickar du på **Resurser > Arbetsbelastningsutjämning** väljer **Schemaläggning** i den övre vänstra listrutan.
1. Klicka **Filter**.
1. I **Sparade filter** i listrutan klickar du på (x) bredvid det filter du vill ta bort. 

## Skapa och ändra filter i avsnittet Schemaläggning (för ett enskilt projekt)

<!--
<p>(NOTE: **** LINKED FROM THE PRODUCT FROM THE PROJECT> STAFFING> SCHEDULING AREA) </p>
-->

Uppgifter och ärenden från användare, team och roller som du definierar i filtret visas på tidslinjen för schemaläggning på fliken Personal. Använd alternativen i filtret för att avgöra vilka användare, team och roller som ska visas på tidslinjen i tidsplanen.

>[!NOTE]
Det går inte att spara ett filter på fliken Tillstånd (för ett enskilt projekt). När du uppdaterar sidan eller navigerar bort från den, återställs filtret till standardinställningarna.

Så här skapar du ett filter för tidslinjen i schemat på fliken Anställning för ett enskilt projekt:

1. Gå till ett projekt och klicka på **Utjämning av arbetsbelastning** i den vänstra panelen och sedan markera **Schemaläggning** i den övre vänstra listrutan.
1. Bestäm vilka användare som ska visas på tidslinjen för tidsplanering genom att ange följande information: (Som standard visas endast användare som är berättigade att tilldelas en uppgift eller ett problem i området Ej tilldelade. När du väljer enskilda användare visas användarna på tidslinjen för schemaläggning oavsett om de är berättigade att tilldelas en uppgift eller ett problem i området Ej tilldelade.) 

   <!--
   <p><span>(NOTE: Alina: [This step is linked to from the context-sensitive help]) </span> </p>
   -->

   * **Användarföretag:** I det här fältet kan du hindra användare från andra företag från att visas på tidslinjen för schemaläggningen.\
      Lämna det här fältet tomt om du vill att användare från ett företag ska läggas till. Om du anger enskilda företag kan bara användare från dessa företag läggas till på tidslinjen för schemaläggning. Om du anger ett företag läggs användare från det företaget inte automatiskt till på tidslinjen för schemaläggning. Använd i stället fälten nedan för att lägga till specifika användare.\
      Det här alternativet påverkar inte vilka uppgifter och problem som visas i området Ej tilldelade.

   * **Användargrupper:** Alla användare från en användargrupp som du anger visas på tidslinjen för schemaläggning.

   * **Team:** Alla användare från det team du anger visas på tidslinjen för schemaläggningen.\
      Det här alternativet påverkar inte vilka uppgifter och problem som visas i området Ej tilldelade.

   * **Roller:** Välj de roller som du vill ska representeras på tidslinjen i tidsplanen.\
      Endast uppgifter som tilldelats den rollen visas i området Ej tilldelade. Endast användare med de roller du väljer som kan tilldelas dessa uppgifter visas.\
      Användare visas på tidslinjen för schemaläggning, ordnade efter jobbroll.

   * **Användare:** Markera de enskilda användare som du vill ska visas på tidslinjen i tidsplanen.\
      Endast de användare du väljer visas, oavsett om de har en rolltilldelning som matchar rolltilldelningen för uppgifter i området Ej tilldelade.\
      Det här alternativet påverkar inte vilka uppgifter och problem som visas i området Ej tilldelade.
   <!--
   <p>(NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->
