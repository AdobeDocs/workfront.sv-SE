---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Konfigurera systemuppdateringar
description: Workfront genererar automatiska systemuppdateringar i ett objekts [!UICONTROL Updates]-område för att registrera de ändringar som användare utför på objektet. Som  [!DNL Workfront] administratör kan du konfigurera vilka objektfält och åtgärder  [!DNL Workfront] spårar som ska registrera systemuppdateringar.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 52ba2457ac2870d23e325f64163b683756f88ad4
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Konfigurera systemuppdateringar

<!-- Audited: 5/2025 -->

[!DNL Adobe Workfront] genererar automatiska systemuppdateringar i ett objekts [!UICONTROL Updates]-område för att registrera följande händelser:

* Ändringar som användare gör i ett objektfält
* Åtgärder som användare utför på ett objekt

Dessa systemuppdateringar innehåller följande typ av information:

* Ändringen gjordes
* Namnet på den användare som gjorde ändringen
* Tid och datum för ändringen

Mer information om systemuppdateringar finns i [Systemspårade uppdateringar](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Som [!DNL Workfront]-administratör kan du konfigurera vilka objektfält och åtgärder [!DNL Workfront] spårar för att registrera systemuppdateringar.

Du kan till exempel låta [!DNL Workfront] spåra alla ändringar som användare gör i namn på problem i hela systemet. Alla ändringar av problemnamn visas sedan som en systemuppdatering i problemområdet [!UICONTROL Updates].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td><p>Nytt: [!UICONTROL Standard]</p>
   eller
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Identifiera vilka fält [!DNL Workfront] spår för en objekttyp

Du kan bestämma vilken information [!DNL Workfront] spårar när användare ändrar information som är kopplad till en viss objekttyp i hela [!DNL Workfront] -gränssnittet. Det gör du genom att lägga till eller ta bort de fält som du vill att [!DNL Workfront] ska spåra för den objekttypen.

>[!NOTE]
>
>* [!DNL Workfront] kan inte spåra och registrera uppdateringar om beräknade anpassade fält.
>* Du kan anpassa systemuppdateringen för projekt, uppgifter, utgåvor, portfolior, program och användare. Du kan inte anpassa systemuppdateringen för mallar, dokument eller tidrapporter, men [!DNL Workfront] registrerar systemuppdateringar för dessa objekt.
>



* [Lägg till fält som du vill att [!DNL Workfront] ska spåra](#add-fields-you-want-workfront-to-track)
* [Ta bort fält som du inte vill spåra](#remove-fields-you-don-t-want-tracked)

### Lägg till fält som [!DNL Workfront] ska spåra {#add-fields-you-want-workfront-to-track}

Du kan lägga till fält som du vill att [!DNL Workfront] ska spåra för en viss typ av objekt i [!DNL Workfront]-gränssnittet. När användare ändrar information i det fältet registrerar [!DNL Workfront] information om ändringen som en systemuppdatering i [!UICONTROL Updates] -området för objektet.

>[!NOTE]
>
>Du kan spåra upp till 300 inbyggda och anpassade fält i uppdateringsflödena. Om du spårar det maximala antalet fält och vill spåra fler fält som inte visas på underfliken [!UICONTROL All Fields] måste du först ta bort några av de spårade fälten för att kunna spåra nya fält. Mer information om hur du tar bort fält från uppdateringsfälten finns i [Ta bort fält som du inte vill spåra](#remove-fields-you-don-t-want-tracked).

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Interface]** i panelen till vänster och sedan på **[!UICONTROL Update Feeds]**.

1. &#x200B; klicka på **[!UICONTROL Add Fields]** och markera sedan det objekt som du vill ska spåras i listrutan.

1. I rutan som visas börjar du skriva antingen ett inbyggt (standard) fält eller ett anpassat fält för objektet och markerar det sedan när det visas i listan.

   >[!NOTE]
   >
   >Om [!DNL Workfront] redan spårar fältet kan du inte lägga till det en andra gång från listan.

1. När du har lagt till alla fält som du vill att [!DNL Workfront] ska spåra klickar du på **[!UICONTROL Add Fields]**. De inbyggda fälten som du har lagt till visas under underfliken **[!UICONTROL Built-in Fields]** och de anpassade fälten visas under underfliken **[!UICONTROL Custom Fields]**.

   Underfliken **[!UICONTROL All Fields]** visar både inbyggda och anpassade fält som spåras.

### Ta bort fält som du inte vill spåra {#remove-fields-you-don-t-want-tracked}

Du kan ta bort fält som du inte vill att systemet ska spåra för en viss typ av objekt genom [!DNL Workfront]-gränssnittet.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Interface]** och sedan på **[!UICONTROL Update Feeds]**.

1. På fliken **[!UICONTROL Tracked Fields]** väljer du underfliken **[!UICONTROL All Fields]**. Både inbyggda och anpassade fält som spåras visas.

1. Markera det fält som du vill stoppa spårningen för och klicka sedan på **[!UICONTROL Remove]**.

1. Bekräfta genom att klicka på **[!UICONTROL Yes, Remove It]** i rutan **[!UICONTROL Remove Field]** som visas.

Uppdateringar om tidigare spårade fält bevaras i området [!UICONTROL Updates] där de spelades in.

## Bestäm vilka åtgärder [!DNL Workfront] spårar för en objekttyp

Du kan låta [!DNL Workfront] spåra följande åtgärder som användare kan utföra på objekt i gränssnittet för [!DNL Workfront].

Du kan till exempel låta [!DNL Workfront] spela in en uppdatering varje gång en användare ändrar en tilldelning till en aktivitet eller ett problem. Ändringen visas sedan som en systemuppdatering i området [!UICONTROL Updates] för uppgiften eller problemet.

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
   <td>Dokumentet har skapats eller tagits bort</td> 
   <td>Projekt, uppgifter, ärenden, portföljer, program</td> 
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
   <td>Projekt, uppgifter, ärenden, dokument, portföljer, program</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
  <tr> 
   <td>Kommentarsobjekt för prenumeration</td> 
   <td>Projekt, uppgifter, problem</td> 
   <td> <p>Aktiverad</p> </td> 
  </tr> 
 </tbody> 
</table>

Så här konfigurerar du vilka åtgärder du vill att [!DNL Workfront] ska spåra:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Interface]** och sedan på **[!UICONTROL Update Feeds]**.

1. Klicka på fliken **[!UICONTROL Actions]**.

1. Markera kryssrutan för en åtgärd om du vill aktivera den, eller avmarkera den om du vill inaktivera den.
1. Klicka på **[!UICONTROL Save]**.

När du inaktiverar en åtgärd behålls alla tidigare inspelade uppdateringar om den åtgärden i området [!UICONTROL Updates] där den spelades in.
