---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Redigera en befintlig kalenderrapport
description: Du kan ändra en befintlig kalender genom att lägga till eller ta bort en länk till ett projekt. Du kan också ändra kalendergrupperingar som är kopplade till en kalenderrapport.
author: Lisa
feature: Reports and Dashboards
exl-id: 494d040c-bd1d-4356-824f-a75890803617
source-git-commit: c8f4d8e460ed9247ca5d89c9a711ecb1ec5ed1e9
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Redigera en befintlig kalenderrapport

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

Du kan ändra en befintlig kalender genom att lägga till eller ta bort en länk till ett projekt. Du kan också ändra kalendergrupperingar som är kopplade till en kalenderrapport.

>[!NOTE]
>
>Du är begränsad till 15 grupperingar i en kalenderrapport.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!UICONTROL Reports], [!UICONTROL Dashboards] och [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>[!UICONTROL Manage] åtkomst till kalenderrapporten</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera en befintlig kalenderrapport i produktion

{{step1-to-calendars}}

1. (Valfritt) Om du vill ändra namnet på kalenderrapporten klickar du på fältet [!UICONTROL calendar name] och gör sedan önskade ändringar. Vi rekommenderar att du endast använder UTF-8-tecken för att undvika kompatibilitetsproblem.

   ![Ändra rapportnamn](assets/titlechange-250x230.png)

   Om du har delat kalenderrapporten med andra användare eller team uppdateras det ändrade kalendernamnet automatiskt i deras kalendervy.

1. (Valfritt) Så här lägger du till ett projekt i kalenderrapporten:

   1. Klicka på **[!UICONTROL Add to Calendar].**
   1. I fältet **[!UICONTROL Project name]** börjar du skriva namnet på ett projekt som du vill lägga till kalenderhändelser från och klickar sedan på namnet när det visas i listrutan.

      ![Välj projektnamnet](assets/calendar-project-name.png)
Objekt från projektet och tillhörande uppgifter och utgåvor läggs till i kalenderrapporten.

1. (Valfritt) Så här lägger du till en kalendergrupp eller ändrar en befintlig kalendergrupp:

   1. Håll markören över projektnamnet, klicka på listrutepilen bredvid projektnamnet och klicka sedan på **[!UICONTROL Edit]**.

      ![Redigera kalendergruppering](assets/editcalendergroup-350x126.png)

   1. Välj hur du vill gruppera dina objekt:

      * [Använd [!UICONTROL Planned Dates] i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
      * [Använd [!UICONTROL Projected Dates] i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
      * [Använd anpassade datumfält i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)


<div class="preview">

## Redigera en befintlig kalenderrapport i Förhandsgranska

{{step1-to-calendars}}

1. (Valfritt) Om du vill ändra namnet på kalenderrapporten klickar du på menyn **Mer** och väljer **Redigera**.
   ![fler meny](assets/new-more-menu-calendar.png)
Om du har delat kalenderrapporten med andra användare eller team uppdateras det ändrade kalendernamnet automatiskt i deras kalendervy.

1. (Valfritt) Så här lägger du till ett projekt i kalenderrapporten:
   1. Klicka på **[!UICONTROL Add to Calendar].**
   1. Börja skriva namnet på ett projekt som du vill lägga till kalenderhändelser från och klicka sedan på namnet när det visas i listrutan.
   1. Klicka på **Lägg till**.
      ![lägg till ett projekt i en kalender](assets/add-a-calendar-project.png)


1. (Valfritt) Så här lägger du till en kalendergrupp eller ändrar en befintlig kalendergrupp:
   1. Klicka på menyn **Mer** bredvid projektnamnet och klicka sedan på **Redigera**.
      ![redigera projekt i kalender](assets/edit-project-in-calendar.png)e

   1. Välj hur du vill gruppera dina objekt:

      * [Använd [!UICONTROL Planned Dates] i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
      * [Använd [!UICONTROL Projected Dates] i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
      * [Använd anpassade datumfält i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)


      </div>