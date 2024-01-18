---
title: projektuppdateringar under tidsramen för version 22.3
description: projektuppdateringar under tidsramen för version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# 2.3 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts i version 2.3 till förhandsvisningsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 juli 2022. En lista över alla ändringar som är tillgängliga i version 2.3 finns i [22.3 Versionsöversikt](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Utanför kontoret

Nu kan du tillfälligt delegera uppgifter och ärenden som tilldelats dig till andra användare när du planerar att vara utanför kontoret under en kort tid. På så sätt kan du vara säker på att din frånvaro inte blir ett hinder för arbetet.

Före den här förbättringen kunde du bara delegera godkännanden.

Nedan följer några av de funktioner som vi har lagt till i den här uppdateringen:

* En inställning i området Inställningar för uppgifter och problem i installationsprogrammet för system- eller gruppadministratören för att aktivera delegering i din miljö.

* Ett nytt alternativ för&quot;Delegera uppgifter och utgåvor&quot; på hemsidan för användare med en Review-licens eller en senare licens att delegera sina arbetsuppgifter.

* Indikation i Hem och i uppdragsområdet för uppgifter och utgivningsrubriker om att objekt har delegerats till andra.

* Händelsemeddelanden i inställningsområdet och e-postmeddelanden i användarprofilen för att styra e-postmeddelanden om delegerat arbete


>[!NOTE]
>
>Endast användare med en granskning eller en högre licens kan delegera sitt arbete till andra. Arbetet kan delegeras till alla användare, oavsett åtkomstnivå. Delegerade användare får samma behörigheter som tilldelningarna för de delegerade objekten. Om de här behörigheterna är lägre än en användares åtkomstnivåkonfiguration kan de delegerade användarna hindras från att utföra vissa av de aktiviteter som rör de uppgifter och problem som har delegerats till dem.


