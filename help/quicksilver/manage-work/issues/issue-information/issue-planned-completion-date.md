---
product-area: projects
navigation-topic: issue-information
title: Översikt över det planerade slutförandedatumet för problemet
description: Det planerade slutförandedatumet för en utgåva är det datum då utgåvan förväntas vara slutförd.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Översikt över det planerade slutförandedatumet för problemet

Det planerade slutförandedatumet för en utgåva är det datum då utgåvan förväntas vara slutförd.

Du kan antingen ange planerat slutförandedatum för ett problem eller låta Adobe Workfront beräkna det utifrån vissa kriterier.

Planerade slutförandedatum för problem påverkar inte projektets planerade slutförandedatum. Det är bara aktivitetens planerade slutförandedatum som påverkar projektets planerade slutförandedatum. Mer information om projektets planerade slutförandedatum finns i [Ange projektets planerade slutförandedatum](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>Det planerade slutförandedatumet för en utgåva skiljer sig från datumet för implementering av utgåvan eller det planerade slutförandedatumet för utgåvan på följande sätt:
>
>* Bekräftelsedatum är det datum då den person som har tilldelats utgåvan manuellt beräknar att utgåvan har slutförts. Mer information finns i följande artiklar:
>
>   * [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interaktion mellan implementeringsdatumet och det planerade slutförandedatumet](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* Det beräknade slutförandedatumet är ett datum som beräknas av Workfront och som tar hänsyn till externa faktorer för att fastställa ett realtidsdatum för när problemet kan slutföras på ett realistiskt sätt. Mer information finns i [Översikt över planerat slutförandedatum för projekt, uppgifter och problem](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Ange manuellt planerat slutförandedatum för ett problem

Du måste ha behörigheten Redigera för problem och Hantera för att kunna uppdatera det planerade slutförandedatumet för problemet.

Du kan ställa in det planerade slutförandedatumet för ett problem manuellt i följande områden i Workfront:

* I rutan Redigera problem eller under Ärendeinformation när du skapar eller redigerar ett problem. Mer information finns i [Redigera problem](../../../manage-work/issues/manage-issues/edit-issues.md).
* Under Hem om Planerat slutförandedatum visas på panelen Sammanfattning av ett problem. Mer information finns i [Uppdatera eller redigera ett arbetsobjekt i hemområdet](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* I utgåvans rubrik. Mer information finns i [Nya objektrubriker](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* I en problemlista eller rapport när fältet Planerat slutförandedatum visas i vyn.

  Mer information finns i [Redigera problem i en lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Hur Workfront automatiskt beräknar det planerade slutförandedatumet för ett problem

När Workfront automatiskt beräknar det planerade slutförandedatumet för ett problem kan följande påverka datumet:

* Planerat startdatum

  Anmälningsdatumet och det planerade startdatumet ska matcha ett problem när du skapar utgåvan första gången.

* Standardvaraktighet enligt konfigurationen i avsnittet Köinformation i projektet. Mer information finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

  Om standardlängden är 0 dagar matchar det planerade slutförandedatumet det planerade startdatumet för utgåvan.

* Projektschema

När detta anges automatiskt bestäms det planerade slutförandedatumet utifrån följande beräkning:

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Exempel:** Om din aktivitet till exempel har startdatumet fredag, 14 januari och standardlängden är 5 dagar, är det planerade slutförandedatumet fredag, 21 januari, om projektschemat är måndag-fredag i 8 timmar om dagen.

Följande situationer finns:

* Om projektet inte har något schema, tas standardschemat i ditt Workfront-system med i beräkningen. Mer information finns i [Översikt över scheman](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Om schemat är måndag-fredag 9.00 till 17.00 (4 timmar om dagen) och det normala antalet timmar per arbetsdag i Workfront är 8 timmar, är det planerade slutförandedatumet den 27 januari.

>[!TIP]
>
>Workfront tar hänsyn till schemalagda undantag som helger och helger vid beräkning av planerade slutförandedatum.


