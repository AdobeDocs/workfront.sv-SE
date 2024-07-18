---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Förstå hur du organiserar rapporter på en kontrollpanel
description: Du kan se om en rapport har lagts till på en kontrollpanel i Adobe Workfront. Detta kan vara användbart när du bestämmer vilka rapporter du kan behålla och vilka som kan tas bort från systemet. Om det finns rapporter på kontrollpaneler kanske användarna fortfarande förlitar sig på dem. Vi rekommenderar att du inte tar bort rapporter som visas på kontrollpaneler som användarna använder. Mer information om hur du lägger till rapporter på kontrollpaneler finns i artikeln Lägga till en rapport på en kontrollpanel.
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Förstå hur du organiserar rapporter på en kontrollpanel

## Åtkomst till instrumentpanelsinformation i en rapportlista

Du kan se om en rapport har lagts till på en kontrollpanel i Adobe Workfront. Detta kan vara användbart när du bestämmer vilka rapporter du kan behålla och vilka som kan tas bort från systemet. Om det finns rapporter på kontrollpaneler kanske användarna fortfarande förlitar sig på dem. Vi rekommenderar att du inte tar bort rapporter som visas på kontrollpaneler som användarna använder.\
Mer information om hur du lägger till rapporter på kontrollpaneler finns i artikeln [Lägg till en rapport på en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Du kan se om en rapport har lagts till på en kontrollpanel genom att göra något av följande:

* Bygga en vy för en lista med rapporter och inkludera instrumentpanelsinformation i kolumnerna
* Filtrera en lista med rapporter från en eller flera specifika instrumentpaneler som du vet används aktivt
* Bygga en rapport för rapportobjektet och använda en vy eller ett filter som innehåller information om instrumentpanelen

Vem som helst kan skapa en vy eller ett filter, men du måste ha behörighet att redigera rapporter på åtkomstnivån för att kunna skapa en rapport.\
Mer information om åtkomst till rapporter finns i artikeln [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa instrumentpanelsinformation i Visa en rapportlista

>[!WARNING]
>
>Om du tar med kontrollpanelskolumnen i en rapportlista kan inläsningstiden öka avsevärt, särskilt för långa rapportlistor.

Så här skapar du en vy med instrumentpanelsinformation för en rapportlista:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.
1. Klicka på listrutan **Visa** i listan med rapporter.
1. Klicka på **Ny vy**.
1. Klicka på **Lägg till kolumn**.
1. Börja skriva &quot;Dashboards&quot; i fältet **Börja skriva fältnamn**.
1. Välj **Kontrollpaneler** under objektet **Rapport**.

1. Klicka på **Spara vy**.\
   Kontrollpanelerna som en rapport visas på i kolumnen Kontrollpaneler i rapportlistan.\
   ![](assets/qs-dashboards-in-report-view.png)

## Filtrera en rapportlista efter instrumentpanelsinformation

Så här filtrerar du en lista över rapporter efter instrumentpanelsinformation:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.

1. Klicka på listrutan **Filter** i rapportlistan.
1. Klicka på **Nytt filter** och sedan på **Lägg till en filterregel**.

1. Börja skriva &quot;Dashboards&quot; i fältet **Börja skriva fältnamn**.

1. Välj **Namn** under objektet **Kontrollpaneler**.

1. Välj **Lika med** i listrutan för modifiering och börja sedan skriva namnet på den instrumentpanel som du vill filtrera efter. Du kan välja flera kontrollpaneler för filtret.\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. Klicka på **Spara + Stäng**.\
   Här visas en lista med rapporter som bara visas på de angivna instrumentpanelerna.\
   Du kan också skapa en rapport för rapportobjektet och använda det här filtret i rapporten.
