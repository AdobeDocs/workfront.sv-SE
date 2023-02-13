---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Konfigurera systemuppdateringar
description: Workfront genererar automatiska systemuppdateringar i ett objekts [!UICONTROL Updates] för att registrera ändringar som användare utför på objektet. Som [!DNL Workfront] administratör, du kan konfigurera vilka objektfält och åtgärder [!DNL Workfront] spår för att registrera systemuppdateringar.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# Konfigurera systemuppdateringar

[!DNL Adobe Workfront] genererar automatiska systemuppdateringar i ett objekts [!UICONTROL Updates] område där följande händelser ska registreras:

* Ändringar som användare gör i ett objektfält
* Åtgärder som användare utför på ett objekt

Dessa systemuppdateringar innehåller ändringar som gjorts, namnet på den användare som gjorde ändringen samt tid och datum för ändringen.

Som [!DNL Workfront] administratör, du kan konfigurera vilka objektfält och åtgärder [!DNL Workfront] spår för att registrera systemuppdateringar.

Du kan till exempel ha [!DNL Workfront] spåra alla ändringar som användare gör i namn på problem i hela systemet. Alla ändringar av problemets namn visas sedan som en systemuppdatering av problemets [!UICONTROL Updates] område.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ange vilka fält [!DNL Workfront] spår för en objekttyp

Du kan avgöra vilken information [!DNL Workfront] spårar när användare ändrar information som är kopplad till en viss objekttyp i hela [!DNL Workfront] gränssnitt. Det gör du genom att lägga till eller ta bort de fält du vill använda [!DNL Workfront] för att spåra för den objekttypen.

>[!NOTE]
>
>* [!DNL Workfront] kan inte spåra och registrera uppdateringar om beräknade anpassade fält.
>* Du kan anpassa systemuppdateringen för projekt, uppgifter, utgåvor, portfolior, program och användare. Du kan inte anpassa systemuppdateringen för mallar, dokument eller tidrapporter, men [!DNL Workfront] registrerar systemuppdateringar för dessa objekt.
>




* [Lägg till fält som du vill ha [!DNL Workfront] att spåra](#add-fields-you-want-workfront-to-track)
* [Ta bort fält som du inte vill spåra](#remove-fields-that-you-don-t-want-tracked)

### Lägg till fält som du vill ha [!DNL Workfront] att spåra {#add-fields-you-want-workfront-to-track}

Du kan lägga till fält [!DNL Workfront] för att spåra en viss typ av objekt i hela [!DNL Workfront] gränssnitt. När användare ändrar information i det fältet, [!DNL Workfront] registrerar information om ändringen som en systemuppdatering i [!UICONTROL Updates] området för objektet.

>[!NOTE]
>
>Du kan spåra upp till 300 inbyggda och anpassade fält i uppdateringsflödena. Om du spårar det maximala antalet fält och vill spåra fler fält som inte visas i [!UICONTROL All Fields] Under fliken måste du först ta bort några av de spårade fälten för att kunna spåra nya fält. Mer information om hur du tar bort fält från uppdateringsfälten finns i [Ta bort fält som du inte vill spåra](#remove-fields-that-you-don-t-want-tracked).

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. &#x200B; **[!UICONTROL Add Fields]** klickar du sedan på det objekt som du vill spåra.

1. I &#x200B; **[!UICONTROL Update Feeds]** som visas börjar du skriva ett inbyggt fält (standard) eller ett anpassat fält för objektet och klickar sedan för att markera det när det visas i listan.

   If [!DNL Workfront] spårar redan fältet, du kan inte lägga till det en andra gång från listan.

1. När du har lagt till alla fält du vill använda [!DNL Workfront] för att spåra, klicka **[!UICONTROL Add Fields]**.

   De inbyggda fälten som du har lagt till visas under **[!UICONTROL Built-in Fields]** underflik.

   De anpassade fält som du har lagt till visas under **[!UICONTROL Custom Fields]** underflik.

   The **[!UICONTROL All Fields]** på en underflik visas både inbyggda och anpassade fält som spåras.

### Ta bort fält som du inte vill spåra {#remove-fields-that-you-don-t-want-tracked}

Du kan ta bort fält som du inte vill att systemet ska spåra för en viss typ av objekt genom hela [!DNL Workfront] gränssnitt.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. På **[!UICONTROL Tracked Fields]** väljer du **[!UICONTROL All Fields]** underflik.

   Detta visar både inbyggda och anpassade fält som spåras.

1. Markera det fält som du vill sluta spåra och klicka sedan på **[!UICONTROL Remove]**.

1. I **[!UICONTROL Remove Field]** visas klickar du på **[!UICONTROL Yes, Remove It]** för att bekräfta.

Uppdateringar om tidigare spårade fält bevaras i [!UICONTROL Updates] det område där de registrerades.

## Bestäm vilka åtgärder som ska utföras [!DNL Workfront] spår för en objekttyp

Du kan ha [!DNL Workfront] spåra följande åtgärder som användare kan utföra på objekt i hela [!DNL Workfront] gränssnitt.

Du kan till exempel ha [!DNL Workfront] spela in en uppdatering varje gång en användare ändrar ett uppdrag till en uppgift eller ett problem. Ändringen visas sedan som en systemuppdatering i [!UICONTROL Updates] området för uppgiften eller utgåvan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Åtgärd</strong> </th> 
   <th><strong>Objekt</strong> </th> 
   <th><strong>Standardstatus</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Tilldelningen har ändrats</td> 
   <td>Uppgifter, problem</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Baslinjen tas bort</td> 
   <td>Projekt</td> 
   <td> <p>Handikappade</p> </td> 
  </tr> 
  <tr> 
   <td>Faktureringsposten skapas eller tas bort</td> 
   <td>Projekt</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Dokumentet skapas eller tas bort</td> 
   <td>Projekt, uppgifter, problem, Portfolio, program</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Utgift skapas eller tas bort</td> 
   <td>Projekt, uppgifter</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Timme loggas eller tas bort</td> 
   <td>Projekt, uppgifter, problem</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Utgåvan har tagits bort</td> 
   <td>Projekt</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Uppgiften har tagits bort</td> 
   <td>Projekt</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Någon har ändrat Åtkomst</td> 
   <td>Projekt, uppgifter, ärenden, dokument, Portfolio, program</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Kommentarsobjekt för prenumeration</td> 
   <td>Projekt, uppgifter, problem</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
 </tbody> 
</table>

Konfigurera vilka åtgärder du vill utföra [!DNL Workfront] att spåra:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. Klicka på **[!UICONTROL Actions]** -fliken.

1. Markera en åtgärd för att aktivera den eller avmarkera en åtgärd för att inaktivera den.
1. Klicka på **[!UICONTROL Save]**.

När du inaktiverar en åtgärd behålls alla tidigare inspelade uppdateringar om den åtgärden i [!UICONTROL Updates] det område där det registrerades.
