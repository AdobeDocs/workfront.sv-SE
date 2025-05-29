---
product-area: programs
navigation-topic: create and manage programs
title: Lägg till ett befintligt program i en Portfolio
description: Du kan lägga till befintliga program i en portfölj. Eftersom program inte kan finnas i två olika portföljer flyttas det om du lägger till ett befintligt program permanent från en portfölj till en annan.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
source-git-commit: 78b4724ca8d5df15ed76e9e882179e3cb127282c
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Lägg till ett befintligt program i en portfölj

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

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

   Rutan **Lägg till program** öppnas. <!--check screen shot - I logged changes for this casing-->

   ![Lägg till programruta](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >Om du lägger till ett befintligt program överförs alla projekt som är kopplade till det programmet till portföljen. Var försiktig så att du inte oavsiktligt flyttar projekt på det här sättet.

1. I fältet **[!UICONTROL Add Programs to this Portfolio]** skriver du namnet på ett program och markerar det när det visas i listan. <!--see the name of this field, I suggested changes here-->

   Du kan lägga till fler än ett program.

1. (Valfritt) Klicka på ikonen **Ta bort** ![Ta bort ](assets/delete-icon.png) bredvid namnet på ett program om du bestämmer dig för att inte lägga till det i portföljen.

1. Klicka på **[!UICONTROL Add Programs]**. <!--check this button in the UI after they implemented the changes??-->

   Programmet visas på fliken **[!UICONTROL Programs]** i den valda portföljen.
