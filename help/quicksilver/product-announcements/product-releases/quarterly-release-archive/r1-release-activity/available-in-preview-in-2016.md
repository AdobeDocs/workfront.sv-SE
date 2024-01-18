---
content-type: release-notes
navigation-topic: product-releases-archive
title: Funktioner som blev tillgängliga i förhandsgranskningen 2016
description: Följande funktioner blev tillgängliga i förhandsvisningsmiljön 2016. Dessa funktioner planeras att lanseras i produktionsmiljön med R1-versionen.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 08e0bd72-5979-449e-9fb2-c4d45f51119e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Funktioner som blev tillgängliga i förhandsgranskningen 2016

Följande funktioner blev tillgängliga i förhandsvisningsmiljön 2016. Dessa funktioner planeras att lanseras i produktionsmiljön med R1-versionen.

## Förbättringar av resursplanering

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Nu kan du se alla uppgifter i projekt som du är resurshanterare för, vilket gör att du kan få mer information när du fattar beslut om schemaläggning.

Allmän information om de verktyg som är tillgängliga för att schemalägga resurser finns i&quot;Kom igång med resursschemaläggning&quot;.

Om du vill justera den information som visas på tidslinjen i tidslinjen skapar du ett filter enligt beskrivningen i Filterinformation i området Schemaläggning.

Förutom att visa uppgifter i de projekt du ansvarar för kan du använda tidslinjen för schemaläggning för att göra ändringar i resurstilldelningar. Mer information om hur du hanterar användartilldelningar på tidslinjen finns i &quot;Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena&quot;.

## Hantera användarallokeringar på tidslinjen för schemaläggning

När du schemalägger resurser med de nya verktygen för resursplanering kan du nu bestämma hur de planerade timmarna för en aktivitet eller utgåva ska fördelas mellan användarna. Du kan dela timmar mellan dagar i aktivitetens varaktighet och mellan tilldelade användare.

Mer information finns i Hantera användartilldelningar i schemaläggningsområden.

## Användarallokeringar är inaktiverade som standard

Skuggning av användarallokering på tidslinjen för schemaläggning när resurser nu schemaläggs är inaktiverat som standard.

Allokeringsskuggning visades tidigare som standard och kunde inte inaktiveras.

Mer information om hur du aktiverar alternativ för användartilldelning finns i Hantera användarallokeringar i schemaläggningsområdena.

## Layoutmall avgör om den nya eller gamla kalendern visas i arbetsytan

**Sandlådan för förhandsgranskning: 7 dec 2016; Tidig åtkomst: 14 dec 2016** 

Den nya kalendern visas som standard i området Mitt arbete när ingen layoutmall används.

Om du väljer det här alternativet kan du konfigurera den äldre kalendern som ska visas på arbetsytan Mitt genom att använda en layoutmall på arbetsytan Min arbetsyta som är konfigurerad att endast visa Genomför-datum för uppgifter och ärenden.

När du använder den äldre kalendern i området Mitt arbete visas endast det arbete du har åtagit dig.

Om du vill konfigurera Workfront så att den nya kalendern visas på arbetsytan Mitt när en layoutmall används, konfigurerar du layoutmallen så att den visar planerat slutförandedatum för uppgifter och ärenden och tilldelar sedan layoutmallen till rätt användare.

Mer information om hur du konfigurerar layoutmallen finns i [Skapa och hantera layoutmallar](../../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md#customizing-my-work) in [Skapa och hantera layoutmallar](../../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Outlook 365 Beta

**Beta: TBD; allmänt tillgänglig: TBD**

Du kan använda Workfront från Outlook för Office 365 enligt beskrivningen i följande avsnitt:

* [Konfigurera Adobe Workfront för Outlook](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)
* &quot;Uppdatera ett befintligt objekt från ett e-postmeddelande med Outlook 365&quot;

## Ändra ordning på kolumner i en lista med dra-och-släpp

**Tidig åtkomst: 20 feb 2016**

Du kan ändra ordningen på kolumnerna i en lista genom att dra en kolumn från en plats och släppa den i en annan.

Detta är särskilt användbart när du visar Gantt-diagrammet och listvyn samtidigt och kolumnen som du vill visa inte visas på sidans vänstra sida. 

Mer information finns i [Ändra kolumnbredd och -ordning](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)

## Uppdaterad Look and Feel i kontrollpanelslistan

Nu när du visar en kontrollpanelslista är utseendet mer modernt och skalbart.

Mer information om kontrollpaneler finns i [Skapa en instrumentpanel](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)

## Kontrollera åtkomst till anpassade Forms

**Förhandsgranskningssandlåda: 23 januari 2016**

Nu kan du styra vem som har åtkomst till ett anpassat formulär genom att ge åtkomst till enskilda användare, team, roller, grupper eller företag. 

Före den här ändringen kunde du bara bevilja åtkomst till grupper.

Mer information finns i [Skapa eller redigera ett anpassat formulär](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Integrering med Adobe Creative Cloud

**Tillägg som kan hämtas: april 2016**

Workfront-tillägget för Adobe Creative Cloud är utformat för att du ska kunna spara och exportera material som du skapar i Creative Cloud till Workfront, vilket snabbar upp godkännande- och granskningsprocessen.