Mer information finns i [Översikt över delegeringsuppgifter och utgåvor](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Ny upplevelse vid konvertering av ett problem till en uppgift

För att få din användning av Workfront att överensstämma med den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att konvertera ett problem till en uppgift.

Uppdateringen innehåller:

* Ett uppdaterat användargränssnitt som matchar resten av Workfront.

* Åtkomst för att konvertera ett problem till aktiviteter från en lista eller rapport.

* Standardformulären som definieras i området Aktivitetsinställningar i målprojektet som läggs till i den nya uppgiften.


Mer information finns i [Konvertera ett problem till en uppgift i Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Ny upplevelse vid konvertering av ett ärende till ett projekt utan mall

För att er användning av Workfront ska vara förenlig med den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att konvertera ett problem till ett projekt utan att använda en mall.

Förutom ett uppdaterat användargränssnitt som matchar resten av den nya Workfront-upplevelsen har vi också lagt till möjligheten att konvertera ett problem till tomma projekt från en lista eller rapport.

Mer information finns i [Konvertera ett problem till ett projekt i Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Smart taggning i uppdateringsflödet

Vi har förbättrat taggningen av användare i uppdateringsströmmen när du skapar en ny uppdatering eller svarar på en befintlig uppdatering. När du taggar en användare så att den inkluderas i en uppdatering visas även användarens primära roll och e-postadress, förutom namnet och avataren. Detta gör det lättare att skilja mellan flera användare med liknande eller identiska namn.

Mer information finns i [Tagga andra för uppdateringar](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Ny syntax för beräkningar i anpassade fält

För att förbereda dig för framtida förbättringar som hjälper dig att lägga till beräkningar i anpassade formulär har vi standardiserat syntaxen för refererade fält som du lägger till i en beräkning. Det är enkelt att använda den nya syntaxen eftersom systemet anger den åt dig när du börjar skriva namnet på ett fält och sedan markerar det.

Mer information finns i avsnittet &quot;Bygg beräkningen för ditt beräknade anpassade fält&quot; i [artikel Lägga till beräknade data i ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Behåll korrekt information när två användare med en gemensam roll deltar i en godkännandeprocess

För att säkerställa att dina data för godkännande av arbete är korrekta har vi gjort en ändring i hur godkännandeinformation registreras för en artikel när en godkännandeprocess för flera roller är kopplad till artikeln.

Vissa godkännandeprocesser kräver godkännande från två olika roller, och två olika godkännare kan ha en av dessa gemensamma roller. När detta inträffar registrerar Workfront varje godkännare och deras respektive roll som är kopplad till godkännandeprocessen.

Före den här ändringen registrerades båda godkännandena för den andra användaren eftersom de delade en av godkännanderollerna med den första godkännaren. I det här fallet skrev den andra godkännaren över den första godkännarens information.

Mer information om godkännandeprocesser i Workfront finns i [Översikt över godkännandeprocessen](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Allokeringstider tas inte längre bort när du ändrar tilldelningar

>[!NOTE]
>
>Den här funktionen var ursprungligen planerad att lanseras med version 2.2. Den släpptes till produktion den 21 april 2022.


För att dina data ska bli korrekta har vi gjort en ändring som bevarar tilldelningstimmar och behåller planerad tid för aktiviteten oförändrad när du ändrar tilldelningar för aktiviteten.

Följande ändringar har gjorts för aktiviteter med en enkel varaktighetstyp:

* Planerade timmar bevaras när alla tilldelningar tas bort.

* Enskilda tilldelningar bevaras när användare och roller ersätts.

* Enskilda tilldelningar bevaras för rollen när användaren tas bort. (Borttagen från release. Planerade timmar anges till 0 när alla tilldelningar har tagits bort.)


Mer information om planerade timmar finns i [Översikt över planerade timmar](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Förbättringar av anslagstavlor

Följande förbättringar har lagts till i Adobe Workfront-ritytor:

* Filteralternativ - Du kan nu filtrera efter förfallodatum eller status på en anslagstavla. Filtret har också uppdaterats med fällningar som kan komprimeras för att separera alternativen.

* Arkivpanel - Nu kan du arkivera en panel medan du är på en panel, i stället för att behöva gå till panelens kontrollpanel.

* Lägg till ett team till en anslagstavla - När du söker efter medlemmar kan du lägga till ett helt team. Om du väljer ett team läggs alla i teamet till i styrelsen.

* Släppzoner i kolumner - När du drar och släpper ett kort från en kartkolumn till en annan visas nu en grå&quot;släppzon&quot; där kortet ska placeras. Tidigare fanns det ingen visuell indikator på kortplaceringen.

* Anslutna kort - Nu kan du lägga till kort som är anslutna till uppgifter och problem i Workfront. Om du uppdaterar namnet, beskrivningen eller tilldelaren på kortet eller uppgiften uppdateras samma fält på den andra platsen.

* Statusfält på alla kort - ett statusfält och en Markera som slutförd-knapp har lagts till både ad hoc-kort och anslutna kort. När du klickar på Markera som slutförd ändras statusen automatiskt till Fullständig.

* Konvertera ad hoc-kort till anslutet kort - Du kan nu välja att konvertera ett ad hoc-kort till ett anslutet kort från kortinformationen.

* Koppla från anslutet kort - Om du kopplar från ett anslutet kort bryts anslutningen till Workfront-objektet. Kortet förblir som ett särskilt kort och Workfront-objektet påverkas inte.

* Statusmappning i kolumner - Med nya kolumninställningar och -profiler kan du definiera status, tilldelad eller tagg som används för kort som flyttas till den kolumnen. Dessutom har standardkolumnnamnen på en ny anslagstavla ändrats till Kolumn 1, Kolumn 2 och Kolumn 3.

* Indikator för fältuppdatering - En indikator visas nu när du sparar ett kort för att bekräfta att uppdateringarna sparades.


Mer information finns i [Kom igång med anslagstavlor i Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Dela mappar endast på de fem översta nivåerna i en mapphierarki

För att säkerställa bästa prestanda för användare som delar mappar begränsar vi för närvarande delningen till de fem högsta nivåerna i en mapphierarki på ett objekt.

Varje mapp på sjätte nivån eller tidigare ärver sina delningskonfigurationer från mappen direkt ovanför den.

Mer information om att dela mappar finns i [Dela en dokumentmapp på den översta nivån](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Workfront Campaigns (beta) - ett nytt sätt att hantera ditt arbete

>[!NOTE]
>
>Den här funktionen kommer att tas bort från förhandsgranskningen den 9 januari 2023. Mer information finns i [23.1 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Den här funktionen ingår inte i 22.3-produktionsversionen. Den kommer att lanseras i Production med en framtida release.


>[!NOTE]
>
>Den här funktionen är endast tillgänglig som betaversion och håller på att byggas. Vi kommer att fortsätta lägga till funktioner för Campaign-arbetsflödet med framtida releaser. Deltagande i betaprogrammet för Workfront Campaigns är frivilligt.

Vi introducerar ett nytt objekt för Adobe Workfront som kan förändra ditt arbetssätt.

Med Workfront Campaigns kan ni ordna projekt från olika portföljer och program i en ny arbetsbehållare. Den nya behållaren kommer att utvecklas i framtida versioner för att till slut inkludera alla arbetsobjekt som för närvarande hanteras i separata vattentäta skott.

Följande funktioner ingår i den här versionen:

* Ett nytt Workfront-objekt som heter Campaign

* Ett nytt kampanjområde (betaversion) på huvudmenyn

* En lista över kampanjer i kampanjområdet

* En kampanjinformationssida som visar ytterligare information om en kampanj

* Möjlighet att lägga till projekt i en kampanj

* Möjlighet att redigera information om en kampanj

* Möjlighet att byta namn på Campaign-objektet från layoutmallen

  Workfront system- och gruppadministratörer kan lägga till området Campaigns (Beta) på huvudmenyn i en layoutmall. Detta gör det tillgängligt för alla användare som är tilldelade mallen. Alla i Workfront kan skapa en kampanj när den är tillgänglig.




