---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Delegera arbetsöversikt
description: När du planerar att vara borta från kontoret under en kort period kan du tillfälligt delegera ditt arbete till andra användare för att säkerställa att din frånvaro inte blir ett hinder för arbetet.
author: Becky
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# Delegera arbetsöversikt

När du planerar att vara borta från kontoret under en kort period kan du tillfälligt delegera ditt arbete till andra användare för att säkerställa att din frånvaro inte blir ett hinder för arbetet.

Om till exempel vissa uppgifter förfaller innan du returnerar dem, men du inte har tid att slutföra dem innan du lämnar dem, kan du delegera dina uppgifter till en annan användare så att de kan slutföra dem i tid och inte fördröja slutförandet av projektet tills du kommer tillbaka.

Du kan delegera följande objekt i [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Uppgifter som tilldelats dig
* Problem som du har tilldelats
* Projekt-, uppgifts- eller utfärdandegodkännanden som tilldelats dig.

  >[!TIP]
  >
  >   Du kan inte delegera tidrapport-, dokument- eller korrekturgodkännanden.


Den här artikeln innehåller allmän information om delegering av uppgifter och ärenden som du har tilldelats.

Mer information om hur du delegerar projekt-, uppgifts- och utfärdandegodkännanden finns i [Delegera godkännandebegäran](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Mer information om hur du delegerar uppgifter och problem finns i [Delegera uppgifter och problem](../../manage-work/delegate-work/how-to-delegate-work.md).

## Översikt över uppgifter och problem i delegering

Tänk på följande när du delegerar uppgifter och ärenden:

* [!DNL Workfront]- eller gruppadministratören måste aktivera delegeringsinställningarna i området [!UICONTROL Setup] innan du kan delegera ditt arbete till andra.

  Mer information finns i [Konfigurera uppgifter och utgåvinställningar för hela systemet](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Du kan endast delegera uppgifter och utgåvor från området [!UICONTROL Home].
* När du delegerar arbete finns det undantag för följande licenstyper:

   * Du kan delegera arbete till granskare eller begärande, men [!DNL Workfront] rekommenderar det inte.
   * Granskare kan delegera arbete till andra. De kan inte visa arbetsobjekt i sitt [!UICONTROL Home]-område. De kan bara visa godkännanden.
   * Beställare kan inte delegera arbete till andra. De kan inte visa arbetsobjekt i sitt [!UICONTROL Home]-område
* Du kan bara delegera de uppgifter och utgåvor som du har tilldelats. Du kan inte delegera uppgifter och ärenden som har tilldelats andra användare, team eller jobbroller.
* Du kan bara delegera uppgifter och ärenden som inte har slutförts före delegeringens startdatum.
* Om en arbetsuppgift slutförs under delegeringens tidsram finns posten kvar i hemområdet för delegaten och för den som tilldelats i två veckor innan [!DNL Workfront] automatiskt tar bort den.
* De användare som du väljer som ombud får samma behörigheter som de uppgifter och utgåvor som du delegerar till dem. Behörigheterna måste fungera inom sina åtkomstnivåer och ibland kan deras åtkomstnivåer vara lägre än dina.

>[!NOTE]
>
>  För objekt som tilldelas efter att delegeringen redan har startats kan det ta upp till en timme efter det att objektet tilldelats [!DNL Workfront] att dela de nyligen tilldelade objekten med delegaten.

* Om du tilldelas ytterligare uppgifter och utgåvor under den tid du har valt att delegera arbetet till andra användare, delegeras det nya tilldelade arbetet automatiskt till samma person för den tidsram du valde om uppgifts- eller utgivningsdatumen ligger inom den tidsramen.
* Samma användare kan väljas som ombud av flera användare.
* Delegerade uppgifter och problem visas inte i resurshanteringsverktyg, som [!UICONTROL Workload Balancer] eller [!UICONTROL Resource Planner] för de delegerade användarna.
* Du kan visa namn på delegerade arbeten och delegater i flera områden i [!DNL Workfront]. Mer information finns i avsnittet Hitta information om delegerade arbeten och delegater i artikeln [Delegera uppgifter och problem](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Om en användare bara har Visa åtkomst till uppgifter på sin åtkomstnivå och du har behörigheten Hantera för de uppgifter som du delegerar till dem, får de behörigheten Hantera för de uppgifter som du delegerar till dem. De kan dock inte utföra samma åtgärder som du för de delegerade uppgifterna. De måste begära Redigera-åtkomst till uppgifter från systemadministratören för att kunna uppdatera uppgifter om du inte är anställd.

* När delegeringen stoppas tas inte de behörigheter som tilldelats de delegerade användarna bort för de uppgifter och problem som de har delegerats till.
* Om ett system eller inaktiverar inställningen [!UICONTROL Allow users to delegate their tasks & issues] i området [!UICONTROL Setup] tas de för närvarande delegerade användarna bort från de uppgifter och utgåvor som de tidigare har delegerats till. Deras behörigheter till uppgifter eller problem tas inte bort.

## Skillnader och likheter mellan uppdrag och delegationer

| Åtgärd | Uppdrag | Delegeringar |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| En tilldelad eller delegerad användare kan redigera eller ta bort arbetsuppgiften som de har tilldelats eller delegerats till | Baserat på behörigheter och åtkomstnivå | Baserat på behörigheter och åtkomstnivå |
| En tilldelad eller delegerad användare visas i arbetsobjektets rubrik | Ja | Ja |
| De tilldelade eller delegerade uppgifterna eller frågorna visas i den tilldelades eller delegatens hemområde | Ja, tills artikeln är slutförd | Ja, endast under delegeringens tidsram |
| Du kan tilldela eller delegera arbete till användare från Hem-området | Ja | Ja |
| Du kan tilldela eller delegera arbete till användare med hjälp av Utjämning av arbetsbelastning | Ja | Nej |
| Du kan tilldela eller delegera arbete till användare i en lista eller från en arbetsuppgifts rubrik | Ja | Nej |
| Alla användare kan tilldela eller delegera andra användare med arbetsobjekt som de inte är kopplade till | Baserat på behörigheter och åtkomstnivå | Nej. Endast den som tilldelats kan delegera sina egna artiklar. |
| Planerade, faktiska eller budgeterade timmar för arbete som tilldelats eller delegerats till en användarvy för den användaren i resurshanteringsverktyg | Ja | Nej |
