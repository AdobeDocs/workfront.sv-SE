---
navigation-topic: business-case-and-scorecards
title: Godkänn ett affärsärende
description: När du har slutfört och skickat in affärsärendet för en projektförfrågan måste affärsärendet godkännas. Detta beror på arbetsflödet i organisationen. Ett projekt kan börja utan att Business Case behöver godkännas, men Adobe Workfront-administratören och projektägarna tycker kanske inte att det är idealiskt.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Godkänn ett affärsärende

<!--Audit: 6/2025-->

När du har slutfört och skickat in affärsärendet för en projektförfrågan måste affärsärendet godkännas. Detta beror på arbetsflödet i organisationen. Ett projekt kan börja utan att Business Case behöver godkännas, men Adobe Workfront-administratören och projektägarna tycker kanske inte att det är idealiskt.

Mer information om hur du fyller i och skickar ett affärsärende finns i artikeln [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
   <p>Aktuell: Prime eller senare</p>
   <p>eller</p>
   <p>Äldre: Business eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
   <p>Aktuell: Standard </p> 
   <p>Äldre: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter för ett projekt</p> <p>Visa eller högre behörigheter för en portfölj</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över godkännande av affärsärende

Tänk på följande när du godkänner ett affärsärende för ett projekt:

* Du måste ha behörigheten Hantera för ett projekt för att kunna godkänna affärsärendet för det.
* Du kommer inte att kunna se de projekt som väntar på att affärsärendet ska godkännas i widgeten Mina godkännanden i Hem.
* Du måste manuellt gå till de enskilda projekt som behöver godkännas av ett affärsärende för att se att de väntar på godkännande. Det finns ingen meddelandefunktion i Workfront som varnar någon om att han eller hon måste godkänna ett projekts affärsfall.
* Du kan hitta projekt som väntar på godkännande av affärsärendet antingen genom att skapa en projektrapport eller genom att öppna portföljen som de är kopplade till.

  Mer information om portföljer finns i artikeln [Portfolio - översikt i Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Godkänn affärsärendet genom att skapa en projektrapport

Du kan skapa en rapport för projekt för att se vilka projekt som behöver godkännas av deras affärsärende.

Så här skapar du en rapport för projekt som väntar på godkännande av sina affärsärenden:

1. Skapa en rapport för projekt.

   Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Välj fliken **Visa** i rapporten och klicka sedan på **Lägg till kolumn**.

1. Börja skriva &quot;Status&quot; i fältet **Visa i den här kolumnen** och markera det här fältet när det visas i listan.

   I den här kolumnen visas projektens status.

1. Välj fliken **Filter** i rapporten och klicka sedan på **Lägg till en filterregel**.

1. Börja skriva &quot;Status&quot; i **Visa bara projekt där fältet ...** finns och markera det när det visas i listan.
1. Välj **Lika med** som filtermodifierare.
1. Börja skriva &quot;Requested&quot; i det tillgängliga fältet.

   Detta garanterar att rapporten endast innehåller projekt som har statusen Begärd.

   ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Valfritt) Klicka på **Lägg till en annan filterregel**.

   Du kan lägga till ytterligare filter om du bara vill visa projekt där du är projektägare, projektsponsor eller Portfolio ägare.

   Du kan till exempel använda följande filtersatser:

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   för att visa projekt där du har utsetts till projektsponsorer

   ```
   Project Owner ID Equals $$USER.ID
   ```

   för att visa projekt där du har utsetts till projektägare

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   för att visa var du är utsedd till Portfolio Manager.

1. Klicka på **Spara+Stäng**.

   Observera att alla projekt i rapporten har statusen **Begärd**.

1. Klicka på namnet på ett projekt i rapporten för att öppna det.
1. Klicka på **Affärsfall** i den vänstra panelen.
1. Klicka på **Godkänn** eller **Avvisa** i området Sammanfattning av affärsärenden för att godkänna eller avvisa affärsärendet.

   ![Affärsärende](assets/business-case-summary-with-rp-information--1-.png)

   Projektstatusen ändras till **Godkänd** om affärsärendet har godkänts.

   Projektstatusen ändras till **Avvisad** om affärsärendet avvisas.

   >[!NOTE]
   >
   >Det finns inga meddelanden som informerar användaren som skickade in godkännandet av affärsärendet om hans/hennes projektförfrågan godkändes eller avvisades.

## Godkänn affärsärendet genom att gå till begärda projekt i en portfölj

Mer information om granskning av begärda projekt finns i artikeln [Granska begärda projekt](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
