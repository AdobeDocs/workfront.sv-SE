---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Skapa en tabellrapport
description: Du kan lägga till en tabellrapport på en Canvas-kontrollpanel för att visa data i ett tabellformat.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 981d86fa7d54d9d26c0a2b6142db98d5989cbed2
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Skapa en tabellrapport

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Mer information finns i [Betaversionsinformation för arbetsytans kontrollpaneler](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Du kan lägga till en tabellrapport på en Canvas-kontrollpanel för att visa data i ett tabellformat.

![Exempel på tabellrapport](assets/table-example-main.png)

+++ Expandera om du vill visa åtkomstkraven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Alla </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Aktuell: Planera </p> 
<p>Nytt: Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td> 
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
  </td> 
  </tr>  
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Förutsättningar

Du måste skapa en kontrollpanel innan du kan skapa en tabellrapport.

## Skapa en tabellrapport på en Canvas Dashboard

Det finns många konfigurationsalternativ för att skapa en tabellrapport. I det här avsnittet går vi igenom den allmänna processen att skapa en.

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på **Ny instrumentpanel** i det övre högra hörnet.

1. I rutan **Skapa instrumentpanel** anger du instrumentpanelens **namn** och **beskrivning**.

1. Klicka på **Skapa**.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Tabell** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. (Valfritt) Följ stegen nedan för att konfigurera avsnittet **Detaljer**:

   1. Ange en rapport **Namn**.

   1. Ange en rapport **Beskrivning**.

1. Följ stegen nedan för att konfigurera avsnittet **Bygg tabell**:

   1. Klicka på ikonen **Tabellkolumner** ![Skapa tabell](assets/drilldown-column.png) i den vänstra panelen.

   1. Klicka på **Lägg till kolumn** och markera sedan det fält som du vill visa som en kolumn i tabellen. Kolumnen visas i förhandsvisningsavsnittet till höger.

   1. Upprepa ovanstående steg för varje kolumn som du vill lägga till.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter** ![Filter](assets/filter-icon.png) i den vänstra panelen.

   1. Välj **Redigera filter**.

   1. Klicka på **Lägg till villkor** och ange sedan fältet som du vill filtrera efter och modifieraren som definierar vilken typ av villkor som fältet måste uppfylla. Kolumnen visas i förhandsvisningsavsnittet till höger.

1. (Valfritt) Klicka på **Lägg till filtergrupp** om du vill lägga till ytterligare en uppsättning filtervillkor. Standardoperatorn mellan uppsättningarna är AND. Klicka på operatorn för att ändra den till ELLER.

1. Följ stegen nedan för att konfigurera avsnittet **Inställningar för grupper med nedladdning**:

   1. Klicka på ikonen **Gruppinställningar** ![Gruppinställningar](assets/drilldown-group-icon.png) i den vänstra panelen.

   1. Klicka på knappen **Lägg till gruppering** och markera sedan det fält som du vill skapa som en gruppering. Grupperingskolumnen visas i förhandsvisningsavsnittet till höger.

1. Klicka på **Spara** för att skapa rapporten och lägga till den på kontrollpanelen.