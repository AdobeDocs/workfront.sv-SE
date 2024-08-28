---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Använd flaggor på artiklar på Kanban-styrelsen
description: På  [!DNL Kanban] board ger flaggor en visuell indikation på när en artikel är klar att flyttas till nästa status. På så sätt kan Kanban-team använda en"pull"-metod i stället för en"push"-metod när de flyttar artiklar mellan olika statusar.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Använd flaggor i artiklar på [!UICONTROL Kanban]-tavlan

På [!DNL Kanban]-panelen ger flaggorna en visuell indikation på när en artikel är klar att flyttas till nästa status. Detta gör att [!UICONTROL Kanban] team kan använda en&quot;pull&quot;-metod i stället för en&quot;push&quot;-metod när artiklar flyttas mellan olika statusar.

**Exempel:** Titta på följande exempel på ett team som använder en pull-metod: Olivia, grafikdesignern i teamet, slutför sitt arbete och anger sedan artikelflaggan som [!UICONTROL Ready to Pull]. Den här flaggan ger en visuell indikation till Tony, copywriter i teamet, att historien är klar för honom att gå vidare till nästa status. Tony flyttar sedan berättelsen till nästa status när han är redo att börja arbeta på den.

Tänk på följande när du använder flaggor i artiklar:

* Flaggor är inte en status, utan snarare en visuell indikation på att artikeln är klar att flyttas till nästa status av en annan teammedlem.
* Flaggor visas inte på artikelkort som finns i kolumnen [!UICONTROL Backlog] eller i kolumnen [!UICONTROL Complete] (eller i någon kolumn där kolumnens status är lika med [!UICONTROL Complete]).

  Mer information om artikelstatus finns i [Använd flaggor på artiklar på Kanban-tavlan](#updating-the-status-of-stories-and-subtasks)

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
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p> 
   eller
   <p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Använd flaggor i artiklar på [!UICONTROL Kanban]-tavlan

Så här ändrar du en flagga för en artikel:

{{step1-to-team}}

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett nytt [!UICONTROL Kanban]-team i listrutan eller sök efter ett team i sökfältet.

1. Gå till [!UICONTROL Kanban]-panelen där du vill ändra en flagga för en artikel.
1. Expandera artikelrutan om du vill visa flaggan.
Flaggan är inställd på **[!UICONTROL On Track]** för varje artikel som standard.
   ![Kanban-kort](assets/agile-storycard-kanban-2021-350x308.png)

1. Klicka på den aktuella flaggan och välj sedan bland följande flaggalternativ:

   * **[!UICONTROL On Track]:** Artikeln har rätt status och ingen åtgärd behöver vidtas just nu.

     Det här är standardflaggan för varje artikel på Kanban-tavlan.
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Is Blocked]:** Artikeln kan inte fortsätta till nästa status. När den här flaggan anges för en artikel räknas artikeln inte mot Pågående arbete-gränsen. (Mer information om PIA-begränsningar finns i artikeln [Konfigurera kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).)

     ![kanban_flag_locked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Ready to Pull]:** Artikeln kan flyttas till nästa status av en annan medlem i teamet.

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
