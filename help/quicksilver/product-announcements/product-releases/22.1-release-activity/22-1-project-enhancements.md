---
title: 2.1 Projektförbättringar
description: 2.1 Projektförbättringar
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 0%

---

# 2.1 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts i version 2.1 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

veckan 17 januari 2022.

En lista över alla ändringar som är tillgängliga i version 2.1 finns i [2.1 Versionsöversikt](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Ändra standardalternativet för föregående aktiviteter när uppgifter kopieras eller flyttas

För att minimera antalet manuella steg när du kopierar eller flyttar uppgifter har vi uppdaterat informationen som kopieras eller flyttas med uppgiften som standard. Nu kopieras eller flyttas alla föregångare med uppgiften som standard, eftersom alternativet Alla föregående användare är markerat som standard.

Före den här förbättringen avmarkerades alternativet Alla föregående som standard när en uppgift kopierades eller flyttades.

Mer information finns i artiklarna:

* [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## Uppdaterat verktygsfält i instrumentpanelslistan och rapporter i instrumentpaneler

Verktygsfältet på fyra kontrollpanelssidor har nu ett modernt utseende som matchar andra Workfront-listor som projekt, uppgifter och problem. Det här intuitiva verktygsfältet gör det nu enklare att lägga till, redigera, dela, kopiera och ta bort kontrollpaneler.

Sidorna med det uppdaterade verktygsfältet är:

* Uppgiftsrapporter (visas på kontrollpaneler)
* Alla instrumentpanelslistor
* Min instrumentpanelslista
* Lista med delade instrumentpaneler

Mer information finns i [Skapa och hantera instrumentpaneler](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Lägga till och redigera en anpassad formulärsammanfattningspanel för dokument

Nu kan du lägga till och redigera anpassade formulär direkt i dokumentsammanfattningspanelen.

Med den här ändringen får du också ett nytt utseende och en ny känsla i dokumentsammanfattningen. Det finns ett nytt avsnitt, Översikt, som innehåller både miniatyrbilden och dokumentinformationen. Du kan även checka in och ut dokument i dokumentinformationsavsnittet.

Tidigare var du tvungen att gå till fliken Egna formulär i Dokumentinformation för att göra ändringar eller lägga till anpassade formulär.

Mer information finns i [Sammanfattning för dokumentöversikt](../../../documents/managing-documents/summary-for-documents.md).

## Ny upplevelse vid kopiering av en eller flera uppgifter

För att få din användning av Workfront att överensstämma med den nya Adobe Workfront-upplevelsen har vi omdesignat gränssnittet när du kopierar en uppgift. Detta är för närvarande tillgängligt när du kopierar en uppgift på aktivitetsnivå eller kopierar en uppgift eller flera uppgifter i en lista.

Några av förbättringarna är:

* All information som du måste uppdatera innan du kopierar uppgiften visas på en kontinuerlig sida.
* Workfront kontrollerar om du har åtkomst till målprojektet direkt efter att du har valt projektet. Före den här förbättringen visades ett varningsmeddelande om att du inte har rätt åtkomst när du har bekräftat kopian, vilket resulterade i extra steg och att kopian inte tillåts.
* Möjlighet att begära åtkomst till ett projekt där du vill kopiera uppgiften utan att lämna rutan Kopiera uppgift.

Mer information finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Ny upplevelse när du flyttar en eller flera uppgifter från en lista

För att ge en konsekvent upplevelse när vi utför samma uppgift har vi nu uppdaterat gränssnittet för att flytta en eller flera uppgifter från en lista så att de matchar upplevelsen när aktiviteten flyttas på aktivitetsnivå. (Vi har uppdaterat upplevelsen av att flytta en uppgift på aktivitetsnivå i en tidigare förhandsversion.)

Mer information finns i [Flytta aktiviteter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Ny upplevelse när en uppgift flyttas på aktivitetsnivå

För att få din användning av Workfront att överensstämma med den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att flytta en uppgift. Detta är för närvarande tillgängligt när du flyttar en uppgift på aktivitetsnivå. I nästa version kommer vi att utöka den här designen till att flytta en uppgift från en lista.

Några av förbättringarna i det nya gränssnittet:

* All information som du måste uppdatera innan flytten visas på en kontinuerlig sida.
* Workfront kontrollerar om du har åtkomst till målprojektet direkt efter att du har valt projektet. Före den här förbättringen varnade Workfront dig för att du inte har rätt åtkomst efter att du har bekräftat flytten som resulterade i extra steg och flytten inte tillåts.
* Möjlighet att begära åtkomst till ett projekt där du vill flytta uppgiften utan att lämna rutan Flytta uppgift.

Mer information finns i [Flytta aktiviteter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Ny upplevelse vid konvertering av ett ärende till ett projekt med hjälp av en mall på problemnivå

>[!NOTE]
>
>Den här funktionen togs tillfälligt bort från produktionsmiljön den 4 mars 2022. Den släpptes senare i en fasad utrullning från den 28 april 2022. Utbyggnaden slutfördes den 5 maj 2022. Det här är nu tillgängligt i Förhandsgranska och produktion för alla kunder. (De senaste uppdateringarna av status för den här funktionsreleasen i Produktion finns i [2.3 Versionsöversikt](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

För att få din användning av Workfront att överensstämma med den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att konvertera ett problem till ett projekt när du använder en mall när du konverterar det från problemsidan.

Nu är det enklare att komma åt din lista med favoriter direkt efter att du har valt att konvertera utgåvan.

Det omdesignade gränssnittet matchar upplevelsen när du skapar ett projekt från en mall som vi också har uppdaterat nyligen.

Mer information finns i [Konvertera ett problem till ett projekt](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Konvertera ärenden till projekt med en mall från listor, rapporter och kontrollpaneler

>[!NOTE]
>
>Den här funktionen togs tillfälligt bort från produktionsmiljön den 4 mars 2022. Den släpptes senare i en fasad utrullning från den 28 april 2022. Utbyggnaden slutfördes den 5 maj 2022. Det här är nu tillgängligt i Förhandsgranska och produktion för alla kunder. (De senaste uppdateringarna av status för den här funktionsreleasen i Produktion finns i [2.3 Versionsöversikt](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

För att effektivisera arbetet och göra det enklare för dig att konvertera utgåvor i en snabbpaketerad miljö har vi lagt till möjligheten att konvertera ett problem till ett projekt med hjälp av en mall från en lista, rapport eller en kontrollpanel.

Före den här förbättringen fanns den här funktionen bara när du konverterade problemet från sidan med utgåvor.

Mer information finns i [Konvertera ett problem till ett projekt i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Filtrera efter användarlista på flexibla anslagstavlor visar användare med de flesta tilldelningar först

>[!NOTE]
>
>Den här funktionen ingår inte i version 22.1. Den togs bort från förhandsvisningsmiljön.

Nu visar filtret de användare som har de flesta uppdrag först så att de blir lättare att hitta utan att bläddra igenom listan.

Tidigare visades listan för filtrering efter användare på både Kanban- och Scrum-tavlor i alfabetisk ordning.

Mer information finns i följande information

* [Filtrera efter användare på Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [Filtrera efter användare på Kanban-tavlan](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Begränsa möjligheten att lägga till dokument i en mall som du delar

Ibland lägger man till dokument i en projektmall som tror att de läggs till i ett projekt. Nu kan du förhindra detta - när du delar en mall med Visa-åtkomst kan du inaktivera den nya avancerade inställningen Lägg till dokument. Detta gör att mottagarna inte kan lägga till dokument i mallen.

Instruktioner om hur du delar en mall finns i [Dela projektmallar](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

Mer information om den nya avancerade inställningen Lägg till dokument finns i avsnittet i artikeln [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Dela en dokumentmapp

Nu kan du dela en dokumentmapp och dess innehåll från området Dokument. Tidigare var detta inte möjligt - du var tvungen att dela varje dokument i en mapp separat.

Mer information finns i [Dela en dokumentmapp](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

