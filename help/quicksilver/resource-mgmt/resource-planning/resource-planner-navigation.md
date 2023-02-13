---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Översikt över navigering i resursplanering
description: Genom att använda Adobe Workfront Resursplanering kan du enkelt förstå tillgängligheten för dina resurser och den tid som behövs för att slutföra arbetet i dina projekt. Du kan sedan hantera tilldelningen av dina användare och deras jobbroller i de projekt de tilldelas till.
author: Alina
feature: Resource Management
exl-id: 5a1be723-e3ac-443a-9c09-85e8839fcbef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2658'
ht-degree: 0%

---

# Översikt över navigering i resursplanering

Genom att använda Adobe Workfront Resursplanering kan du enkelt förstå tillgängligheten för dina resurser och den tid som behövs för att slutföra arbetet i dina projekt. Du kan sedan hantera tilldelningen av dina användare och deras jobbroller i de projekt de tilldelas till.

>[!TIP]
>
>Du kan inte hantera grupptilldelningen för de uppgifter som de har tilldelats i resursplaneraren.

Du måste uppfylla kraven för att kunna använda resursplaneraren fullt ut. Mer information om resursplaneraren finns i [Översikt över resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

![](assets/rp-project-view-all-functionality-350x117.png)

I följande avsnitt beskrivs alla områden i resursplaneraren.

## Tidslinje för projekt

![](assets/timeline-calendar-resource-planner-nwe-350x25.png)



Använd kalendern högst upp i resursplaneraren för att navigera på tidslinjen för de projekt som du visar. Tidslinjen börjar som standard med dagens månad.\
Mer information om hur du ändrar tidsramen för tidslinjen som du visar i resursplaneraren finns i avsnittet [Val av tidsram](#timeframe-selection) i den här artikeln.

## Val av tidsram  {#timeframe-selection}

![time_frame_selection_in_the_resource_planner.png](assets/time-frame-selection-in-the-resource-planner-350x61.png)

Resursplaneraren visar som standard resursinformation i tre eller fyra månader i taget, med början den aktuella månaden. Hur många tidsperioder som visas beror på skärmens bredd.

>[!TIP]
>
>Du kan inte visa mer än fyra tidsperioder i taget i resursplaneraren.

Så här navigerar du på tidslinjen:

1. Klicka på bakåt- och framåtpilarna för att flytta bakåt och framåt på tidslinjen.
1. Välj bland följande datumintervallalternativ i Resursplanering genom att klicka på lämpliga knappar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vecka</td> 
      <td>Visar information per vecka.<br>Antalet veckor visas bredvid datumen i kolumnrubriken. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Månad</td> 
      <td> Visar information per månad.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kvartal</td> 
      <td>Visar information per kvartal.<br>Numret på kvartalet visas bredvid datumen i kolumnrubriken.<br>Anpassade kvartal visas inte i resursplaneraren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Idag</td> 
      <td>Återgår till dagens månad, vecka eller kvartal.</td> 
     </tr> 
    </tbody> 
   </table>

## Projekt/roll/Val av användarvy

![](assets/nwe-project-role-user-view-selection-resource-planner.png)

Du kan ändra vyn i resursplaneraren beroende på hur du vill att informationen ska visas.

Resursplaneraren visas som standard i användarvyn. Du kan ändra vyn till projekt- eller rollvyer. När du ändrar den till en annan vy blir ditt val standardvy.

När du ändrar vyn ändras även följande information:

* Objekthierarkin (information i rader i resursplaneraren).
* Information om timallokering (information i kolumnerna i resursplaneraren).

   Mer information om vad kolumnerna visas i resursplaneraren, beroende på vilken vy du väljer, finns i [Granska resurstillgänglighet och tilldelning med Adobe Workfront Resource Planner](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

För att kunna visa korrekt information i resursplaneraren måste du uppfylla en uppsättning krav. Mer information om förutsättningarna finns i avsnittet Krav för att arbeta i resursplaneraren i [Översikt över resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planner.md) artikel.  Så här ändrar du vyn i resursplaneraren:

1. Gå till **Resursplanering**.\
   Mer information om åtkomst till resursplaneraren finns i [Leta reda på resursplaneraren](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) i [Översikt över resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planner.md) artikel.

1. I **Visa efter** väljer du en av följande vyer:

   * [Visa efter projekt](#view-by-project)
   * [Visa efter roll](#view-by-role)
   * [Visa efter användare](#view-by-user)

### Visa efter projekt {#view-by-project}

Tänk på följande när du väljer projektvyn i resursplaneraren:

* Du kan se projekt som du har behörighet att åtminstone visa.
* När du öppnar resursplaneraren för första gången kan du se projekt som filtreras med standardfiltret.\
   Mer information om filtrering av information i resursplaneraren finns i [Filtrera information i resursplaneraren](../../resource-mgmt/resource-planning/filter-resource-planner.md).

* Antalet objekt som du visar eller kan exportera från projektvyn är begränsat, vilket förbättrar prestandan.\
   Mer information om begränsningar när du visar resursplaneraren i projektvyn finns i [Begränsningar i projektvyn](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md#project-view-limits) i [Resursplanering - visningsbegränsningar](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) artikel.

* Projekten listas i den ordning de har i projektvyn.\
   Mer information om projektprioritet i Resursplanering finns i [Projektplaneringsprioritet](#project-planning-priority) i den här artikeln.

* När du expanderar varje projekt kan du visa de jobbroller som är kopplade till det.\
   När du expanderar varje roll kan du visa användare som är kopplade till den.\
   Rulla för att läsa in fler roller och användare under varje projekt.

* När den här vyn används lägger rolltimmarna, FTE eller Kostnaden till högst projekttimmarna, FTE eller Kostnad.\
   ![resource_planner_view_by_project.png](assets/resource-planner-view-by-project-350x228.png)

* Du kan visa följande timma-, FTE- eller kostnadsinformation i projektvyn:

   * Tillgänglig
   * Planerad
   * Budgeterad
   * Varians
   * Net

      Mer information finns i [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

### Visa efter roll {#view-by-role}

Tänk på följande när du väljer rollvyn i resursplaneraren:

* Du måste ha minst behörigheten Visa åtkomst till resurshantering och visa behörigheter för projekt för att kunna visa rollerna som är kopplade till dessa projekt.
* Du kan expandera varje roll för att visa en lista över projekt och varje projekt för att visa en lista över användare som kan uppfylla de rollerna i projekten.
* Antalet objekt som du visar eller kan exportera från rollvyn är begränsat, vilket förbättrar prestandan.\
   Mer information om begränsningar när du visar resursplaneraren i rollvyn finns i [Begränsningar i rollvyn](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md#role-view-limits) avsnitt i [Resursplanering - visningsbegränsningar](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

* Projekten listas under jobbrollen i samma prioriteringsordning som de listas i projektvyn.
* När den här vyn används läggs projekttimmar, heltidsekvivalenter eller kostnad till upp till rolltimmarna, heltidsekvivalenten eller kostnaden.\
   ![resource_planner_view_by_role.png](assets/resource-planner-view-by-role-350x222.png)

* Du kan visa följande timma-, FTE- eller kostnadsinformation i rollvyn:

   * Tillgänglig
   * Planerad
   * Budgeterad
   * Varians
   * Net

      Mer information finns i [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

### Visa efter användare {#view-by-user}

Du kan visa resursplaneraren i användarvyn för att förstå skillnaden mellan den planerade och tillgängliga timmar eller FTE för dina användare eller för att se hur många faktiska timmar de har loggat.

Du kan inte budgetera dina resurser när du använder användarvyn i resursplaneraren. Du måste budgetera dina resurser med projekt- eller rollvyerna och använda användarvyn för att granska användarnas tilldelning och tillgänglighet i relation till det planerade arbetet.* *

Användarvyn är standardvyn för resursplaneraren.

![RP_STORM_user_view_with_link.png](assets/rp-user-view-with-link-350x101.png)

Tänk på följande när du väljer användarvyn i resursplaneraren:

* Du kan se alla användare som du har behörighet att visa, upp till 2 000 användare, som är aktiva och har loggat in på Adobe Workfront minst en gång.\
   Filtrera användarlistan efter team, jobbroll eller pooler för att visa användare som bara är associerade med dessa entiteter.
* Om du har filtrerat listan över användare efter projekt kan bara de användare som är kopplade till de filtrerade projekten expanderas och även visa timinformation.\
   Mer information om filtrering av information i resursplaneraren finns i [Filtrera information i resursplaneraren](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

* Antalet objekt som du visar eller kan exportera från användarvyn är begränsat, vilket förbättrar prestandan.\
   Mer information om begränsningar när du visar resursplaneringen i användarvyn finns i [Begränsningar i användarvyn](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md#user-view-limits) avsnitt i [Resursplanering - visningsbegränsningar](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

* Projekten listas under användarens namn i samma prioritetsordning som de listas i projektvyn.\
   Mer information om projektprioritet i Resursplanering finns i [Projektplaneringsprioritet](#project-planning-priority) i den här artikeln.

* Om användarna inte har någon associerad jobbroll visas timvärdena eller FTE-värdena under **Ingen roll** -avsnitt.
* När den här vyn används läggs projekttimmar eller FTE till i användartimmar eller FTE.

   >[!TIP]
   >
   >Du kan inte visa allokeringen och tillgängligheten för användarna per kostnad i användarvyn.

* Dina behörigheter till projekt och uppgifter avgör vad som visas under namnen på de användare som visas i användarvyn.\
   Följande scenarier finns:

   * När du inte har behörighet att visa projekt och de uppgifter eller problem som är tilldelade användarna visas i resursplaneraren, visas dessa objekt under **Otillgängliga objekt** -avsnitt. The **Otillgängliga objekt** -avsnitten ersätter projekt- eller uppgiftsavsnitten i det här fallet.

   * När du inte har behörighet att visa projekten, men du har tillgång till uppgifterna eller problemen i projekten, visas projekten, aktiviteterna och problemen under namnen på de användare som tilldelats dem.
   * När du har behörighet att visa projekten, men inte några uppgifter eller problem i projekten, visas projektnamnet och aktiviteterna och problemen listas under **Otillgängliga objekt** -avsnitt.\
      Mer information om behörigheter i Workfront finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

      ![](assets/inaccessible-items-in-rp-with---column-and-red-outline--1--350x187.png)
    

* Du kan visa följande timma- och FTE-information i användarvyn:

   * Tillgänglig
   * Planerad
   * Faktisk
   * Skillnad mellan planerad och faktisk
   * Procentandel av planerad allokering

      Mer information finns i [Visa tillgängliga, planerade och faktiska timmar eller FTE i resursplaneraren när du använder användarvyn](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)

## Projektnamn

![](assets/project-name-highlighted-resource-planner-350x445.png)

Följande projekt visas i resursplaneraren:

* Projekt som du har behörighet att åtminstone visa.

   Du måste också ha tillgång till minst Visa resurshantering på din åtkomstnivå.

   Mer information om åtkomst som krävs för att använda resursplaneraren finns i [Tillgång till budgetresurser i Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Projekt som begränsas av filtret som används i resursplaneraren.

   Mer information om filtrering av information i resursplaneraren finns i [Filtrera information i resursplaneraren](../../resource-mgmt/resource-planning/filter-resource-planner.md).

   >[!NOTE]
   >
   >Vi rekommenderar att du använder filter för att minska antalet projekt som visas i resursplaneraren.

## Projektplaneringsprioritet {#project-planning-priority}

Projekt listas i prioritetsordning i resursplaneraren med det viktigaste projektet överst. Prioriteten anges med ett nummer framför projektnamnet.

![](assets/rp-planner-priority-highlighted-350x186.png)

Du kan även aktivera en inställning för att visa projektprioriteter utifrån deras portföljer när de är kopplade till en portfölj. Mer information om hur du prioriterar projekt och visar portföljprioriteringar i resursplaneraren finns i [Prioritera projekt i resursplaneraren](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

## Namn på jobbroll

![](assets/role-highlighted-resource-planner-350x243.png)

Följande kategorier av jobbroller visas i resursplaneraren:

* Jobbrollerna som tilldelas aktiviteter.
* De jobbroller som inte har tilldelats aktiviteter, men som är de primära jobbrollerna för användarna som är kopplade till projektens resurspooler.
* De sekundära jobbrollerna för användare som är tilldelade till uppgifter i de jobbrollerna.
* De sekundära jobbrollerna för användare som har en giltig **Procent tillgängliga heltidsanställda** i sin profil.\
   Mer information om **Procent tillgängliga heltidsanställda** för jobbroller, se [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) .

>[!NOTE]
>
>Jobbroller som tilldelats ärenden visas också när **Inkludera timmar från utleverans** inställningen är aktiverad. Mer information om hur du aktiverar utgivningstimmar i Resursplaneraren finns i [Inställningar](#settings) -avsnitt.

## Användarnamn

![](assets/user-highlighted-resource-planner-350x272.png)

De användare som visas i projekt- och rollvyerna i resursplaneraren tillhör de resurspooler som är associerade med projekten.\
Mer information om hur du fyller i resurspooler med användare finns i [Associera resurspooler med användare](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

Alla användare som du har åtkomst till Visa och som har loggat in på Workfront minst en gång visas i användarvyn.

I projekt- och rollvyerna kan användare visas i listan under följande typer av jobbroller:

* Deras primära roll
* Deras sekundära jobbroll i följande scenarier:

   * Om den sekundära jobbrollen har ett giltigt nummer för **Procent tillgängliga heltidsanställda** i användarprofilen.
   * Om användaren är tilldelad aktiviteter i dessa roller.

Mer information om **Procent tillgängliga heltidsanställda** för en jobbroll, se [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) .

## Avsnitten &quot;Ingen roll&quot; och &quot;Ingen användare&quot;

* [Avsnittet &quot;Ingen roll&quot;](#no-role-section)
* [Avsnittet &quot;Ingen användare&quot;](#no-user-section)

### Avsnittet &quot;Ingen roll&quot;  {#no-role-section}

När en användare tillhör en resurspool som är associerad med ett projekt, men inte har någon jobbroll associerad med dem, visas de i **Ingen roll** i stället för under en specifik jobbroll.

Du kan inte budgetera timmar för en användare i en **Ingen roll** -avsnitt. Användaren måste ha minst en associerad jobbroll för att kunna budgeteras för arbete.\
![no_role_with_user__res_planner.png](assets/no-role-with-user---res-planner-350x165.png)

### Avsnittet &quot;Ingen användare&quot;  {#no-user-section}

När du tilldelar en uppgift till ett team, eller låter den vara otilldelad, visas de planerade timmarna under **Ingen användare** som visas under **Ingen roll** i resursplaneraren. Dessa uppgifter visas inte i resursplaneraren när du använder **Visa efter användare** vy.

Du kan se hur många planerade timmar som tilldelats aktiviteter i projektet i **Ingen användare** i resursplaneraren, men du kan inte budgetera för dessa allokeringar.

![no_user_and_no_role___res_planner.png](assets/no-user-and-no-role---res-planner-350x129.png)

 

## Filter

Med filter kan du begränsa den information som visas i resursplaneraren.

![RP_filter_komprimerad.png](assets/rp-filter-collapsed-350x112.png)

Mer information om filtrering i resursplaneraren finns i [Filtrera information i resursplaneraren](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

## Inställningar {#settings}

I området Inställningar kan du aktivera eller inaktivera alternativ för att visa eller dölja information i resursplaneraren.

Så här aktiverar du inställningar i resursplaneraren:

1. Öppna resursplaneraren.
1. Klicka på **Inställningar** ikon.

   ![](assets/rp-settings-icon-edit-1.png)

   Rutan Resursplaneringsinställningar visas.

   ![](assets/rp-settings-without-actual-hours-350x211.png)

1. Aktivera **Inkludera timmar från ärenden** om du vill visa Planerade timmar från problem i resursplaneraren. Den här inställningen är inaktiverad som standard.

   Tänk på följande när du aktiverar den här inställningen:

   * Namnet på den användare som är tilldelad problemen visas under den jobbroll som är associerad med dem i utgåvan och du kan ange budgeterade timmar för användaren och jobbrollen i projekt- och rollvyerna.
   * De problem som användarna tilldelas visas under namnen på jobbrollerna i användarvyn.

      >[!IMPORTANT]
      >
      >**När de planerade start- och slutförandedatumen för utgåvan ligger utanför tidslinjen för projektet visas de planerade timmarna för utgåvan enligt datumet för utgåvan. Om projekttidslinjen till exempel är mellan januari och mars, men tidslinjen för problemen är i augusti, visas de planerade timmarna för utgåvorna under tidsperioden i augusti.**

1. (Villkorligt och valfritt) Om du har valt projektvyn aktiverar du inställningen Visa Portfolio-prioriteter så att projektprioriteterna visas enligt Portfolio. Projektens prioritet enligt portföljerna visas bredvid resursplaneringsprioriteten. Den här inställningen är inaktiverad som standard.

   Mer information om hur du prioriterar projekt i resursplaneraren finns i [Prioritera projekt i resursplaneraren](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

## Helskärmsalternativ

Du kan visa resursplaneraren i helskärmsläge för att förstora mängden information som du kan visa på skärmen.

Alternativet att visa information i helskärmsläge är tillgängligt för alla vyer av resursplaneraren.

Så här visar du resursplaneraren i helskärmsläge:

1. Gå till **Resursplanering**.
1. Klicka på **Helskärmsikon** om du vill visa resursplaneraren i helskärmsläge.\
   ![RP_sull_sccreen_area_User_View__1_.png](assets/rp-full-screen-icon-highlighted-user-view--350x260.png)\
   Resursplaneraren utökas så att hela webbläsarfönstret visas och ikonen ändras till en **Stäng helskärmsläget** visningsalternativ.

1. (Valfritt) Klicka på **Stäng helskärmsikonen** för att återgå till föregående visning.

## Exportalternativ

![](assets/export-button-highlighted-resource-planner-350x92.png)

Du kan exportera information till en Excel-fil (.xlsx) från valfri vy i resursplaneraren.\
Mer information om hur du exporterar information från resursplaneraren finns i [Exportera information från resursplaneraren](../../resource-mgmt/resource-planning/export-resource-planner.md).

Du kan hantera mängden information och visningen av den exporterade filen.\
Information om vilken information du kan exportera från Resursplanering och hur du hanterar utseendet på den exporterade filen finns i [Resursplanering - visningsbegränsningar](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).
