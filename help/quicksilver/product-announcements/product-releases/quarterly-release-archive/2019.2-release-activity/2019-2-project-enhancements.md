---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2 Projektförbättringar
description: Den här sidan beskriver alla projektförbättringar som ingår i version 2019.2. Funktionen planeras bli tillgänglig i produktionsmiljön den 20 maj 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# 2019.2 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som ingår i version 2019.2. Funktionen planeras bli tillgänglig i produktionsmiljön den 20 maj 2019.

En lista över alla ändringar som gjorts under 2019.2 finns i [2019.2 Release Activity Overview](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Hitta grupper snabbare när du anpassar statusvärden

Den nedrullningsbara menyn på fliken Status i inställningsområdet är nu en huvudmeny. På så sätt kan du snabbt söka efter och hitta valfri grupp i systemet, vilket gör det enklare att anpassa statusen.

Tidigare visade listrutan ett begränsat antal grupper. Om gruppen som du ville visa inte visades var du tvungen att navigera till Inställningar > Grupper och hitta den specifika gruppen för att kunna anpassa gruppens status.

Mer information finns i [Skapa eller redigera en status](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Koppla standardprocesser för anpassade Forms och godkännanden till aktiviteter

Nu kan du konfigurera anpassade formulär och godkännandeprocesser som ska bifogas till uppgifter när du lägger till uppgifter i ett projekt. Du kan konfigurera standardinställningarna på projektnivå.

Mer information om hur du konfigurerar anpassade standardformulär och godkännandeprocesser för uppgifter på projektnivå finns i avsnittet Åtgärder i artikeln [Redigera projekt](../../../../manage-work/projects/manage-projects/edit-projects.md).

## Visa hela raden för en överordnad aktivitet i fetstil i en uppgiftslista

I en uppgiftslista visas raden som innehåller en överordnad uppgift i fetstil. Den här ändringen är synlig när listan sorteras efter arbetsfördelningsstrukturen eller efter aktivitetsnumret i stigande ordning.

## Invertera ändringar i uppgiftslistor

Med en ny Spara automatiskt-knapp i uppgiftslistan kan du välja om du vill att de ändringar du gör ska sparas automatiskt eller om du vill se vilka effekter ändringarna ger innan du sparar dem. Den här inställningen gäller både för uppgiftslistan och Gantt-diagrammet.

Före den här förbättringen har alla ändringar alltid sparats automatiskt.

Mer information om hur du redigerar uppgifter i en uppgiftslista finns i [Redigera uppgifter](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Mer information om hur du redigerar uppgifter i Gantt-schemat finns i [Uppdatera information i Gantt-schemat för uppgiftslistor](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Standardvärden för ny kolumnbredd i nya listor

Nu justerar Workfront automatiskt kolumnbredden enligt värdeformatinformationen i varje kolumn. Kolumner som visar ett tal är till exempel bredare än de som visar fältet Beskrivning.

Före den här förbättringen ställdes kolumnbredderna i det nya projektet och i uppgiftsvyn in på 100 pixlar, om inget annat anges.

Mer information om kolumnbredder finns i [Ändra kolumnbredd och -ordning](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Inaktivera oanvända objekt

>[!NOTE]
>
>Den här funktionen släpptes direkt till produktionsmiljön under 2019.2-förhandsgranskningen.

Om du har objekt som inte längre används kan du nu inaktivera dem för att dölja dem från listor, så att användare inte kan associera dem med andra objekt.

När du nu redigerar något av objekten nedan kan du ange om de ska vara aktiva. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt. Objekt som inte är inställda på Aktiv visas inte i rullgardinsmenyer och textframåt-fält som ska kopplas till andra objekt.

* Godkännandeprocesser
* Företag
* Anpassad Forms
* Milstolpbanor
* Portfolio
* Program
* Mallar

Allt du inaktiverar som används fortsätter att fungera som det alltid har gjort och tas inte bort eller blockeras.

>[!IMPORTANT]
>
>När du skapar dessa objekt via Workfront API är standardvärdet för parametern&quot;isActive&quot; true. Detta är ett nytt fält för alla objekt och är inte tillgängligt för redigering före version 11 av API:t. Det här fältet fanns tidigare för Portfolio, förutom att standardvärdet var false. Det kommer att ändras till standardvärdet true med början från version 11 av API:t.

## Visa BCWS (Budgeted Cost of Work Scheduled) och BCWP (Performed) i Vyer

Du kan nu visa BCWS (Budgeted Cost of Work Scheduled) och BCWP (Budgeted Cost of Work Performed) i projekt- och uppgiftsvyer.

Även om dessa projektresultatvärden användes vid finansiella beräkningar i Workfront tidigare, var de inte synliga i systemet före den här förbättringen.

Mer information om hur du beräknar BCWS finns i [Beräkna budgeterad kostnad för schemalagt arbete (BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Mer information om hur du beräknar BCWP finns i [Beräkna budgeterad kostnad för utfört arbete (BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

