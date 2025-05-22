---
product-area: programs
navigation-topic: create and manage programs
title: Lägg till ett befintligt program i en Portfolio
description: Du kan lägga till befintliga program i en portfölj. Eftersom program inte kan finnas i två olika portföljer flyttas det om du lägger till ett befintligt program permanent från en portfölj till en annan.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
source-git-commit: 05512c4cfdc094e90abea471b5356337955119be
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Lägg till ett befintligt program i en portfölj

<!--Audited: 5/2025-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Samma funktioner kommer också att vara tillgängliga i produktionsmiljön för alla kunder efter en vecka från förhandsversionen. </span>

<span class="preview">Mer information finns i [Modernisering av gränssnitt](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>

Du kan lägga till befintliga program i en portfölj. Eftersom program inte kan finnas i två olika portföljer flyttas det om du lägger till ett befintligt program permanent från en portfölj till en annan.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>Nytt: [!UICONTROL Standard] </p><p>eller </p><p>Aktuell: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] tillgång till portföljer och program </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till portföljen och programmet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till ett befintligt program i en portfölj

1. Gå till en portfölj och klicka sedan på **[!UICONTROL Programs]** i den vänstra panelen.
1. Klicka på **[!UICONTROL New Program]**.
1. Klicka på **[!UICONTROL Existing Program]**.

   <span class="preview">Rutan **Lägg till program** öppnas.</span> <!--check screen shot - I logged changes for this casing-->

   <span class="preview">![Lägg till programruta](assets/add-programs-box.png)</span>

   >[!IMPORTANT]
   >
   >Om du lägger till ett befintligt program överförs alla projekt som är kopplade till det programmet till portföljen. Var försiktig så att du inte oavsiktligt flyttar projekt på det här sättet.

1. I fältet **[!UICONTROL Add Programs to this Portfolio]** skriver du namnet på ett program och markerar det när det visas i listan. <!--see the name of this field, I suggested changes here-->

   Du kan lägga till fler än ett program.

1. (Valfritt) Klicka på ikonen <span class="preview">**Ta bort** ![Ta bort ](assets/delete-icon.png)</span> bredvid namnet på ett program om du bestämmer dig för att inte lägga till det i portföljen.

1. Klicka på **[!UICONTROL Add Programs]**. <!--check this button in the UI after they implemented the changes??-->

   Programmet visas på fliken **[!UICONTROL Programs]** i den valda portföljen.
