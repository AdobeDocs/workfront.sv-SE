---
product-area: projects
navigation-topic: create-tasks
title: Skapa aktivitetsöversikt
description: Du kan bara skapa uppgifter i ett projekt efter att du har skapat projektet.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Skapa uppgiftsöversikt

Du kan bara skapa uppgifter i ett projekt efter att du har skapat projektet.

När du har skapat ett projekt kanske du vill lägga till uppgifter och ändra dem för att ordna projektplanen. Mer information om hur du skapar ett projekt finns i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md). Mer information om hur du skapar uppgifter finns i [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

I den här artikeln beskrivs överväganden, begränsningar och standardinställningar som gäller när du skapar uppgifter.

## Olika sätt att skapa uppgifter i ett projekt

Du kan skapa uppgifter i ett projekt på följande sätt:

* Från grunden, enligt beskrivningen i [Skapa aktiviteter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Kopiera uppgifter till samma projekt eller till ett nytt projekt eller duplicera uppgifter i samma projekt, enligt beskrivningen i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Flytta aktiviteter från ett projekt till ett annat enligt beskrivningen i [Flytta aktiviteter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Begränsningar för att skapa uppgifter

När du har rätt behörighet och behörighet kan du skapa uppgifter i ett projekt. I följande fall kanske du inte kan skapa uppgifter:

* Din Adobe Workfront-administratör eller en gruppadministratör måste aktivera möjligheten att lägga till uppgifter i ett projekt som har statusen Slutfört eller Borttaget i området Projektinställningar. Mer information om hur du anger projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Du kan inte lägga till uppgifter i ett projekt som väntar på godkännande.

## Högsta tillåtna antal uppgifter för ett projekt

Ett projekt kan innehålla upp till 5 000 uppgifter. Ett varningsmeddelande visas i projektet när du närmar dig gränsen, när du har nått gränsen och om du försöker att överskrida gränsen.

Beroende på antalet uppgifter i dina projekt när den här begränsningen infördes, kan din Workfront-instans tillåta mer än 5 000 uppgifter i ett enda projekt.

Om du kan ta med mer än 5 000 uppgifter i ett och samma projekt bör du tänka på följande:

* Uppgiftsgränsen för din Workfront-miljö är det aktuella antalet uppgifter i ditt största projekt plus ytterligare 10 %.

  Om ett projekt i din Workfront-instans till exempel innehåller 10 000 uppgifter är gränsen för varje projekt i hela Workfront-instansen 11 000 uppgifter.

* Mindre projekt förbättrar resultatet och minimerar de hanteringsproblem som medföljer stora projekt.

## Som standard för uppgifter när du lägger till uppgifter i ett projekt

Det finns två typer av standardinformation som Workfront automatiskt uppdaterar för uppgifter när du skapar dem:

* Standardinformation på systemnivå

  Workfront-administratören eller en gruppadministratör fastställer standardinställningarna på systemnivå för uppgifter i området Åtgärder och problem i projektinställningarna. Mer information om inställningar för aktiviteter och problem finns i [Konfigurera inställningar för aktiviteter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) eller [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Standardinformation på projektnivå

  I resten av det här avsnittet beskrivs de standardinställningar på projektnivå som du som projektledare kan definiera för alla nya uppgifter som läggs till i ett projekt

När du lägger till en uppgift i ett projekt kan Workfront automatiskt bifoga en godkännandeprocess eller anpassade formulär till uppgiften, beroende på hur projektet är konfigurerat.

Mer information om hur du konfigurerar ett projekt att lägga till dessa som standard finns i avsnittet Åtgärder i artikeln [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md) .

När du definierar standardinformation som ska kopplas till uppgifter som lagts till i ett projekt på projektnivå bör du tänka på följande:

* Du måste ha behörigheten Hantera i projektet för att definiera standardinställningarna för uppgiftsgodkännandeprocessen och anpassade formulär.
* Alla nya åtgärder skapas med godkännandeprocessen och de anpassade formulär som definieras när projektet redigeras.
* Du kan ändra standardinställningarna när du lägger till uppgifter med rutan Redigera uppgift, men inte när du lägger till uppgifter i en intern redigering.
* Du kan definiera godkännandeprocessen och de anpassade formulären för uppgifter i en mall.

   * När ett projekt skapas från den här mallen tillämpas godkännandeprocessen och anpassade formulär automatiskt på projektet.
   * När en mall bifogas till ett befintligt projekt bevarar projektet den ursprungliga godkännandeprocessen och anpassade formulärinställningar om de har definierats. Om de inte är definierade blir inställningarna från mallen inställningarna för projektet.
   * När en mall bifogas till ett befintligt projekt behåller de uppgifter som lagts till i projektet från mallen godkännandeprocessen och anpassade formulärinställningar som de hade i mallen, oavsett projektets aktivitetsinställningar.

  Mer information om hur du bifogar en mall till ett projekt finns i [Koppla en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* När du kopierar projektet överförs uppgiftens standardinställningar till det nya projektet.

  Mer information om hur du kopierar ett projekt finns i [Kopiera ett projekt](../../../manage-work/projects/manage-projects/copy-project.md).

* När du kopierar uppgifter från ett projekt till ett annat och målprojektet har olika standardinställningar för uppgifter, behåller de kopierade uppgifterna standardinställningarna från det ursprungliga projektet, såvida de inte rensas i kopieringsprocessen.
* När du duplicerar en uppgift i samma projekt överförs de anpassade formulären och godkännandeprocessen till den duplicerade uppgiften.

  Mer information om att kopiera och duplicera uppgifter finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* När du flyttar aktiviteten till ett annat projekt sparas standardinställningarna för aktiviteten på aktiviteterna från det ursprungliga projektet, oavsett standardinställningarna för aktiviteten i det nya projektet.

  Mer information om att flytta uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md).
