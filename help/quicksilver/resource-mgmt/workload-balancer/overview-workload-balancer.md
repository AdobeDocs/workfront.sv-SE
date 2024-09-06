---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Översikt över belastningsutjämnare
description: När projektledare har planerat arbetet i projekt genom att skapa uppgifter och när resursansvariga har allokerat jobbrollresurser till projekt i resursplaneraren kan projektägare och teamchefer använda arbetsbelastningsutjämnaren för att tilldela användare arbetsobjekt.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 0%

---

# Översikt över belastningsutjämnare

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

När projektledare har planerat arbetet i projekt genom att skapa uppgifter och när resursansvariga har allokerat jobbrollresurser till projekt i resursplaneraren kan projektägare och teamchefer använda arbetsbelastningsutjämnaren för att tilldela användare arbetsobjekt.

>[!IMPORTANT]
>
>Du kan använda belastningsutjämnaren för att tilldela användare verkligt arbete (uppgifter och ärenden).
>
>Du måste använda Resursplanering och inte Utjämning av arbetsbelastning för att beräkna rollallokeringar för dina projekt på en hög nivå. Mer information om resursplaneraren finns i [Översikt över resursplaneraren](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

I den här artikeln beskrivs det allmänna syftet med Utjämning av arbetsbelastning och några av de bästa sätten att konfigurera projekt och resurser så att de kan användas.

Gå till sidan [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html) om du vill se videosjälvstudiekurser om arbetsbelastningsutjämnaren. Välj **Hantera resurser** > **Utjämning av arbetsbelastning** på den vänstra menyn och välj en självstudiekurs.

## Leta reda på arbetsbelastningsutjämnaren

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Vi rekommenderar att du använder Utjämning av arbetsbelastning i följande områden för att schemalägga resurser:

* På systemnivå i området Resurser.
* På projektnivå i avsnittet Arbetsbelastningsutjämning i ett projekt.
* På teamnivå, i avsnittet Arbetsbelastningsutjämning i ett team.

Mer information om hur du hittar arbetsbelastningsutjämnaren finns i [Hitta arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Fördelar med Utjämning av arbetsbelastning

Tänk på följande fördelar när du använder arbetsbelastningsutjämnaren:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Få en tydlig visuell mappning av resursöverbeläggning och underutnyttjande som är transparent för alla intressenter.
* Som personledare kan ni skydda era medarbetare från bränning och ge dem möjlighet att göra sitt bästa med bättre fokus, kvalitet och engagemang. Ni kan se till att de används fullt ut, bryta vattentäta skott och göra det möjligt att anpassa arbetet mellan olika team.
* När du tilldelar arbete på aktivitets- eller problemnivå har du inte insikt i hur mycket en användare kan vara upptagen. När du använder Utjämning av arbetsbelastning kan du visa vilka användare som har tillgänglighet i sin arbetsbelastning för att slutföra uppgiften eller problemet i tid. Detta inkluderar deras ledig tid och information om schemaläggningsundantag.

  Mer information finns i [Översikt över hur du tilldelar arbete i Arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  Du kan också tilldela flera arbetsobjekt samtidigt, vilket gör det enklare att distribuera flera arbetsobjekt samtidigt i flera projekt. Mer information finns i [Tilldela flera arbeten samtidigt med hjälp av arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Cheferna kan fatta vältajmade personalbeslut genom öppenhet och insyn i hur de använder sina anställda.
* Teammedlemmarna drar nytta av bättre samarbete eftersom de alla kan se vad deras medarbetare arbetar med vid en viss tidpunkt. Mer information om den åtkomst som behövs för att visa eller hantera resurser i arbetsbelastningsutjämnaren finns i [Åtkomst som behövs för att hantera resurser i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Dela den med alla som inte har tillgång till resursområdet genom att bädda in en länk till den på en anpassad flik. Mer information finns i [Dela arbetsbelastningsutjämnaren med en länk](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualisera och hantera människors arbetsbelastning och efterfrågan i en vy på global nivå, projekt- eller teamnivå, beroende på din roll. När du hanterar projekt omfattar detta inte bara resurstilldelning för projektet, utan även visualisering av resursallokeringen från Adobe Workfront Scenario Planner. Anställda använder Workfront Scenario Planner för att hantera jobbfärdigheter i hela organisationen. Scenarioplaneraren är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

  >[!NOTE]
  >
  >  Scenario Planner kräver ytterligare licens. Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../scenario-planner/scenario-planner-overview.md).


## Bästa tillvägagångssätt för att använda belastningsutjämnaren

Vi rekommenderar följande metodtips för att planera projekt, konfigurera användare och använda filter innan du börjar schemalägga resurser med hjälp av Utjämning av arbetsbelastning.

* [Bästa tillvägagångssätt för att visa information i arbetsbelastningsutjämnaren](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Bästa tillvägagångssätt för att konfigurera användare](#best-practices-for-setting-up-users)
* [Bästa tillvägagångssätt för att konfigurera uppgifter och problem](#best-practices-for-setting-up-tasks-and-issues)

### Bästa tillvägagångssätt för att visa information i arbetsbelastningsutjämnaren {#best-practices-for-displaying-information-in-the-workload-balancer}

Vi rekommenderar att du använder filter så att du bara kan visa den information som är relevant för dig för både ej tilldelade och tilldelade arbetsuppgifter.

Mer information om hur du skapar och använder filter i Arbetsbelastningsutjämnaren finns i [Filtrera information i Arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Bästa tillvägagångssätt för att konfigurera användare

* Som den användare som schemalägger arbete åt andra måste du ha rätt behörighet och behörighet för att schemalägga resurser för arbete.

  Mer information om åtkomsten som krävs för att hantera arbetsbelastningen för dina resurser i arbetsbelastningsutjämnaren finns i [Åtkomst som behövs för att hantera resurser i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* De användare vars arbetsbelastning du vill hantera måste uppfylla följande kriterier så att informationen om deras tillgänglighet och kompetens är korrekt:

   * Ha scheman och jobbroller associerade med sin profil.

     Mer information om hur du associerar scheman och jobbroller med användare finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Om en användare inte är associerad med ett schema, är standardschemat i ditt Workfront-system associerat med användaren som standard för resurshantering.
   * Se till att scheman för schemaundantag uppdateras.

     Mer information om att skapa scheman finns i [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Få sin&quot;Time Off&quot;-kalender uppdaterad i sin profil.

     Mer information om hur du uppdaterar en användares Tid utanför kalendern finns i [Konfigurera personlig tid för ](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Workfront-administratören måste bestämma hur Workfront ska beräkna tillgängligheten för användare. De kan avgöra om Workfront använder standardschemat för systemet eller användarens schema för att beräkna den tid som användaren är tillgänglig för arbete genom att justera inställningarna för resurshantering i inställningsområdet i Workfront.

  Mer information finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Bästa tillvägagångssätt för att konfigurera uppgifter och problem {#best-practices-for-setting-up-tasks-and-issues}

Se till att följande konfigurering av uppgifter och utgåvor finns innan du börjar tilldela arbete till användare i arbetsbelastningsutjämnaren:

* Överordnade uppgifter tilldelas inte till användare eller roller. Överordnade uppgifter visas inte i arbetsbelastningsutjämnaren.
* Aktiviteter och ärenden har ett värde för Planerade timmar som är större än noll.

* Aktiviteter och ärenden har ett värde för Varaktighet som är större än noll.
* Planerade datum för problemen ligger inom tidslinjen för projektet.

## Innan du börjar använda arbetsbelastningsutjämnaren

* Granska följande artiklar innan du börjar använda Utjämning av arbetsbelastning:

   * I den här artikeln beskrivs hur du navigerar i arbetsbelastningsutjämnaren för att utföra följande åtgärder: [Navigera i arbetsbelastningsutjämnaren](../workload-balancer/navigate-the-workload-balancer.md).

   * I följande artiklar beskrivs hur du tilldelar arbete och hanterar användartilldelningar:

      * [Översikt över tilldelning av arbete i arbetsbelastningsutjämnaren](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Hantera användarallokeringar i arbetsbelastningsutjämnaren](../workload-balancer/manage-user-allocations-workload-balancer.md).

* Utjämningen av arbetsbelastning finns i flera olika delar av Workfront. Mer information om var du kan hitta arbetsbelastningsutjämnaren finns i [Leta reda på arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Åtkomst krävs för att använda arbetsbelastningsutjämnaren

Du måste ha rätt åtkomst och behörighet för Workfront till specifika projekt för att kunna visa och använda arbetsbelastningsutjämnaren i Workfront. Mer information om den åtkomst som behövs för att använda arbetsbelastningsutjämnaren finns i artikeln [Åtkomst som behövs för att hantera resurser i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
