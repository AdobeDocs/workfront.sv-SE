---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Förbättrad resurshantering
description: Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 20.3 till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 10 augusti 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 Förbättrad resurshantering

Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 20.3 till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 10 augusti 2020.

En lista över alla ändringar som är tillgängliga i version 20.3 finns i [20.3 versionsöversikt](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Inkludera timmar från utleveranser i området Tilldelad arbetsyta i belastningsutjämnaren

För att du ska kunna se en fullständig bild av alla dina personers arbetsbelastningar har vi infört en inställning som gör att du kan inkludera timmar från utgåvor i området Tilldelat arbete i Utjämning av arbetsbelastning.

Mer information om hur du arbetar i Arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Justera allokeringar för lediga dagar i Utjämning av arbetsbelastning

Du kan justera allokeringar för resurser för icke-arbetsdagar med hjälp av Utjämning av arbetsbelastning.

Mer information om hur du hanterar allokeringar i Arbetsbelastningsutjämnaren finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Variabelfilter som är tillgängliga i Utjämning av arbetsbelastning

För att förbättra din upplevelse och ge dig större flexibilitet när du delar information har vi nu implementerat variabelfilter för belastningsutjämnaren. Följande filter har lagts till i arbetsbelastningsutjämnaren:

* &quot;Me&quot; (vid filtrering efter användare)
* &quot;Min primära roll&quot; (vid filtrering efter roller)
* &quot;My Home Team&quot; eller &quot;All My Teams&quot; (när jag filtrerar efter team).

De här filtren ersätter jokerfiltervariablerna för $$USER.ID, $$USER.roleID, $$USER.homeTeamID och $$USER.teamID

När du tillämpar något av dessa filter och sedan delar arbetsbelastningsutjämnaren eller placerar den på en kontrollpanel, kommer alla andra användare att se sin egen information.

Mer information om hur du använder filter i Utjämning av arbetsbelastning finns i [Filtrera information i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Ny sortering för projekt i Utjämning av arbetsbelastning

Utjämning av arbetsbelastning sorterar nu projekt först baserat på det tidigaste planerade startdatumet och sedan på det senaste planerade slutförandedatumet för aktiviteterna i projektet som inträffar under den tidsram som användaren visar på skärmen. På så sätt kan du ordna arbetet i en trädliknande hierarki, vilket gör det enklare att identifiera arbetet för en dag.

Mer information om hur du visar projekt och arbetsobjekt i Utjämning av arbetsbelastning finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visa faktiskt arbete i Utjämning av arbetsbelastning

För att du ska få ett korrekt perspektiv på arbetsbelastningens förlopp har vi introducerat en ny inställning i Utjämning av arbetsbelastning som visar tidslinjen för uppgifter och ärenden enligt deras planerade datum. Du kan aktivera inställningen Visa planerade datum för att visa den planerade tidslinjen för arbetsuppgiften förutom den planerade tidslinjen.

I och med den här förbättringen, om en uppgift eller ett problem har slutförts tidigare än det planerade slutförandedatumet, slås även de tilldelade timmarna från de återstående dagarna igenom för att visa att de inte räknas in i användarens totala tilldelning.

Mer information om hur du navigerar i arbetsbelastningsutjämnaren och aktiverar inställningar finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Funktioner för belastningsutjämnare som tidigare meddelats som släppta i version 20.2

* [Justera daglig och veckovis allokering i Utjämning av arbetsbelastning](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Uppdatera aktivitetsplanerade timmar i arbetsbelastningsutjämnaren](#update-task-planned-hours-in-the-workload-balancer)
* [Ett bekvämare sätt att uppdatera allokeringar i arbetsbelastningsutjämnaren](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Justera daglig och veckovis allokering i Utjämning av arbetsbelastning {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

För att undvika att resurser belastas kan du nu justera användarnas dagliga och veckovisa allokering så att de fungerar med hjälp av Utjämning av arbetsbelastning.

Före den här förbättringen var detta bara möjligt med verktygen för resursplanering.

Mer information om hur du hanterar allokeringar i Arbetsbelastningsutjämnaren finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Finns i följande miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

### Uppdatera aktivitetsplanerade timmar i arbetsbelastningsutjämnaren {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Den här förbättringen kommer att vara tillgänglig i produktionen strax efter version 2020.2.

Ett nytt alternativ i området Resurshantering på åtkomstnivån ger nu användare med den här åtkomsten möjlighet att redigera Planerade timmar från belastningsutjämnaren. När du justerar allokeringar i belastningsutjämnaren behöver den totala dagliga allokeringen inte matcha antalet planerade timmar för aktiviteterna. När du har sparat dina allokeringar blir det totala antalet allokeringstimmar antalet planerade timmar för uppgiften. Detta är bara möjligt för aktiviteter som har en enkel varaktighetstyp.

Mer information om hur du hanterar allokeringar i Arbetsbelastningsutjämnaren finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Mer information om hur du beviljar åtkomst till resurshantering finns i [Bevilja åtkomst till resurshantering](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Ett bekvämare sätt att uppdatera allokeringar i arbetsbelastningsutjämnaren {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

För att göra det enklare att hantera en användares tilldelningar till en arbetsuppgift i Utjämning av arbetsbelastning kan du nu dubbelklicka på arbetsposten. Du kan även använda menyalternativet Redigera allokeringar. Dessutom behöver du inte längre aktivera displaying-allokeringar för att kunna uppdatera dem.

Mer information om hur du hanterar allokeringar i Arbetsbelastningsutjämnaren finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
