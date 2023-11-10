---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: Översikt över tidrapporter
description: Du kan använda tidrapporter för att spåra den tid du tillbringar på arbetet. Mer information om tidrapportslayouten i Adobe Workfront finns i Förstå tidrapportslayouten.
author: Alina
feature: Timesheets
exl-id: 2174a879-4a19-4a0f-803a-f19a8909f227
source-git-commit: 48f46abab1958325aba6832b85247dc2c80f4e80
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Översikt över tidrapporter

Du kan använda tidrapporter för att hålla reda på hur mycket du spenderar på att arbeta i Adobe Workfront.

Som Workfront- eller gruppadministratör kan du skapa tidrapporter och associera dem med dina användare. Mer information om hur du skapar tidrapporter finns i [Skapa och hantera tidrapporter](../create-and-manage-timesheets/create-and-manage-timesheets.md).

En tidrapport är en tabell som påminner om ett rutnät och som visar arbetsobjekt och ett kalenderområde. Du kan logga tiden för artiklar och associera den med den dag då arbetet utfördes. Detta spårar din faktiska arbetstid i Workfront. Det finns också ett område i tidrapporten där du kan logga tid för icke-arbetsrelaterade objekt som möten, utbildning eller tid utanför kontoret.

Mer information om tidrapportslayouten i Adobe Workfront finns i [Förstå layouten för tidrapporten](../../timesheets/timesheets/timesheet-layout.md).

![](assets/timesheet-example.png)

Du kan logga tid i Workfront på flera olika sätt, vanligtvis på projektnivå, aktivitetsnivå eller på ett problem där arbetet utförs. Den tid som loggas mot uppgifter, problem och projekt visas också i din tidrapport.

Du kan också logga tiden för icke-projektarbeten under Allmänna timmar. Allmän timtid kan endast registreras i din tidrapport.

Mer information om var du kan logga in i Workfront finns i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!TIP]
>
>Med Workfront mobilapp kan du också publicera uppdateringar, ändra loggad tid, ange kommentarer och stänga din tidrapport.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste ha administrativ åtkomst till tidrapporter. </p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.


## Förstå projekttid jämfört med icke-projekttid

Tidrapporter gör det enkelt att hålla reda på tiden, både när det gäller projekt och icke-projektarbeten:

* **Projekttid:** Direkt från uppgiften eller projektet där du vill hålla reda på tiden.

  Timmar som registreras för uppgifter, utleveranser och projekt via en tidrapport kopplas till respektive arbetsobjekt för att ge en korrekt bild av den insats som har gjorts för projekt och uppgifter. Utan korrekt tidsangivelse kanske dina data inte är korrekta om de är avsedda för fakturering.

  När en resurs registrerar timmar direkt i uppgifter, visas dessutom automatiskt utleveranser och projekt när användaren öppnar tidrapporten. Detta förutsätter att datumintervallet för tidrapporten sträcker sig över de datum då timmarna registrerades.

* **Ej projekttid:** Direkt på användarens tidrapport. Mer information om hur du spårar tid i Workfront finns i   [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

  På en tidrapport kan en resurs registrera semestertimmar, sjuka timmar, öppettider, timmar som använts för att reparera eller underhålla utrustning, eller vilka allmänna intäktstyper du vill skapa.

## Få åtkomst till tidrapporter i området Tidrapporter

Mer information om alla områden i Workfront där du kan logga tid finns i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

Så här öppnar du en tidrapport:

1. Klicka på **Huvudmeny** icon ![](assets/dots-main-menu.png) i det övre högra hörnet eller **Huvudmeny** icon ![](assets/lines-main-menu.png) i det övre vänstra hörnet av Workfront, om tillgängligt, och klicka sedan på Tidrapporter.

   Området Tidrapporter visas som standard och alla tidrapporter som tillhör dig eller du har åtkomst till att visa.

   ![](assets/all-timesheets-list-nwe-350x68.png)

1. Klicka på något av följande alternativ i det övre högra hörnet om du vill visa ett begränsat antal tidrapporter:

   * **Mina tidrapporter** för att bara visa dina tidrapporter.

   ![](assets/my-timesheets-list-various-statuses-nwe-350x60.png)

   * **Mina tidrapportgodkännanden** om du bara vill visa tidrapporter som du godkänner.

     ![](assets/timesheets-i-approve-list-with0filters-new-nwe-350x61.png)

   En filtrerad lista med tidrapporter visas.

1. (Valfritt) Uppdatera vyn, filtret och grupperingen högst upp i listan med tidrapporter. Mer information finns i [Rapportelement: filter, vyer och grupperingar](../../reports-and-dashboards/reports/reporting-elements/reporting-elements-overview.md).

1. Klicka på **Datumintervall** av en tidrapport för att öppna den.

   Varje tidrapport visar alla uppgifter, ärenden och projekt som du har loggat in på. I en tidrapport visas även upp till 45 uppgifter, utgåvor eller projekt som du har tilldelats med datum inom tidrapportens tidsram, men som du kanske inte har loggat tid för ännu.

   Mer information finns i [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).



