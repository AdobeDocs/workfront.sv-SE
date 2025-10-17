---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Dela en kalenderrapport
description: Du kan dela en kalender med andra användare och göra den tillgänglig för allmänheten, så att någon utan en [!DNL Adobe Workfront] licens kan visa den.
author: Jenny
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Dela en kalenderrapport


Du kan dela en kalender med andra användare och du kan göra den tillgänglig för allmänheten, så att någon utan en [!DNL Adobe Workfront]-licens kan visa den.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Ljus</p>
       <p>Granska</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p> Visa eller öka åtkomst till rapporter, instrumentpaneler och kalendrar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Visa eller högre behörigheter i kalenderrapporten, med tillgång till delning</td> 
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
1. Klicka på menyn **Mer** bredvid kalendernamnet och klicka sedan på **Delning**.
   ![kalendermer meny](assets/more-menu-calendar.png)
1. I fältet **[!UICONTROL Give Calendar access to]** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela kalendern med och klickar sedan på namnet när det visas i listrutan.\
   Mer information om att ange behörigheter finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Valfritt) Upprepa steg 3 för varje användare, team, roll eller grupp som du vill ge åtkomst till kalendern.
1. Ange behörigheter för varje användare, team, roll, grupp eller företag som du har lagt till i steg 3 genom att klicka på den nedrullningsbara menyn och sedan välja den behörighetsnivå som du vill ge:

   * **[!UICONTROL View]:** Användare kan granska och dela kalendern.

     ![Dela kalendern med visningsåtkomst](assets/view-calendar.png)

   * **[!UICONTROL Manage]:** Användare har fullständig åtkomst till kalendern, minus administrativa behörigheter, som ges på åtkomstnivån, plus alla visningsbehörigheter.

     ![Dela kalendern med hantera åtkomst](assets/manage-calendar.png)

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
1. Klicka på menyn **Mer** bredvid kalendernamnet.
   ![kalendermer meny](assets/more-menu-calendar.png)
Klicka på **Kopiera offentlig länk**.
1. Klicka på **[!UICONTROL Save]**.

## Dela en kalender med en privat länk

Du kan dela en privat kalenderlänk med [!DNL Workfront] användare. Användarna måste logga in för att kunna visa kalendern när de använder länken.

1. Gå till kalendern som du vill dela.
1. Klicka på menyn **Mer** bredvid kalendernamnet och klicka sedan på **[!UICONTROL Get Sharable Link]**.
   ![kalendermer meny](assets/more-menu-calendar.png)

   >[!NOTE]
   >
   >[!DNL Workfront] användare måste ha åtkomst till kalendern för att kunna komma åt den med länken. Information om hur du beviljar åtkomst finns i [Dela en kalender med [!DNL Workfront] användare](#share-a-calendar-with-workfront-users).\
   >Om användarna inte har åtkomst kan de begära det efter att länken har klistrats in i webbläsaren.
