---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Dela en kalenderrapport
description: Du kan dela en kalender med andra användare och göra den tillgänglig för allmänheten, så att någon utan en [!DNL Adobe Workfront] licens kan visa den.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: 041e812d0663304b4bd51134020209d3a67e1423
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Dela en kalenderrapport

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

Du kan dela en kalender med andra användare och du kan göra den tillgänglig för allmänheten, så att någon utan en [!DNL Adobe Workfront]-licens kan visa den.

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
   <td><p>Ny: ljus</p>
       <p>eller</p>
       <p>Aktuell: Granska</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL View] eller senare åtkomst till [!UICONTROL Reports], [!UICONTROL Dashboards] och [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>[!UICONTROL View] eller högre behörigheter till kalenderrapporten, med tillgång till delning</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dela en kalender med [!DNL Workfront] användare {#share-a-calendar-with-workfront-users}

Att dela en kalender påminner om att dela andra objekt. Mer information om delning av objekt i [!DNL Adobe Workfront] finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Kalendrar som har delats med dig visas med en asterisk (&#42;) bredvid kalendernamnet.

Så här delar du en kalender i [!DNL Workfront]:

1. Gå till kalendern som du vill dela.
1. <span class="preview">Klicka på menyn **Mer** bredvid kalendernamnet i förhandsgranskningen och klicka sedan på **Dela**.
   ![kalendermer meny](assets/more-menu-calendar.png)</span>
1. Klicka på **[!UICONTROL Calendar Actions]** och sedan på **[!UICONTROL Sharing]**.

1. I fältet **[!UICONTROL Give Calendar access to]** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela kalendern med och klickar sedan på namnet när det visas i listrutan.\
   Mer information om att ange behörigheter finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Valfritt) Upprepa steg 3 för varje användare, team, roll eller grupp som du vill ge åtkomst till kalendern.
1. Ange behörigheter för varje användare, team, roll, grupp eller företag som du har lagt till i steg 3 genom att klicka på den nedrullningsbara menyn och sedan välja den behörighetsnivå som du vill ge:

   * **[!UICONTROL View]:** Användare kan granska och dela kalendern.

     ![Dela kalender med Visa åtkomst](assets/calendar-share-view-permissions-350x249.png)
     <!--![Share calendar with view access](assets/view-calendar.png)-->

   * **[!UICONTROL Manage]:** Användare har fullständig åtkomst till kalendern, minus administrativa behörigheter, som ges på åtkomstnivån, plus alla visningsbehörigheter.

     ![Dela kalendern med Hantera åtkomst](assets/calendar-share-manage-permissions-350x241.png)
     <!--![Share calendar with manage access](assets/manage-calendar.png)-->

     >[!NOTE]
     >
     >Administratören [!DNL Workfront] och den som skapat kalendern kan ta bort behörigheter från entiteterna.

1. (Valfritt) Beroende på en användares roll kan du klicka på **[!UICONTROL Advanced Options]** och sedan klicka på &#x200B; **[!UICONTROL Share]** så att användaren kan dela kalendern med andra användare.

   Mer information om behörighetsnivåer finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Valfritt) Om du vill göra kalendern tillgänglig för alla [!DNL Workfront]-användare klickar du på kugghjulsikonen och sedan på **[!UICONTROL Make this visible system-wide]** i listrutan för att göra objektet tillgängligt för alla [!DNL Workfront] -användare.\
   Alla användare kan se objektet baserat på de behörigheter som du anger.

1. Klicka på **[!UICONTROL Save]**.

## Dela en kalender med en offentlig länk

Du kan göra en kalender offentlig och dela en länk med personer som inte har någon [!DNL Workfront]-licens.

1. Gå till kalendern som du vill dela.
1. Klicka på **[!UICONTROL Calendar Actions]** och sedan på **[!UICONTROL Sharing]**.
1. <span class="preview">Klicka på menyn **Mer** bredvid kalendernamnet i förhandsgranskningen.
   ![kalendermer meny](assets/more-menu-calendar.png)</span>

1. Klicka på kugghjulsikonen och sedan på **[!UICONTROL Make this public to external users]**.
1. Klicka på **[!UICONTROL Copy link]**.
1. <span class="preview">Klicka på **Kopiera offentlig länk** i förhandsgranskningen.</span>
1. Klicka på **[!UICONTROL Save]**.

## Dela en kalender med en privat länk

Du kan dela en privat kalenderlänk med [!DNL Workfront] användare. Användarna måste logga in för att kunna visa kalendern när de använder länken.

1. Gå till kalendern som du vill dela.
1. <span class="preview">Klicka på menyn **Mer** bredvid kalendernamnet i förhandsgranskningen och klicka sedan på **[!UICONTROL Get Sharable Link]**.
   ![kalendermer meny](assets/more-menu-calendar.png)</span>
1. Klicka på **[!UICONTROL Calendar Actions]** och sedan på **[!UICONTROL Get Sharable Link]**.
1. Klicka på **[!UICONTROL Copy Link]**.

   >[!NOTE]
   >
   >[!DNL Workfront] användare måste ha åtkomst till kalendern för att kunna komma åt den med länken. Information om hur du beviljar åtkomst finns i [Dela en kalender med [!DNL Workfront] användare](#share-a-calendar-with-workfront-users).\
   >Om användarna inte har åtkomst kan de begära det efter att länken har klistrats in i webbläsaren.
