---
title: 20.4 Förbättrad resurshantering
description: 20.4 Förbättrad resurshantering
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# 20.4 Förbättrad resurshantering

Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 20.4 till förhandsvisningsmiljön. Dessa förbättringar kommer att bli tillgängliga i produktionsmiljön den 9 november 2020.

En lista över alla ändringar som är tillgängliga i version 20.4 finns i [20.4 versionsöversikt](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planera arbete med hjälp av Arbetskraft i stället för planerade timmar

För att ge dig flexibilitet när du planerar att arbeta med dina projekt har vi introducerat det nya konceptet med arbetsinsatser för uppgifter. Du kan uppskatta om arbetsinsatsen för en uppgift är liten, medelstor eller stor utan att manuellt uppskatta antalet planerade timmar för uppgiften. Varje ansträngningsnivå beräknas utifrån en procentandel av tiden från de vanliga timmarna per dag som konfigurerats i din instans.

Följande förbättringar är nu tillgängliga med den här nya funktionen:

* Aktivera den här inställningen för projekt och mallar för att göra den tillgänglig för uppgifter och malluppgifter
* Uppdatera den här inställningen för varje aktivitet med en enkel varaktighetstyp som automatiskt uppdaterar aktivitetens planerade timmar
* Inaktivera den här inställningen med en layoutmall för användare som hellre vill fortsätta använda Planerade timmar.
* Visa värdet för det nya fältet i en uppgiftslista eller rapport.

Mer information om arbetsinsats finns i [Översikt över arbetsinsats](../../../manage-work/tasks/task-information/work-effort.md).

Den här funktionen ingår nu i [Grundläggande om planering, del 2 inlärningsväg](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) på Workfront One.

## Projektstatusbaserade färger för arbetsobjekt i Utjämning av arbetsbelastning

För bättre synlighet och ökad anpassning av din upplevelse i Utjämning av arbetsbelastning kan du nu ändra färgerna för projekten och deras arbetsobjekt så att de matchar statusen för projekten. Färgerna motsvarar projektstatus på gruppnivå eller systemnivå. De färger som visas kan motsvara både system- och anpassad projektstatus.

Mer information om hur du anpassar vyn i Arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Justera användarallokering med procentvärden i Utjämning av arbetsbelastning

Nu kan du hantera användarnas tilldelningar i Utjämning av arbetsbelastning med procentandelar i stället för timmar.

Mer information om hur du hanterar allokeringar i Arbetsbelastningsutjämnaren finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Visa eller dölj slutfört arbete i Utjämning av arbetsbelastning

Med en ny inställning kan du nu visa eller dölja slutförda arbetsobjekt i Utjämning av arbetsbelastning. Inställningen är aktiverad som standard och slutförda arbetsobjekt som matchar filtervillkoren och den valda tidsramen visas i arbetsbelastningsutjämnaren.

Före den här förbättringen visas alltid slutförda arbetsobjekt i arbetsbelastningsutjämnaren.

Mer information om hur du justerar inställningar i Arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Förbättrad användbarhet i Utjämning av arbetsbelastning

För att säkerställa en smidig och användarvänlig upplevelse när du hanterar dina resurser i Utjämning av arbetsbelastning finns nu följande förbättringar av användbarheten:

* Nu kan du öppna Sammanfattning för problem och uppgifter från ikonen Sammanfattning i stället för menyn Mer. Den här upplevelsen är nu densamma som i listor.

   >[!NOTE]
   >
   >Det här alternativet är endast tillgängligt i den nya Adobe Workfront-upplevelsen.

* Du kan öppna menyn Mer till vänster om ett objektfält i stället för i slutet av ett objektfält. Det gör det enklare att hitta objekt som sträcker sig över en lång tidsperiod.
* Du kan komma åt uppdragsfunktionerna med ett kortkommando. Tidigare var detta bara tillgängligt från menyn Mer.
* Du kan läsa in alla återstående objekt under en användares namn i stället för bara följande 20 objekt genom att klicka på Läs in mer.

Mer information om hur du navigerar i arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Användarallokeringsdiagram i Utjämning av arbetsbelastning

För att du ska kunna ha en visuell representation på hög nivå av användarens allokering inom en given tidsram, aktiverar nu en ny inställning en diagramvy för hur allokeringarna visas i Utjämning av arbetsbelastning. Om du aktiverar den här inställningen visas användarens tilldelning i ett linjediagram som anger överbeläggningar i röda block och underbeläggningar i blått.

Mer information om hur du konfigurerar inställningar i Arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visa slutfört arbete i Utjämning av arbetsbelastning

För att du enkelt ska kunna identifiera arbete som redan har slutförts så att du kan hantera användartilldelningar på rätt sätt har vi aktiverat en visuell indikator i belastningsutjämnaren som visar när objekt för en vald tidsram har slutförts. Nu kan du se en grön bockmarkering för uppgifter, utgåvor när de är klara. I projektet visas även den gröna bockmarkeringen när arbetsobjekt har slutförts under den tidsram som visas på skärmen.

Mer information om hur du visar information i Arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nytt standardfilter för den tilldelade arbetsytan i Utjämning av arbetsbelastning

Standardfiltret för området Tilldelat arbete i Utjämning av arbetsbelastning visar nu endast användare som är medlemmar i alla team som du, som är inloggad användare, är kopplad till. Det nya filtret visar nu den mest relevanta informationen som standard.

Innan den här förbättringen visades alla användare som du hade åtkomst till i det här området.

Mer information om hur du använder filter i Arbetsbelastningsutjämnaren finns i [Hantera filter i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Ny ikon för växling mellan timmar- och procentvärden eller allokerad och återstående tid i Utjämning av arbetsbelastning

Vi har lagt till en ny inställning som gör att du kan växla mellan tilldelade timmar och procentvärden när du visar Utjämning av arbetsbelastning. Med den här nya ikonen har vi även tagit bort avsnittet Användararbetsbelastning på panelen Inställningar. I Utjämning av arbetsbelastning visas tilldelad tid som standard, och vi har flyttat inställningen Återstående timmar till den nya ikonen Procentandel eller Timmar.

Den här förbättringen eliminerar klickningar och gör det enklare och effektivare att navigera i arbetsbelastningsutjämnaren.

Mer information om hur du hanterar inställningar för Utjämning av arbetsbelastning finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ett nytt inbyggt filter för Utjämning av arbetsbelastning: Användare i projekt

Vi har lagt till ett nytt inbyggt filter på arbetsytan Tilldelad arbetsyta för att göra din filtreringsupplevelse i belastningsutjämnaren mer effektiv. Du kan nu använda filtret Användare i projekt som visar användare som har tilldelats uppgifter och ärenden i de projekt du anger.

Mer information om hur du använder filter i Arbetsbelastningsutjämnaren finns i [Filtrera information i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

