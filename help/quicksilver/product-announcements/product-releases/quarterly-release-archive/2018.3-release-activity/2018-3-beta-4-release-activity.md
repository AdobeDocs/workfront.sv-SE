---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 4 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.3 Beta 4. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 30 augusti 2018. Den kommer att göras tillgänglig i produktionsmiljön i november 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b40eda2c-8ad4-4945-a7e3-cb28ed8a14db
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 0%

---

# 2018.3 Beta 4 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.3 Beta 4. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 30 augusti 2018. Den kommer att göras tillgänglig i produktionsmiljön i november 2018.

En lista över alla ändringar som gjorts under 2018.3 finns på  [Aktivitetsöversikt för version 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

2018.3 Beta 4 innehåller förbättringar både för Workfront-administratörer och andra användare:

**För administratörer**

* [Uppdatera rapporteringsstrukturen i användarprofilen som gruppadministratör](#update-reporting-structure-in-the-user-profile-as-a-group-administrator) 

**För alla användare**

* [Exportera mer information från resursplaneraren](#export-more-information-from-the-resource-planner)
* [Förbättringar av uppgiftslistan](#task-list-improvements) har tagits bort från versionen
* [Förbättringar av projektlista](#project-list-improvements)
* [Redigera uppgiftslistan i Gantt-schemats redigeringsläge](#editing-the-task-list-in-gantt-chart-edit-mode) Borttagen från release
* [Mätningsverktygets färger](#measurement-tool-colors)
* [Korrektur öppna på en ny flik](#proofs-open-in-a-new-tab) Borttagen från release

* [Förbättringar av utskriftssammanfattning](#print-summary-enhancements)
* [Logga tid i dagar i Workfront Mobile App](#log-time-in-days-in-the-workfront-mobile-app)

## Uppdatera rapporteringsstrukturen i användarprofilen som gruppadministratör {#update-reporting-structure-in-the-user-profile-as-a-group-administrator}

Gruppadministratörer kan nu redigera fälten Direktrapporter och Rapporter till för användare i de grupper de administrerar.

Tidigare var det bara Workfront administratörer och användare med administrativ åtkomst till användare som hade denna möjlighet.

Mer information om gruppadministratörer finns i [Gruppadministratörer](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Exportera mer information från resursplaneraren {#export-more-information-from-the-resource-planner}

Du kan nu exportera information från upp till 52 veckor, 36 månader eller 12 kvartal i resursplaneraren. Om den mängd information du exporterar är för stor får du ett e-postmeddelande med den exporterade filen bifogad. Du kan hämta filen i upp till en vecka från det att hämtningen startades.

Tidigare kunde du bara exportera upp till högst fyra veckor, månader eller kvartal i taget.

Mer information finns i [Exportera information från resursplaneraren](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Förbättringar av uppgiftslistan {#task-list-improvements}

>[!NOTE]
>
>* Den här funktionen har tagits bort från förhandsvisningsmiljön och kommer inte att inkluderas i version 2018.3. Den kommer att släppas vid en senare tidpunkt.

En ny upplevelse är nu tillgänglig när du visar en lista över uppgifter. Den här upplevelsen innebär bättre prestanda och smidigare och snabbare navigering i listor.

Följande synliga ändringar är också tillgängliga:

* Grupperingar komprimeras som standard.\
  Före den här ändringen expanderades grupperingarna som standard.
* Snabbfilter har lagts till i uppgiftslistan.
* Projekthuvudet förblir synligt när du bläddrar nedåt i uppgiftslistan.
* Nya statusikoner är tillgängliga.

Följande funktioner har ändrats i uppgiftslistor:

* Möjlighet att högerklicka och den snabbmeny som den tillhandahåller.\
  I stället för att högerklicka på uppgifter för att redigera dem kan du göra följande:

   * När du markerar en enskild åtgärd kan du nu använda menyn Mer med samma alternativ som den föregående högerklicksmenyn.
   * När du markerar flera uppgifter kan du använda ikonerna längst upp i listan för att utföra någon av de åtgärder som ingår i den föregående högerklicksmenyn.

     Alla ändringar visas i uppgiftslistorna i projekt, samt på fliken Underuppgifter under uppgifter.

Mer information om hur du arbetar i listor finns i [Kom igång med listor i Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Mer information om att kedja aktiviteter i Gantt-schemat finns i [Skapa föregående relationer genom att kedja aktiviteter](../../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).

## Förbättringar av projektlista {#project-list-improvements}

Möjligheten att sortera om kolumner har lagts till i en lista med projekt på följande underflikar:

* Projekt jag äger
* Projekt som jag är på
* Alla projekt

Den här funktionen togs bort i version 2018.2.

Mer information om hur du arbetar i listor finns i [Kom igång med listor i Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Redigera uppgiftslistan i Gantt-schemats redigeringsläge {#editing-the-task-list-in-gantt-chart-edit-mode}

>[!NOTE]
>
>* Den här funktionen har tagits bort från förhandsvisningsmiljön och kommer inte att inkluderas i version 2018.3. Den kommer att släppas vid en senare tidpunkt.

Du kan nu utföra följande åtgärder för uppgifter i ett projekt när de visas i redigeringsläget i Gantt-schemat:

* Lägga till uppgifter
* Ta bort uppgifter
* Inline-redigeringsuppgifter

Även om du kan se hur ändringarna påverkar tidslinjen i projektet är ändringarna inte omedelbara. Du kan spara dem för att uppdatera projekttidslinjen eller avbryta dem.

Tidigare kunde du inte utföra dessa åtgärder på uppgifter när de visades i redigeringsläget i Gantt-diagrammet. Du kan göra dessa ändringar i en uppgiftslista som inte visades i Gantt-diagrammet, men som gjordes direkt.

Mer information om hur du redigerar uppgifter i Gantt-schemat finns i [Uppdatera information i Gantt-schemat för uppgiftslistor](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Mätningsverktygets färger {#measurement-tool-colors}

När du mäter områden i ett korrektur med mätverktyget kan du nu ändra verktygets färg och opacitet. Workfront kommer ihåg dessa inställningar i alla korrektur som du öppnar tills du tömmer webbläsarcachen.

Standardfärgen är nu röd.

Tidigare visades mätverktyget endast i blått, vilket gjorde det svårt att se på korrekturinnehåll som innehåller liknande nyanser av blått.

## Öppna korrektur på en ny flik {#proofs-open-in-a-new-tab}

>[!NOTE]
>
>* Den här funktionen har tagits bort från förhandsvisningsmiljön och kommer inte att ingå i version 2018.3.

När du öppnar ett korrektur var som helst i Workfront eller Workfront Proof öppnas korrekturläsaren nu på en ny flik i webbläsaren och fokus växlar till den fliken. Du kan arbeta i flera webbläsarflikar, granska korrektur och fortsätta arbeta med projekt, uppgifter och problem i Workfront eller Workfront Proof.

Tidigare startades korrekturläsaren i en bildruta ovanpå den aktuella webbläsarfliken i Workfront eller Workfront Proof, vilket gjorde den fliken otillgänglig tills du stängde korrekturläsaren.

Mer information finns i .

## Förbättringar av utskriftssammanfattning {#print-summary-enhancements}

Följande förbättringar är nu tillgängliga på utskriftssammanfattningssidan när du skriver ut ett korrektur eller sparar det som en PDF- eller XLS-fil:

* Du kan sortera korrekturens kommentarer efter vem som skapat dem.

  Tidigare kunde du sortera kommentarerna i den ordning de skapades eller i vilken ordning de visades på varje sida.

* Du kan filtrera korrekturens kommentarer efter författare, åtgärd och olöst status.

  Tidigare var kommentarfiltrering inte tillgängligt på sidan för utskriftssammanfattning.

* Nu ingår faser tillsammans med information om varje fas.

  Tidigare inkluderades inte faser.

Mer information finns i [Skriva ut en korrektursammanfattning i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

## Logga tid i dagar i Workfront Mobile App {#log-time-in-days-in-the-workfront-mobile-app}

Nu kan du logga tid i dagar i Workfront mobilapp. 

Tidigare kunde du bara logga tid med timmar i mobilappen, även när din profilinställning var inställd på att logga tid i dagar.

Mer information om loggningstid i mobilappen finns i . 

Den här funktionen är omedelbart tillgänglig för testning med Android Beta. 
