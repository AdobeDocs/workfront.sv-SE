---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Skapa en diagramrapport
description: En diagramrapport som visualiserar dina data som stapel-, kolumn-, linje- eller cirkeldiagram kan läggas till på en Canvas-kontrollpanel.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: ba9256255905e139c281099555a6d129fc570984
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# Skapa en diagramrapport

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Mer information finns i [Betaversionsinformation för arbetsytans kontrollpaneler](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Du kan skapa och lägga till en diagramrapport på en Canvas Dashboard för att visa dina data som stapel-, kolumn-, linje- eller cirkeldiagram.

![Diagramrapport](assets/chart-report-main.png)

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

Du måste skapa en kontrollpanel innan du kan skapa en diagramrapport.

## Skapa en diagramrapport på en Canvas Dashboard

Det finns många konfigurationsalternativ för att skapa en diagramrapport. I det här avsnittet går vi igenom den allmänna processen att skapa en.

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på **Ny instrumentpanel** i det övre högra hörnet.

1. I rutan **Skapa instrumentpanel** anger du instrumentpanelens **namn** och **beskrivning**.

1. Klicka på **Skapa**.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Diagram** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. (Valfritt) Följ stegen nedan för att konfigurera avsnittet **Detaljer**:

   1. Ange en rapport **Namn**.

   1. Ange en rapport **Beskrivning**.

   1. Om du vill kan du avmarkera rutan **Visa extra serier som Annan**.

      >[!NOTE]
      >
      >Det finns ett maximalt antal serier som kan visas i ett diagram. När den här rutan är markerad konsolideras alla serier över gränsen till en **annan**-gruppering i diagrammet.

1. Följ stegen nedan för att konfigurera avsnittet **Bygg diagram**:

   1. Klicka på ikonen **Skapa diagram** ![Skapa diagram](assets/build-chart-icon.png) i den vänstra panelen.

   1. Välj den typ av diagram du vill skapa i listrutan **Diagramtyp**:

      * **Bar**
      * **Kolumn**
      * **Rad**
      * **Cirkel**

   1. Välj kolumntyp i listrutan **Kolumntyp**:
      * **Enkel**
      * **Flera serier**
      * **Staplad**

   1. Markera knappen **Uppdatera fält** i det första avsnittet, leta reda på och markera det fält som innehåller data som ska summeras i diagrammet.
   1. I listrutan **Aggregeringstyp** väljer du hur data ska sammanfogas för att skapa diagramutdata.

   1. Markera knappen **Uppdatera fält** under det andra avsnittet, leta reda på och markera det andra fältet som du vill visa i diagrammet.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter**![ Filter](assets/filter-icon.png) i den vänstra panelen.
   1. Välj **Redigera filter**.
   1. Klicka på **Lägg till villkor** och ange sedan fältet som du vill filtrera efter och modifieraren som definierar vilken typ av villkor som fältet måste uppfylla.
   1. (Valfritt) Klicka på **Lägg till filtergrupp** om du vill lägga till ytterligare en uppsättning filtervillkor. Standardoperatorn mellan uppsättningarna är AND. Klicka på operatorn för att ändra den till ELLER.

1. Följ stegen nedan för att konfigurera avsnittet **Inställningar för nedåtriktad kolumn**:

   1. I den vänstra panelen klickar du på ikonen **Detaljerade kolumner** ![Detaljerade kolumner](assets/drilldown-column.png) . Fälten i diagrammet visas automatiskt som kolumner i förhandsvisningsavsnittet till höger.

   1. (Valfritt) Om du vill uppdatera någon av de befintliga kolumnkonfigurationerna markerar du den kolumn som du vill uppdatera i avsnittet **Aktuella kolumner** och uppdaterar sedan informationen (t.ex. etikett, länkad status och villkor).

   1. Klicka på **Lägg till kolumn** och markera sedan det fält som du vill visa som en kolumn i tabellen. Upprepa den här processen för varje kolumn som du vill lägga till.

1. Följ stegen nedan för att konfigurera avsnittet **Inställningar för grupper med nedladdning**:

   1. Klicka på ikonen **Gruppinställningar** ![Gruppinställningar](assets/drilldown-group-icon.png) i den vänstra panelen.

   1. Klicka på knappen **Lägg till gruppering** och markera sedan det fält som du vill skapa som en gruppering.

1. Klicka på **Spara** för att skapa rapporten och lägga till den på kontrollpanelen.

## Exempel på en diagramrapport

I det här avsnittet går vi igenom stegen för att skapa ett kolumndiagram som visar försenade uppgifter per projektägare.


{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på **Ny instrumentpanel** i det övre högra hörnet.

1. I rutan **Skapa instrumentpanel** anger du instrumentpanelens **namn** och **beskrivning**.

1. Klicka på **Skapa**.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Diagram** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Ange en rapport **Namn** (t.ex. *Försenade uppgifter per projektägare*).

   1. Ange en rapport **Beskrivning**.

1. Följ stegen nedan för att konfigurera avsnittet **Bygg diagram**:

   1. Klicka på ikonen **Skapa diagram** i den vänstra panelen.

   1. Välj **Kolumn** i listrutan **Diagramtyp**.

   1. Välj **Enkel** i listrutan **Kolumntyp**.

   1. Välj knappen **Uppdatera fält** under avsnittet **Nedersta (X) axeln** och leta sedan upp och välj fältet **Aktivitet** > **Projekt** > **Ägare** > **Namn**.

      ![Uppdatera fält](assets/bottom-x-axis.png)

   1. Klicka på knappen **Markera fält** under avsnittet **Vänster (Y) axel** och leta sedan upp och välj fältet **Aktivitet** > **Namn**.

   1. Välj **Antal** i listrutan **Aggregationstyp**.

      ![Sammanslagningstypfält](assets/left-y-axis.png)

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter** i den vänstra panelen.

   1. Välj **Redigera filter**.

   1. Klicka på **Lägg till villkor**.

   1. Klicka i det tomma villkorsområdet och välj sedan **Välj fält**.

   1. Markera fältet **Procent färdigt**.

   1. I listrutan **Operatorer** väljer du **Mindre än** och anger sedan *100* i utvärderarfältet.

   1. Klicka på **Lägg till villkor** och sedan på **Välj fält**.

   1. Markera fältet **Planerat slutförandedatum**.

   1. I listrutan **Operatorer** väljer du **Mindre än**.

   1. Växla **Ange relativt datum** till **ON**.

   1. Ange *$$TODAY* i utvärderingsfältet.

      ![Utvärderarfält](assets/add-condition.png)

1. Följ stegen nedan för att konfigurera avsnittet **Inställningar för nedåtriktad kolumn**:

   1. Klicka på ikonen **Kolumner med detaljnivåer** ![Kolumner med detaljnivå](assets/drilldown-column.png) i den vänstra panelen. Fälten i diagrammet visas automatiskt som kolumner i förhandsvisningsavsnittet till höger.

   1. Klicka på **Lägg till kolumn** och markera sedan fältet **Tilldelad** > **Namn**.

   1. Klicka på **Lägg till kolumn** och markera sedan fältet **Planerat startdatum**.

   1. Klicka på **Lägg till kolumn** och markera sedan fältet **Planerat slutförandedatum**.

   1. Klicka på **Lägg till kolumn** och markera sedan fältet **Senaste uppdateringsdatum**.

   1. (Valfritt) Om du vill visa uppdateringstiden markerar du alternativet **Senaste uppdateringsdatum** i fältet **Aktuella kolumner** och väljer sedan ett tidsvärde i listrutan **Datumformat** .

1. Följ stegen nedan för att konfigurera avsnittet **Inställningar för grupper med nedladdning**:

   1. Klicka på ikonen **Gruppinställningar** ![Gruppinställningar](assets/drilldown-group-icon.png) i den vänstra panelen.

   1. Klicka på knappen **Lägg till gruppering** och välj sedan fältet **Projekt** > **Namn**.

1. Klicka på **Spara** för att skapa rapporten och lägga till den på kontrollpanelen.