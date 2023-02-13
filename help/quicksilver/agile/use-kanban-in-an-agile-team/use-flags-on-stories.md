---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Använd flaggor på artiklar på Kanban-tavlan
description: På [!DNL Kanban] board, flags ger en visuell indikation på när en artikel är klar att övergå till nästa status. På så sätt kan Kanban-team använda en"pull"-metod i stället för en"push"-metod när de flyttar artiklar mellan olika statusar.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Använd flaggor i artiklar på sidan [!UICONTROL Kanban] board

På [!DNL Kanban] board, flags ger en visuell indikation på när en artikel är klar att övergå till nästa status. Detta aktiverar [!UICONTROL Kanban] team använder en&quot;pull&quot;-strategi i stället för en&quot;push&quot;-strategi när de flyttar artiklar mellan olika statusar.

**Exempel:** Titta på följande exempel på ett team som använder&quot;pull&quot;-metoden: Olivia, teamets grafiska formgivare, avslutar sitt arbete och anger sedan artikelflaggan som[!UICONTROL Ready to Pull].&quot; Den här flaggan ger en visuell indikation till Tony, copywriter i teamet, att historien är klar för honom att gå vidare till nästa status. Tony flyttar sedan berättelsen till nästa status när han är redo att börja arbeta på den.

Tänk på följande när du använder flaggor i artiklar:

* Flaggor är inte en status, utan snarare en visuell indikation på att artikeln är klar att flyttas till nästa status av en annan teammedlem.
* Flaggor visas inte på några artikelkort som finns i [!UICONTROL Backlog] kolumn eller i [!UICONTROL Complete] kolumn (eller i en kolumn där kolumnens status är lika med [!UICONTROL Complete]).

   Mer information om artikelstatus finns i [Använd flaggor på artiklar på Kanban-tavlan](#updating-the-status-of-stories-and-subtasks)

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Använd flaggor i artiklar på sidan [!UICONTROL Kanban] board

Så här ändrar du en flagga för en artikel:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)och sedan antingen välja en ny [!UICONTROL Kanban] i listrutan eller sök efter ett team i sökfältet.

1. Gå till [!UICONTROL Kanban] bräda där du vill ändra en flagga för en artikel.
1. Expandera artikelrutan om du vill visa flaggan.\
   Flaggan är inställd på **[!UICONTROL On Track]** för varje artikel som standard.\
   ![Kanban-kort](assets/agile-storycard-kanban-2021-350x308.png)

1. Klicka på den aktuella flaggan och välj sedan bland följande flaggalternativ:

   * **[!UICONTROL On Track]:** Artikeln har rätt status och ingen åtgärd behöver vidtas just nu.\

      Det här är standardflaggan för varje artikel på Kanban-tavlan.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Is Blocked]:** Artikeln kan inte fortsätta till nästa status. När den här flaggan anges för en artikel räknas artikeln inte mot Pågående arbete-gränsen. (Mer information om PIA-begränsningar finns i artikeln [Konfigurera Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_locked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Ready to Pull]:** Artikeln kan flyttas till nästa status av en annan medlem i teamet.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
