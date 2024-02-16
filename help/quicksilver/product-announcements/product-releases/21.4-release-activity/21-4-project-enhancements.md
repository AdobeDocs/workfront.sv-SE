---
title: 21.4 Projektförbättringar
description: 21.4 Projektförbättringar
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 0%

---

# 21.4 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts i version 21.4 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 4 oktober 2021.

En lista över alla ändringar som är tillgängliga i version 21.4 finns i [21.4 Versionsöversikt](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Inkludera bilder i uppdateringar

På fliken Uppdateringar för ett objekt kan du nu lägga till bilder genom att klicka på ikonen Bild i verktygsfältet. Du kan också dra och släppa en bild i uppdateringsområdet. Observera att Workfront-administratören måste aktivera bildtillägg innan du kan se bildikonen.

Du kan lägga till bilder i både uppdateringar och svar. En miniatyrbild i uppdateringen anger att mottagarna kan förhandsgranska bilden i webbläsaren eller hämta den, och e-post- och appmeddelanden visar att bilder är kopplade till uppdateringen.

Tidigare var det enda sättet att dela en bild i Workfront att bifoga den till ett objekt som ett dokument. Bilder som läggs till på fliken Uppdateringar är bara tillgängliga på den fliken och inte på fliken Dokument.

Mer information finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Innan Workfront-användare kan inkludera bilder i uppdateringar måste den här funktionen först aktiveras av Adobe Workfront-administratören enligt beskrivningen i [Konfigurera inställningar för användaruppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Uppdaterad algoritm för smarta tilldelning

Vi har förbättrat algoritmen som används för smarta tilldelningar. Med den nya förbättringen tittar Workfront på de 30 senaste uppdragen som gjorts av den inloggade användaren för att ge förslag när de tilldelar uppgifter och ärenden. Listan med förslag kan innehålla upp till 50 användare.

Före den här förbättringen övervägde Workfront tilldelningarna för de överordnade uppgifterna och andra användarattribut som är relaterade till tilldelningarna när de föreslog användare.

Mer information om smarta tilldelningar finns i [Översikt över smarta uppdrag](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Ny upplevelse när du skapar ett projekt från en mall

Vi har gjort om gränssnittet för att skapa ett projekt från en mall så att du kan använda Workfront på ett sätt som är förenligt med den nya Workfront-upplevelsen. Funktionen för att skapa ett projekt med en mall har inte ändrats. Några av förbättringarna i det nya gränssnittet är dock följande:

* Förhandsgranska mallinformation innan den bifogas
* Lägga till mallar i en lista med favoriter när projektet skapas

Vi har uppdaterat gränssnittet för att skapa projektet både när du skapar det från både projektet och mallområdet.

För information, [Skapa ett projekt med en mall](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Ny upplevelse när mallar bifogas till projekt

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

För att din användning av Workfront ska vara förenlig med den nya Workfront-upplevelsen har vi gjort om gränssnittet för att bifoga en mall till ett projekt. Funktionen för att bifoga en mall har inte ändrats. Det finns dock några förbättringar i det nya gränssnittet som innehåller följande:

* Förhandsgranska mallinformation innan den bifogas
* Lägga till mallar i en lista med favoriter under bilageprocessen
* Visa alla alternativ för att hantera mall- och projektinställningar på en sammanhängande sida

Mer information finns i [Bifoga en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Enhetliga värden för varaktighet och varaktighet för uppgifter

För en renare och mer strömlinjeformad användarupplevelse har värdet för fältet Varaktighet sammanfogats med tidsenheten. Före den här förbättringen visas tidsenheten i ett separat nedrullningsbart fält efter fältet Varaktighet.

Förutom varaktighetsfälten i rutorna Uppgiftsinformation, Redigera uppgifter och Ny uppgift uppdaterar vi även följande fält så att de matchar den här funktionen:

* Varaktighetsfält vid avancerade tilldelningar
* Fältet Nivåfördröjning när du skapar eller redigerar en uppgift
* Frekvensfält när en återkommande uppgift skapas (tillgängligt snart)
* Laga fält när en föregångare läggs till (tillgängligt snart)

Mer information finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Inaktivera infogning av fel i projekt

För att säkerställa att användarna ger korrekt information när de lägger till problem i projekt genom att fylla i ett utgivningsformulär har vi infört en ny inställning som gör att du kan hantera om de kan lägga till problem i ett projekt eller dess uppgifter internt. Den här inställningen är aktiverad som standard i området för nya inställningar för problem i rutan Redigera projekt. Om du inaktiverar det nedtonas alternativet Lägg till fler problem i avsnittet Problem i ett projekt så att användarna inte kan lägga till fler problem i listan. Användarna kan fortfarande lägga till problem i projekten genom att använda alternativet Nytt problem i avsnittet Problem eller genom att använda en frågekö om en sådan har konfigurerats för projektet.

>[!NOTE]
>
>Den här inställningen är bara tillgänglig i den nya Workfront-upplevelsen. Användare som arbetar i Workfront Classic kan fortfarande lägga till fel i ett projekt eller dess uppgifter, även om den här inställningen har inaktiverats för projektet av en användare som arbetar i den nya Workfront-upplevelsen.

Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

## Förbättrad anpassad fältvisning för kryssrutor och alternativknappar

Det har blivit enklare att visa och markera kryssrutor och alternativknappar i anpassade formulär - ett anpassat fält med många kryssrutor och alternativknappar visas nu i flera kolumner på sidan. Tidigare visades de i en enda kolumn, vilket krävde extra bläddring för användare som fyller i formuläret.

Detta beror på hur du placerar fälten i det anpassade formuläret. Om du placerar ett annat fält på samma rad med kryssrutan eller alternativknappsfältet kan det hända att alternativen bara har tillräckligt mycket vågrätt utrymme för att visas i en enda kolumn.

Mer information om hur du fyller i ett anpassat formulär finns i [Redigera information i anpassade formulärfält](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Mer information om hur du skapar en kryssruta eller ett alternativknappsfält i ett anpassat formulär finns i avsnitten [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) och [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) i artikeln [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

