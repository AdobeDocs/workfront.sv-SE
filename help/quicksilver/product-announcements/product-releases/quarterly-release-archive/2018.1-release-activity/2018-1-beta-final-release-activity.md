---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta Final Release Activity
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i Beta Final-utgåvan 2018.1. Funktionen gjordes tillgänglig i förhandsvisningsmiljön den 31 januari 2018. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 2018.1 Beta Final Release Activity

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i Beta Final-utgåvan 2018.1. Funktionen gjordes tillgänglig i förhandsvisningsmiljön den 31 januari 2018. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.1 finns på  [Aktivitetsöversikt för version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Beta Final-utgåvan 2018.1 innehåller förbättringar för både Workfront-administratörer och andra användare:

**För administratörer**

* [Konfigurera resurstillgänglighet och användarallokeringar som ska beräknas baserat på användarschemat](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**För alla användare**

* [Mobila förbättringar](#mobile-enhancements)
* [Jira-integrering](#jira-integration)
* [Uppdatera till namn på korrekturläsare](#update-to-proofing-viewer-names)
* [Ändra till synkroniseringskopia vid synkronisering från produktionsmiljön för korrektur till förhandsgranskning](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [Varningsmeddelande visas när gränsen på 2 000 objekt nås i resursplaneraren](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Mobilförbättringar {#mobile-enhancements}

Följande funktionalitet kommer till Mobile App Store i början av mars 2018:

* Ny navigering: Startsidan för våra mobilappar har fått en ny design.
* Hem på mobilen: Våra nya hemfunktioner har nu uppdaterats även för våra mobilappar.

Den nya funktionaliteten stöds för både iOS och Android.

## Jira-integrering {#jira-integration}

Du kan nu länka Jira-problem till Workfront-uppgifter eller problem genom att installera och konfigurera Workfront-tillägget för Jira. Med den här integreringen kan projektledarna fortsätta att arbeta i Workfront, medan utvecklarna kan fortsätta att arbeta i Jira, medan deras individuella objekt länkas genom integreringen av Workfront med Jira.

Du kan konfigurera följande genom den här integreringen:

* Upprätta triggers för Workfront-uppdrag för att automatiskt skapa Jira-problem när de inträffar.
* Länka Jira-problem manuellt till Workfront-uppgifter eller problem som har skapats tidigare.
* Ange fält som ska synkroniseras på de länkade objekten så fort ett av objekten uppdateras i något av programmen.

Workfront-tillägget kommer att vara tillgängligt för både On-Premise- och On-Demand-versionerna av Jira. Tillägget är kostnadsfritt och kan laddas ned från Atlassian Marketplace i början av mars 2018.

Mer information om Workfront-tillägget för Jira, inklusive en länk för att ladda ned det, finns i [Använda Workfront med Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Uppdatera till namn på korrekturläsare {#update-to-proofing-viewer-names}

Namnen på det HTML5-baserade korrekturläsaren och de Flash-baserade korrekturläsarna har namnändrats i hela Workfront. De föregående och uppdaterade namnen är följande: 

| **Föregående namn** | **Uppdaterat namn** |
|---|---|
| korrekturläsare för HTML 5 | Nytt korrekturläsare |
| Språkkontroll för Flash | Språkkontroll för äldre användare |

{style="table-layout:auto"}

 Mer information om hur du använder det nya korrekturläsaren finns i [Granska korrektur i korrekturläsaren.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Konfigurera resurstillgänglighet och användarallokeringar som ska beräknas baserat på användarschemat {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Workfront-administratören kan nu avgöra hur Workfront beräknar resurstillgänglighet och användartilldelning på systemnivå (med hänsyn till öppettider och FTE). Workfront-administratören kan konfigurera resurstillgänglighet och användarallokering som ska beräknas antingen med standardschemat eller användarens schema.

Den här inställningen påverkar användarens tillgänglighet under följande omständigheter när resurser schemaläggs:

* När du tillåter att Workfront automatiskt tilldelar resurser, enligt beskrivningen i Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena.

* När allokeringsindikatorer visas, enligt beskrivningen i Hantera användarallokeringar i schemaläggningsområdena.

Mer information finns i&quot;Konfigurera hur Workfront beräknar resurstimme och FTE-tillgänglighet för schemaläggningsområdet&quot;.

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Växla till synkroniseringskadens vid synkronisering från produktionsmiljön för korrektur till förhandsgranskning {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Denna ändring träder i kraft den 11 februari 2018.

Data från Workfront Proof produktionsmiljö synkroniseras nu till Workfront Proof Preview-miljön varje vecka.

Före den här ändringen synkroniserades data från Workfront Proof produktionsmiljö till förhandsvisningsmiljön en gång i månaden, medan data från Workfront produktionsmiljö synkroniserades med Workfront förhandsvisningsmiljö en gång i veckan. Den här diskrepansen orsakade vissa synkroniseringsfel när språkfunktionerna i Workfront Preview-miljön användes. 

Mer information finns i [Testmiljö för förhandsvisning av sandlådor - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## Varningsmeddelande visas när gränsen på 2 000 objekt nås i resursplaneraren {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Eftersom vi för närvarande arbetar på en mer permanent lösning för att förbättra prestandan i resursplaneraren har vi infört en begränsning på 2 000 objekt för varje vy som du kan använda i resursplaneraren:

* I användarvyn visas endast 2 000 tilldelningar
* I projektvyn visas endast 2 000 projekt
* I rollvyn visas endast 2 000 roller

När resursplaneraren försöker läsa in fler än 2 000 objekt visas ett meddelande som meddelar att endast 2 000 objekt kan visas.

Mer information om dessa begränsningar och hur de påverkar Resursplaneraren finns i [Resursplanerarens visningsbegränsningar](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
